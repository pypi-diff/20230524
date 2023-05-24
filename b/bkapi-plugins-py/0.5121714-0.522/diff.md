# Comparing `tmp/bkapi-plugins-py-0.5121714.tar.gz` & `tmp/bkapi-plugins-py-0.522.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bkapi-plugins-py-0.5121714.tar", last modified: Fri May 12 09:14:55 2023, max compression
+gzip compressed data, was "bkapi-plugins-py-0.522.tar", last modified: Mon May 22 06:43:13 2023, max compression
```

## Comparing `bkapi-plugins-py-0.5121714.tar` & `bkapi-plugins-py-0.522.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 09:14:55.621156 bkapi-plugins-py-0.5121714/
--rw-rw-rw-   0        0        0       39 2023-04-17 10:01:55.000000 bkapi-plugins-py-0.5121714/MANIFEST.in
--rw-rw-rw-   0        0        0      261 2023-05-12 09:14:55.621156 bkapi-plugins-py-0.5121714/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-12 09:14:55.595646 bkapi-plugins-py-0.5121714/bkapi_plugins/
-drwxrwxrwx   0        0        0        0 2023-05-12 09:14:55.609120 bkapi-plugins-py-0.5121714/bkapi_plugins/files/
--rw-rw-rw-   0        0        0  4663879 2023-05-12 08:47:34.000000 bkapi-plugins-py-0.5121714/bkapi_plugins/files/code.zip
-drwxrwxrwx   0        0        0        0 2023-05-12 09:14:55.620090 bkapi-plugins-py-0.5121714/bkapi_plugins_py.egg-info/
--rw-rw-rw-   0        0        0      261 2023-05-12 09:14:55.000000 bkapi-plugins-py-0.5121714/bkapi_plugins_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-12 09:14:55.000000 bkapi-plugins-py-0.5121714/bkapi_plugins_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 09:14:55.000000 bkapi-plugins-py-0.5121714/bkapi_plugins_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 09:14:55.000000 bkapi-plugins-py-0.5121714/bkapi_plugins_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 09:14:55.623153 bkapi-plugins-py-0.5121714/setup.cfg
--rw-rw-rw-   0        0        0      894 2023-05-12 09:14:53.000000 bkapi-plugins-py-0.5121714/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:43:13.873771 bkapi-plugins-py-0.522/
+-rw-rw-rw-   0        0        0       39 2023-04-17 10:01:55.000000 bkapi-plugins-py-0.522/MANIFEST.in
+-rw-rw-rw-   0        0        0      257 2023-05-22 06:43:13.873771 bkapi-plugins-py-0.522/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-22 06:43:13.845750 bkapi-plugins-py-0.522/bkapi_plugins/
+drwxrwxrwx   0        0        0        0 2023-05-22 06:43:13.851749 bkapi-plugins-py-0.522/bkapi_plugins/files/
+-rw-rw-rw-   0        0        0  9435808 2023-05-22 06:40:59.000000 bkapi-plugins-py-0.522/bkapi_plugins/files/kafka-exporter.zip
+drwxrwxrwx   0        0        0        0 2023-05-22 06:43:13.871772 bkapi-plugins-py-0.522/bkapi_plugins_py.egg-info/
+-rw-rw-rw-   0        0        0      257 2023-05-22 06:43:13.000000 bkapi-plugins-py-0.522/bkapi_plugins_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-05-22 06:43:13.000000 bkapi-plugins-py-0.522/bkapi_plugins_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 06:43:13.000000 bkapi-plugins-py-0.522/bkapi_plugins_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 06:43:13.000000 bkapi-plugins-py-0.522/bkapi_plugins_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 06:43:13.874770 bkapi-plugins-py-0.522/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-05-22 06:43:01.000000 bkapi-plugins-py-0.522/setup.py
```

### Comparing `bkapi-plugins-py-0.5121714/setup.py` & `bkapi-plugins-py-0.522/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 readme = ''
 
 setup(
     description='',
     long_description=readme,
     name='bkapi-plugins-py', # 包的名字
-    version='0.5121714', # 版本号每次打包完要改一下
+    version='0.522', # 版本号每次打包完要改一下
     python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*',
     author='fadewalk',
     license='Apach License 2.0',
     # packages=find_packages(),
     # namespace_packages=['bkapi_plugins'],
     package_dir={'': '.'},
     include_package_data=True,
```

