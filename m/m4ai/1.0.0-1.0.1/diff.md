# Comparing `tmp/m4ai-1.0.0.tar.gz` & `tmp/m4ai-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m4ai-1.0.0.tar", last modified: Wed May 24 11:43:21 2023, max compression
+gzip compressed data, was "m4ai-1.0.1.tar", last modified: Wed May 24 11:55:27 2023, max compression
```

## Comparing `m4ai-1.0.0.tar` & `m4ai-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 11:43:22.000000 m4ai-1.0.0/
--rw-rw-rw-   0        0        0      540 2023-05-24 11:43:22.000000 m4ai-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      412 2023-05-24 11:24:52.000000 m4ai-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 11:43:22.000000 m4ai-1.0.0/m4ai.egg-info/
--rw-rw-rw-   0        0        0      540 2023-05-24 11:43:22.000000 m4ai-1.0.0/m4ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-05-24 11:43:22.000000 m4ai-1.0.0/m4ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 11:43:22.000000 m4ai-1.0.0/m4ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-24 11:43:22.000000 m4ai-1.0.0/m4ai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 11:43:22.000000 m4ai-1.0.0/m4ai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 11:43:22.000000 m4ai-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      793 2023-05-24 11:43:12.000000 m4ai-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 11:55:28.000000 m4ai-1.0.1/
+-rw-rw-rw-   0        0        0      543 2023-05-24 11:55:28.000000 m4ai-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-05-24 11:24:52.000000 m4ai-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 11:55:28.000000 m4ai-1.0.1/m4ai.egg-info/
+-rw-rw-rw-   0        0        0      543 2023-05-24 11:55:28.000000 m4ai-1.0.1/m4ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-05-24 11:55:28.000000 m4ai-1.0.1/m4ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 11:55:28.000000 m4ai-1.0.1/m4ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-24 11:55:28.000000 m4ai-1.0.1/m4ai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 11:55:28.000000 m4ai-1.0.1/m4ai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 11:55:28.000000 m4ai-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      797 2023-05-24 11:55:28.000000 m4ai-1.0.1/setup.py
```

### Comparing `m4ai-1.0.0/PKG-INFO` & `m4ai-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: m4ai
-Version: 1.0.0
+Version: 1.0.1
 Summary: 冰淇淋
 Home-page: https://github.com/zacharylyj/m4ai
-Author: zac
+Author: zachar
 Author-email: zacharylyj@example.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `m4ai-1.0.0/m4ai.egg-info/PKG-INFO` & `m4ai-1.0.1/m4ai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: m4ai
-Version: 1.0.0
+Version: 1.0.1
 Summary: 冰淇淋
 Home-page: https://github.com/zacharylyj/m4ai
-Author: zac
+Author: zachar
 Author-email: zacharylyj@example.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `m4ai-1.0.0/setup.py` & `m4ai-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='m4ai',
-    version='1.0.0',
-    author='zac',
+    version='1.0.1',
+    author='zachary',
     author_email='zacharylyj@example.com',
     description='冰淇淋',
     long_description='现在我有冰淇淋',
     long_description_content_type='text/markdown',
     url='https://github.com/zacharylyj/m4ai',
     packages=find_packages(),
     classifiers=[
```

