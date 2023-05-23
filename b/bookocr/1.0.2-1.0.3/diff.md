# Comparing `tmp/bookocr-1.0.2.tar.gz` & `tmp/bookocr-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookocr-1.0.2.tar", last modified: Tue May 23 03:43:48 2023, max compression
+gzip compressed data, was "bookocr-1.0.3.tar", last modified: Tue May 23 23:14:55 2023, max compression
```

## Comparing `bookocr-1.0.2.tar` & `bookocr-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 03:43:48.542777 bookocr-1.0.2/
--rw-rw-rw-   0        0        0     1092 2023-05-22 23:35:20.000000 bookocr-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1452 2023-05-23 03:43:48.540774 bookocr-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      973 2023-05-23 00:41:08.000000 bookocr-1.0.2/README.md
--rw-rw-rw-   0        0        0      840 2023-05-23 03:42:58.000000 bookocr-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 03:43:48.542777 bookocr-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 03:43:48.376852 bookocr-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 03:43:48.500089 bookocr-1.0.2/src/bookocr/
--rw-rw-rw-   0        0        0       45 2023-05-16 15:03:36.000000 bookocr-1.0.2/src/bookocr/__init__.py
--rw-rw-rw-   0        0        0     2314 2023-05-23 03:35:41.000000 bookocr-1.0.2/src/bookocr/_char_ocr.py
--rw-rw-rw-   0        0        0     1230 2023-05-22 18:30:41.000000 bookocr-1.0.2/src/bookocr/_json.py
--rw-rw-rw-   0        0        0     4462 2023-05-21 17:23:34.000000 bookocr-1.0.2/src/bookocr/_service.py
--rw-rw-rw-   0        0        0    13007 2023-05-21 17:38:34.000000 bookocr-1.0.2/src/bookocr/_stats.py
--rw-rw-rw-   0        0        0     1236 2023-05-22 16:33:07.000000 bookocr-1.0.2/src/bookocr/config.py
--rw-rw-rw-   0        0        0  2099296 2023-05-19 12:56:58.000000 bookocr-1.0.2/src/bookocr/model.h5
--rw-rw-rw-   0        0        0    20769 2023-05-22 17:47:03.000000 bookocr-1.0.2/src/bookocr/ocr.py
--rw-rw-rw-   0        0        0     1089 2023-05-22 15:58:23.000000 bookocr-1.0.2/src/bookocr/stats_config.py
-drwxrwxrwx   0        0        0        0 2023-05-23 03:43:48.538776 bookocr-1.0.2/src/bookocr.egg-info/
--rw-rw-rw-   0        0        0     1452 2023-05-23 03:43:48.000000 bookocr-1.0.2/src/bookocr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      412 2023-05-23 03:43:48.000000 bookocr-1.0.2/src/bookocr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 03:43:48.000000 bookocr-1.0.2/src/bookocr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-05-23 03:43:48.000000 bookocr-1.0.2/src/bookocr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-23 03:43:48.000000 bookocr-1.0.2/src/bookocr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 23:14:55.683309 bookocr-1.0.3/
+-rw-rw-rw-   0        0        0     1092 2023-05-23 04:02:50.000000 bookocr-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1452 2023-05-23 23:14:55.682309 bookocr-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      973 2023-05-23 04:02:50.000000 bookocr-1.0.3/README.md
+-rw-rw-rw-   0        0        0      840 2023-05-23 20:14:08.000000 bookocr-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 23:14:55.683309 bookocr-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 23:14:55.533439 bookocr-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 23:14:55.645336 bookocr-1.0.3/src/bookocr/
+-rw-rw-rw-   0        0        0      124 2023-05-23 20:07:08.000000 bookocr-1.0.3/src/bookocr/__init__.py
+-rw-rw-rw-   0        0        0     2314 2023-05-23 20:09:37.000000 bookocr-1.0.3/src/bookocr/_char_ocr.py
+-rw-rw-rw-   0        0        0     1230 2023-05-23 04:02:50.000000 bookocr-1.0.3/src/bookocr/_json.py
+-rw-rw-rw-   0        0        0     4462 2023-05-23 04:02:50.000000 bookocr-1.0.3/src/bookocr/_service.py
+-rw-rw-rw-   0        0        0    13007 2023-05-23 04:02:50.000000 bookocr-1.0.3/src/bookocr/_stats.py
+-rw-rw-rw-   0        0        0     1236 2023-05-23 04:02:50.000000 bookocr-1.0.3/src/bookocr/config.py
+-rw-rw-rw-   0        0        0  2099296 2023-05-23 04:02:50.000000 bookocr-1.0.3/src/bookocr/model.h5
+-rw-rw-rw-   0        0        0    20769 2023-05-23 04:02:50.000000 bookocr-1.0.3/src/bookocr/ocr.py
+-rw-rw-rw-   0        0        0     1089 2023-05-23 04:02:50.000000 bookocr-1.0.3/src/bookocr/stats_config.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:14:55.680310 bookocr-1.0.3/src/bookocr.egg-info/
+-rw-rw-rw-   0        0        0     1452 2023-05-23 23:14:55.000000 bookocr-1.0.3/src/bookocr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-05-23 23:14:55.000000 bookocr-1.0.3/src/bookocr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 23:14:55.000000 bookocr-1.0.3/src/bookocr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-05-23 23:14:55.000000 bookocr-1.0.3/src/bookocr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-23 23:14:55.000000 bookocr-1.0.3/src/bookocr.egg-info/top_level.txt
```

### Comparing `bookocr-1.0.2/LICENSE` & `bookocr-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bookocr-1.0.2/PKG-INFO` & `bookocr-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookocr
-Version: 1.0.2
+Version: 1.0.3
 Summary: Optical character recognition (OCR) tool for printed book pages
 Author-email: Artem Poliakov <artem4250@gmail.com>
 Project-URL: Homepage, https://github.com/Artem259/bookocr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `bookocr-1.0.2/README.md` & `bookocr-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bookocr-1.0.2/pyproject.toml` & `bookocr-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bookocr"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Artem Poliakov", email="artem4250@gmail.com" },
 ]
 description = "Optical character recognition (OCR) tool for printed book pages"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `bookocr-1.0.2/src/bookocr/_char_ocr.py` & `bookocr-1.0.3/src/bookocr/_char_ocr.py`

 * *Files identical despite different names*

### Comparing `bookocr-1.0.2/src/bookocr/_json.py` & `bookocr-1.0.3/src/bookocr/_json.py`

 * *Files identical despite different names*

### Comparing `bookocr-1.0.2/src/bookocr/_service.py` & `bookocr-1.0.3/src/bookocr/_service.py`

 * *Files identical despite different names*

### Comparing `bookocr-1.0.2/src/bookocr/_stats.py` & `bookocr-1.0.3/src/bookocr/_stats.py`

 * *Files identical despite different names*

### Comparing `bookocr-1.0.2/src/bookocr/config.py` & `bookocr-1.0.3/src/bookocr/config.py`

 * *Files identical despite different names*

### Comparing `bookocr-1.0.2/src/bookocr/model.h5` & `bookocr-1.0.3/src/bookocr/model.h5`

 * *Files identical despite different names*

### Comparing `bookocr-1.0.2/src/bookocr/ocr.py` & `bookocr-1.0.3/src/bookocr/ocr.py`

 * *Files identical despite different names*

### Comparing `bookocr-1.0.2/src/bookocr/stats_config.py` & `bookocr-1.0.3/src/bookocr/stats_config.py`

 * *Files identical despite different names*

### Comparing `bookocr-1.0.2/src/bookocr.egg-info/PKG-INFO` & `bookocr-1.0.3/src/bookocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookocr
-Version: 1.0.2
+Version: 1.0.3
 Summary: Optical character recognition (OCR) tool for printed book pages
 Author-email: Artem Poliakov <artem4250@gmail.com>
 Project-URL: Homepage, https://github.com/Artem259/bookocr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

