# Comparing `tmp/jintonic-0.2.3.tar.gz` & `tmp/jintonic-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jintonic-0.2.3.tar", last modified: Mon May 22 17:34:01 2023, max compression
+gzip compressed data, was "jintonic-0.2.4.tar", last modified: Wed May 24 16:48:02 2023, max compression
```

## Comparing `jintonic-0.2.3.tar` & `jintonic-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 daedalus   (501) staff       (20)        0 2023-05-22 17:34:01.597189 jintonic-0.2.3/
--rw-r--r--   0 daedalus   (501) staff       (20)     1068 2023-05-21 09:38:33.000000 jintonic-0.2.3/LICENSE
--rw-r--r--   0 daedalus   (501) staff       (20)     1036 2023-05-22 17:34:01.597051 jintonic-0.2.3/PKG-INFO
--rw-r--r--   0 daedalus   (501) staff       (20)      659 2023-05-21 19:08:21.000000 jintonic-0.2.3/README.md
--rw-r--r--   0 daedalus   (501) staff       (20)      848 2023-05-22 17:33:51.000000 jintonic-0.2.3/pyproject.toml
--rw-r--r--   0 daedalus   (501) staff       (20)        0 2023-05-21 09:39:10.000000 jintonic-0.2.3/requirements.txt
--rw-r--r--   0 daedalus   (501) staff       (20)       38 2023-05-22 17:34:01.597226 jintonic-0.2.3/setup.cfg
-drwxr-xr-x   0 daedalus   (501) staff       (20)        0 2023-05-22 17:34:01.594329 jintonic-0.2.3/src/
-drwxr-xr-x   0 daedalus   (501) staff       (20)        0 2023-05-22 17:34:01.595709 jintonic-0.2.3/src/jintonic/
--rw-r--r--   0 daedalus   (501) staff       (20)      243 2023-05-21 09:39:35.000000 jintonic-0.2.3/src/jintonic/__init__.py
--rw-r--r--   0 daedalus   (501) staff       (20)       35 2023-05-21 09:39:35.000000 jintonic-0.2.3/src/jintonic/__main__.py
--rw-r--r--   0 daedalus   (501) staff       (20)     9898 2023-05-22 17:26:57.000000 jintonic-0.2.3/src/jintonic/chords.py
--rw-r--r--   0 daedalus   (501) staff       (20)     2876 2023-05-22 17:16:30.000000 jintonic-0.2.3/src/jintonic/harmonics.py
--rw-r--r--   0 daedalus   (501) staff       (20)    14037 2023-05-22 17:16:30.000000 jintonic-0.2.3/src/jintonic/intervals.py
--rw-r--r--   0 daedalus   (501) staff       (20)     7899 2023-05-22 17:16:30.000000 jintonic-0.2.3/src/jintonic/lattice.py
--rw-r--r--   0 daedalus   (501) staff       (20)     1773 2023-05-22 17:16:30.000000 jintonic-0.2.3/src/jintonic/primes.py
--rw-r--r--   0 daedalus   (501) staff       (20)    15260 2023-05-22 17:32:07.000000 jintonic-0.2.3/src/jintonic/scales.py
-drwxr-xr-x   0 daedalus   (501) staff       (20)        0 2023-05-22 17:34:01.596851 jintonic-0.2.3/src/jintonic.egg-info/
--rw-r--r--   0 daedalus   (501) staff       (20)     1036 2023-05-22 17:34:01.000000 jintonic-0.2.3/src/jintonic.egg-info/PKG-INFO
--rw-r--r--   0 daedalus   (501) staff       (20)      427 2023-05-22 17:34:01.000000 jintonic-0.2.3/src/jintonic.egg-info/SOURCES.txt
--rw-r--r--   0 daedalus   (501) staff       (20)        1 2023-05-22 17:34:01.000000 jintonic-0.2.3/src/jintonic.egg-info/dependency_links.txt
--rw-r--r--   0 daedalus   (501) staff       (20)       52 2023-05-22 17:34:01.000000 jintonic-0.2.3/src/jintonic.egg-info/entry_points.txt
--rw-r--r--   0 daedalus   (501) staff       (20)        9 2023-05-22 17:34:01.000000 jintonic-0.2.3/src/jintonic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:48:02.566449 jintonic-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-24 16:47:33.000000 jintonic-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-24 16:48:02.566449 jintonic-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-24 16:47:33.000000 jintonic-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-24 16:47:33.000000 jintonic-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:47:33.000000 jintonic-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:48:02.566449 jintonic-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:48:02.566449 jintonic-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:48:02.566449 jintonic-0.2.4/src/jintonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-24 16:47:33.000000 jintonic-0.2.4/src/jintonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 16:47:33.000000 jintonic-0.2.4/src/jintonic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-05-24 16:47:33.000000 jintonic-0.2.4/src/jintonic/chords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-24 16:47:33.000000 jintonic-0.2.4/src/jintonic/harmonics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14037 2023-05-24 16:47:33.000000 jintonic-0.2.4/src/jintonic/intervals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-05-24 16:47:33.000000 jintonic-0.2.4/src/jintonic/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-24 16:47:33.000000 jintonic-0.2.4/src/jintonic/primes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15260 2023-05-24 16:47:33.000000 jintonic-0.2.4/src/jintonic/scales.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:48:02.566449 jintonic-0.2.4/src/jintonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-24 16:48:02.000000 jintonic-0.2.4/src/jintonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-24 16:48:02.000000 jintonic-0.2.4/src/jintonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:48:02.000000 jintonic-0.2.4/src/jintonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-24 16:48:02.000000 jintonic-0.2.4/src/jintonic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 16:48:02.000000 jintonic-0.2.4/src/jintonic.egg-info/top_level.txt
```

### Comparing `jintonic-0.2.3/LICENSE` & `jintonic-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jintonic-0.2.3/PKG-INFO` & `jintonic-0.2.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jintonic
-Version: 0.2.3
+Version: 0.2.4
 Summary: Utilities for computer assisted composition in just intonation
 Author: Ismail Negm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -27,7 +27,11 @@
 [Just Intonation Primer](http://www.dbdoty.com/Words/Primer1.html).
 
 ## Installing
 
 ```
 pip install jintonic
 ```
+
+## Documentation
+
+[Full documentation is available here.](https://inegm.github.io/jintonic/)
```

### Comparing `jintonic-0.2.3/README.md` & `jintonic-0.2.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -14,8 +14,12 @@
 I strongly recommend his book :
 [Just Intonation Primer](http://www.dbdoty.com/Words/Primer1.html).
 
 ## Installing
 
 ```
 pip install jintonic
-```
+```
+
+## Documentation
+
+[Full documentation is available here.](https://inegm.github.io/jintonic/)
```

### Comparing `jintonic-0.2.3/pyproject.toml` & `jintonic-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jintonic-0.2.3/src/jintonic/chords.py` & `jintonic-0.2.4/src/jintonic/chords.py`

 * *Files identical despite different names*

### Comparing `jintonic-0.2.3/src/jintonic/harmonics.py` & `jintonic-0.2.4/src/jintonic/harmonics.py`

 * *Files identical despite different names*

### Comparing `jintonic-0.2.3/src/jintonic/intervals.py` & `jintonic-0.2.4/src/jintonic/intervals.py`

 * *Files identical despite different names*

### Comparing `jintonic-0.2.3/src/jintonic/lattice.py` & `jintonic-0.2.4/src/jintonic/lattice.py`

 * *Files identical despite different names*

### Comparing `jintonic-0.2.3/src/jintonic/primes.py` & `jintonic-0.2.4/src/jintonic/primes.py`

 * *Files identical despite different names*

### Comparing `jintonic-0.2.3/src/jintonic/scales.py` & `jintonic-0.2.4/src/jintonic/scales.py`

 * *Files identical despite different names*

### Comparing `jintonic-0.2.3/src/jintonic.egg-info/PKG-INFO` & `jintonic-0.2.4/src/jintonic.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jintonic
-Version: 0.2.3
+Version: 0.2.4
 Summary: Utilities for computer assisted composition in just intonation
 Author: Ismail Negm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -27,7 +27,11 @@
 [Just Intonation Primer](http://www.dbdoty.com/Words/Primer1.html).
 
 ## Installing
 
 ```
 pip install jintonic
 ```
+
+## Documentation
+
+[Full documentation is available here.](https://inegm.github.io/jintonic/)
```

