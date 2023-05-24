# Comparing `tmp/cioseq-0.1.8.tar.gz` & `tmp/cioseq-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cioseq-0.1.8.tar", last modified: Wed Mar 10 03:35:09 2021, max compression
+gzip compressed data, was "cioseq-0.1.9.tar", last modified: Wed Mar 10 03:56:33 2021, max compression
```

## Comparing `cioseq-0.1.8.tar` & `cioseq-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-10 03:35:09.890325 cioseq-0.1.8/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2021-03-10 03:34:49.000000 cioseq-0.1.8/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7446 2021-03-10 03:35:09.890325 cioseq-0.1.8/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3970 2021-03-10 03:34:49.000000 cioseq-0.1.8/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-10 03:35:09.890325 cioseq-0.1.8/cioseq/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-03-10 03:34:49.000000 cioseq-0.1.8/cioseq/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19699 2021-03-10 03:34:49.000000 cioseq-0.1.8/cioseq/sequence.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-10 03:35:09.890325 cioseq-0.1.8/cioseq.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7446 2021-03-10 03:35:09.000000 cioseq-0.1.8/cioseq.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      295 2021-03-10 03:35:09.000000 cioseq-0.1.8/cioseq.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-03-10 03:35:09.000000 cioseq-0.1.8/cioseq.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-03-10 03:35:09.000000 cioseq-0.1.8/cioseq.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       15 2021-03-10 03:35:09.000000 cioseq-0.1.8/cioseq.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       13 2021-03-10 03:35:09.000000 cioseq-0.1.8/cioseq.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2021-03-10 03:35:09.890325 cioseq-0.1.8/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1748 2021-03-10 03:34:49.000000 cioseq-0.1.8/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-10 03:35:09.890325 cioseq-0.1.8/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-03-10 03:34:49.000000 cioseq-0.1.8/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23943 2021-03-10 03:34:49.000000 cioseq-0.1.8/tests/test_sequence.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-10 03:56:33.720636 cioseq-0.1.9/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2021-03-10 03:55:53.000000 cioseq-0.1.9/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7446 2021-03-10 03:56:33.720636 cioseq-0.1.9/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3970 2021-03-10 03:55:53.000000 cioseq-0.1.9/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-10 03:56:33.520635 cioseq-0.1.9/cioseq/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-03-10 03:55:53.000000 cioseq-0.1.9/cioseq/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19699 2021-03-10 03:55:53.000000 cioseq-0.1.9/cioseq/sequence.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-10 03:56:33.720636 cioseq-0.1.9/cioseq.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7446 2021-03-10 03:56:33.000000 cioseq-0.1.9/cioseq.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      295 2021-03-10 03:56:33.000000 cioseq-0.1.9/cioseq.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-03-10 03:56:33.000000 cioseq-0.1.9/cioseq.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-03-10 03:56:33.000000 cioseq-0.1.9/cioseq.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       15 2021-03-10 03:56:33.000000 cioseq-0.1.9/cioseq.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       13 2021-03-10 03:56:33.000000 cioseq-0.1.9/cioseq.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2021-03-10 03:56:33.720636 cioseq-0.1.9/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1748 2021-03-10 03:55:53.000000 cioseq-0.1.9/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-03-10 03:56:33.520635 cioseq-0.1.9/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-03-10 03:55:53.000000 cioseq-0.1.9/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23943 2021-03-10 03:55:53.000000 cioseq-0.1.9/tests/test_sequence.py
```

### Comparing `cioseq-0.1.8/PKG-INFO` & `cioseq-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cioseq
-Version: 0.1.8
+Version: 0.1.9
 Summary: Manage sequences of frame numbers.
 Home-page: https://github.com/ConductorTechnologies/sequence
 Author: conductor
 Author-email: info@conductortech.com
 License: UNKNOWN
 Description: # sequence
         Manage sequences of frame numbers
@@ -230,15 +230,15 @@
         Pull requests welcome. 
         
         ## License
         [MIT](LICENSE)
         
         ## Changelog
         
-        ### Version:0.1.8 -- 09 Mar 2021
+        ### Version:0.1.9 -- 09 Mar 2021
         
         * Fixed wrong pypi registry. [a3d82e1]
         
         ### Version:0.1.6 -- 09 Mar 2021
         
         * Adds release flow to circleci. [71bbca2]
         * Add .circleci/config.yml. [30fd9d9]
```

### Comparing `cioseq-0.1.8/README.md` & `cioseq-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cioseq-0.1.8/cioseq/sequence.py` & `cioseq-0.1.9/cioseq/sequence.py`

 * *Files identical despite different names*

### Comparing `cioseq-0.1.8/cioseq.egg-info/PKG-INFO` & `cioseq-0.1.9/cioseq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cioseq
-Version: 0.1.8
+Version: 0.1.9
 Summary: Manage sequences of frame numbers.
 Home-page: https://github.com/ConductorTechnologies/sequence
 Author: conductor
 Author-email: info@conductortech.com
 License: UNKNOWN
 Description: # sequence
         Manage sequences of frame numbers
@@ -230,15 +230,15 @@
         Pull requests welcome. 
         
         ## License
         [MIT](LICENSE)
         
         ## Changelog
         
-        ### Version:0.1.8 -- 09 Mar 2021
+        ### Version:0.1.9 -- 09 Mar 2021
         
         * Fixed wrong pypi registry. [a3d82e1]
         
         ### Version:0.1.6 -- 09 Mar 2021
         
         * Adds release flow to circleci. [71bbca2]
         * Add .circleci/config.yml. [30fd9d9]
```

### Comparing `cioseq-0.1.8/setup.py` & `cioseq-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `cioseq-0.1.8/tests/test_sequence.py` & `cioseq-0.1.9/tests/test_sequence.py`

 * *Files identical despite different names*

