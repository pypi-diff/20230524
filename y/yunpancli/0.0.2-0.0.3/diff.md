# Comparing `tmp/yunpancli-0.0.2.tar.gz` & `tmp/yunpancli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunpancli-0.0.2.tar", last modified: Wed May 24 10:16:11 2023, max compression
+gzip compressed data, was "yunpancli-0.0.3.tar", last modified: Wed May 24 10:34:33 2023, max compression
```

## Comparing `yunpancli-0.0.2.tar` & `yunpancli-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-24 10:16:11.950970 yunpancli-0.0.2/
--rw-r--r--   0 mac        (501) staff       (20)     1063 2023-05-02 10:51:07.000000 yunpancli-0.0.2/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)      413 2023-05-24 10:16:11.950795 yunpancli-0.0.2/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-03 08:16:36.000000 yunpancli-0.0.2/README.md
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-05-24 10:16:11.951019 yunpancli-0.0.2/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      692 2023-05-24 10:15:55.000000 yunpancli-0.0.2/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-24 10:16:11.949968 yunpancli-0.0.2/yunpancli/
--rw-r--r--   0 mac        (501) staff       (20)       39 2023-05-03 08:15:03.000000 yunpancli-0.0.2/yunpancli/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     8499 2023-05-03 10:18:36.000000 yunpancli-0.0.2/yunpancli/baidu_pan_sdk.py
--rw-r--r--   0 mac        (501) staff       (20)     6723 2023-05-24 10:11:30.000000 yunpancli-0.0.2/yunpancli/base.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-24 10:16:11.950598 yunpancli-0.0.2/yunpancli.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      413 2023-05-24 10:16:11.000000 yunpancli-0.0.2/yunpancli.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      261 2023-05-24 10:16:11.000000 yunpancli-0.0.2/yunpancli.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-24 10:16:11.000000 yunpancli-0.0.2/yunpancli.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       45 2023-05-24 10:16:11.000000 yunpancli-0.0.2/yunpancli.egg-info/entry_points.txt
--rw-r--r--   0 mac        (501) staff       (20)       10 2023-05-24 10:16:11.000000 yunpancli-0.0.2/yunpancli.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-24 10:34:33.900999 yunpancli-0.0.3/
+-rw-r--r--   0 mac        (501) staff       (20)     1063 2023-05-02 10:51:07.000000 yunpancli-0.0.3/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)      413 2023-05-24 10:34:33.900831 yunpancli-0.0.3/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-03 08:16:36.000000 yunpancli-0.0.3/README.md
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-05-24 10:34:33.901066 yunpancli-0.0.3/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      692 2023-05-24 10:34:23.000000 yunpancli-0.0.3/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-24 10:34:33.900032 yunpancli-0.0.3/yunpancli/
+-rw-r--r--   0 mac        (501) staff       (20)       39 2023-05-03 08:15:03.000000 yunpancli-0.0.3/yunpancli/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     8499 2023-05-03 10:18:36.000000 yunpancli-0.0.3/yunpancli/baidu_pan_sdk.py
+-rw-r--r--   0 mac        (501) staff       (20)     6857 2023-05-24 10:33:36.000000 yunpancli-0.0.3/yunpancli/base.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-24 10:34:33.900668 yunpancli-0.0.3/yunpancli.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      413 2023-05-24 10:34:33.000000 yunpancli-0.0.3/yunpancli.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      261 2023-05-24 10:34:33.000000 yunpancli-0.0.3/yunpancli.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-24 10:34:33.000000 yunpancli-0.0.3/yunpancli.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       45 2023-05-24 10:34:33.000000 yunpancli-0.0.3/yunpancli.egg-info/entry_points.txt
+-rw-r--r--   0 mac        (501) staff       (20)       10 2023-05-24 10:34:33.000000 yunpancli-0.0.3/yunpancli.egg-info/top_level.txt
```

### Comparing `yunpancli-0.0.2/LICENSE` & `yunpancli-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yunpancli-0.0.2/setup.py` & `yunpancli-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yunpancli",
     entry_points={"console_scripts": ["yunpancli=yunpancli:main"]},
-    version="0.0.2",
+    version="0.0.3",
     author="Tang Yubin",
     author_email="tang-yu-bin@qq.com",
     description="cloud storage CLI (Command Line Interface)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/aierwiki/yunpancli",
     packages=setuptools.find_packages(),
```

### Comparing `yunpancli-0.0.2/yunpancli/baidu_pan_sdk.py` & `yunpancli-0.0.3/yunpancli/baidu_pan_sdk.py`

 * *Files identical despite different names*

### Comparing `yunpancli-0.0.2/yunpancli/base.py` & `yunpancli-0.0.3/yunpancli/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 class PanCLI():
     ACCOUNT_CONFIG_FILE = os.path.expanduser('~/.cache/pancli/account_info.json')
     
     def __init__(self):
         self.account_info = {}
         self.sdk = BaiduPanSDK()
+	if os.path.exists(os.path.dirname(PanCLI.ACCOUNT_CONFIG_FILE)):
+            os.makedirs(os.path.dirname(PanCLI.ACCOUNT_CONFIG_FILE))
     
     def load_config(self):
         if not os.path.exists(PanCLI.ACCOUNT_CONFIG_FILE):
             logger.debug(f"{PanCLI.ACCOUNT_CONFIG_FILE} not exist!")
             return False
         account_info = {}
         with open(PanCLI.ACCOUNT_CONFIG_FILE, 'r') as f:
```

