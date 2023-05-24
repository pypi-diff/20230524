# Comparing `tmp/corby-0.0.5.tar.gz` & `tmp/corby-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corby-0.0.5.tar", last modified: Wed May 24 15:20:10 2023, max compression
+gzip compressed data, was "corby-0.0.6.tar", last modified: Wed May 24 15:21:55 2023, max compression
```

## Comparing `corby-0.0.5.tar` & `corby-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 15:20:10.276769 corby-0.0.5/
--rw-r--r--   0 ji.hervas   (504) staff       (20)      253 2023-05-24 15:20:10.276335 corby-0.0.5/PKG-INFO
--rw-r--r--   0 ji.hervas   (504) staff       (20)        9 2023-05-24 14:54:54.000000 corby-0.0.5/README.md
-drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 15:20:10.269858 corby-0.0.5/corby/
--rw-r--r--   0 ji.hervas   (504) staff       (20)      244 2023-05-24 15:19:34.000000 corby-0.0.5/corby/__init__.py
-drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 15:20:10.273206 corby-0.0.5/corby/generator/
--rw-r--r--   0 ji.hervas   (504) staff       (20)      180 2023-05-24 14:39:56.000000 corby-0.0.5/corby/generator/__init__.py
-drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 15:20:10.275640 corby-0.0.5/corby/generator/chatbot/
--rw-r--r--   0 ji.hervas   (504) staff       (20)      180 2023-05-24 14:39:59.000000 corby-0.0.5/corby/generator/chatbot/__init__.py
--rw-r--r--   0 ji.hervas   (504) staff       (20)     2028 2023-05-24 14:28:51.000000 corby-0.0.5/corby/generator/chatbot/cli.py
--rw-r--r--   0 ji.hervas   (504) staff       (20)      392 2023-05-24 13:28:19.000000 corby-0.0.5/corby/generator/chatbot/index.py
--rw-r--r--   0 ji.hervas   (504) staff       (20)     1203 2023-05-24 15:18:03.000000 corby-0.0.5/corby/index.py
-drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 15:20:10.272699 corby-0.0.5/corby.egg-info/
--rw-r--r--   0 ji.hervas   (504) staff       (20)      253 2023-05-24 15:20:10.000000 corby-0.0.5/corby.egg-info/PKG-INFO
--rw-r--r--   0 ji.hervas   (504) staff       (20)      323 2023-05-24 15:20:10.000000 corby-0.0.5/corby.egg-info/SOURCES.txt
--rw-r--r--   0 ji.hervas   (504) staff       (20)        1 2023-05-24 15:20:10.000000 corby-0.0.5/corby.egg-info/dependency_links.txt
--rw-r--r--   0 ji.hervas   (504) staff       (20)       26 2023-05-24 15:20:10.000000 corby-0.0.5/corby.egg-info/requires.txt
--rw-r--r--   0 ji.hervas   (504) staff       (20)        6 2023-05-24 15:20:10.000000 corby-0.0.5/corby.egg-info/top_level.txt
--rw-r--r--   0 ji.hervas   (504) staff       (20)       38 2023-05-24 15:20:10.276937 corby-0.0.5/setup.cfg
--rw-r--r--   0 ji.hervas   (504) staff       (20)      518 2023-05-24 15:20:02.000000 corby-0.0.5/setup.py
+drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 15:21:55.135316 corby-0.0.6/
+-rw-r--r--   0 ji.hervas   (504) staff       (20)      253 2023-05-24 15:21:55.132611 corby-0.0.6/PKG-INFO
+-rw-r--r--   0 ji.hervas   (504) staff       (20)        9 2023-05-24 14:54:54.000000 corby-0.0.6/README.md
+drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 15:21:55.116561 corby-0.0.6/corby/
+-rw-r--r--   0 ji.hervas   (504) staff       (20)      244 2023-05-24 15:21:28.000000 corby-0.0.6/corby/__init__.py
+drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 15:21:55.125714 corby-0.0.6/corby/generator/
+-rw-r--r--   0 ji.hervas   (504) staff       (20)      180 2023-05-24 14:39:56.000000 corby-0.0.6/corby/generator/__init__.py
+drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 15:21:55.130653 corby-0.0.6/corby/generator/chatbot/
+-rw-r--r--   0 ji.hervas   (504) staff       (20)      180 2023-05-24 14:39:59.000000 corby-0.0.6/corby/generator/chatbot/__init__.py
+-rw-r--r--   0 ji.hervas   (504) staff       (20)     2028 2023-05-24 14:28:51.000000 corby-0.0.6/corby/generator/chatbot/cli.py
+-rw-r--r--   0 ji.hervas   (504) staff       (20)      392 2023-05-24 13:28:19.000000 corby-0.0.6/corby/generator/chatbot/index.py
+-rw-r--r--   0 ji.hervas   (504) staff       (20)     1186 2023-05-24 15:21:48.000000 corby-0.0.6/corby/index.py
+drwxr-xr-x   0 ji.hervas   (504) staff       (20)        0 2023-05-24 15:21:55.125030 corby-0.0.6/corby.egg-info/
+-rw-r--r--   0 ji.hervas   (504) staff       (20)      253 2023-05-24 15:21:55.000000 corby-0.0.6/corby.egg-info/PKG-INFO
+-rw-r--r--   0 ji.hervas   (504) staff       (20)      323 2023-05-24 15:21:55.000000 corby-0.0.6/corby.egg-info/SOURCES.txt
+-rw-r--r--   0 ji.hervas   (504) staff       (20)        1 2023-05-24 15:21:55.000000 corby-0.0.6/corby.egg-info/dependency_links.txt
+-rw-r--r--   0 ji.hervas   (504) staff       (20)       26 2023-05-24 15:21:55.000000 corby-0.0.6/corby.egg-info/requires.txt
+-rw-r--r--   0 ji.hervas   (504) staff       (20)        6 2023-05-24 15:21:55.000000 corby-0.0.6/corby.egg-info/top_level.txt
+-rw-r--r--   0 ji.hervas   (504) staff       (20)       38 2023-05-24 15:21:55.135774 corby-0.0.6/setup.cfg
+-rw-r--r--   0 ji.hervas   (504) staff       (20)      518 2023-05-24 15:21:51.000000 corby-0.0.6/setup.py
```

### Comparing `corby-0.0.5/corby/generator/chatbot/cli.py` & `corby-0.0.6/corby/generator/chatbot/cli.py`

 * *Files identical despite different names*

### Comparing `corby-0.0.5/corby/index.py` & `corby-0.0.6/corby/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 import argparse
 from string import Template
 from .generator.chatbot.index import create_chatbot
-from .__init__ import __version__
+
+__version__ = "0.0.6"
 
 # We'll include more features in the future
 available_actions = ['new']
 
 available_entities = ['chatbot', 'notebook']
 
 parser = argparse.ArgumentParser(
@@ -14,15 +15,15 @@
         available_actions=' | '.join(available_actions), 
         available_entities=' | '.join(available_entities)
     )
 )
 
 parser.add_argument('action', choices=available_actions, help='Action to perform')
 parser.add_argument('entity', choices=available_entities, help='Entity to work with')
-parser.add_argument('-v','--version', action='version', version=corby.__version__, help='Show version')
+parser.add_argument('-v','--version', action='version', version=__version__, help='Show version')
 parser.add_argument('-d', '--debug', action='store_true', help='Debug mode')
 args = parser.parse_args()
 
 def main():
     if args.action:
         if args.action == 'new':
             if args.entity == 'notebook':
```

### Comparing `corby-0.0.5/setup.py` & `corby-0.0.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 python_requires='>=3.6',
 
 setup(
     name="corby",
-    version="0.0.5",
+    version="0.0.6",
     description="⚡ Create your LLMs applications from zero to deploy in minutes ⚡",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Jose Hervás Díaz",
     author_email='jhervasdiaz@gmail.com',
     license='MIT',
     packages=find_packages(),
```

