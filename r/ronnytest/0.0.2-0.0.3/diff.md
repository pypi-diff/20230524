# Comparing `tmp/ronnytest-0.0.2.tar.gz` & `tmp/ronnytest-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ronnytest-0.0.2.tar", last modified: Wed May 24 11:43:42 2023, max compression
+gzip compressed data, was "dist/ronnytest-0.0.3.tar", last modified: Wed May 24 11:56:13 2023, max compression
```

## Comparing `ronnytest-0.0.2.tar` & `ronnytest-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 11:43:42.000000 ronnytest-0.0.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 11:43:42.000000 ronnytest-0.0.2/ronnytest.egg-info/
--rw-r--r--   0 root         (0) root         (0)      434 2023-05-24 11:43:42.000000 ronnytest-0.0.2/ronnytest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 11:43:42.000000 ronnytest-0.0.2/ronnytest.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-24 11:43:42.000000 ronnytest-0.0.2/ronnytest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 11:43:42.000000 ronnytest-0.0.2/ronnytest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 11:30:26.000000 ronnytest-0.0.2/README.md
--rw-r--r--   0 root         (0) root         (0)     1073 2023-05-15 11:35:28.000000 ronnytest-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      434 2023-05-24 11:43:42.000000 ronnytest-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 11:43:42.000000 ronnytest-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1049 2023-05-24 11:43:34.000000 ronnytest-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 11:56:13.000000 ronnytest-0.0.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 11:56:13.000000 ronnytest-0.0.3/ronnytest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-24 11:56:13.000000 ronnytest-0.0.3/ronnytest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 11:56:13.000000 ronnytest-0.0.3/ronnytest.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-05-24 11:56:13.000000 ronnytest-0.0.3/ronnytest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 11:56:13.000000 ronnytest-0.0.3/ronnytest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2023-05-24 11:51:40.000000 ronnytest-0.0.3/README.md
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-05-15 11:35:28.000000 ronnytest-0.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-24 11:56:13.000000 ronnytest-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 11:56:13.000000 ronnytest-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-05-24 11:56:09.000000 ronnytest-0.0.3/setup.py
```

### Comparing `ronnytest-0.0.2/LICENSE` & `ronnytest-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ronnytest-0.0.2/setup.py` & `ronnytest-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 class PostInstallCommand(install):
     """Post-installation for installation mode."""
     def run(self):
         install.run(self)
         print('请检查pip指令是否有使用--index-url强制下载内部源,禁止非私有源的外部同名包！'.encode('utf-8').decode('latin1'))
         # os.system("cat testing.egg-info/PKG-INFO")
 
-with open("README.md", "r", encoding='utf-8') as fh:
+with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="ronnytest",
-  version="0.0.2",
+  version="0.0.3",
   author="wxpay_sec_team",
   author_email="wxpay_sec_team@tencent.com",
   description="ronnytest",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypi/ronnytest",
   packages=setuptools.find_packages(),
```

