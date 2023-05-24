# Comparing `tmp/std_daq_client-1.0.0.tar.gz` & `tmp/std_daq_client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "std_daq_client-1.0.0.tar", last modified: Wed May 24 09:48:22 2023, max compression
+gzip compressed data, was "std_daq_client-1.0.1.tar", last modified: Wed May 24 09:52:22 2023, max compression
```

## Comparing `std_daq_client-1.0.0.tar` & `std_daq_client-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-24 09:48:22.553039 std_daq_client-1.0.0/
--rw-r--r--   0 babic_a    (501) staff       (20)      393 2023-05-24 09:48:22.552543 std_daq_client-1.0.0/PKG-INFO
--rw-r--r--   0 babic_a    (501) staff       (20)    11059 2023-05-12 12:51:12.000000 std_daq_client-1.0.0/README.md
--rw-r--r--   0 babic_a    (501) staff       (20)       38 2023-05-24 09:48:22.553182 std_daq_client-1.0.0/setup.cfg
--rw-r--r--   0 babic_a    (501) staff       (20)     1317 2023-05-16 08:33:36.000000 std_daq_client-1.0.0/setup.py
--rw-r--r--   0 babic_a    (501) staff       (20)     1007 2023-05-24 09:48:17.000000 std_daq_client-1.0.0/setup_client.py
-drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-24 09:48:22.547326 std_daq_client-1.0.0/std_daq_client/
--rw-r--r--   0 babic_a    (501) staff       (20)       68 2023-05-24 09:15:21.000000 std_daq_client-1.0.0/std_daq_client/__init__.py
--rw-r--r--   0 babic_a    (501) staff       (20)     2344 2023-05-24 09:15:21.000000 std_daq_client-1.0.0/std_daq_client/client.py
-drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-24 09:48:22.551947 std_daq_client-1.0.0/std_daq_client.egg-info/
--rw-r--r--   0 babic_a    (501) staff       (20)      393 2023-05-24 09:48:22.000000 std_daq_client-1.0.0/std_daq_client.egg-info/PKG-INFO
--rw-r--r--   0 babic_a    (501) staff       (20)      316 2023-05-24 09:48:22.000000 std_daq_client-1.0.0/std_daq_client.egg-info/SOURCES.txt
--rw-r--r--   0 babic_a    (501) staff       (20)        1 2023-05-24 09:48:22.000000 std_daq_client-1.0.0/std_daq_client.egg-info/dependency_links.txt
--rw-r--r--   0 babic_a    (501) staff       (20)      306 2023-05-24 09:48:22.000000 std_daq_client-1.0.0/std_daq_client.egg-info/entry_points.txt
--rw-r--r--   0 babic_a    (501) staff       (20)        9 2023-05-24 09:48:22.000000 std_daq_client-1.0.0/std_daq_client.egg-info/requires.txt
--rw-r--r--   0 babic_a    (501) staff       (20)       15 2023-05-24 09:48:22.000000 std_daq_client-1.0.0/std_daq_client.egg-info/top_level.txt
+drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-24 09:52:22.276363 std_daq_client-1.0.1/
+-rw-r--r--   0 babic_a    (501) staff       (20)      359 2023-05-24 09:52:22.275697 std_daq_client-1.0.1/PKG-INFO
+-rw-r--r--   0 babic_a    (501) staff       (20)    11059 2023-05-12 12:51:12.000000 std_daq_client-1.0.1/README.md
+-rw-r--r--   0 babic_a    (501) staff       (20)       38 2023-05-24 09:52:22.276503 std_daq_client-1.0.1/setup.cfg
+-rw-r--r--   0 babic_a    (501) staff       (20)     1317 2023-05-16 08:33:36.000000 std_daq_client-1.0.1/setup.py
+-rw-r--r--   0 babic_a    (501) staff       (20)     1003 2023-05-24 09:52:05.000000 std_daq_client-1.0.1/setup_client.py
+drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-24 09:52:22.267372 std_daq_client-1.0.1/std_daq_client/
+-rw-r--r--   0 babic_a    (501) staff       (20)       68 2023-05-24 09:15:21.000000 std_daq_client-1.0.1/std_daq_client/__init__.py
+drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-24 09:52:22.274855 std_daq_client-1.0.1/std_daq_client/cli/
+-rw-r--r--   0 babic_a    (501) staff       (20)        0 2023-05-24 09:17:15.000000 std_daq_client-1.0.1/std_daq_client/cli/__init__.py
+-rw-r--r--   0 babic_a    (501) staff       (20)      414 2023-05-24 09:28:27.000000 std_daq_client-1.0.1/std_daq_client/cli/get_config.py
+-rw-r--r--   0 babic_a    (501) staff       (20)      436 2023-05-24 09:29:27.000000 std_daq_client-1.0.1/std_daq_client/cli/get_deploy_status.py
+-rw-r--r--   0 babic_a    (501) staff       (20)      516 2023-05-24 09:30:26.000000 std_daq_client-1.0.1/std_daq_client/cli/get_logs.py
+-rw-r--r--   0 babic_a    (501) staff       (20)      412 2023-05-24 09:28:47.000000 std_daq_client-1.0.1/std_daq_client/cli/get_stats.py
+-rw-r--r--   0 babic_a    (501) staff       (20)      414 2023-05-24 09:28:02.000000 std_daq_client-1.0.1/std_daq_client/cli/get_status.py
+-rw-r--r--   0 babic_a    (501) staff       (20)     2344 2023-05-24 09:15:21.000000 std_daq_client-1.0.1/std_daq_client/client.py
+drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-24 09:52:22.270677 std_daq_client-1.0.1/std_daq_client.egg-info/
+-rw-r--r--   0 babic_a    (501) staff       (20)      359 2023-05-24 09:52:22.000000 std_daq_client-1.0.1/std_daq_client.egg-info/PKG-INFO
+-rw-r--r--   0 babic_a    (501) staff       (20)      516 2023-05-24 09:52:22.000000 std_daq_client-1.0.1/std_daq_client.egg-info/SOURCES.txt
+-rw-r--r--   0 babic_a    (501) staff       (20)        1 2023-05-24 09:52:22.000000 std_daq_client-1.0.1/std_daq_client.egg-info/dependency_links.txt
+-rw-r--r--   0 babic_a    (501) staff       (20)      306 2023-05-24 09:52:22.000000 std_daq_client-1.0.1/std_daq_client.egg-info/entry_points.txt
+-rw-r--r--   0 babic_a    (501) staff       (20)        9 2023-05-24 09:52:22.000000 std_daq_client-1.0.1/std_daq_client.egg-info/requires.txt
+-rw-r--r--   0 babic_a    (501) staff       (20)       15 2023-05-24 09:52:22.000000 std_daq_client-1.0.1/std_daq_client.egg-info/top_level.txt
```

### Comparing `std_daq_client-1.0.0/README.md` & `std_daq_client-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `std_daq_client-1.0.0/setup.py` & `std_daq_client-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `std_daq_client-1.0.0/setup_client.py` & `std_daq_client-1.0.1/setup_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import os
 
 from setuptools import setup
 
-CLIENT_VERSION = "1.0.0"
+CLIENT_VERSION = "1.0.1"
 
 with open(os.path.join(os.path.dirname(__file__), 'std_daq_client/', 'README.md')) as readme:
     long_description = readme.read()
 
 setup(
     version=CLIENT_VERSION,
     name='std_daq_client',
-    packages=['std_daq_client'],
+    packages=['std_daq_client',
+              'std_daq_client.cli'],
     install_requires=[
         'requests',
     ],
     entry_points='''
         [console_scripts]
         std_cli_get_config=std_daq_client.cli.get_config:main
         std_cli_get_deploy_status=std_daq_client.cli.get_deploy_status:main
         std_cli_get_logs=std_daq_client.cli.get_logs:main
         std_cli_get_stats=std_daq_client.cli.get_stats:main
         std_cli_get_status=std_daq_client.cli.get_status:main
     ''',
 
     author="Paul Scherrer Institute",
-    author_email='andrej.babic@psi.ch',
     url='https://github.com/paulscherrerinstitute/std_daq_service',
     description='Python client for standard-daq',
     long_description=long_description,
     long_description_content_type='text/markdown',
 )
```

### Comparing `std_daq_client-1.0.0/std_daq_client/client.py` & `std_daq_client-1.0.1/std_daq_client/client.py`

 * *Files identical despite different names*

