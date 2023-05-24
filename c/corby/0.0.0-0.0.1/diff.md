# Comparing `tmp/corby-0.0.0.tar.gz` & `tmp/corby-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corby-0.0.0.tar", last modified: Wed May 24 14:55:58 2023, max compression
+gzip compressed data, was "corby-0.0.1.tar", last modified: Wed May 24 15:03:11 2023, max compression
```

## Comparing `corby-0.0.0.tar` & `corby-0.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 14:55:58.978234 corby-0.0.0/
--rw-r--r--   0 ji.hervas   (504) staff       (20)      253 2023-05-24 14:55:58.977460 corby-0.0.0/PKG-INFO
--rw-r--r--   0 ji.hervas   (504) staff       (20)        9 2023-05-24 14:54:54.000000 corby-0.0.0/README.md
-drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 14:55:58.962828 corby-0.0.0/corby/
--rw-r--r--   0 ji.hervas   (504) staff       (20)      203 2023-05-24 11:56:23.000000 corby-0.0.0/corby/__init__.py
-drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 14:55:58.970130 corby-0.0.0/corby/generator/
--rw-r--r--   0 ji.hervas   (504) staff       (20)      180 2023-05-24 14:39:56.000000 corby-0.0.0/corby/generator/__init__.py
-drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 14:55:58.973321 corby-0.0.0/corby/generator/chatbot/
--rw-r--r--   0 ji.hervas   (504) staff       (20)      180 2023-05-24 14:39:59.000000 corby-0.0.0/corby/generator/chatbot/__init__.py
--rw-r--r--   0 ji.hervas   (504) staff       (20)     2028 2023-05-24 14:28:51.000000 corby-0.0.0/corby/generator/chatbot/cli.py
--rw-r--r--   0 ji.hervas   (504) staff       (20)      392 2023-05-24 13:28:19.000000 corby-0.0.0/corby/generator/chatbot/index.py
--rw-r--r--   0 ji.hervas   (504) staff       (20)     1175 2023-05-24 14:54:10.000000 corby-0.0.0/corby/index.py
-drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 14:55:58.969298 corby-0.0.0/corby.egg-info/
--rw-r--r--   0 ji.hervas   (504) staff       (20)      253 2023-05-24 14:55:58.000000 corby-0.0.0/corby.egg-info/PKG-INFO
--rw-r--r--   0 ji.hervas   (504) staff       (20)      323 2023-05-24 14:55:58.000000 corby-0.0.0/corby.egg-info/SOURCES.txt
--rw-r--r--   0 ji.hervas   (504) staff       (20)        1 2023-05-24 14:55:58.000000 corby-0.0.0/corby.egg-info/dependency_links.txt
--rw-r--r--   0 ji.hervas   (504) staff       (20)       26 2023-05-24 14:55:58.000000 corby-0.0.0/corby.egg-info/requires.txt
--rw-r--r--   0 ji.hervas   (504) staff       (20)        6 2023-05-24 14:55:58.000000 corby-0.0.0/corby.egg-info/top_level.txt
--rw-r--r--   0 ji.hervas   (504) staff       (20)       38 2023-05-24 14:55:58.978465 corby-0.0.0/setup.cfg
--rw-r--r--   0 ji.hervas   (504) staff       (20)      518 2023-05-24 14:55:52.000000 corby-0.0.0/setup.py
+drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 15:03:11.516081 corby-0.0.1/
+-rw-r--r--   0 ji.hervas   (504) staff       (20)      253 2023-05-24 15:03:11.515740 corby-0.0.1/PKG-INFO
+-rw-r--r--   0 ji.hervas   (504) staff       (20)        9 2023-05-24 14:54:54.000000 corby-0.0.1/README.md
+drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 15:03:11.508992 corby-0.0.1/corby/
+-rw-r--r--   0 ji.hervas   (504) staff       (20)      267 2023-05-24 15:01:44.000000 corby-0.0.1/corby/__init__.py
+drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 15:03:11.512087 corby-0.0.1/corby/generator/
+-rw-r--r--   0 ji.hervas   (504) staff       (20)      180 2023-05-24 14:39:56.000000 corby-0.0.1/corby/generator/__init__.py
+drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 15:03:11.514828 corby-0.0.1/corby/generator/chatbot/
+-rw-r--r--   0 ji.hervas   (504) staff       (20)      180 2023-05-24 14:39:59.000000 corby-0.0.1/corby/generator/chatbot/__init__.py
+-rw-r--r--   0 ji.hervas   (504) staff       (20)     2028 2023-05-24 14:28:51.000000 corby-0.0.1/corby/generator/chatbot/cli.py
+-rw-r--r--   0 ji.hervas   (504) staff       (20)      392 2023-05-24 13:28:19.000000 corby-0.0.1/corby/generator/chatbot/index.py
+-rw-r--r--   0 ji.hervas   (504) staff       (20)     1175 2023-05-24 14:54:10.000000 corby-0.0.1/corby/index.py
+drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 15:03:11.511567 corby-0.0.1/corby.egg-info/
+-rw-r--r--   0 ji.hervas   (504) staff       (20)      253 2023-05-24 15:03:11.000000 corby-0.0.1/corby.egg-info/PKG-INFO
+-rw-r--r--   0 ji.hervas   (504) staff       (20)      323 2023-05-24 15:03:11.000000 corby-0.0.1/corby.egg-info/SOURCES.txt
+-rw-r--r--   0 ji.hervas   (504) staff       (20)        1 2023-05-24 15:03:11.000000 corby-0.0.1/corby.egg-info/dependency_links.txt
+-rw-r--r--   0 ji.hervas   (504) staff       (20)       26 2023-05-24 15:03:11.000000 corby-0.0.1/corby.egg-info/requires.txt
+-rw-r--r--   0 ji.hervas   (504) staff       (20)        6 2023-05-24 15:03:11.000000 corby-0.0.1/corby.egg-info/top_level.txt
+-rw-r--r--   0 ji.hervas   (504) staff       (20)       38 2023-05-24 15:03:11.516201 corby-0.0.1/setup.cfg
+-rw-r--r--   0 ji.hervas   (504) staff       (20)      518 2023-05-24 15:03:07.000000 corby-0.0.1/setup.py
```

### Comparing `corby-0.0.0/corby/generator/chatbot/cli.py` & `corby-0.0.1/corby/generator/chatbot/cli.py`

 * *Files identical despite different names*

### Comparing `corby-0.0.0/corby/index.py` & `corby-0.0.1/corby/index.py`

 * *Files identical despite different names*

### Comparing `corby-0.0.0/setup.py` & `corby-0.0.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 python_requires='>=3.6',
 
 setup(
     name="corby",
-    version="0.0.0",
+    version="0.0.1",
     description="⚡ Create your LLMs applications from zero to deploy in minutes ⚡",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Jose Hervás Díaz",
     author_email='jhervasdiaz@gmail.com',
     license='MIT',
     packages=find_packages(),
```

