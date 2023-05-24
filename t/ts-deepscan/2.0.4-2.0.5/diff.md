# Comparing `tmp/ts-deepscan-2.0.4.tar.gz` & `tmp/ts-deepscan-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts-deepscan-2.0.4.tar", last modified: Wed May 24 16:43:20 2023, max compression
+gzip compressed data, was "ts-deepscan-2.0.5.tar", last modified: Wed May 24 17:27:32 2023, max compression
```

## Comparing `ts-deepscan-2.0.4.tar` & `ts-deepscan-2.0.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 16:43:20.004013 ts-deepscan-2.0.4/
--rw-r--r--   0 markin     (501) staff       (20)    11340 2020-12-10 19:17:15.000000 ts-deepscan-2.0.4/LICENSE
--rw-rw----   0 markin     (501) staff       (20)      174 2020-11-03 19:33:21.000000 ts-deepscan-2.0.4/MANIFEST.in
--rw-r--r--   0 markin     (501) staff       (20)      342 2023-05-24 16:43:20.004131 ts-deepscan-2.0.4/PKG-INFO
--rw-r--r--   0 markin     (501) staff       (20)     8684 2023-05-16 15:13:39.000000 ts-deepscan-2.0.4/README.md
--rw-rw----   0 markin     (501) staff       (20)       26 2017-03-20 16:02:56.000000 ts-deepscan-2.0.4/_config.yml
--rw-rw----   0 markin     (501) staff       (20)       79 2023-05-24 16:43:20.004567 ts-deepscan-2.0.4/setup.cfg
--rw-r--r--   0 markin     (501) staff       (20)     1110 2023-05-24 16:17:04.000000 ts-deepscan-2.0.4/setup.py
--rwxr-xr-x   0 markin     (501) staff       (20)       94 2023-04-03 13:51:08.000000 ts-deepscan-2.0.4/ts-deepscan
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 16:43:19.984646 ts-deepscan-2.0.4/ts_deepscan/
--rw-r--r--   0 markin     (501) staff       (20)     4853 2023-05-24 16:11:20.000000 ts-deepscan-2.0.4/ts_deepscan/__init__.py
--rw-r--r--   0 markin     (501) staff       (20)      145 2023-04-03 13:51:08.000000 ts-deepscan-2.0.4/ts_deepscan/__main__.py
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 16:43:19.997312 ts-deepscan-2.0.4/ts_deepscan/analyser/
--rw-r--r--   0 markin     (501) staff       (20)     2494 2023-04-03 13:51:08.000000 ts-deepscan-2.0.4/ts_deepscan/analyser/CommentAnalyser.py
--rw-r--r--   0 markin     (501) staff       (20)      922 2023-04-03 13:51:08.000000 ts-deepscan-2.0.4/ts_deepscan/analyser/CryptoAnalyser.py
--rw-r--r--   0 markin     (501) staff       (20)     2419 2023-04-03 13:51:08.000000 ts-deepscan-2.0.4/ts_deepscan/analyser/Dataset.py
--rw-r--r--   0 markin     (501) staff       (20)     1183 2023-04-03 13:51:08.000000 ts-deepscan-2.0.4/ts_deepscan/analyser/LicenseAnalyser.py
--rw-r--r--   0 markin     (501) staff       (20)      731 2023-04-03 13:51:08.000000 ts-deepscan-2.0.4/ts_deepscan/analyser/__init__.py
--rw-r--r--   0 markin     (501) staff       (20)  2702144 2023-01-06 17:43:03.000000 ts-deepscan-2.0.4/ts_deepscan/analyser/licenses.json
--rw-r--r--   0 markin     (501) staff       (20)     2472 2023-04-03 13:51:08.000000 ts-deepscan-2.0.4/ts_deepscan/analyser/spdx.py
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 16:43:19.998192 ts-deepscan-2.0.4/ts_deepscan/analyser/textutils/
--rw-r--r--   0 markin     (501) staff       (20)     7695 2023-04-03 15:08:19.000000 ts-deepscan-2.0.4/ts_deepscan/analyser/textutils/__init__.py
--rw-r--r--   0 markin     (501) staff       (20)     2171 2023-05-24 16:11:45.000000 ts-deepscan-2.0.4/ts_deepscan/cli.py
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 16:43:19.998828 ts-deepscan-2.0.4/ts_deepscan/commentparser/
--rw-rw----   0 markin     (501) staff       (20)     6865 2020-12-09 20:37:42.000000 ts-deepscan-2.0.4/ts_deepscan/commentparser/__init__.py
--rw-rw----   0 markin     (501) staff       (20)     6712 2020-12-09 20:37:42.000000 ts-deepscan-2.0.4/ts_deepscan/commentparser/language.py
--rw-r--r--   0 markin     (501) staff       (20)      582 2022-06-10 12:08:39.000000 ts-deepscan-2.0.4/ts_deepscan/config.py
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 16:43:19.999145 ts-deepscan-2.0.4/ts_deepscan/scancode/
--rw-r--r--   0 markin     (501) staff       (20)       94 2020-12-10 19:16:09.000000 ts-deepscan-2.0.4/ts_deepscan/scancode/__init__.py
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 16:43:20.002325 ts-deepscan-2.0.4/ts_deepscan/scancode/cluecode/
--rw-r--r--   0 markin     (501) staff       (20)        0 2020-12-10 19:15:52.000000 ts-deepscan-2.0.4/ts_deepscan/scancode/cluecode/__init__.py
--rw-r--r--   0 markin     (501) staff       (20)   103777 2020-12-10 19:14:48.000000 ts-deepscan-2.0.4/ts_deepscan/scancode/cluecode/copyrights.py
--rw-r--r--   0 markin     (501) staff       (20)     3538 2020-12-10 19:14:55.000000 ts-deepscan-2.0.4/ts_deepscan/scancode/cluecode/copyrights_hint.py
--rw-r--r--   0 markin     (501) staff       (20)     3272 2020-12-10 19:15:05.000000 ts-deepscan-2.0.4/ts_deepscan/scancode/cluecode/utils.py
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 16:43:20.003594 ts-deepscan-2.0.4/ts_deepscan/scanner/
--rw-r--r--   0 markin     (501) staff       (20)     4123 2023-04-03 13:51:08.000000 ts-deepscan-2.0.4/ts_deepscan/scanner/ParallelScanner.py
--rw-r--r--   0 markin     (501) staff       (20)     4050 2023-04-03 13:51:08.000000 ts-deepscan-2.0.4/ts_deepscan/scanner/Scanner.py
--rw-r--r--   0 markin     (501) staff       (20)     2376 2023-04-03 13:51:08.000000 ts-deepscan-2.0.4/ts_deepscan/scanner/__init__.py
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 16:43:19.987097 ts-deepscan-2.0.4/ts_deepscan.egg-info/
--rw-r--r--   0 markin     (501) staff       (20)      342 2023-05-24 16:43:19.000000 ts-deepscan-2.0.4/ts_deepscan.egg-info/PKG-INFO
--rw-r--r--   0 markin     (501) staff       (20)     1049 2023-05-24 16:43:19.000000 ts-deepscan-2.0.4/ts_deepscan.egg-info/SOURCES.txt
--rw-r--r--   0 markin     (501) staff       (20)        1 2023-05-24 16:43:19.000000 ts-deepscan-2.0.4/ts_deepscan.egg-info/dependency_links.txt
--rw-r--r--   0 markin     (501) staff       (20)       53 2023-05-24 16:43:19.000000 ts-deepscan-2.0.4/ts_deepscan.egg-info/entry_points.txt
--rw-r--r--   0 markin     (501) staff       (20)      113 2023-05-24 16:43:19.000000 ts-deepscan-2.0.4/ts_deepscan.egg-info/requires.txt
--rw-r--r--   0 markin     (501) staff       (20)       12 2023-05-24 16:43:19.000000 ts-deepscan-2.0.4/ts_deepscan.egg-info/top_level.txt
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 17:27:32.463036 ts-deepscan-2.0.5/
+-rw-r--r--   0 markin     (501) staff       (20)    11340 2020-12-10 19:17:15.000000 ts-deepscan-2.0.5/LICENSE
+-rw-rw----   0 markin     (501) staff       (20)      174 2020-11-03 19:33:21.000000 ts-deepscan-2.0.5/MANIFEST.in
+-rw-r--r--   0 markin     (501) staff       (20)      342 2023-05-24 17:27:32.463175 ts-deepscan-2.0.5/PKG-INFO
+-rw-r--r--   0 markin     (501) staff       (20)     8684 2023-05-16 15:13:39.000000 ts-deepscan-2.0.5/README.md
+-rw-rw----   0 markin     (501) staff       (20)       26 2017-03-20 16:02:56.000000 ts-deepscan-2.0.5/_config.yml
+-rw-rw----   0 markin     (501) staff       (20)       79 2023-05-24 17:27:32.463621 ts-deepscan-2.0.5/setup.cfg
+-rw-r--r--   0 markin     (501) staff       (20)     1110 2023-05-24 17:25:45.000000 ts-deepscan-2.0.5/setup.py
+-rwxr-xr-x   0 markin     (501) staff       (20)       94 2023-04-03 13:51:08.000000 ts-deepscan-2.0.5/ts-deepscan
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 17:27:32.450832 ts-deepscan-2.0.5/ts_deepscan/
+-rw-r--r--   0 markin     (501) staff       (20)     4853 2023-05-24 16:11:20.000000 ts-deepscan-2.0.5/ts_deepscan/__init__.py
+-rw-r--r--   0 markin     (501) staff       (20)      145 2023-04-03 13:51:08.000000 ts-deepscan-2.0.5/ts_deepscan/__main__.py
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 17:27:32.458870 ts-deepscan-2.0.5/ts_deepscan/analyser/
+-rw-r--r--   0 markin     (501) staff       (20)     2494 2023-04-03 13:51:08.000000 ts-deepscan-2.0.5/ts_deepscan/analyser/CommentAnalyser.py
+-rw-r--r--   0 markin     (501) staff       (20)      922 2023-04-03 13:51:08.000000 ts-deepscan-2.0.5/ts_deepscan/analyser/CryptoAnalyser.py
+-rw-r--r--   0 markin     (501) staff       (20)     2419 2023-04-03 13:51:08.000000 ts-deepscan-2.0.5/ts_deepscan/analyser/Dataset.py
+-rw-r--r--   0 markin     (501) staff       (20)     1183 2023-04-03 13:51:08.000000 ts-deepscan-2.0.5/ts_deepscan/analyser/LicenseAnalyser.py
+-rw-r--r--   0 markin     (501) staff       (20)      731 2023-04-03 13:51:08.000000 ts-deepscan-2.0.5/ts_deepscan/analyser/__init__.py
+-rw-r--r--   0 markin     (501) staff       (20)  2702144 2023-01-06 17:43:03.000000 ts-deepscan-2.0.5/ts_deepscan/analyser/licenses.json
+-rw-r--r--   0 markin     (501) staff       (20)     2472 2023-04-03 13:51:08.000000 ts-deepscan-2.0.5/ts_deepscan/analyser/spdx.py
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 17:27:32.459189 ts-deepscan-2.0.5/ts_deepscan/analyser/textutils/
+-rw-r--r--   0 markin     (501) staff       (20)     7695 2023-04-03 15:08:19.000000 ts-deepscan-2.0.5/ts_deepscan/analyser/textutils/__init__.py
+-rw-r--r--   0 markin     (501) staff       (20)     2171 2023-05-24 17:25:32.000000 ts-deepscan-2.0.5/ts_deepscan/cli.py
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 17:27:32.459814 ts-deepscan-2.0.5/ts_deepscan/commentparser/
+-rw-rw----   0 markin     (501) staff       (20)     6865 2020-12-09 20:37:42.000000 ts-deepscan-2.0.5/ts_deepscan/commentparser/__init__.py
+-rw-rw----   0 markin     (501) staff       (20)     6712 2020-12-09 20:37:42.000000 ts-deepscan-2.0.5/ts_deepscan/commentparser/language.py
+-rw-r--r--   0 markin     (501) staff       (20)      582 2022-06-10 12:08:39.000000 ts-deepscan-2.0.5/ts_deepscan/config.py
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 17:27:32.460158 ts-deepscan-2.0.5/ts_deepscan/scancode/
+-rw-r--r--   0 markin     (501) staff       (20)       94 2020-12-10 19:16:09.000000 ts-deepscan-2.0.5/ts_deepscan/scancode/__init__.py
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 17:27:32.461778 ts-deepscan-2.0.5/ts_deepscan/scancode/cluecode/
+-rw-r--r--   0 markin     (501) staff       (20)        0 2020-12-10 19:15:52.000000 ts-deepscan-2.0.5/ts_deepscan/scancode/cluecode/__init__.py
+-rw-r--r--   0 markin     (501) staff       (20)   103777 2020-12-10 19:14:48.000000 ts-deepscan-2.0.5/ts_deepscan/scancode/cluecode/copyrights.py
+-rw-r--r--   0 markin     (501) staff       (20)     3538 2020-12-10 19:14:55.000000 ts-deepscan-2.0.5/ts_deepscan/scancode/cluecode/copyrights_hint.py
+-rw-r--r--   0 markin     (501) staff       (20)     3272 2020-12-10 19:15:05.000000 ts-deepscan-2.0.5/ts_deepscan/scancode/cluecode/utils.py
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 17:27:32.462761 ts-deepscan-2.0.5/ts_deepscan/scanner/
+-rw-r--r--   0 markin     (501) staff       (20)     4123 2023-04-03 13:51:08.000000 ts-deepscan-2.0.5/ts_deepscan/scanner/ParallelScanner.py
+-rw-r--r--   0 markin     (501) staff       (20)     4050 2023-04-03 13:51:08.000000 ts-deepscan-2.0.5/ts_deepscan/scanner/Scanner.py
+-rw-r--r--   0 markin     (501) staff       (20)     2376 2023-04-03 13:51:08.000000 ts-deepscan-2.0.5/ts_deepscan/scanner/__init__.py
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-24 17:27:32.452693 ts-deepscan-2.0.5/ts_deepscan.egg-info/
+-rw-r--r--   0 markin     (501) staff       (20)      342 2023-05-24 17:27:32.000000 ts-deepscan-2.0.5/ts_deepscan.egg-info/PKG-INFO
+-rw-r--r--   0 markin     (501) staff       (20)     1049 2023-05-24 17:27:32.000000 ts-deepscan-2.0.5/ts_deepscan.egg-info/SOURCES.txt
+-rw-r--r--   0 markin     (501) staff       (20)        1 2023-05-24 17:27:32.000000 ts-deepscan-2.0.5/ts_deepscan.egg-info/dependency_links.txt
+-rw-r--r--   0 markin     (501) staff       (20)       53 2023-05-24 17:27:32.000000 ts-deepscan-2.0.5/ts_deepscan.egg-info/entry_points.txt
+-rw-r--r--   0 markin     (501) staff       (20)      113 2023-05-24 17:27:32.000000 ts-deepscan-2.0.5/ts_deepscan.egg-info/requires.txt
+-rw-r--r--   0 markin     (501) staff       (20)       12 2023-05-24 17:27:32.000000 ts-deepscan-2.0.5/ts_deepscan.egg-info/top_level.txt
```

### Comparing `ts-deepscan-2.0.4/LICENSE` & `ts-deepscan-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.4/README.md` & `ts-deepscan-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.4/setup.py` & `ts-deepscan-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         'ts_deepscan.analyser',
         'ts_deepscan.analyser.textutils',
         'ts_deepscan.commentparser',
         'ts_deepscan.scanner',
         'ts_deepscan.scancode',
         'ts_deepscan.scancode.cluecode'
     ],
-    version='2.0.4',
+    version='2.0.5',
     description='Repository scanner for the identification of effective licenses and copyright information.',
     author='EACG GmbH',
     license='Apache 2.0',
     url='https://github.com/TrustSource/ts-deepscan.git',
     download_url='',
     keywords=['DeepScan', 'TrustSource'],
     classifiers=[],
@@ -24,15 +24,15 @@
         'six',
         'spacy>=2.2.0,<3.0.0',
         'nltk',
         'text-unidecode',
         'requests',
         'progress',
         'osadl_matrix',
-        'ts-python-client>=2.0.3',
+        'ts-python-client>=2.0.4',
         'pyminr>=0.1.0'
     ],
     scripts=['ts-deepscan'],
     entry_points={
         'console_scripts': ['ts-deepscan=ts_deepscan.cli:main'],
     },
     setup_requires=[
```

### Comparing `ts-deepscan-2.0.4/ts_deepscan/__init__.py` & `ts-deepscan-2.0.5/ts_deepscan/__init__.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.4/ts_deepscan/analyser/CommentAnalyser.py` & `ts-deepscan-2.0.5/ts_deepscan/analyser/CommentAnalyser.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.4/ts_deepscan/analyser/CryptoAnalyser.py` & `ts-deepscan-2.0.5/ts_deepscan/analyser/CryptoAnalyser.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.4/ts_deepscan/analyser/Dataset.py` & `ts-deepscan-2.0.5/ts_deepscan/analyser/Dataset.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.4/ts_deepscan/analyser/LicenseAnalyser.py` & `ts-deepscan-2.0.5/ts_deepscan/analyser/LicenseAnalyser.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.4/ts_deepscan/analyser/__init__.py` & `ts-deepscan-2.0.5/ts_deepscan/analyser/__init__.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.4/ts_deepscan/analyser/licenses.json` & `ts-deepscan-2.0.5/ts_deepscan/analyser/licenses.json`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.4/ts_deepscan/analyser/spdx.py` & `ts-deepscan-2.0.5/ts_deepscan/analyser/spdx.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.4/ts_deepscan/analyser/textutils/__init__.py` & `ts-deepscan-2.0.5/ts_deepscan/analyser/textutils/__init__.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.4/ts_deepscan/cli.py` & `ts-deepscan-2.0.5/ts_deepscan/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from .scanner import Scan
 from . import create_scanner, execute_scan, upload_data, deepscanBaseUrl
 
 from ts_python_client.cli import get_start_cmd, scan
 
 
-start = get_start_cmd(version='2.0.3')
+start = get_start_cmd(version='2.0.5')
 
 def main():
     start()
 
 
 @click.option('-j', '--jobs',
               default=-1 if sys.platform != 'win32' else 1, # Turn off multitasking due to the long spawn on Windows
```

### Comparing `ts-deepscan-2.0.4/ts_deepscan/commentparser/__init__.py` & `ts-deepscan-2.0.5/ts_deepscan/commentparser/__init__.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.4/ts_deepscan/commentparser/language.py` & `ts-deepscan-2.0.5/ts_deepscan/commentparser/language.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.4/ts_deepscan/config.py` & `ts-deepscan-2.0.5/ts_deepscan/config.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.4/ts_deepscan/scancode/cluecode/copyrights.py` & `ts-deepscan-2.0.5/ts_deepscan/scancode/cluecode/copyrights.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.4/ts_deepscan/scancode/cluecode/copyrights_hint.py` & `ts-deepscan-2.0.5/ts_deepscan/scancode/cluecode/copyrights_hint.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.4/ts_deepscan/scancode/cluecode/utils.py` & `ts-deepscan-2.0.5/ts_deepscan/scancode/cluecode/utils.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.4/ts_deepscan/scanner/ParallelScanner.py` & `ts-deepscan-2.0.5/ts_deepscan/scanner/ParallelScanner.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.4/ts_deepscan/scanner/Scanner.py` & `ts-deepscan-2.0.5/ts_deepscan/scanner/Scanner.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.4/ts_deepscan/scanner/__init__.py` & `ts-deepscan-2.0.5/ts_deepscan/scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.4/ts_deepscan.egg-info/SOURCES.txt` & `ts-deepscan-2.0.5/ts_deepscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

