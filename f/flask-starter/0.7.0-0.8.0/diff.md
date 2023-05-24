# Comparing `tmp/flask-starter-0.7.0.tar.gz` & `tmp/flask-starter-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-starter-0.7.0.tar", last modified: Wed May 24 13:50:28 2023, max compression
+gzip compressed data, was "flask-starter-0.8.0.tar", last modified: Wed May 24 13:52:50 2023, max compression
```

## Comparing `flask-starter-0.7.0.tar` & `flask-starter-0.8.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 proshan   (1003) proshan   (1003)        0 2023-05-24 13:50:28.613422 flask-starter-0.7.0/
--rw-rw-r--   0 proshan   (1003) proshan   (1003)     1070 2023-05-24 13:35:35.000000 flask-starter-0.7.0/LICENSE
--rw-rw-r--   0 proshan   (1003) proshan   (1003)     2353 2023-05-24 13:50:28.613422 flask-starter-0.7.0/PKG-INFO
--rw-rw-r--   0 proshan   (1003) proshan   (1003)     1711 2023-05-24 13:35:35.000000 flask-starter-0.7.0/README.rst
-drwxrwxr-x   0 proshan   (1003) proshan   (1003)        0 2023-05-24 13:50:28.613422 flask-starter-0.7.0/flask_starter.egg-info/
--rw-rw-r--   0 proshan   (1003) proshan   (1003)     2353 2023-05-24 13:50:28.000000 flask-starter-0.7.0/flask_starter.egg-info/PKG-INFO
--rw-rw-r--   0 proshan   (1003) proshan   (1003)      300 2023-05-24 13:50:28.000000 flask-starter-0.7.0/flask_starter.egg-info/SOURCES.txt
--rw-rw-r--   0 proshan   (1003) proshan   (1003)        1 2023-05-24 13:50:28.000000 flask-starter-0.7.0/flask_starter.egg-info/dependency_links.txt
--rw-rw-r--   0 proshan   (1003) proshan   (1003)       54 2023-05-24 13:50:28.000000 flask-starter-0.7.0/flask_starter.egg-info/entry_points.txt
--rw-rw-r--   0 proshan   (1003) proshan   (1003)       30 2023-05-24 13:50:28.000000 flask-starter-0.7.0/flask_starter.egg-info/requires.txt
--rw-rw-r--   0 proshan   (1003) proshan   (1003)        7 2023-05-24 13:50:28.000000 flask-starter-0.7.0/flask_starter.egg-info/top_level.txt
--rw-rw-r--   0 proshan   (1003) proshan   (1003)      943 2023-05-24 13:46:32.000000 flask-starter-0.7.0/script.py
--rw-rw-r--   0 proshan   (1003) proshan   (1003)       38 2023-05-24 13:50:28.613422 flask-starter-0.7.0/setup.cfg
--rw-rw-r--   0 proshan   (1003) proshan   (1003)     1055 2023-05-24 13:48:47.000000 flask-starter-0.7.0/setup.py
-drwxrwxr-x   0 proshan   (1003) proshan   (1003)        0 2023-05-24 13:50:28.613422 flask-starter-0.7.0/tests/
--rw-rw-r--   0 proshan   (1003) proshan   (1003)        0 2023-05-24 13:35:35.000000 flask-starter-0.7.0/tests/test_libs.py
--rw-rw-r--   0 proshan   (1003) proshan   (1003)      342 2023-05-24 13:35:35.000000 flask-starter-0.7.0/tests/test_views.py
+drwxrwxr-x   0 proshan   (1003) proshan   (1003)        0 2023-05-24 13:52:50.537366 flask-starter-0.8.0/
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)     1070 2023-05-24 13:35:35.000000 flask-starter-0.8.0/LICENSE
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)     2360 2023-05-24 13:52:50.537366 flask-starter-0.8.0/PKG-INFO
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)     1718 2023-05-24 13:52:03.000000 flask-starter-0.8.0/README.rst
+drwxrwxr-x   0 proshan   (1003) proshan   (1003)        0 2023-05-24 13:52:50.537366 flask-starter-0.8.0/flask_starter.egg-info/
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)     2360 2023-05-24 13:52:50.000000 flask-starter-0.8.0/flask_starter.egg-info/PKG-INFO
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)      300 2023-05-24 13:52:50.000000 flask-starter-0.8.0/flask_starter.egg-info/SOURCES.txt
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)        1 2023-05-24 13:52:50.000000 flask-starter-0.8.0/flask_starter.egg-info/dependency_links.txt
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)       54 2023-05-24 13:52:50.000000 flask-starter-0.8.0/flask_starter.egg-info/entry_points.txt
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)       30 2023-05-24 13:52:50.000000 flask-starter-0.8.0/flask_starter.egg-info/requires.txt
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)        7 2023-05-24 13:52:50.000000 flask-starter-0.8.0/flask_starter.egg-info/top_level.txt
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)      943 2023-05-24 13:46:32.000000 flask-starter-0.8.0/script.py
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)       38 2023-05-24 13:52:50.537366 flask-starter-0.8.0/setup.cfg
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)     1055 2023-05-24 13:52:41.000000 flask-starter-0.8.0/setup.py
+drwxrwxr-x   0 proshan   (1003) proshan   (1003)        0 2023-05-24 13:52:50.537366 flask-starter-0.8.0/tests/
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)        0 2023-05-24 13:35:35.000000 flask-starter-0.8.0/tests/test_libs.py
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)      342 2023-05-24 13:35:35.000000 flask-starter-0.8.0/tests/test_views.py
```

### Comparing `flask-starter-0.7.0/LICENSE` & `flask-starter-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-starter-0.7.0/PKG-INFO` & `flask-starter-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-starter
-Version: 0.7.0
+Version: 0.8.0
 Summary: A flask extension which contains a basic app and is configured in your local machine through a command line utility 
 Home-page: https://github.com/princekrroshan01/flask-starter
 Author: Prince Roshan
 Author-email: princekrroshan01@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -51,15 +51,15 @@
        - pip install git+https://github.com/Agent-Hellboy/flask-starter.git
 	      
 
 using
 ------
 
 open the terminal and type 
-```flask-starter-project your-project-name``` this will build a basic project with inbuilt auth and admin interface for you
+```flask-starter-project --name=your-project-name``` this will build a basic project with inbuilt auth and admin interface for you
 
 you can access admin interface by adding `/admin` in your base url 
 
 just write core logic in libs and present your prototype
 
 
 Contributing
```

### Comparing `flask-starter-0.7.0/README.rst` & `flask-starter-0.8.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
        - pip install git+https://github.com/Agent-Hellboy/flask-starter.git
 	      
 
 using
 ------
 
 open the terminal and type 
-```flask-starter-project your-project-name``` this will build a basic project with inbuilt auth and admin interface for you
+```flask-starter-project --name=your-project-name``` this will build a basic project with inbuilt auth and admin interface for you
 
 you can access admin interface by adding `/admin` in your base url 
 
 just write core logic in libs and present your prototype
 
 
 Contributing
```

### Comparing `flask-starter-0.7.0/flask_starter.egg-info/PKG-INFO` & `flask-starter-0.8.0/flask_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-starter
-Version: 0.7.0
+Version: 0.8.0
 Summary: A flask extension which contains a basic app and is configured in your local machine through a command line utility 
 Home-page: https://github.com/princekrroshan01/flask-starter
 Author: Prince Roshan
 Author-email: princekrroshan01@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -51,15 +51,15 @@
        - pip install git+https://github.com/Agent-Hellboy/flask-starter.git
 	      
 
 using
 ------
 
 open the terminal and type 
-```flask-starter-project your-project-name``` this will build a basic project with inbuilt auth and admin interface for you
+```flask-starter-project --name=your-project-name``` this will build a basic project with inbuilt auth and admin interface for you
 
 you can access admin interface by adding `/admin` in your base url 
 
 just write core logic in libs and present your prototype
 
 
 Contributing
```

### Comparing `flask-starter-0.7.0/script.py` & `flask-starter-0.8.0/script.py`

 * *Files identical despite different names*

### Comparing `flask-starter-0.7.0/setup.py` & `flask-starter-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="flask-starter",
-    version="0.7.0",
+    version="0.8.0",
     author="Prince Roshan",
     author_email="princekrroshan01@gmail.com",
     url="https://github.com/princekrroshan01/flask-starter",
     description=(
         "A flask extension which contains a basic app and is configured in your local machine through a command line utility "
     ),
     long_description=read("README.rst"),
```

