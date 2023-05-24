# Comparing `tmp/yze-0.0.2.tar.gz` & `tmp/yze-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yze-0.0.2.tar", last modified: Thu Apr 27 12:56:11 2023, max compression
+gzip compressed data, was "yze-0.0.4.tar", last modified: Wed May 24 12:15:33 2023, max compression
```

## Comparing `yze-0.0.2.tar` & `yze-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-27 12:56:11.003690 yze-0.0.2/
--rw-r--r--   0 nicolas    (501) staff       (20)     4123 2023-04-27 12:56:11.003570 yze-0.0.2/PKG-INFO
--rw-r--r--   0 nicolas    (501) staff       (20)     3625 2023-04-27 12:53:16.000000 yze-0.0.2/README.md
--rw-r--r--   0 nicolas    (501) staff       (20)      735 2023-04-27 12:53:55.000000 yze-0.0.2/pyproject.toml
--rw-r--r--   0 nicolas    (501) staff       (20)       38 2023-04-27 12:56:11.003722 yze-0.0.2/setup.cfg
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-27 12:56:11.001676 yze-0.0.2/src/
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-27 12:56:11.002647 yze-0.0.2/src/yze/
--rw-r--r--   0 nicolas    (501) staff       (20)        0 2023-04-17 19:54:16.000000 yze-0.0.2/src/yze/__init__.py
--rw-r--r--   0 nicolas    (501) staff       (20)     4193 2023-04-24 07:10:59.000000 yze-0.0.2/src/yze/benchmark_mutant.py
--rw-r--r--   0 nicolas    (501) staff       (20)     9364 2023-04-25 11:31:30.000000 yze-0.0.2/src/yze/dice.py
--rw-r--r--   0 nicolas    (501) staff       (20)     5162 2023-04-27 12:49:37.000000 yze-0.0.2/src/yze/mutant_odds_of_pushing.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-27 12:56:11.003275 yze-0.0.2/src/yze.egg-info/
--rw-r--r--   0 nicolas    (501) staff       (20)     4123 2023-04-27 12:56:10.000000 yze-0.0.2/src/yze.egg-info/PKG-INFO
--rw-r--r--   0 nicolas    (501) staff       (20)      303 2023-04-27 12:56:11.000000 yze-0.0.2/src/yze.egg-info/SOURCES.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-04-27 12:56:10.000000 yze-0.0.2/src/yze.egg-info/dependency_links.txt
--rw-r--r--   0 nicolas    (501) staff       (20)      120 2023-04-27 12:56:10.000000 yze-0.0.2/src/yze.egg-info/entry_points.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        4 2023-04-27 12:56:10.000000 yze-0.0.2/src/yze.egg-info/top_level.txt
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-27 12:56:11.003394 yze-0.0.2/tests/
--rw-r--r--   0 nicolas    (501) staff       (20)     1988 2023-04-27 11:06:19.000000 yze-0.0.2/tests/test_yze_dice.py
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-24 12:15:33.906108 yze-0.0.4/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4123 2023-05-24 12:15:33.906108 yze-0.0.4/PKG-INFO
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     3625 2023-05-24 12:10:16.000000 yze-0.0.4/README.md
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      735 2023-05-24 12:10:58.000000 yze-0.0.4/pyproject.toml
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)       38 2023-05-24 12:15:33.906108 yze-0.0.4/setup.cfg
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-24 12:15:33.894107 yze-0.0.4/src/
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-24 12:15:33.906108 yze-0.0.4/src/yze/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4193 2023-04-26 10:10:00.000000 yze-0.0.4/src/yze/benchmark_mutant.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)    17913 2023-05-24 12:08:52.000000 yze-0.0.4/src/yze/dice.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     5162 2023-05-24 11:38:28.000000 yze-0.0.4/src/yze/mutant_odds_of_pushing.py
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-24 12:15:33.906108 yze-0.0.4/src/yze.egg-info/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4123 2023-05-24 12:15:33.000000 yze-0.0.4/src/yze.egg-info/PKG-INFO
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      283 2023-05-24 12:15:33.000000 yze-0.0.4/src/yze.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)        1 2023-05-24 12:15:33.000000 yze-0.0.4/src/yze.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      120 2023-05-24 12:15:33.000000 yze-0.0.4/src/yze.egg-info/entry_points.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)        4 2023-05-24 12:15:33.000000 yze-0.0.4/src/yze.egg-info/top_level.txt
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-24 12:15:33.906108 yze-0.0.4/tests/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     3611 2023-05-24 11:53:49.000000 yze-0.0.4/tests/test_yze_dice.py
```

### Comparing `yze-0.0.2/PKG-INFO` & `yze-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yze
-Version: 0.0.2
+Version: 0.0.4
 Summary: A small package to handle YZE games mechanics
 Author-email: Nicolas Legrand <nicolas.legrand@gmail.com>
 Project-URL: Homepage, https://github.com/nlegrand/yze
 Project-URL: Bug Tracker, https://github.com/nlegrand/yze/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
@@ -13,17 +13,17 @@
 
 The main goal of this Python library is to propose an object to emulate
 Year Zero Engine dice throwing.
 
 # System supported:
 - [X] Mutant: Year Zero
 - [X] Forbidden Lands
-- [ ] Twilight 2000
+- [X] Twilight 2000
 - [X] Alien
-- [ ] Blade Runner
+- [X] Blade Runner
 
 # Example
 ```
 . my_py_venv/bin/activate
 git clone https://github.com/nlegrand/yze.git
 cd yze
 python -m pip install -e .
```

### Comparing `yze-0.0.2/README.md` & `yze-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 The main goal of this Python library is to propose an object to emulate
 Year Zero Engine dice throwing.
 
 # System supported:
 - [X] Mutant: Year Zero
 - [X] Forbidden Lands
-- [ ] Twilight 2000
+- [X] Twilight 2000
 - [X] Alien
-- [ ] Blade Runner
+- [X] Blade Runner
 
 # Example
 ```
 . my_py_venv/bin/activate
 git clone https://github.com/nlegrand/yze.git
 cd yze
 python -m pip install -e .
```

### Comparing `yze-0.0.2/pyproject.toml` & `yze-0.0.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "yze"
-version = "0.0.2"
+version = "0.0.4"
 authors = [
   { name="Nicolas Legrand", email="nicolas.legrand@gmail.com" },
 ]
 description = "A small package to handle YZE games mechanics"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `yze-0.0.2/src/yze/benchmark_mutant.py` & `yze-0.0.4/src/yze/benchmark_mutant.py`

 * *Files identical despite different names*

### Comparing `yze-0.0.2/src/yze/mutant_odds_of_pushing.py` & `yze-0.0.4/src/yze/mutant_odds_of_pushing.py`

 * *Files identical despite different names*

### Comparing `yze-0.0.2/src/yze.egg-info/PKG-INFO` & `yze-0.0.4/src/yze.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yze
-Version: 0.0.2
+Version: 0.0.4
 Summary: A small package to handle YZE games mechanics
 Author-email: Nicolas Legrand <nicolas.legrand@gmail.com>
 Project-URL: Homepage, https://github.com/nlegrand/yze
 Project-URL: Bug Tracker, https://github.com/nlegrand/yze/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
@@ -13,17 +13,17 @@
 
 The main goal of this Python library is to propose an object to emulate
 Year Zero Engine dice throwing.
 
 # System supported:
 - [X] Mutant: Year Zero
 - [X] Forbidden Lands
-- [ ] Twilight 2000
+- [X] Twilight 2000
 - [X] Alien
-- [ ] Blade Runner
+- [X] Blade Runner
 
 # Example
 ```
 . my_py_venv/bin/activate
 git clone https://github.com/nlegrand/yze.git
 cd yze
 python -m pip install -e .
```

