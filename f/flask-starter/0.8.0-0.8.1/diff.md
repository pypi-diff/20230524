# Comparing `tmp/flask-starter-0.8.0.tar.gz` & `tmp/flask-starter-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-starter-0.8.0.tar", last modified: Wed May 24 13:52:50 2023, max compression
+gzip compressed data, was "flask-starter-0.8.1.tar", last modified: Wed May 24 14:19:28 2023, max compression
```

## Comparing `flask-starter-0.8.0.tar` & `flask-starter-0.8.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 proshan   (1003) proshan   (1003)        0 2023-05-24 13:52:50.537366 flask-starter-0.8.0/
--rw-rw-r--   0 proshan   (1003) proshan   (1003)     1070 2023-05-24 13:35:35.000000 flask-starter-0.8.0/LICENSE
--rw-rw-r--   0 proshan   (1003) proshan   (1003)     2360 2023-05-24 13:52:50.537366 flask-starter-0.8.0/PKG-INFO
--rw-rw-r--   0 proshan   (1003) proshan   (1003)     1718 2023-05-24 13:52:03.000000 flask-starter-0.8.0/README.rst
-drwxrwxr-x   0 proshan   (1003) proshan   (1003)        0 2023-05-24 13:52:50.537366 flask-starter-0.8.0/flask_starter.egg-info/
--rw-rw-r--   0 proshan   (1003) proshan   (1003)     2360 2023-05-24 13:52:50.000000 flask-starter-0.8.0/flask_starter.egg-info/PKG-INFO
--rw-rw-r--   0 proshan   (1003) proshan   (1003)      300 2023-05-24 13:52:50.000000 flask-starter-0.8.0/flask_starter.egg-info/SOURCES.txt
--rw-rw-r--   0 proshan   (1003) proshan   (1003)        1 2023-05-24 13:52:50.000000 flask-starter-0.8.0/flask_starter.egg-info/dependency_links.txt
--rw-rw-r--   0 proshan   (1003) proshan   (1003)       54 2023-05-24 13:52:50.000000 flask-starter-0.8.0/flask_starter.egg-info/entry_points.txt
--rw-rw-r--   0 proshan   (1003) proshan   (1003)       30 2023-05-24 13:52:50.000000 flask-starter-0.8.0/flask_starter.egg-info/requires.txt
--rw-rw-r--   0 proshan   (1003) proshan   (1003)        7 2023-05-24 13:52:50.000000 flask-starter-0.8.0/flask_starter.egg-info/top_level.txt
--rw-rw-r--   0 proshan   (1003) proshan   (1003)      943 2023-05-24 13:46:32.000000 flask-starter-0.8.0/script.py
--rw-rw-r--   0 proshan   (1003) proshan   (1003)       38 2023-05-24 13:52:50.537366 flask-starter-0.8.0/setup.cfg
--rw-rw-r--   0 proshan   (1003) proshan   (1003)     1055 2023-05-24 13:52:41.000000 flask-starter-0.8.0/setup.py
-drwxrwxr-x   0 proshan   (1003) proshan   (1003)        0 2023-05-24 13:52:50.537366 flask-starter-0.8.0/tests/
--rw-rw-r--   0 proshan   (1003) proshan   (1003)        0 2023-05-24 13:35:35.000000 flask-starter-0.8.0/tests/test_libs.py
--rw-rw-r--   0 proshan   (1003) proshan   (1003)      342 2023-05-24 13:35:35.000000 flask-starter-0.8.0/tests/test_views.py
+drwxr-xr-x   0 agent-hellboy   (501) staff       (20)        0 2023-05-24 14:19:28.995137 flask-starter-0.8.1/
+-rw-r--r--   0 agent-hellboy   (501) staff       (20)     1070 2023-05-24 14:17:07.000000 flask-starter-0.8.1/LICENSE
+-rw-r--r--   0 agent-hellboy   (501) staff       (20)     2360 2023-05-24 14:19:28.995042 flask-starter-0.8.1/PKG-INFO
+-rw-r--r--   0 agent-hellboy   (501) staff       (20)     1718 2023-05-24 14:17:07.000000 flask-starter-0.8.1/README.rst
+drwxr-xr-x   0 agent-hellboy   (501) staff       (20)        0 2023-05-24 14:19:28.994711 flask-starter-0.8.1/flask_starter.egg-info/
+-rw-r--r--   0 agent-hellboy   (501) staff       (20)     2360 2023-05-24 14:19:28.000000 flask-starter-0.8.1/flask_starter.egg-info/PKG-INFO
+-rw-r--r--   0 agent-hellboy   (501) staff       (20)      300 2023-05-24 14:19:28.000000 flask-starter-0.8.1/flask_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 agent-hellboy   (501) staff       (20)        1 2023-05-24 14:19:28.000000 flask-starter-0.8.1/flask_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 agent-hellboy   (501) staff       (20)       54 2023-05-24 14:19:28.000000 flask-starter-0.8.1/flask_starter.egg-info/entry_points.txt
+-rw-r--r--   0 agent-hellboy   (501) staff       (20)       30 2023-05-24 14:19:28.000000 flask-starter-0.8.1/flask_starter.egg-info/requires.txt
+-rw-r--r--   0 agent-hellboy   (501) staff       (20)        7 2023-05-24 14:19:28.000000 flask-starter-0.8.1/flask_starter.egg-info/top_level.txt
+-rw-r--r--   0 agent-hellboy   (501) staff       (20)     1772 2023-05-24 14:17:07.000000 flask-starter-0.8.1/script.py
+-rw-r--r--   0 agent-hellboy   (501) staff       (20)       38 2023-05-24 14:19:28.995167 flask-starter-0.8.1/setup.cfg
+-rw-r--r--   0 agent-hellboy   (501) staff       (20)     1055 2023-05-24 14:17:07.000000 flask-starter-0.8.1/setup.py
+drwxr-xr-x   0 agent-hellboy   (501) staff       (20)        0 2023-05-24 14:19:28.994904 flask-starter-0.8.1/tests/
+-rw-r--r--   0 agent-hellboy   (501) staff       (20)        0 2023-05-24 14:17:07.000000 flask-starter-0.8.1/tests/test_libs.py
+-rw-r--r--   0 agent-hellboy   (501) staff       (20)      342 2023-05-24 14:17:07.000000 flask-starter-0.8.1/tests/test_views.py
```

### Comparing `flask-starter-0.8.0/LICENSE` & `flask-starter-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-starter-0.8.0/PKG-INFO` & `flask-starter-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-starter
-Version: 0.8.0
+Version: 0.8.1
 Summary: A flask extension which contains a basic app and is configured in your local machine through a command line utility 
 Home-page: https://github.com/princekrroshan01/flask-starter
 Author: Prince Roshan
 Author-email: princekrroshan01@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flask-starter-0.8.0/README.rst` & `flask-starter-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `flask-starter-0.8.0/flask_starter.egg-info/PKG-INFO` & `flask-starter-0.8.1/flask_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-starter
-Version: 0.8.0
+Version: 0.8.1
 Summary: A flask extension which contains a basic app and is configured in your local machine through a command line utility 
 Home-page: https://github.com/princekrroshan01/flask-starter
 Author: Prince Roshan
 Author-email: princekrroshan01@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flask-starter-0.8.0/setup.py` & `flask-starter-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="flask-starter",
-    version="0.8.0",
+    version="0.8.1",
     author="Prince Roshan",
     author_email="princekrroshan01@gmail.com",
     url="https://github.com/princekrroshan01/flask-starter",
     description=(
         "A flask extension which contains a basic app and is configured in your local machine through a command line utility "
     ),
     long_description=read("README.rst"),
```

