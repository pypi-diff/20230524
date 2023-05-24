# Comparing `tmp/strelok-0.0.1.tar.gz` & `tmp/strelok-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strelok-0.0.1.tar", last modified: Wed May 24 08:13:54 2023, max compression
+gzip compressed data, was "strelok-0.0.2.tar", last modified: Wed May 24 08:26:05 2023, max compression
```

## Comparing `strelok-0.0.1.tar` & `strelok-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 juliusriel   (501) staff       (20)        0 2023-05-24 08:13:54.387515 strelok-0.0.1/
--rw-r--r--   0 juliusriel   (501) staff       (20)    14843 2023-05-24 08:13:54.387223 strelok-0.0.1/PKG-INFO
--rw-r--r--   0 juliusriel   (501) staff       (20)    14168 2023-05-24 06:07:42.000000 strelok-0.0.1/README.rst
--rw-r--r--   0 juliusriel   (501) staff       (20)       38 2023-05-24 08:13:54.387563 strelok-0.0.1/setup.cfg
--rw-r--r--   0 juliusriel   (501) staff       (20)      981 2023-05-24 08:13:36.000000 strelok-0.0.1/setup.py
-drwxr-xr-x   0 juliusriel   (501) staff       (20)        0 2023-05-24 08:13:54.386297 strelok-0.0.1/src/
-drwxr-xr-x   0 juliusriel   (501) staff       (20)        0 2023-05-24 08:13:54.387041 strelok-0.0.1/src/strelok.egg-info/
--rw-r--r--   0 juliusriel   (501) staff       (20)    14843 2023-05-24 08:13:54.000000 strelok-0.0.1/src/strelok.egg-info/PKG-INFO
--rw-r--r--   0 juliusriel   (501) staff       (20)      159 2023-05-24 08:13:54.000000 strelok-0.0.1/src/strelok.egg-info/SOURCES.txt
--rw-r--r--   0 juliusriel   (501) staff       (20)        1 2023-05-24 08:13:54.000000 strelok-0.0.1/src/strelok.egg-info/dependency_links.txt
--rw-r--r--   0 juliusriel   (501) staff       (20)        1 2023-05-24 08:13:54.000000 strelok-0.0.1/src/strelok.egg-info/top_level.txt
+drwxr-xr-x   0 juliusriel   (501) staff       (20)        0 2023-05-24 08:26:05.004585 strelok-0.0.2/
+-rw-r--r--   0 juliusriel   (501) staff       (20)    14843 2023-05-24 08:26:05.004325 strelok-0.0.2/PKG-INFO
+-rw-r--r--   0 juliusriel   (501) staff       (20)    14168 2023-05-24 06:07:42.000000 strelok-0.0.2/README.rst
+-rw-r--r--   0 juliusriel   (501) staff       (20)       38 2023-05-24 08:26:05.004626 strelok-0.0.2/setup.cfg
+-rw-r--r--   0 juliusriel   (501) staff       (20)     1056 2023-05-24 08:25:17.000000 strelok-0.0.2/setup.py
+drwxr-xr-x   0 juliusriel   (501) staff       (20)        0 2023-05-24 08:26:05.003254 strelok-0.0.2/src/
+drwxr-xr-x   0 juliusriel   (501) staff       (20)        0 2023-05-24 08:26:05.004155 strelok-0.0.2/src/strelok.egg-info/
+-rw-r--r--   0 juliusriel   (501) staff       (20)    14843 2023-05-24 08:26:04.000000 strelok-0.0.2/src/strelok.egg-info/PKG-INFO
+-rw-r--r--   0 juliusriel   (501) staff       (20)      193 2023-05-24 08:26:04.000000 strelok-0.0.2/src/strelok.egg-info/SOURCES.txt
+-rw-r--r--   0 juliusriel   (501) staff       (20)        1 2023-05-24 08:26:04.000000 strelok-0.0.2/src/strelok.egg-info/dependency_links.txt
+-rw-r--r--   0 juliusriel   (501) staff       (20)       37 2023-05-24 08:26:04.000000 strelok-0.0.2/src/strelok.egg-info/requires.txt
+-rw-r--r--   0 juliusriel   (501) staff       (20)        1 2023-05-24 08:26:04.000000 strelok-0.0.2/src/strelok.egg-info/top_level.txt
```

### Comparing `strelok-0.0.1/PKG-INFO` & `strelok-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strelok
-Version: 0.0.1
+Version: 0.0.2
 Summary: Strelok is a simple Python package that provides FEAT, a feature engineering automation toolkit. With a focus on simplicity, it offers user definable pipelines to streamline the feature engineering process and improve the performance of machine learning models
 Author: Julius Riel
 Author-email: julius.riel@icloud.com
 License: UNKNOWN
 Keywords: strelok,feature,selection,machine learning
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `strelok-0.0.1/README.rst` & `strelok-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `strelok-0.0.1/setup.py` & `strelok-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(
     name="strelok",
-    version="0.0.1",
+    version="0.0.2",
     author="Julius Riel",
     author_email="julius.riel@icloud.com",
     description="Strelok is a simple Python package that provides FEAT, a feature engineering automation toolkit. With a focus on simplicity, it offers user definable pipelines to streamline the feature engineering process and improve the performance of machine learning models",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     #url="https://github.com/yourusername/strelok",
+    install_requires=['numpy', 'pandas', 'sklearn', 'scipy', 'itertools'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

### Comparing `strelok-0.0.1/src/strelok.egg-info/PKG-INFO` & `strelok-0.0.2/src/strelok.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strelok
-Version: 0.0.1
+Version: 0.0.2
 Summary: Strelok is a simple Python package that provides FEAT, a feature engineering automation toolkit. With a focus on simplicity, it offers user definable pipelines to streamline the feature engineering process and improve the performance of machine learning models
 Author: Julius Riel
 Author-email: julius.riel@icloud.com
 License: UNKNOWN
 Keywords: strelok,feature,selection,machine learning
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

