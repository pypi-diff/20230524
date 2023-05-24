# Comparing `tmp/vbimage-0.1.8.tar.gz` & `tmp/vbimage-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbimage-0.1.8.tar", max compression
+gzip compressed data, was "vbimage-0.1.9.tar", max compression
```

## Comparing `vbimage-0.1.8.tar` & `vbimage-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0        0 2023-03-19 12:51:54.741259 vbimage-0.1.8/README.md
--rw-r--r--   0        0        0      391 2023-03-24 12:02:36.540112 vbimage-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 12:51:54.741200 vbimage-0.1.8/vbimage/__init__.py
--rw-r--r--   0        0        0       55 2023-03-19 12:55:17.108021 vbimage-0.1.8/vbimage/__main__.py
--rw-r--r--   0        0        0     1193 2023-03-19 12:56:49.194174 vbimage-0.1.8/vbimage/info.py
--rw-r--r--   0        0        0      412 2023-03-22 19:08:15.338222 vbimage-0.1.8/vbimage/main.py
--rw-r--r--   0        0        0      864 2023-03-24 03:59:52.482676 vbimage-0.1.8/vbimage/pixelate.py
--rw-r--r--   0        0        0     1643 2023-03-24 12:02:13.266543 vbimage-0.1.8/vbimage/removebg.py
--rw-r--r--   0        0        0     1268 2023-03-21 04:02:13.822736 vbimage-0.1.8/vbimage/resize.py
--rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 vbimage-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-19 12:51:54.741259 vbimage-0.1.9/README.md
+-rw-r--r--   0        0        0      381 2023-03-24 15:26:40.362981 vbimage-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 12:51:54.741200 vbimage-0.1.9/vbimage/__init__.py
+-rw-r--r--   0        0        0       55 2023-03-19 12:55:17.108021 vbimage-0.1.9/vbimage/__main__.py
+-rw-r--r--   0        0        0      969 2023-03-24 15:25:30.123036 vbimage-0.1.9/vbimage/blur.py
+-rw-r--r--   0        0        0     1193 2023-03-19 12:56:49.194174 vbimage-0.1.9/vbimage/info.py
+-rw-r--r--   0        0        0      457 2023-03-24 15:25:07.363226 vbimage-0.1.9/vbimage/main.py
+-rw-r--r--   0        0        0      864 2023-03-24 03:59:52.482676 vbimage-0.1.9/vbimage/pixelate.py
+-rw-r--r--   0        0        0     1643 2023-03-24 12:02:13.266543 vbimage-0.1.9/vbimage/removebg.py
+-rw-r--r--   0        0        0     1268 2023-03-21 04:02:13.822736 vbimage-0.1.9/vbimage/resize.py
+-rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 vbimage-0.1.9/PKG-INFO
```

### Comparing `vbimage-0.1.8/vbimage/info.py` & `vbimage-0.1.9/vbimage/info.py`

 * *Files identical despite different names*

### Comparing `vbimage-0.1.8/vbimage/pixelate.py` & `vbimage-0.1.9/vbimage/pixelate.py`

 * *Files identical despite different names*

### Comparing `vbimage-0.1.8/vbimage/removebg.py` & `vbimage-0.1.9/vbimage/removebg.py`

 * *Files identical despite different names*

### Comparing `vbimage-0.1.8/vbimage/resize.py` & `vbimage-0.1.9/vbimage/resize.py`

 * *Files identical despite different names*

