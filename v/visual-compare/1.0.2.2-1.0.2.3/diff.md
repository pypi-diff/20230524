# Comparing `tmp/visual-compare-1.0.2.2.tar.gz` & `tmp/visual-compare-1.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visual-compare-1.0.2.2.tar", last modified: Fri May 19 10:25:13 2023, max compression
+gzip compressed data, was "visual-compare-1.0.2.3.tar", last modified: Wed May 24 06:27:54 2023, max compression
```

## Comparing `visual-compare-1.0.2.2.tar` & `visual-compare-1.0.2.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 10:25:13.163708 visual-compare-1.0.2.2/
--rw-rw-rw-   0        0        0     2562 2023-05-19 10:25:13.163708 visual-compare-1.0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1743 2023-05-19 06:57:05.000000 visual-compare-1.0.2.2/README.md
--rw-rw-rw-   0        0        0      145 2023-05-19 10:25:13.163708 visual-compare-1.0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1611 2023-05-19 10:22:10.000000 visual-compare-1.0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 10:25:13.132167 visual-compare-1.0.2.2/visual_compare/
--rw-rw-rw-   0        0        0      376 2023-05-11 08:57:00.000000 visual-compare-1.0.2.2/visual_compare/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 10:25:13.147795 visual-compare-1.0.2.2/visual_compare/doc/
--rw-rw-rw-   0        0        0      378 2023-05-06 03:02:28.000000 visual-compare-1.0.2.2/visual_compare/doc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 10:25:13.147795 visual-compare-1.0.2.2/visual_compare/doc/image/
--rw-rw-rw-   0        0        0      378 2023-05-06 02:02:25.000000 visual-compare-1.0.2.2/visual_compare/doc/image/__init__.py
--rw-rw-rw-   0        0        0    30266 2023-05-19 10:20:52.000000 visual-compare-1.0.2.2/visual_compare/doc/image/compare_image.py
--rw-rw-rw-   0        0        0     3984 2023-05-19 06:57:06.000000 visual-compare-1.0.2.2/visual_compare/doc/image/image.py
--rw-rw-rw-   0        0        0    10447 2023-05-19 06:57:06.000000 visual-compare-1.0.2.2/visual_compare/doc/image/ocr.py
--rw-rw-rw-   0        0        0     2955 2023-05-12 09:18:28.000000 visual-compare-1.0.2.2/visual_compare/doc/match.py
--rw-rw-rw-   0        0        0      672 2023-05-19 06:57:06.000000 visual-compare-1.0.2.2/visual_compare/doc/models.py
--rw-rw-rw-   0        0        0     2164 2023-05-15 07:15:15.000000 visual-compare-1.0.2.2/visual_compare/doc/pdf.py
--rw-rw-rw-   0        0        0    12294 2023-05-09 03:42:47.000000 visual-compare-1.0.2.2/visual_compare/doc/pdf_test.py
--rw-rw-rw-   0        0        0    58395 2023-05-19 10:18:11.000000 visual-compare-1.0.2.2/visual_compare/doc/visual.py
-drwxrwxrwx   0        0        0        0 2023-05-19 10:25:13.163708 visual-compare-1.0.2.2/visual_compare/tests/
--rw-rw-rw-   0        0        0      378 2023-05-06 06:06:48.000000 visual-compare-1.0.2.2/visual_compare/tests/__init__.py
--rw-rw-rw-   0        0        0      376 2023-05-08 10:05:50.000000 visual-compare-1.0.2.2/visual_compare/tests/conftest.py
--rw-rw-rw-   0        0        0      714 2023-05-11 08:57:00.000000 visual-compare-1.0.2.2/visual_compare/tests/test_downloader.py
--rw-rw-rw-   0        0        0     2241 2023-05-19 06:57:06.000000 visual-compare-1.0.2.2/visual_compare/tests/test_image.py
--rw-rw-rw-   0        0        0     4216 2023-05-19 06:57:06.000000 visual-compare-1.0.2.2/visual_compare/tests/test_ocr.py
--rw-rw-rw-   0        0        0     2735 2023-05-19 06:57:06.000000 visual-compare-1.0.2.2/visual_compare/tests/test_paddle.py
--rw-rw-rw-   0        0        0      799 2023-05-15 07:04:57.000000 visual-compare-1.0.2.2/visual_compare/tests/test_pdf.py
--rw-rw-rw-   0        0        0      833 2023-05-19 06:57:06.000000 visual-compare-1.0.2.2/visual_compare/tests/test_torch.py
--rw-rw-rw-   0        0        0     3021 2023-05-19 10:18:11.000000 visual-compare-1.0.2.2/visual_compare/tests/test_visual.py
-drwxrwxrwx   0        0        0        0 2023-05-19 10:25:13.163708 visual-compare-1.0.2.2/visual_compare/utils/
--rw-rw-rw-   0        0        0      378 2023-05-06 02:26:53.000000 visual-compare-1.0.2.2/visual_compare/utils/__init__.py
--rw-rw-rw-   0        0        0     1002 2023-05-15 03:07:32.000000 visual-compare-1.0.2.2/visual_compare/utils/common.py
--rw-rw-rw-   0        0        0     1626 2023-05-11 09:04:51.000000 visual-compare-1.0.2.2/visual_compare/utils/downloader.py
-drwxrwxrwx   0        0        0        0 2023-05-19 10:25:13.147795 visual-compare-1.0.2.2/visual_compare.egg-info/
--rw-rw-rw-   0        0        0     2562 2023-05-19 10:25:13.000000 visual-compare-1.0.2.2/visual_compare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1013 2023-05-19 10:25:13.000000 visual-compare-1.0.2.2/visual_compare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 10:25:13.000000 visual-compare-1.0.2.2/visual_compare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-08 07:02:46.000000 visual-compare-1.0.2.2/visual_compare.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      206 2023-05-19 10:25:13.000000 visual-compare-1.0.2.2/visual_compare.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-19 10:25:13.000000 visual-compare-1.0.2.2/visual_compare.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 06:27:54.325872 visual-compare-1.0.2.3/
+-rw-rw-rw-   0        0        0     2562 2023-05-24 06:27:54.325872 visual-compare-1.0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1743 2023-05-19 06:57:05.000000 visual-compare-1.0.2.3/README.md
+-rw-rw-rw-   0        0        0      145 2023-05-24 06:27:54.325872 visual-compare-1.0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1638 2023-05-24 06:25:06.000000 visual-compare-1.0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 06:27:54.310289 visual-compare-1.0.2.3/visual_compare/
+-rw-rw-rw-   0        0        0      376 2023-05-11 08:57:00.000000 visual-compare-1.0.2.3/visual_compare/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 06:27:54.310289 visual-compare-1.0.2.3/visual_compare/doc/
+-rw-rw-rw-   0        0        0      378 2023-05-06 03:02:28.000000 visual-compare-1.0.2.3/visual_compare/doc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 06:27:54.325872 visual-compare-1.0.2.3/visual_compare/doc/image/
+-rw-rw-rw-   0        0        0      378 2023-05-06 02:02:25.000000 visual-compare-1.0.2.3/visual_compare/doc/image/__init__.py
+-rw-rw-rw-   0        0        0    30266 2023-05-19 10:20:52.000000 visual-compare-1.0.2.3/visual_compare/doc/image/compare_image.py
+-rw-rw-rw-   0        0        0     3984 2023-05-19 06:57:06.000000 visual-compare-1.0.2.3/visual_compare/doc/image/image.py
+-rw-rw-rw-   0        0        0    10447 2023-05-19 06:57:06.000000 visual-compare-1.0.2.3/visual_compare/doc/image/ocr.py
+-rw-rw-rw-   0        0        0     2955 2023-05-12 09:18:28.000000 visual-compare-1.0.2.3/visual_compare/doc/match.py
+-rw-rw-rw-   0        0        0      672 2023-05-19 06:57:06.000000 visual-compare-1.0.2.3/visual_compare/doc/models.py
+-rw-rw-rw-   0        0        0     2164 2023-05-15 07:15:15.000000 visual-compare-1.0.2.3/visual_compare/doc/pdf.py
+-rw-rw-rw-   0        0        0    12294 2023-05-09 03:42:47.000000 visual-compare-1.0.2.3/visual_compare/doc/pdf_test.py
+-rw-rw-rw-   0        0        0    58395 2023-05-19 10:28:55.000000 visual-compare-1.0.2.3/visual_compare/doc/visual.py
+drwxrwxrwx   0        0        0        0 2023-05-24 06:27:54.325872 visual-compare-1.0.2.3/visual_compare/tests/
+-rw-rw-rw-   0        0        0      378 2023-05-06 06:06:48.000000 visual-compare-1.0.2.3/visual_compare/tests/__init__.py
+-rw-rw-rw-   0        0        0      376 2023-05-08 10:05:50.000000 visual-compare-1.0.2.3/visual_compare/tests/conftest.py
+-rw-rw-rw-   0        0        0      714 2023-05-11 08:57:00.000000 visual-compare-1.0.2.3/visual_compare/tests/test_downloader.py
+-rw-rw-rw-   0        0        0     2241 2023-05-19 06:57:06.000000 visual-compare-1.0.2.3/visual_compare/tests/test_image.py
+-rw-rw-rw-   0        0        0     4216 2023-05-19 06:57:06.000000 visual-compare-1.0.2.3/visual_compare/tests/test_ocr.py
+-rw-rw-rw-   0        0        0     2735 2023-05-19 06:57:06.000000 visual-compare-1.0.2.3/visual_compare/tests/test_paddle.py
+-rw-rw-rw-   0        0        0      799 2023-05-15 07:04:57.000000 visual-compare-1.0.2.3/visual_compare/tests/test_pdf.py
+-rw-rw-rw-   0        0        0      833 2023-05-19 06:57:06.000000 visual-compare-1.0.2.3/visual_compare/tests/test_torch.py
+-rw-rw-rw-   0        0        0     3021 2023-05-19 10:28:55.000000 visual-compare-1.0.2.3/visual_compare/tests/test_visual.py
+drwxrwxrwx   0        0        0        0 2023-05-24 06:27:54.325872 visual-compare-1.0.2.3/visual_compare/utils/
+-rw-rw-rw-   0        0        0      378 2023-05-06 02:26:53.000000 visual-compare-1.0.2.3/visual_compare/utils/__init__.py
+-rw-rw-rw-   0        0        0     1002 2023-05-15 03:07:32.000000 visual-compare-1.0.2.3/visual_compare/utils/common.py
+-rw-rw-rw-   0        0        0     1626 2023-05-11 09:04:51.000000 visual-compare-1.0.2.3/visual_compare/utils/downloader.py
+drwxrwxrwx   0        0        0        0 2023-05-24 06:27:54.310289 visual-compare-1.0.2.3/visual_compare.egg-info/
+-rw-rw-rw-   0        0        0     2562 2023-05-24 06:27:54.000000 visual-compare-1.0.2.3/visual_compare.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1013 2023-05-24 06:27:54.000000 visual-compare-1.0.2.3/visual_compare.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 06:27:54.000000 visual-compare-1.0.2.3/visual_compare.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-08 07:02:46.000000 visual-compare-1.0.2.3/visual_compare.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      221 2023-05-24 06:27:54.000000 visual-compare-1.0.2.3/visual_compare.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-24 06:27:54.000000 visual-compare-1.0.2.3/visual_compare.egg-info/top_level.txt
```

### Comparing `visual-compare-1.0.2.2/PKG-INFO` & `visual-compare-1.0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visual-compare
-Version: 1.0.2.2
+Version: 1.0.2.3
 Summary: Image and PDF Compare
 Home-page: https://github.com/cuidingyong/visual-compare
 Author: Dillon
 Author-email: cuidingyong@yeah.net
 License: MIT
 Keywords: visual compare image pdf diff
 Platform: UNKNOWN
```

### Comparing `visual-compare-1.0.2.2/README.md` & `visual-compare-1.0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.2.2/setup.py` & `visual-compare-1.0.2.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="visual-compare",
-    version="1.0.2.2",
+    version="1.0.2.3",
     description="Image and PDF Compare",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cuidingyong/visual-compare",
     author="Dillon",
     author_email="cuidingyong@yeah.net",
     license="MIT",
@@ -39,11 +39,12 @@
         "pytesseract~=0.3.10",
         "parsimonious~=0.10",
         "PyMuPDF~=1.22",
         "pyzbar~=0.1.9",
         "pylibdmtx~=0.1.10",
         "Wand~=0.6.11",
         "pydantic~=1.8.2",
-        "deepdiff~=6.3.0"
+        "deepdiff~=6.3.0",
+        "easyocr~=1.6.2"
     ],
     zip_safe=False,
 )
```

### Comparing `visual-compare-1.0.2.2/visual_compare/doc/image/compare_image.py` & `visual-compare-1.0.2.3/visual_compare/doc/image/compare_image.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.2.2/visual_compare/doc/image/image.py` & `visual-compare-1.0.2.3/visual_compare/doc/image/image.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.2.2/visual_compare/doc/image/ocr.py` & `visual-compare-1.0.2.3/visual_compare/doc/image/ocr.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.2.2/visual_compare/doc/match.py` & `visual-compare-1.0.2.3/visual_compare/doc/match.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.2.2/visual_compare/doc/models.py` & `visual-compare-1.0.2.3/visual_compare/doc/models.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.2.2/visual_compare/doc/pdf.py` & `visual-compare-1.0.2.3/visual_compare/doc/pdf.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.2.2/visual_compare/doc/pdf_test.py` & `visual-compare-1.0.2.3/visual_compare/doc/pdf_test.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.2.2/visual_compare/doc/visual.py` & `visual-compare-1.0.2.3/visual_compare/doc/visual.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.2.2/visual_compare/tests/test_downloader.py` & `visual-compare-1.0.2.3/visual_compare/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.2.2/visual_compare/tests/test_image.py` & `visual-compare-1.0.2.3/visual_compare/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.2.2/visual_compare/tests/test_ocr.py` & `visual-compare-1.0.2.3/visual_compare/tests/test_ocr.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.2.2/visual_compare/tests/test_paddle.py` & `visual-compare-1.0.2.3/visual_compare/tests/test_paddle.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.2.2/visual_compare/tests/test_pdf.py` & `visual-compare-1.0.2.3/visual_compare/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.2.2/visual_compare/tests/test_torch.py` & `visual-compare-1.0.2.3/visual_compare/tests/test_torch.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.2.2/visual_compare/tests/test_visual.py` & `visual-compare-1.0.2.3/visual_compare/tests/test_visual.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.2.2/visual_compare/utils/common.py` & `visual-compare-1.0.2.3/visual_compare/utils/common.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.2.2/visual_compare/utils/downloader.py` & `visual-compare-1.0.2.3/visual_compare/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `visual-compare-1.0.2.2/visual_compare.egg-info/PKG-INFO` & `visual-compare-1.0.2.3/visual_compare.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visual-compare
-Version: 1.0.2.2
+Version: 1.0.2.3
 Summary: Image and PDF Compare
 Home-page: https://github.com/cuidingyong/visual-compare
 Author: Dillon
 Author-email: cuidingyong@yeah.net
 License: MIT
 Keywords: visual compare image pdf diff
 Platform: UNKNOWN
```

### Comparing `visual-compare-1.0.2.2/visual_compare.egg-info/SOURCES.txt` & `visual-compare-1.0.2.3/visual_compare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

