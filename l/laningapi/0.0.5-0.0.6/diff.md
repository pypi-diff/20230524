# Comparing `tmp/laningapi-0.0.5.tar.gz` & `tmp/laningapi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laningapi-0.0.5.tar", last modified: Tue Apr  4 01:35:38 2023, max compression
+gzip compressed data, was "laningapi-0.0.6.tar", last modified: Wed May 24 08:30:59 2023, max compression
```

## Comparing `laningapi-0.0.5.tar` & `laningapi-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 changwei   (501) staff       (20)        0 2023-04-04 01:35:38.507059 laningapi-0.0.5/
--rw-r--r--   0 changwei   (501) staff       (20)       94 2023-04-04 01:34:16.000000 laningapi-0.0.5/MANIFEST.in
--rw-r--r--   0 changwei   (501) staff       (20)      181 2023-04-04 01:35:38.506946 laningapi-0.0.5/PKG-INFO
--rw-r--r--   0 changwei   (501) staff       (20)      395 2022-12-08 06:35:53.000000 laningapi-0.0.5/README.md
-drwxr-xr-x   0 changwei   (501) staff       (20)        0 2023-04-04 01:35:38.506748 laningapi-0.0.5/laningapi/
--rw-r--r--   0 changwei   (501) staff       (20)      174 2023-04-04 01:34:16.000000 laningapi-0.0.5/laningapi/__init__.py
--rw-r--r--   0 changwei   (501) staff       (20)     1025 2023-04-04 01:34:16.000000 laningapi-0.0.5/laningapi/_mock.py
--rw-r--r--   0 changwei   (501) staff       (20)     2968 2023-04-04 01:34:16.000000 laningapi-0.0.5/laningapi/base.py
--rw-r--r--   0 changwei   (501) staff       (20)     1171 2023-04-04 01:34:16.000000 laningapi-0.0.5/laningapi/dictionary.py
--rw-r--r--   0 changwei   (501) staff       (20)     1061 2023-04-04 01:34:16.000000 laningapi-0.0.5/laningapi/oplog.py
--rw-r--r--   0 changwei   (501) staff       (20)     1324 2023-04-04 01:34:16.000000 laningapi-0.0.5/laningapi/series.py
--rw-r--r--   0 changwei   (501) staff       (20)     3802 2023-04-04 01:34:16.000000 laningapi-0.0.5/laningapi/target.py
--rw-r--r--   0 changwei   (501) staff       (20)        0 2022-12-08 06:35:50.000000 laningapi-0.0.5/laningapi/task.py
-drwxr-xr-x   0 changwei   (501) staff       (20)        0 2023-04-04 01:35:38.506825 laningapi-0.0.5/laningapi.egg-info/
--rwx------   0 changwei   (501) staff       (20)      190 2023-04-04 01:35:38.000000 laningapi-0.0.5/laningapi.egg-info/SOURCES.txt
--rw-r--r--   0 changwei   (501) staff       (20)       38 2023-04-04 01:35:38.507094 laningapi-0.0.5/setup.cfg
--rw-r--r--   0 changwei   (501) staff       (20)      724 2023-04-04 01:34:39.000000 laningapi-0.0.5/setup.py
+drwxr-xr-x   0 changwei   (501) staff       (20)        0 2023-05-24 08:30:59.769670 laningapi-0.0.6/
+-rw-r--r--   0 changwei   (501) staff       (20)       94 2023-04-04 01:34:16.000000 laningapi-0.0.6/MANIFEST.in
+-rw-r--r--   0 changwei   (501) staff       (20)      181 2023-05-24 08:30:59.769565 laningapi-0.0.6/PKG-INFO
+-rw-r--r--   0 changwei   (501) staff       (20)      395 2022-12-08 06:35:53.000000 laningapi-0.0.6/README.md
+drwxr-xr-x   0 changwei   (501) staff       (20)        0 2023-05-24 08:30:59.769364 laningapi-0.0.6/laningapi/
+-rw-r--r--   0 changwei   (501) staff       (20)      174 2023-04-04 01:34:16.000000 laningapi-0.0.6/laningapi/__init__.py
+-rw-r--r--   0 changwei   (501) staff       (20)     1025 2023-04-04 01:34:16.000000 laningapi-0.0.6/laningapi/_mock.py
+-rw-r--r--   0 changwei   (501) staff       (20)     3144 2023-05-24 08:27:18.000000 laningapi-0.0.6/laningapi/base.py
+-rw-r--r--   0 changwei   (501) staff       (20)     1171 2023-04-04 01:34:16.000000 laningapi-0.0.6/laningapi/dictionary.py
+-rw-r--r--   0 changwei   (501) staff       (20)     1061 2023-04-04 01:34:16.000000 laningapi-0.0.6/laningapi/oplog.py
+-rw-r--r--   0 changwei   (501) staff       (20)     1324 2023-04-04 01:34:16.000000 laningapi-0.0.6/laningapi/series.py
+-rw-r--r--   0 changwei   (501) staff       (20)     3802 2023-04-04 01:34:16.000000 laningapi-0.0.6/laningapi/target.py
+-rw-r--r--   0 changwei   (501) staff       (20)        0 2022-12-08 06:35:50.000000 laningapi-0.0.6/laningapi/task.py
+drwxr-xr-x   0 changwei   (501) staff       (20)        0 2023-05-24 08:30:59.769443 laningapi-0.0.6/laningapi.egg-info/
+-rwx------   0 changwei   (501) staff       (20)      190 2023-05-24 08:30:59.000000 laningapi-0.0.6/laningapi.egg-info/SOURCES.txt
+-rw-r--r--   0 changwei   (501) staff       (20)       38 2023-05-24 08:30:59.769725 laningapi-0.0.6/setup.cfg
+-rw-r--r--   0 changwei   (501) staff       (20)      724 2023-05-24 08:30:40.000000 laningapi-0.0.6/setup.py
```

### Comparing `laningapi-0.0.5/laningapi/_mock.py` & `laningapi-0.0.6/laningapi/_mock.py`

 * *Files identical despite different names*

### Comparing `laningapi-0.0.5/laningapi/base.py` & `laningapi-0.0.6/laningapi/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,20 @@
 
 
 class TransportInternal(Transport):
     def init(self):
         pass
 
     def post(self, url, *, json) -> Response:
-        return requests.post(url, json=json)
+        headers = {
+            "x-forwarded-for-zl": "127.0.0.1",
+            "x-current-user-id": 1,
+            "x-current-username": "laningapi"
+        }
+        return requests.post(url, json=json, headers=headers)
 
 
 class TransportExternal(Transport):
     def __init__(self):
         self.token = None
 
         # self.username = None
```

### Comparing `laningapi-0.0.5/laningapi/dictionary.py` & `laningapi-0.0.6/laningapi/dictionary.py`

 * *Files identical despite different names*

### Comparing `laningapi-0.0.5/laningapi/oplog.py` & `laningapi-0.0.6/laningapi/oplog.py`

 * *Files identical despite different names*

### Comparing `laningapi-0.0.5/laningapi/series.py` & `laningapi-0.0.6/laningapi/series.py`

 * *Files identical despite different names*

### Comparing `laningapi-0.0.5/laningapi/target.py` & `laningapi-0.0.6/laningapi/target.py`

 * *Files identical despite different names*

### Comparing `laningapi-0.0.5/setup.py` & `laningapi-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- encoding: UTF-8 -*-
 from setuptools import setup, find_packages
 
 setup(
     name="laningapi",  # 包名
     author="laning",
     author_email="nkchwfree@163.com",
-    version="0.0.5",  # 版本信息
+    version="0.0.6",  # 版本信息
     packages=["laningapi"],
     include_package_data=True,  # 自动打包文件夹内所有数据
     zip_safe=True,  # 设定项目包为安全，不用每次都检测其安全性
     install_requires=[  # 安装依赖的其他包（测试数据）
     ],
 
     # 设置程序的入口为path
```

