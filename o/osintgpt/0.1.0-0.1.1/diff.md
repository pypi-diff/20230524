# Comparing `tmp/osintgpt-0.1.0.tar.gz` & `tmp/osintgpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osintgpt-0.1.0.tar", last modified: Mon May 22 13:01:40 2023, max compression
+gzip compressed data, was "osintgpt-0.1.1.tar", last modified: Wed May 24 00:46:26 2023, max compression
```

## Comparing `osintgpt-0.1.0.tar` & `osintgpt-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 13:01:40.756982 osintgpt-0.1.0/
--rw-rw-rw-   0        0        0     4024 2023-05-22 13:01:40.755980 osintgpt-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2861 2023-05-15 16:47:53.000000 osintgpt-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 13:01:40.718035 osintgpt-0.1.0/osintgpt/
--rw-rw-rw-   0        0        0      484 2023-04-23 18:37:18.000000 osintgpt-0.1.0/osintgpt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:01:40.727693 osintgpt-0.1.0/osintgpt/databases/
--rw-rw-rw-   0        0        0       69 2023-05-10 16:50:39.000000 osintgpt-0.1.0/osintgpt/databases/__init__.py
--rw-rw-rw-   0        0        0     7548 2023-05-20 16:50:46.000000 osintgpt-0.1.0/osintgpt/databases/sql_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:01:40.730695 osintgpt-0.1.0/osintgpt/embeddings/
--rw-rw-rw-   0        0        0       81 2023-04-25 01:08:29.000000 osintgpt-0.1.0/osintgpt/embeddings/__init__.py
--rw-rw-rw-   0        0        0     6287 2023-05-13 17:07:35.000000 osintgpt-0.1.0/osintgpt/embeddings/openai_embeddings.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:01:40.734709 osintgpt-0.1.0/osintgpt/exceptions/
--rw-rw-rw-   0        0        0       28 2023-05-05 00:54:36.000000 osintgpt-0.1.0/osintgpt/exceptions/__init__.py
--rw-rw-rw-   0        0        0      744 2023-05-05 00:40:59.000000 osintgpt-0.1.0/osintgpt/exceptions/errors.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:01:40.738731 osintgpt-0.1.0/osintgpt/gpt/
--rw-rw-rw-   0        0        0       59 2023-05-07 17:34:59.000000 osintgpt-0.1.0/osintgpt/gpt/__init__.py
--rw-rw-rw-   0        0        0    22625 2023-05-21 17:05:36.000000 osintgpt-0.1.0/osintgpt/gpt/openai_gpt.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:01:40.740731 osintgpt-0.1.0/osintgpt/utils/
--rw-rw-rw-   0        0        0      551 2023-05-19 16:42:58.000000 osintgpt-0.1.0/osintgpt/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:01:40.755018 osintgpt-0.1.0/osintgpt/vector_store/
--rw-rw-rw-   0        0        0      104 2023-05-20 17:02:52.000000 osintgpt-0.1.0/osintgpt/vector_store/__init__.py
--rw-rw-rw-   0        0        0     1393 2023-05-08 18:05:29.000000 osintgpt-0.1.0/osintgpt/vector_store/base.py
--rw-rw-rw-   0        0        0    10118 2023-05-21 14:55:49.000000 osintgpt-0.1.0/osintgpt/vector_store/qdrant.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:01:40.723710 osintgpt-0.1.0/osintgpt.egg-info/
--rw-rw-rw-   0        0        0     4024 2023-05-22 13:01:40.000000 osintgpt-0.1.0/osintgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      542 2023-05-22 13:01:40.000000 osintgpt-0.1.0/osintgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 13:01:40.000000 osintgpt-0.1.0/osintgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 13:01:40.000000 osintgpt-0.1.0/osintgpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 13:01:40.756982 osintgpt-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1644 2023-05-21 13:33:42.000000 osintgpt-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 00:46:26.689513 osintgpt-0.1.1/
+-rw-rw-rw-   0        0        0     6230 2023-05-24 00:46:26.688513 osintgpt-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5067 2023-05-24 00:39:08.000000 osintgpt-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 00:46:26.647930 osintgpt-0.1.1/osintgpt/
+-rw-rw-rw-   0        0        0      484 2023-04-23 18:37:18.000000 osintgpt-0.1.1/osintgpt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 00:46:26.669436 osintgpt-0.1.1/osintgpt/databases/
+-rw-rw-rw-   0        0        0       69 2023-05-23 22:00:35.000000 osintgpt-0.1.1/osintgpt/databases/__init__.py
+-rw-rw-rw-   0        0        0     7548 2023-05-23 22:12:27.000000 osintgpt-0.1.1/osintgpt/databases/sql_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-24 00:46:26.672432 osintgpt-0.1.1/osintgpt/embeddings/
+-rw-rw-rw-   0        0        0       81 2023-04-25 01:08:29.000000 osintgpt-0.1.1/osintgpt/embeddings/__init__.py
+-rw-rw-rw-   0        0        0     6287 2023-05-13 17:07:35.000000 osintgpt-0.1.1/osintgpt/embeddings/openai_embeddings.py
+drwxrwxrwx   0        0        0        0 2023-05-24 00:46:26.674965 osintgpt-0.1.1/osintgpt/exceptions/
+-rw-rw-rw-   0        0        0       28 2023-05-05 00:54:36.000000 osintgpt-0.1.1/osintgpt/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      744 2023-05-05 00:40:59.000000 osintgpt-0.1.1/osintgpt/exceptions/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-24 00:46:26.677981 osintgpt-0.1.1/osintgpt/llms/
+-rw-rw-rw-   0        0        0       59 2023-05-07 17:34:59.000000 osintgpt-0.1.1/osintgpt/llms/__init__.py
+-rw-rw-rw-   0        0        0    32400 2023-05-24 00:24:53.000000 osintgpt-0.1.1/osintgpt/llms/openai_gpt.py
+drwxrwxrwx   0        0        0        0 2023-05-24 00:46:26.681012 osintgpt-0.1.1/osintgpt/semantic_operations/
+-rw-rw-rw-   0        0        0       66 2023-05-24 00:22:44.000000 osintgpt-0.1.1/osintgpt/semantic_operations/__init__.py
+-rw-rw-rw-   0        0        0    11938 2023-05-24 00:25:03.000000 osintgpt-0.1.1/osintgpt/semantic_operations/operations.py
+drwxrwxrwx   0        0        0        0 2023-05-24 00:46:26.681981 osintgpt-0.1.1/osintgpt/utils/
+-rw-rw-rw-   0        0        0      551 2023-05-19 16:42:58.000000 osintgpt-0.1.1/osintgpt/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 00:46:26.686534 osintgpt-0.1.1/osintgpt/vector_store/
+-rw-rw-rw-   0        0        0      104 2023-05-20 17:02:52.000000 osintgpt-0.1.1/osintgpt/vector_store/__init__.py
+-rw-rw-rw-   0        0        0     1392 2023-05-23 21:55:23.000000 osintgpt-0.1.1/osintgpt/vector_store/base.py
+-rw-rw-rw-   0        0        0    10118 2023-05-23 23:28:21.000000 osintgpt-0.1.1/osintgpt/vector_store/qdrant.py
+drwxrwxrwx   0        0        0        0 2023-05-24 00:46:26.666435 osintgpt-0.1.1/osintgpt.egg-info/
+-rw-rw-rw-   0        0        0     6230 2023-05-24 00:46:26.000000 osintgpt-0.1.1/osintgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      659 2023-05-24 00:46:26.000000 osintgpt-0.1.1/osintgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 00:46:26.000000 osintgpt-0.1.1/osintgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-05-24 00:46:26.000000 osintgpt-0.1.1/osintgpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-24 00:46:26.000000 osintgpt-0.1.1/osintgpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 00:46:26.689513 osintgpt-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1658 2023-05-24 00:45:48.000000 osintgpt-0.1.1/setup.py
```

### Comparing `osintgpt-0.1.0/osintgpt/databases/sql_manager.py` & `osintgpt-0.1.1/osintgpt/databases/sql_manager.py`

 * *Files identical despite different names*

### Comparing `osintgpt-0.1.0/osintgpt/embeddings/openai_embeddings.py` & `osintgpt-0.1.1/osintgpt/embeddings/openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `osintgpt-0.1.0/osintgpt/exceptions/errors.py` & `osintgpt-0.1.1/osintgpt/exceptions/errors.py`

 * *Files identical despite different names*

### Comparing `osintgpt-0.1.0/osintgpt/utils/__init__.py` & `osintgpt-0.1.1/osintgpt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `osintgpt-0.1.0/osintgpt/vector_store/base.py` & `osintgpt-0.1.1/osintgpt/vector_store/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # =================================================================================
 # osintgpt
 #
 # Author: @estebanpdl
 #
 # File: base.py
-# Description: `BaseVectorEngine`` is an abstract base class that serves as a common
+# Description: `BaseVectorEngine` is an abstract base class that serves as a common
 #   interface for different vector search engine implementations.
 # =================================================================================
 
 # import submodules
 from abc import ABC, abstractmethod
 
 # type hints
```

### Comparing `osintgpt-0.1.0/osintgpt/vector_store/qdrant.py` & `osintgpt-0.1.1/osintgpt/vector_store/qdrant.py`

 * *Files identical despite different names*

### Comparing `osintgpt-0.1.0/osintgpt.egg-info/SOURCES.txt` & `osintgpt-0.1.1/osintgpt.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 README.md
 setup.py
 osintgpt/__init__.py
 osintgpt.egg-info/PKG-INFO
 osintgpt.egg-info/SOURCES.txt
 osintgpt.egg-info/dependency_links.txt
+osintgpt.egg-info/requires.txt
 osintgpt.egg-info/top_level.txt
 osintgpt/databases/__init__.py
 osintgpt/databases/sql_manager.py
 osintgpt/embeddings/__init__.py
 osintgpt/embeddings/openai_embeddings.py
 osintgpt/exceptions/__init__.py
 osintgpt/exceptions/errors.py
-osintgpt/gpt/__init__.py
-osintgpt/gpt/openai_gpt.py
+osintgpt/llms/__init__.py
+osintgpt/llms/openai_gpt.py
+osintgpt/semantic_operations/__init__.py
+osintgpt/semantic_operations/operations.py
 osintgpt/utils/__init__.py
 osintgpt/vector_store/__init__.py
 osintgpt/vector_store/base.py
 osintgpt/vector_store/qdrant.py
```

### Comparing `osintgpt-0.1.0/setup.py` & `osintgpt-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # install requires > read requirements.txt
 with open('./requirements.txt', 'r', encoding='utf-8') as f:
     install_requires = f.read().splitlines()
 
 # setup package
 setup(
     name='osintgpt',
-    version='0.1.0',
+    version='0.1.1',
     author='Esteban Ponce de Leon',
     description='A Python OSINT tool using Large Language Models',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/estebanpdl/osintgpt',
     packages=find_packages(),
     classifiers=[
@@ -36,9 +36,9 @@
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Text Processing',
         'Topic :: Text Processing :: General',
         'Topic :: Text Processing :: Indexing',
         'Topic :: Utilities'
     ],
     python_requires='>=3.7',
-    install_requires=[]
+    install_requires=install_requires
 )
```

