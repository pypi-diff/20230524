# Comparing `tmp/py3d-0.0.91.tar.gz` & `tmp/py3d-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3d-0.0.91.tar", last modified: Mon May 22 17:31:58 2023, max compression
+gzip compressed data, was "py3d-0.0.92.tar", last modified: Wed May 24 01:03:14 2023, max compression
```

## Comparing `py3d-0.0.91.tar` & `py3d-0.0.92.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 17:31:58.946662 py3d-0.0.91/
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-22 17:31:58.946662 py3d-0.0.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-05-22 17:31:49.000000 py3d-0.0.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 17:31:58.946662 py3d-0.0.91/py3d/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-22 17:31:49.000000 py3d-0.0.91/py3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    26933 2023-05-22 17:31:49.000000 py3d-0.0.91/py3d/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    22511 2023-05-22 17:31:49.000000 py3d-0.0.91/py3d/viewer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 17:31:58.946662 py3d-0.0.91/py3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-22 17:31:58.000000 py3d-0.0.91/py3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-22 17:31:58.000000 py3d-0.0.91/py3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 17:31:58.000000 py3d-0.0.91/py3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-22 17:31:58.000000 py3d-0.0.91/py3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-22 17:31:58.000000 py3d-0.0.91/py3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 17:31:58.946662 py3d-0.0.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-22 17:31:49.000000 py3d-0.0.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 01:03:14.742548 py3d-0.0.92/
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-24 01:03:14.742548 py3d-0.0.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-05-24 01:03:04.000000 py3d-0.0.92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 01:03:14.742548 py3d-0.0.92/py3d/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-24 01:03:04.000000 py3d-0.0.92/py3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26933 2023-05-24 01:03:04.000000 py3d-0.0.92/py3d/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22243 2023-05-24 01:03:04.000000 py3d-0.0.92/py3d/viewer.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 01:03:14.742548 py3d-0.0.92/py3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-24 01:03:14.000000 py3d-0.0.92/py3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-24 01:03:14.000000 py3d-0.0.92/py3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 01:03:14.000000 py3d-0.0.92/py3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-24 01:03:14.000000 py3d-0.0.92/py3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-24 01:03:14.000000 py3d-0.0.92/py3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-24 01:03:14.742548 py3d-0.0.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-24 01:03:04.000000 py3d-0.0.92/setup.py
```

### Comparing `py3d-0.0.91/PKG-INFO` & `py3d-0.0.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.0.91
+Version: 0.0.92
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.0.91/README.md` & `py3d-0.0.92/README.md`

 * *Files identical despite different names*

### Comparing `py3d-0.0.91/py3d/core.py` & `py3d-0.0.92/py3d/core.py`

 * *Files identical despite different names*

### Comparing `py3d-0.0.91/py3d/viewer.html` & `py3d-0.0.92/py3d/viewer.html`

 * *Files 0% similar despite different names*

```diff
@@ -93,27 +93,19 @@
             let x = array.filter((v, i) => i % 3 == 0)
             let y = array.filter((v, i) => i % 3 == 1)
             let z = array.filter((v, i) => i % 3 == 2)
             return [Math.min(...x), Math.max(...x), Math.min(...y), Math.max(...y), Math.min(...z), Math.max(...z)]
         }
         static ticks(min, max, step) {
             if (max <= min) {
-                return [[min], min, max, 0]
+                return [[min], min, max]
             }
             let dig = Math.round(Math.log10(step))
-            let tick_min = min - min % step
-            if (min < tick_min) {
-                tick_min -= step
-            }
-            let tick_max = max - max % step
-            if (max > tick_max) {
-                tick_max += step
-            }
-            let size = Math.ceil((tick_max - tick_min) / step) + 1
-            let ticks = Array.from({ length: size }, (v, i) => Number((tick_min + step * i).toFixed(Math.max(-dig, 0))))
+            let size = Math.ceil((max - min) / step) + 1
+            let ticks = Array.from({ length: size }, (v, i) => Number((min + step * i).toFixed(Math.max(-dig, 0))))
             return [ticks, ticks[0], ticks[ticks.length - 1]]
         }
     }
     class Camera {
         PERSPECTIVE = "P"
         ORTHOGRAPHIC = "O"
         constructor(type, fovy, aspect, near, far, min, max) {
```

### Comparing `py3d-0.0.91/py3d.egg-info/PKG-INFO` & `py3d-0.0.92/py3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.0.91
+Version: 0.0.92
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.0.91/setup.py` & `py3d-0.0.92/setup.py`

 * *Files identical despite different names*

