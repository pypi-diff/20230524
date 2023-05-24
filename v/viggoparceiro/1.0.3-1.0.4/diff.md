# Comparing `tmp/viggoparceiro-1.0.3.tar.gz` & `tmp/viggoparceiro-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viggoparceiro-1.0.3.tar", last modified: Tue Mar 14 16:49:41 2023, max compression
+gzip compressed data, was "viggoparceiro-1.0.4.tar", last modified: Tue Mar 14 17:52:30 2023, max compression
```

## Comparing `viggoparceiro-1.0.3.tar` & `viggoparceiro-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:49:41.635323 viggoparceiro-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-14 16:48:53.000000 viggoparceiro-1.0.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-14 16:48:53.000000 viggoparceiro-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-14 16:49:41.635323 viggoparceiro-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-14 16:48:53.000000 viggoparceiro-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 16:49:41.635323 viggoparceiro-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-14 16:48:53.000000 viggoparceiro-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:49:41.631323 viggoparceiro-1.0.3/viggoparceiro/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-03-14 16:48:53.000000 viggoparceiro-1.0.3/viggoparceiro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-14 16:48:53.000000 viggoparceiro-1.0.3/viggoparceiro/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:49:41.631323 viggoparceiro-1.0.3/viggoparceiro/subsystem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 16:48:53.000000 viggoparceiro-1.0.3/viggoparceiro/subsystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:49:41.635323 viggoparceiro-1.0.3/viggoparceiro/subsystem/parceiro/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-14 16:48:53.000000 viggoparceiro-1.0.3/viggoparceiro/subsystem/parceiro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-14 16:48:53.000000 viggoparceiro-1.0.3/viggoparceiro/subsystem/parceiro/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-03-14 16:48:53.000000 viggoparceiro-1.0.3/viggoparceiro/subsystem/parceiro/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:49:41.635323 viggoparceiro-1.0.3/viggoparceiro/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 16:48:53.000000 viggoparceiro-1.0.3/viggoparceiro/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:49:41.635323 viggoparceiro-1.0.3/viggoparceiro/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-14 16:48:53.000000 viggoparceiro-1.0.3/viggoparceiro/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-03-14 16:48:53.000000 viggoparceiro-1.0.3/viggoparceiro/tests/functional/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:49:41.631323 viggoparceiro-1.0.3/viggoparceiro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-14 16:49:41.000000 viggoparceiro-1.0.3/viggoparceiro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-14 16:49:41.000000 viggoparceiro-1.0.3/viggoparceiro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 16:49:41.000000 viggoparceiro-1.0.3/viggoparceiro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-14 16:49:41.000000 viggoparceiro-1.0.3/viggoparceiro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-14 16:49:41.000000 viggoparceiro-1.0.3/viggoparceiro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 17:52:30.776719 viggoparceiro-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-14 17:51:49.000000 viggoparceiro-1.0.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-14 17:51:49.000000 viggoparceiro-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-14 17:52:30.776719 viggoparceiro-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-14 17:51:49.000000 viggoparceiro-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 17:52:30.776719 viggoparceiro-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-14 17:51:49.000000 viggoparceiro-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 17:52:30.776719 viggoparceiro-1.0.4/viggoparceiro/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-03-14 17:51:49.000000 viggoparceiro-1.0.4/viggoparceiro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-14 17:51:49.000000 viggoparceiro-1.0.4/viggoparceiro/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 17:52:30.776719 viggoparceiro-1.0.4/viggoparceiro/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 17:51:49.000000 viggoparceiro-1.0.4/viggoparceiro/subsystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 17:52:30.776719 viggoparceiro-1.0.4/viggoparceiro/subsystem/parceiro/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-14 17:51:49.000000 viggoparceiro-1.0.4/viggoparceiro/subsystem/parceiro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-14 17:51:49.000000 viggoparceiro-1.0.4/viggoparceiro/subsystem/parceiro/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-03-14 17:51:49.000000 viggoparceiro-1.0.4/viggoparceiro/subsystem/parceiro/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 17:52:30.776719 viggoparceiro-1.0.4/viggoparceiro/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 17:51:49.000000 viggoparceiro-1.0.4/viggoparceiro/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 17:52:30.776719 viggoparceiro-1.0.4/viggoparceiro/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-14 17:51:49.000000 viggoparceiro-1.0.4/viggoparceiro/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-03-14 17:51:49.000000 viggoparceiro-1.0.4/viggoparceiro/tests/functional/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 17:52:30.776719 viggoparceiro-1.0.4/viggoparceiro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-14 17:52:30.000000 viggoparceiro-1.0.4/viggoparceiro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-14 17:52:30.000000 viggoparceiro-1.0.4/viggoparceiro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 17:52:30.000000 viggoparceiro-1.0.4/viggoparceiro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-14 17:52:30.000000 viggoparceiro-1.0.4/viggoparceiro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-14 17:52:30.000000 viggoparceiro-1.0.4/viggoparceiro.egg-info/top_level.txt
```

### Comparing `viggoparceiro-1.0.3/viggoparceiro/__init__.py` & `viggoparceiro-1.0.4/viggoparceiro/__init__.py`

 * *Files identical despite different names*

### Comparing `viggoparceiro-1.0.3/viggoparceiro/subsystem/parceiro/resource.py` & `viggoparceiro-1.0.4/viggoparceiro/subsystem/parceiro/resource.py`

 * *Files identical despite different names*

### Comparing `viggoparceiro-1.0.3/viggoparceiro/tests/functional/fixtures.py` & `viggoparceiro-1.0.4/viggoparceiro/tests/functional/fixtures.py`

 * *Files identical despite different names*

### Comparing `viggoparceiro-1.0.3/viggoparceiro.egg-info/SOURCES.txt` & `viggoparceiro-1.0.4/viggoparceiro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

