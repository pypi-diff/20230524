# Comparing `tmp/flashy-0.0.1.tar.gz` & `tmp/flashy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashy-0.0.1.tar", last modified: Tue May 23 14:40:50 2023, max compression
+gzip compressed data, was "flashy-0.0.2.tar", last modified: Wed May 24 19:48:56 2023, max compression
```

## Comparing `flashy-0.0.1.tar` & `flashy-0.0.2.tar`

### file list

```diff
@@ -1,40 +1,75 @@
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-23 14:40:50.628027 flashy-0.0.1/
--rw-r--r--   0 defossez   (501) staff       (20)     1087 2023-01-26 18:22:48.000000 flashy-0.0.1/LICENSE
--rw-r--r--   0 defossez   (501) staff       (20)     7824 2023-05-23 14:40:50.628492 flashy-0.0.1/PKG-INFO
--rw-r--r--   0 defossez   (501) staff       (20)     6011 2023-01-26 18:22:52.000000 flashy-0.0.1/README.md
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-23 14:40:50.589435 flashy-0.0.1/flashy/
--rw-r--r--   0 defossez   (501) staff       (20)      436 2023-05-23 14:38:02.000000 flashy-0.0.1/flashy/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     3690 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/adversarial.py
--rw-r--r--   0 defossez   (501) staff       (20)     9899 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/distrib.py
--rw-r--r--   0 defossez   (501) staff       (20)     3531 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/formatter.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-23 14:40:50.617684 flashy-0.0.1/flashy/loggers/
--rw-r--r--   0 defossez   (501) staff       (20)      322 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/loggers/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     3692 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/loggers/base.py
--rw-r--r--   0 defossez   (501) staff       (20)     6836 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/loggers/localfs.py
--rw-r--r--   0 defossez   (501) staff       (20)     8183 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/loggers/tensorboard.py
--rw-r--r--   0 defossez   (501) staff       (20)     4667 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/loggers/utils.py
--rw-r--r--   0 defossez   (501) staff       (20)     8616 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/loggers/wandb.py
--rw-r--r--   0 defossez   (501) staff       (20)    11939 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/logging.py
--rw-r--r--   0 defossez   (501) staff       (20)        0 2022-06-20 16:51:50.000000 flashy-0.0.1/flashy/py.typed
--rw-r--r--   0 defossez   (501) staff       (20)     8336 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/solver.py
--rw-r--r--   0 defossez   (501) staff       (20)     2633 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/state.py
--rw-r--r--   0 defossez   (501) staff       (20)     2159 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/utils.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-23 14:40:50.612441 flashy-0.0.1/flashy.egg-info/
--rw-r--r--   0 defossez   (501) staff       (20)     7824 2023-05-23 14:40:50.000000 flashy-0.0.1/flashy.egg-info/PKG-INFO
--rw-r--r--   0 defossez   (501) staff       (20)      686 2023-05-23 14:40:50.000000 flashy-0.0.1/flashy.egg-info/SOURCES.txt
--rw-r--r--   0 defossez   (501) staff       (20)        1 2023-05-23 14:40:50.000000 flashy-0.0.1/flashy.egg-info/dependency_links.txt
--rw-r--r--   0 defossez   (501) staff       (20)       85 2023-05-23 14:40:50.000000 flashy-0.0.1/flashy.egg-info/requires.txt
--rw-r--r--   0 defossez   (501) staff       (20)       13 2023-05-23 14:40:50.000000 flashy-0.0.1/flashy.egg-info/top_level.txt
--rw-r--r--   0 defossez   (501) staff       (20)       50 2023-01-03 13:51:29.000000 flashy-0.0.1/pyproject.toml
--rw-r--r--   0 defossez   (501) staff       (20)      100 2023-05-23 14:40:50.630323 flashy-0.0.1/setup.cfg
--rw-r--r--   0 defossez   (501) staff       (20)     1769 2023-01-26 18:22:48.000000 flashy-0.0.1/setup.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-23 14:40:50.624652 flashy-0.0.1/tests/
--rw-r--r--   0 defossez   (501) staff       (20)      198 2023-01-26 18:22:48.000000 flashy-0.0.1/tests/__init__.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-23 14:40:50.627197 flashy-0.0.1/tests/dummy/
--rw-r--r--   0 defossez   (501) staff       (20)      198 2023-01-26 18:22:48.000000 flashy-0.0.1/tests/dummy/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     3733 2023-01-26 18:22:48.000000 flashy-0.0.1/tests/dummy/train.py
--rw-r--r--   0 defossez   (501) staff       (20)     2708 2023-01-26 18:22:48.000000 flashy-0.0.1/tests/test_distrib.py
--rw-r--r--   0 defossez   (501) staff       (20)      198 2023-01-26 18:22:48.000000 flashy-0.0.1/tests/test_formatter.py
--rw-r--r--   0 defossez   (501) staff       (20)      879 2023-01-26 18:22:48.000000 flashy-0.0.1/tests/test_integ.py
--rw-r--r--   0 defossez   (501) staff       (20)      197 2023-01-26 18:22:48.000000 flashy-0.0.1/tests/test_solver.py
--rw-r--r--   0 defossez   (501) staff       (20)      197 2023-01-26 18:22:48.000000 flashy-0.0.1/tests/test_state.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-24 19:48:56.383854 flashy-0.0.2/
+-rw-r--r--   0 defossez   (501) staff       (20)      319 2023-05-24 19:48:53.000000 flashy-0.0.2/CHANGELOG.md
+-rw-r--r--   0 defossez   (501) staff       (20)     3355 2023-01-03 11:31:00.000000 flashy-0.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 defossez   (501) staff       (20)      579 2023-01-03 11:31:37.000000 flashy-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0 defossez   (501) staff       (20)     1087 2023-01-26 18:22:48.000000 flashy-0.0.2/LICENSE
+-rw-r--r--   0 defossez   (501) staff       (20)      191 2023-05-24 19:48:22.000000 flashy-0.0.2/MANIFEST.in
+-rw-r--r--   0 defossez   (501) staff       (20)      621 2023-05-23 14:40:47.000000 flashy-0.0.2/Makefile
+-rw-r--r--   0 defossez   (501) staff       (20)     7824 2023-05-24 19:48:56.384188 flashy-0.0.2/PKG-INFO
+-rw-r--r--   0 defossez   (501) staff       (20)     6011 2023-01-26 18:22:52.000000 flashy-0.0.2/README.md
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-24 19:48:56.309415 flashy-0.0.2/docs/
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-24 19:48:56.335776 flashy-0.0.2/docs/flashy/
+-rw-r--r--   0 defossez   (501) staff       (20)    20174 2022-08-04 16:04:15.000000 flashy-0.0.2/docs/flashy/adversarial.html
+-rw-r--r--   0 defossez   (501) staff       (20)    25247 2022-08-04 16:04:15.000000 flashy-0.0.2/docs/flashy/distrib.html
+-rw-r--r--   0 defossez   (501) staff       (20)    16189 2022-08-04 16:04:15.000000 flashy-0.0.2/docs/flashy/formatter.html
+-rw-r--r--   0 defossez   (501) staff       (20)     8969 2022-08-04 16:04:15.000000 flashy-0.0.2/docs/flashy/index.html
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-24 19:48:56.342416 flashy-0.0.2/docs/flashy/loggers/
+-rw-r--r--   0 defossez   (501) staff       (20)    25622 2022-08-04 16:04:15.000000 flashy-0.0.2/docs/flashy/loggers/base.html
+-rw-r--r--   0 defossez   (501) staff       (20)     7799 2022-08-04 16:04:15.000000 flashy-0.0.2/docs/flashy/loggers/index.html
+-rw-r--r--   0 defossez   (501) staff       (20)    24215 2022-08-04 16:04:15.000000 flashy-0.0.2/docs/flashy/loggers/localfs.html
+-rw-r--r--   0 defossez   (501) staff       (20)    28211 2022-08-04 16:04:15.000000 flashy-0.0.2/docs/flashy/loggers/tensorboard.html
+-rw-r--r--   0 defossez   (501) staff       (20)    10703 2022-08-04 16:04:15.000000 flashy-0.0.2/docs/flashy/loggers/utils.html
+-rw-r--r--   0 defossez   (501) staff       (20)    32096 2022-08-04 16:04:15.000000 flashy-0.0.2/docs/flashy/loggers/wandb.html
+-rw-r--r--   0 defossez   (501) staff       (20)    48569 2022-08-04 16:04:15.000000 flashy-0.0.2/docs/flashy/logging.html
+-rw-r--r--   0 defossez   (501) staff       (20)    44415 2022-08-04 16:04:15.000000 flashy-0.0.2/docs/flashy/solver.html
+-rw-r--r--   0 defossez   (501) staff       (20)    30803 2022-08-04 16:04:15.000000 flashy-0.0.2/docs/flashy/state.html
+-rw-r--r--   0 defossez   (501) staff       (20)    11072 2022-08-04 16:04:15.000000 flashy-0.0.2/docs/flashy/utils.html
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-24 19:48:56.311091 flashy-0.0.2/examples/
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-24 19:48:56.344319 flashy-0.0.2/examples/basic/
+-rw-r--r--   0 defossez   (501) staff       (20)      198 2023-01-26 18:22:48.000000 flashy-0.0.2/examples/basic/__init__.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-24 19:48:56.345186 flashy-0.0.2/examples/basic/config/
+-rw-r--r--   0 defossez   (501) staff       (20)      132 2022-08-18 13:00:16.000000 flashy-0.0.2/examples/basic/config/config.yaml
+-rw-r--r--   0 defossez   (501) staff       (20)     1973 2023-01-26 18:22:48.000000 flashy-0.0.2/examples/basic/train.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-24 19:48:56.348059 flashy-0.0.2/examples/cifar/
+-rw-r--r--   0 defossez   (501) staff       (20)      198 2023-01-26 18:22:48.000000 flashy-0.0.2/examples/cifar/__init__.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-24 19:48:56.349378 flashy-0.0.2/examples/cifar/config/
+-rw-r--r--   0 defossez   (501) staff       (20)      222 2022-08-18 13:00:16.000000 flashy-0.0.2/examples/cifar/config/config.yaml
+-rw-r--r--   0 defossez   (501) staff       (20)     2176 2023-01-26 18:22:48.000000 flashy-0.0.2/examples/cifar/solver.py
+-rw-r--r--   0 defossez   (501) staff       (20)     1903 2023-01-26 18:22:48.000000 flashy-0.0.2/examples/cifar/train.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-24 19:48:56.358884 flashy-0.0.2/flashy/
+-rw-r--r--   0 defossez   (501) staff       (20)      436 2023-05-24 19:48:36.000000 flashy-0.0.2/flashy/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)     3690 2023-01-26 18:22:48.000000 flashy-0.0.2/flashy/adversarial.py
+-rw-r--r--   0 defossez   (501) staff       (20)     9899 2023-01-26 18:22:48.000000 flashy-0.0.2/flashy/distrib.py
+-rw-r--r--   0 defossez   (501) staff       (20)     3531 2023-01-26 18:22:48.000000 flashy-0.0.2/flashy/formatter.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-24 19:48:56.372185 flashy-0.0.2/flashy/loggers/
+-rw-r--r--   0 defossez   (501) staff       (20)      322 2023-01-26 18:22:48.000000 flashy-0.0.2/flashy/loggers/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)     3692 2023-01-26 18:22:48.000000 flashy-0.0.2/flashy/loggers/base.py
+-rw-r--r--   0 defossez   (501) staff       (20)     6836 2023-01-26 18:22:48.000000 flashy-0.0.2/flashy/loggers/localfs.py
+-rw-r--r--   0 defossez   (501) staff       (20)     8183 2023-01-26 18:22:48.000000 flashy-0.0.2/flashy/loggers/tensorboard.py
+-rw-r--r--   0 defossez   (501) staff       (20)     4667 2023-01-26 18:22:48.000000 flashy-0.0.2/flashy/loggers/utils.py
+-rw-r--r--   0 defossez   (501) staff       (20)     8616 2023-01-26 18:22:48.000000 flashy-0.0.2/flashy/loggers/wandb.py
+-rw-r--r--   0 defossez   (501) staff       (20)    11939 2023-01-26 18:22:48.000000 flashy-0.0.2/flashy/logging.py
+-rw-r--r--   0 defossez   (501) staff       (20)        0 2022-06-20 16:51:50.000000 flashy-0.0.2/flashy/py.typed
+-rw-r--r--   0 defossez   (501) staff       (20)     8336 2023-01-26 18:22:48.000000 flashy-0.0.2/flashy/solver.py
+-rw-r--r--   0 defossez   (501) staff       (20)     2633 2023-01-26 18:22:48.000000 flashy-0.0.2/flashy/state.py
+-rw-r--r--   0 defossez   (501) staff       (20)     2159 2023-01-26 18:22:48.000000 flashy-0.0.2/flashy/utils.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-24 19:48:56.366116 flashy-0.0.2/flashy.egg-info/
+-rw-r--r--   0 defossez   (501) staff       (20)     7824 2023-05-24 19:48:56.000000 flashy-0.0.2/flashy.egg-info/PKG-INFO
+-rw-r--r--   0 defossez   (501) staff       (20)     1359 2023-05-24 19:48:56.000000 flashy-0.0.2/flashy.egg-info/SOURCES.txt
+-rw-r--r--   0 defossez   (501) staff       (20)        1 2023-05-24 19:48:56.000000 flashy-0.0.2/flashy.egg-info/dependency_links.txt
+-rw-r--r--   0 defossez   (501) staff       (20)       85 2023-05-24 19:48:56.000000 flashy-0.0.2/flashy.egg-info/requires.txt
+-rw-r--r--   0 defossez   (501) staff       (20)       13 2023-05-24 19:48:56.000000 flashy-0.0.2/flashy.egg-info/top_level.txt
+-rw-r--r--   0 defossez   (501) staff       (20)       50 2023-01-03 13:51:29.000000 flashy-0.0.2/pyproject.toml
+-rw-r--r--   0 defossez   (501) staff       (20)       33 2023-05-23 14:37:47.000000 flashy-0.0.2/requirements.txt
+-rw-r--r--   0 defossez   (501) staff       (20)      100 2023-05-24 19:48:56.385215 flashy-0.0.2/setup.cfg
+-rw-r--r--   0 defossez   (501) staff       (20)     1769 2023-01-26 18:22:48.000000 flashy-0.0.2/setup.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-24 19:48:56.380789 flashy-0.0.2/tests/
+-rw-r--r--   0 defossez   (501) staff       (20)      198 2023-01-26 18:22:48.000000 flashy-0.0.2/tests/__init__.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-24 19:48:56.383012 flashy-0.0.2/tests/dummy/
+-rw-r--r--   0 defossez   (501) staff       (20)      198 2023-01-26 18:22:48.000000 flashy-0.0.2/tests/dummy/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)     3733 2023-01-26 18:22:48.000000 flashy-0.0.2/tests/dummy/train.py
+-rw-r--r--   0 defossez   (501) staff       (20)     2708 2023-01-26 18:22:48.000000 flashy-0.0.2/tests/test_distrib.py
+-rw-r--r--   0 defossez   (501) staff       (20)      198 2023-01-26 18:22:48.000000 flashy-0.0.2/tests/test_formatter.py
+-rw-r--r--   0 defossez   (501) staff       (20)      879 2023-01-26 18:22:48.000000 flashy-0.0.2/tests/test_integ.py
+-rw-r--r--   0 defossez   (501) staff       (20)      197 2023-01-26 18:22:48.000000 flashy-0.0.2/tests/test_solver.py
+-rw-r--r--   0 defossez   (501) staff       (20)      197 2023-01-26 18:22:48.000000 flashy-0.0.2/tests/test_state.py
```

### Comparing `flashy-0.0.1/LICENSE` & `flashy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flashy-0.0.1/PKG-INFO` & `flashy-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Minimal solver for deep learning
 Home-page: https://github.com/fairinternal/flashy
 Author: Alexandre Défossez
 Author-email: defossez@fb.com
 License: MIT
 Description: 
         # Flashy
```

### Comparing `flashy-0.0.1/README.md` & `flashy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `flashy-0.0.1/flashy/adversarial.py` & `flashy-0.0.2/flashy/adversarial.py`

 * *Files identical despite different names*

### Comparing `flashy-0.0.1/flashy/distrib.py` & `flashy-0.0.2/flashy/distrib.py`

 * *Files identical despite different names*

### Comparing `flashy-0.0.1/flashy/formatter.py` & `flashy-0.0.2/flashy/formatter.py`

 * *Files identical despite different names*

### Comparing `flashy-0.0.1/flashy/loggers/base.py` & `flashy-0.0.2/flashy/loggers/base.py`

 * *Files identical despite different names*

### Comparing `flashy-0.0.1/flashy/loggers/localfs.py` & `flashy-0.0.2/flashy/loggers/localfs.py`

 * *Files identical despite different names*

### Comparing `flashy-0.0.1/flashy/loggers/tensorboard.py` & `flashy-0.0.2/flashy/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flashy-0.0.1/flashy/loggers/utils.py` & `flashy-0.0.2/flashy/loggers/utils.py`

 * *Files identical despite different names*

### Comparing `flashy-0.0.1/flashy/loggers/wandb.py` & `flashy-0.0.2/flashy/loggers/wandb.py`

 * *Files identical despite different names*

### Comparing `flashy-0.0.1/flashy/logging.py` & `flashy-0.0.2/flashy/logging.py`

 * *Files identical despite different names*

### Comparing `flashy-0.0.1/flashy/solver.py` & `flashy-0.0.2/flashy/solver.py`

 * *Files identical despite different names*

### Comparing `flashy-0.0.1/flashy/state.py` & `flashy-0.0.2/flashy/state.py`

 * *Files identical despite different names*

### Comparing `flashy-0.0.1/flashy/utils.py` & `flashy-0.0.2/flashy/utils.py`

 * *Files identical despite different names*

### Comparing `flashy-0.0.1/flashy.egg-info/PKG-INFO` & `flashy-0.0.2/flashy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Minimal solver for deep learning
 Home-page: https://github.com/fairinternal/flashy
 Author: Alexandre Défossez
 Author-email: defossez@fb.com
 License: MIT
 Description: 
         # Flashy
```

### Comparing `flashy-0.0.1/setup.py` & `flashy-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `flashy-0.0.1/tests/dummy/train.py` & `flashy-0.0.2/tests/dummy/train.py`

 * *Files identical despite different names*

### Comparing `flashy-0.0.1/tests/test_distrib.py` & `flashy-0.0.2/tests/test_distrib.py`

 * *Files identical despite different names*

### Comparing `flashy-0.0.1/tests/test_integ.py` & `flashy-0.0.2/tests/test_integ.py`

 * *Files identical despite different names*

