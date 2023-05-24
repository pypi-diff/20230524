# Comparing `tmp/ts-python-client-2.0.3.tar.gz` & `tmp/ts-python-client-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts-python-client-2.0.3.tar", last modified: Wed May  3 16:31:53 2023, max compression
+gzip compressed data, was "ts-python-client-2.0.4.tar", last modified: Wed May 24 17:20:32 2023, max compression
```

## Comparing `ts-python-client-2.0.3.tar` & `ts-python-client-2.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-03 16:31:53.163692 ts-python-client-2.0.3/
--rw-r--r--   0 markin     (501) staff       (20)    11346 2020-11-12 11:29:27.000000 ts-python-client-2.0.3/LICENSE
--rw-rw----   0 markin     (501) staff       (20)      156 2017-03-24 15:47:43.000000 ts-python-client-2.0.3/MANIFEST.in
--rw-r--r--   0 markin     (501) staff       (20)      381 2023-05-03 16:31:53.163769 ts-python-client-2.0.3/PKG-INFO
--rw-r--r--   0 markin     (501) staff       (20)     1129 2022-04-03 12:51:16.000000 ts-python-client-2.0.3/README.md
--rw-rw----   0 markin     (501) staff       (20)       26 2017-03-20 16:02:56.000000 ts-python-client-2.0.3/_config.yml
--rw-rw----   0 markin     (501) staff       (20)       79 2023-05-03 16:31:53.164153 ts-python-client-2.0.3/setup.cfg
--rw-r--r--   0 markin     (501) staff       (20)      653 2023-05-03 15:27:25.000000 ts-python-client-2.0.3/setup.py
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-03 16:31:53.161221 ts-python-client-2.0.3/ts_python_client/
--rw-r--r--   0 markin     (501) staff       (20)       81 2023-04-03 13:46:33.000000 ts-python-client-2.0.3/ts_python_client/__init__.py
--rw-r--r--   0 markin     (501) staff       (20)     1314 2023-05-03 16:24:51.000000 ts-python-client-2.0.3/ts_python_client/cli.py
--rw-r--r--   0 markin     (501) staff       (20)     4228 2022-06-07 21:36:28.000000 ts-python-client-2.0.3/ts_python_client/client.py
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-03 16:31:53.163493 ts-python-client-2.0.3/ts_python_client/commands/
--rw-r--r--   0 markin     (501) staff       (20)     1403 2023-04-03 13:46:33.000000 ts-python-client-2.0.3/ts_python_client/commands/ScanCommand.py
--rw-r--r--   0 markin     (501) staff       (20)     2292 2023-04-03 13:46:33.000000 ts-python-client-2.0.3/ts_python_client/commands/UploadCommand.py
--rw-r--r--   0 markin     (501) staff       (20)      410 2023-04-03 13:46:33.000000 ts-python-client-2.0.3/ts_python_client/commands/__init__.py
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-03 16:31:53.162594 ts-python-client-2.0.3/ts_python_client.egg-info/
--rw-r--r--   0 markin     (501) staff       (20)      381 2023-05-03 16:31:53.000000 ts-python-client-2.0.3/ts_python_client.egg-info/PKG-INFO
--rw-r--r--   0 markin     (501) staff       (20)      461 2023-05-03 16:31:53.000000 ts-python-client-2.0.3/ts_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 markin     (501) staff       (20)        1 2023-05-03 16:31:53.000000 ts-python-client-2.0.3/ts_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 markin     (501) staff       (20)       22 2023-05-03 16:31:53.000000 ts-python-client-2.0.3/ts_python_client.egg-info/requires.txt
--rw-r--r--   0 markin     (501) staff       (20)       17 2023-05-03 16:31:53.000000 ts-python-client-2.0.3/ts_python_client.egg-info/top_level.txt
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 17:20:32.482006 ts-python-client-2.0.4/
+-rw-r--r--   0 markin     (501) staff       (20)    11346 2020-11-12 11:29:27.000000 ts-python-client-2.0.4/LICENSE
+-rw-rw----   0 markin     (501) staff       (20)      156 2017-03-24 15:47:43.000000 ts-python-client-2.0.4/MANIFEST.in
+-rw-r--r--   0 markin     (501) staff       (20)      381 2023-05-24 17:20:32.482128 ts-python-client-2.0.4/PKG-INFO
+-rw-r--r--   0 markin     (501) staff       (20)     1129 2022-04-03 12:51:16.000000 ts-python-client-2.0.4/README.md
+-rw-rw----   0 markin     (501) staff       (20)       26 2017-03-20 16:02:56.000000 ts-python-client-2.0.4/_config.yml
+-rw-rw----   0 markin     (501) staff       (20)       79 2023-05-24 17:20:32.482603 ts-python-client-2.0.4/setup.cfg
+-rw-r--r--   0 markin     (501) staff       (20)      653 2023-05-24 17:18:20.000000 ts-python-client-2.0.4/setup.py
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 17:20:32.477879 ts-python-client-2.0.4/ts_python_client/
+-rw-r--r--   0 markin     (501) staff       (20)       81 2023-04-03 13:46:33.000000 ts-python-client-2.0.4/ts_python_client/__init__.py
+-rw-r--r--   0 markin     (501) staff       (20)     1290 2023-05-24 17:17:04.000000 ts-python-client-2.0.4/ts_python_client/cli.py
+-rw-r--r--   0 markin     (501) staff       (20)     4228 2022-06-07 21:36:28.000000 ts-python-client-2.0.4/ts_python_client/client.py
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 17:20:32.481513 ts-python-client-2.0.4/ts_python_client/commands/
+-rw-r--r--   0 markin     (501) staff       (20)     1403 2023-04-03 13:46:33.000000 ts-python-client-2.0.4/ts_python_client/commands/ScanCommand.py
+-rw-r--r--   0 markin     (501) staff       (20)     2292 2023-04-03 13:46:33.000000 ts-python-client-2.0.4/ts_python_client/commands/UploadCommand.py
+-rw-r--r--   0 markin     (501) staff       (20)      410 2023-04-03 13:46:33.000000 ts-python-client-2.0.4/ts_python_client/commands/__init__.py
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 17:20:32.479741 ts-python-client-2.0.4/ts_python_client.egg-info/
+-rw-r--r--   0 markin     (501) staff       (20)      381 2023-05-24 17:20:32.000000 ts-python-client-2.0.4/ts_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 markin     (501) staff       (20)      461 2023-05-24 17:20:32.000000 ts-python-client-2.0.4/ts_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 markin     (501) staff       (20)        1 2023-05-24 17:20:32.000000 ts-python-client-2.0.4/ts_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 markin     (501) staff       (20)       22 2023-05-24 17:20:32.000000 ts-python-client-2.0.4/ts_python_client.egg-info/requires.txt
+-rw-r--r--   0 markin     (501) staff       (20)       17 2023-05-24 17:20:32.000000 ts-python-client-2.0.4/ts_python_client.egg-info/top_level.txt
```

### Comparing `ts-python-client-2.0.3/LICENSE` & `ts-python-client-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ts-python-client-2.0.3/README.md` & `ts-python-client-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ts-python-client-2.0.3/setup.py` & `ts-python-client-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 setup(
     name='ts-python-client',
     python_requires='>=3.8',
     packages=[
         'ts_python_client',
         'ts_python_client.commands'
     ],
-    version='2.0.3',
+    version='2.0.4',
     description='A python client for TrustSource (https://app.trustsource.io) to manage open source code compliance',
     author='EACG GmbH',
     license='Apache-2.0',
     url='https://github.com/trustsource/ts-python-client.git',
     download_url='',
     keywords=['scanning', 'dependencies', 'modules', 'TrustSource'],
     classifiers=[],
```

### Comparing `ts-python-client-2.0.3/ts_python_client/cli.py` & `ts-python-client-2.0.4/ts_python_client/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import pathlib
 import typing as t
 
 from .commands.ScanCommand import ScanCommand
 from .commands.UploadCommand import UploadCommand
 
 @click.group()
-@click.version_option()
 def _start():
     pass
 
 @_start.command(cls=ScanCommand)
 @click.option('-o', '--output', 'output_path', required=False, type=click.Path(path_type=pathlib.Path), help='Output path for the scan')
 @click.argument('path', type=click.Path(exists=True, path_type=pathlib.Path), nargs=-1)
 def scan(path, output_path, *args, **kwargs):
```

### Comparing `ts-python-client-2.0.3/ts_python_client/client.py` & `ts-python-client-2.0.4/ts_python_client/client.py`

 * *Files identical despite different names*

### Comparing `ts-python-client-2.0.3/ts_python_client/commands/ScanCommand.py` & `ts-python-client-2.0.4/ts_python_client/commands/ScanCommand.py`

 * *Files identical despite different names*

### Comparing `ts-python-client-2.0.3/ts_python_client/commands/UploadCommand.py` & `ts-python-client-2.0.4/ts_python_client/commands/UploadCommand.py`

 * *Files identical despite different names*

