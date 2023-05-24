# Comparing `tmp/ronnytest-0.0.3.tar.gz` & `tmp/ronnytest-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ronnytest-0.0.3.tar", last modified: Wed May 24 11:56:13 2023, max compression
+gzip compressed data, was "dist/ronnytest-0.0.4.tar", last modified: Wed May 24 12:01:44 2023, max compression
```

## Comparing `ronnytest-0.0.3.tar` & `ronnytest-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 11:56:13.000000 ronnytest-0.0.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 11:56:13.000000 ronnytest-0.0.3/ronnytest.egg-info/
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-24 11:56:13.000000 ronnytest-0.0.3/ronnytest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 11:56:13.000000 ronnytest-0.0.3/ronnytest.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-24 11:56:13.000000 ronnytest-0.0.3/ronnytest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 11:56:13.000000 ronnytest-0.0.3/ronnytest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      122 2023-05-24 11:51:40.000000 ronnytest-0.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)     1073 2023-05-15 11:35:28.000000 ronnytest-0.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-24 11:56:13.000000 ronnytest-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 11:56:13.000000 ronnytest-0.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1031 2023-05-24 11:56:09.000000 ronnytest-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:44.000000 ronnytest-0.0.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:44.000000 ronnytest-0.0.4/ronnytest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-24 12:01:44.000000 ronnytest-0.0.4/ronnytest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 12:01:44.000000 ronnytest-0.0.4/ronnytest.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-05-24 12:01:44.000000 ronnytest-0.0.4/ronnytest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 12:01:44.000000 ronnytest-0.0.4/ronnytest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2023-05-24 11:51:40.000000 ronnytest-0.0.4/README.md
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-05-15 11:35:28.000000 ronnytest-0.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-24 12:01:44.000000 ronnytest-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 12:01:44.000000 ronnytest-0.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-05-24 12:00:22.000000 ronnytest-0.0.4/setup.py
```

### Comparing `ronnytest-0.0.3/ronnytest.egg-info/PKG-INFO` & `ronnytest-0.0.4/ronnytest.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ronnytest
-Version: 0.0.3
+Version: 0.0.4
 Summary: ronnytest
 Home-page: https://github.com/pypi/ronnytest
 Author: wxpay_sec_team
 Author-email: wxpay_sec_team@tencent.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ronnytest-0.0.3/LICENSE` & `ronnytest-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ronnytest-0.0.3/PKG-INFO` & `ronnytest-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ronnytest
-Version: 0.0.3
+Version: 0.0.4
 Summary: ronnytest
 Home-page: https://github.com/pypi/ronnytest
 Author: wxpay_sec_team
 Author-email: wxpay_sec_team@tencent.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ronnytest-0.0.3/setup.py` & `ronnytest-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from setuptools.command.install import install
 import os
 
 class PostInstallCommand(install):
     """Post-installation for installation mode."""
     def run(self):
         install.run(self)
-        print('请检查pip指令是否有使用--index-url强制下载内部源,禁止非私有源的外部同名包！'.encode('utf-8').decode('latin1'))
-        # os.system("cat testing.egg-info/PKG-INFO")
+        # print('请检查pip指令是否有使用--index-url强制下载内部源,禁止非私有源的外部同名包！'.encode('utf-8').decode('latin1'))
+        os.system("cat ronnytest.egg-info/PKG-INFO")
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="ronnytest",
-  version="0.0.3",
+  version="0.0.4",
   author="wxpay_sec_team",
   author_email="wxpay_sec_team@tencent.com",
   description="ronnytest",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypi/ronnytest",
   packages=setuptools.find_packages(),
```

