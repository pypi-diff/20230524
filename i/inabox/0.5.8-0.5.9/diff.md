# Comparing `tmp/inabox-0.5.8.tar.gz` & `tmp/inabox-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inabox-0.5.8.tar", max compression
+gzip compressed data, was "inabox-0.5.9.tar", max compression
```

## Comparing `inabox-0.5.8.tar` & `inabox-0.5.9.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-05-24 09:29:17.480400 inabox-0.5.8/LICENSE
--rw-r--r--   0        0        0     1036 2023-05-24 09:29:17.480400 inabox-0.5.8/inabox.py
--rw-r--r--   0        0        0      388 2023-05-24 09:29:17.484400 inabox-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 inabox-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-24 09:29:17.480400 inabox-0.5.9/LICENSE
+-rw-r--r--   0        0        0     1036 2023-05-24 09:29:17.480400 inabox-0.5.9/inabox.py
+-rw-r--r--   0        0        0     1680 2023-05-24 09:47:42.602812 inabox-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 inabox-0.5.9/PKG-INFO
```

### Comparing `inabox-0.5.8/inabox.py` & `inabox-0.5.9/inabox.py`

 * *Files identical despite different names*

### Comparing `inabox-0.5.8/PKG-INFO` & `inabox-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inabox
-Version: 0.5.8
+Version: 0.5.9
 Summary: Knowit Automation lifecycle management
 Home-page: https://inabox.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

