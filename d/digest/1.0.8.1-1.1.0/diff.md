# Comparing `tmp/digest-1.0.8.1.tar.gz` & `tmp/digest-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digest-1.0.8.1.tar", last modified: Wed Apr 13 19:17:14 2022, max compression
+gzip compressed data, was "digest-1.1.0.tar", last modified: Wed May 24 16:03:08 2023, max compression
```

## Comparing `digest-1.0.8.1.tar` & `digest-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 bmc        (501) staff       (20)        0 2022-04-13 19:17:14.714882 digest-1.0.8.1/
--rw-r--r--   0 bmc        (501) staff       (20)     2117 2022-04-13 19:17:14.715210 digest-1.0.8.1/PKG-INFO
--rw-r--r--   0 bmc        (501) staff       (20)      600 2022-04-13 16:29:11.000000 digest-1.0.8.1/README.md
-drwxr-xr-x   0 bmc        (501) staff       (20)        0 2022-04-13 19:17:14.704557 digest-1.0.8.1/digest/
--rw-r--r--   0 bmc        (501) staff       (20)     5115 2022-04-13 19:16:38.000000 digest-1.0.8.1/digest/__init__.py
-drwxr-xr-x   0 bmc        (501) staff       (20)        0 2022-04-13 19:17:14.714296 digest-1.0.8.1/digest.egg-info/
--rw-r--r--   0 bmc        (501) staff       (20)     2117 2022-04-13 19:17:14.000000 digest-1.0.8.1/digest.egg-info/PKG-INFO
--rw-r--r--   0 bmc        (501) staff       (20)      200 2022-04-13 19:17:14.000000 digest-1.0.8.1/digest.egg-info/SOURCES.txt
--rw-r--r--   0 bmc        (501) staff       (20)        1 2022-04-13 19:17:14.000000 digest-1.0.8.1/digest.egg-info/dependency_links.txt
--rw-r--r--   0 bmc        (501) staff       (20)       38 2022-04-13 19:17:14.000000 digest-1.0.8.1/digest.egg-info/entry_points.txt
--rw-r--r--   0 bmc        (501) staff       (20)        7 2022-04-13 19:17:14.000000 digest-1.0.8.1/digest.egg-info/top_level.txt
--rw-r--r--   0 bmc        (501) staff       (20)       63 2022-04-13 19:17:14.718642 digest-1.0.8.1/setup.cfg
--rw-r--r--   0 bmc        (501) staff       (20)     2108 2022-04-13 17:21:55.000000 digest-1.0.8.1/setup.py
+drwxr-xr-x   0 bmc        (501) staff       (20)        0 2023-05-24 16:03:08.822172 digest-1.1.0/
+-rw-r--r--   0 bmc        (501) staff       (20)    11355 2023-05-24 15:13:06.000000 digest-1.1.0/LICENSE.md
+-rw-r--r--   0 bmc        (501) staff       (20)     1903 2023-05-24 16:03:08.822303 digest-1.1.0/PKG-INFO
+-rw-r--r--   0 bmc        (501) staff       (20)      974 2023-05-24 15:15:27.000000 digest-1.1.0/README.md
+drwxr-xr-x   0 bmc        (501) staff       (20)        0 2023-05-24 16:03:08.820157 digest-1.1.0/digest/
+-rw-r--r--   0 bmc        (501) staff       (20)     6816 2023-05-24 15:31:39.000000 digest-1.1.0/digest/__init__.py
+drwxr-xr-x   0 bmc        (501) staff       (20)        0 2023-05-24 16:03:08.821880 digest-1.1.0/digest.egg-info/
+-rw-r--r--   0 bmc        (501) staff       (20)     1903 2023-05-24 16:03:08.000000 digest-1.1.0/digest.egg-info/PKG-INFO
+-rw-r--r--   0 bmc        (501) staff       (20)      211 2023-05-24 16:03:08.000000 digest-1.1.0/digest.egg-info/SOURCES.txt
+-rw-r--r--   0 bmc        (501) staff       (20)        1 2023-05-24 16:03:08.000000 digest-1.1.0/digest.egg-info/dependency_links.txt
+-rw-r--r--   0 bmc        (501) staff       (20)       39 2023-05-24 16:03:08.000000 digest-1.1.0/digest.egg-info/entry_points.txt
+-rw-r--r--   0 bmc        (501) staff       (20)        7 2023-05-24 16:03:08.000000 digest-1.1.0/digest.egg-info/top_level.txt
+-rw-r--r--   0 bmc        (501) staff       (20)       63 2023-05-24 16:03:08.822817 digest-1.1.0/setup.cfg
+-rw-r--r--   0 bmc        (501) staff       (20)     2108 2022-04-13 17:21:55.000000 digest-1.1.0/setup.py
```

### Comparing `digest-1.0.8.1/PKG-INFO` & `digest-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: digest
-Version: 1.0.8.1
+Version: 1.1.0
 Summary: Calculate message digests of files or standard input
 Home-page: http://software.clapper.org/digest/
 Author: Brian M. Clapper
 Author-email: bmc@clapper.org
-License: BSD-style license
-Description: 
-        Calculate a cryptohash on a file or standard input.
-        
-        Usage:
-        
-            **digest** -h
-            **digest** [-e encoding] *algorithm* [file] ...
-        
-        The *digest* utility calculates message digests of files or, if no file
-        is specified, standard input. The set of supported digests depends on the
-        current Python interpreter and the version of OpenSSL present on the system.
-        However, at a minimum, *digest* supports the following algorithms:
-        
-            +-------------+--------------------------------------+
-            | Argument    | Algorithm                            |
-            +=============+======================================+
-            | md5         | The MD5 algorithm                    |
-            +-------------+--------------------------------------+
-            | sha1        | The SHA-1 algorithm                  |
-            +-------------+--------------------------------------+
-            | sha224      | The SHA-224 algorithm                |
-            +-------------+--------------------------------------+
-            | sha256      | The SHA-256 algorithm                |
-            +-------------+--------------------------------------+
-            | sha384      | The SHA-384 algorithm                |
-            +-------------+--------------------------------------+
-            | sha512      | The SHA-512 algorithm                |
-            +-------------+--------------------------------------+
-        
-Platform: UNKNOWN
+License: Apache Software License Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Utilities
 Description-Content-Type: text/x-rst
+License-File: LICENSE.md
+
+
+Calculate a cryptohash on a file or standard input.
+
+Usage:
+
+    **digest** -h
+    **digest** [-e encoding] *algorithm* [file] ...
+
+The *digest* utility calculates message digests of files or, if no file
+is specified, standard input. The set of supported digests depends on the
+current Python interpreter and the version of OpenSSL present on the system.
+However, at a minimum, *digest* supports the following algorithms:
+
+    +-------------+--------------------------------------+
+    | Argument    | Algorithm                            |
+    +=============+======================================+
+    | md5         | The MD5 algorithm                    |
+    +-------------+--------------------------------------+
+    | sha1        | The SHA-1 algorithm                  |
+    +-------------+--------------------------------------+
+    | sha224      | The SHA-224 algorithm                |
+    +-------------+--------------------------------------+
+    | sha256      | The SHA-256 algorithm                |
+    +-------------+--------------------------------------+
+    | sha384      | The SHA-384 algorithm                |
+    +-------------+--------------------------------------+
+    | sha512      | The SHA-512 algorithm                |
+    +-------------+--------------------------------------+
```

### Comparing `digest-1.0.8.1/digest.egg-info/PKG-INFO` & `digest-1.1.0/digest.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: digest
-Version: 1.0.8.1
+Version: 1.1.0
 Summary: Calculate message digests of files or standard input
 Home-page: http://software.clapper.org/digest/
 Author: Brian M. Clapper
 Author-email: bmc@clapper.org
-License: BSD-style license
-Description: 
-        Calculate a cryptohash on a file or standard input.
-        
-        Usage:
-        
-            **digest** -h
-            **digest** [-e encoding] *algorithm* [file] ...
-        
-        The *digest* utility calculates message digests of files or, if no file
-        is specified, standard input. The set of supported digests depends on the
-        current Python interpreter and the version of OpenSSL present on the system.
-        However, at a minimum, *digest* supports the following algorithms:
-        
-            +-------------+--------------------------------------+
-            | Argument    | Algorithm                            |
-            +=============+======================================+
-            | md5         | The MD5 algorithm                    |
-            +-------------+--------------------------------------+
-            | sha1        | The SHA-1 algorithm                  |
-            +-------------+--------------------------------------+
-            | sha224      | The SHA-224 algorithm                |
-            +-------------+--------------------------------------+
-            | sha256      | The SHA-256 algorithm                |
-            +-------------+--------------------------------------+
-            | sha384      | The SHA-384 algorithm                |
-            +-------------+--------------------------------------+
-            | sha512      | The SHA-512 algorithm                |
-            +-------------+--------------------------------------+
-        
-Platform: UNKNOWN
+License: Apache Software License Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Utilities
 Description-Content-Type: text/x-rst
+License-File: LICENSE.md
+
+
+Calculate a cryptohash on a file or standard input.
+
+Usage:
+
+    **digest** -h
+    **digest** [-e encoding] *algorithm* [file] ...
+
+The *digest* utility calculates message digests of files or, if no file
+is specified, standard input. The set of supported digests depends on the
+current Python interpreter and the version of OpenSSL present on the system.
+However, at a minimum, *digest* supports the following algorithms:
+
+    +-------------+--------------------------------------+
+    | Argument    | Algorithm                            |
+    +=============+======================================+
+    | md5         | The MD5 algorithm                    |
+    +-------------+--------------------------------------+
+    | sha1        | The SHA-1 algorithm                  |
+    +-------------+--------------------------------------+
+    | sha224      | The SHA-224 algorithm                |
+    +-------------+--------------------------------------+
+    | sha256      | The SHA-256 algorithm                |
+    +-------------+--------------------------------------+
+    | sha384      | The SHA-384 algorithm                |
+    +-------------+--------------------------------------+
+    | sha512      | The SHA-512 algorithm                |
+    +-------------+--------------------------------------+
```

### Comparing `digest-1.0.8.1/setup.py` & `digest-1.1.0/setup.py`

 * *Files identical despite different names*

