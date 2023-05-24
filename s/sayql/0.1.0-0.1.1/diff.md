# Comparing `tmp/sayql-0.1.0.tar.gz` & `tmp/sayql-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sayql-0.1.0.tar", max compression
+gzip compressed data, was "sayql-0.1.1.tar", max compression
```

## Comparing `sayql-0.1.0.tar` & `sayql-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-05-24 19:48:38.138391 sayql-0.1.0/LICENSE
--rw-r--r--   0        0        0      349 2023-05-24 19:50:34.916216 sayql-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 19:52:34.513666 sayql-0.1.0/sayql/__init__.py
--rw-r--r--   0        0        0      619 2023-05-24 19:52:37.355225 sayql-0.1.0/setup.py
--rw-r--r--   0        0        0      399 2023-05-24 19:52:37.355374 sayql-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-24 19:48:38.138391 sayql-0.1.1/LICENSE
+-rw-r--r--   0        0        0      391 2023-05-24 21:11:48.989846 sayql-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-05-24 21:05:56.491898 sayql-0.1.1/sayql/__init__.py
+-rw-r--r--   0        0        0      734 2023-05-24 20:51:26.879684 sayql-0.1.1/sayql/prompt.py
+-rw-r--r--   0        0        0     1374 2023-05-24 21:09:39.652773 sayql-0.1.1/sayql/sayql.py
+-rw-r--r--   0        0        0      679 2023-05-24 21:12:15.707109 sayql-0.1.1/setup.py
+-rw-r--r--   0        0        0      486 2023-05-24 21:12:15.707290 sayql-0.1.1/PKG-INFO
```

### Comparing `sayql-0.1.0/LICENSE` & `sayql-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sayql-0.1.0/setup.py` & `sayql-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 packages = \
 ['sayql']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['duckdb>=0.8.0,<0.9.0', 'pandas>=2.0.1,<3.0.0']
+['duckdb>=0.8.0,<0.9.0',
+ 'langchain>=0.0.179,<0.0.180',
+ 'openai>=0.27.7,<0.28.0',
+ 'pandas>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'sayql',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Talk to your data',
     'long_description': None,
     'author': 'Ryan',
     'author_email': 'ryan.sudhakaran@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

