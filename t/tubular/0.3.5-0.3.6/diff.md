# Comparing `tmp/tubular-0.3.5.tar.gz` & `tmp/tubular-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tubular-0.3.5.tar", last modified: Thu Apr 27 10:17:30 2023, max compression
+gzip compressed data, was "tubular-0.3.6.tar", last modified: Wed May 24 15:54:28 2023, max compression
```

## Comparing `tubular-0.3.5.tar` & `tubular-0.3.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 10:17:30.464595 tubular-0.3.5/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1550 2023-04-27 10:11:36.000000 tubular-0.3.5/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4335 2023-04-27 10:17:30.464595 tubular-0.3.5/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3706 2023-04-27 10:11:36.000000 tubular-0.3.5/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-27 10:17:30.464595 tubular-0.3.5/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1457 2023-04-27 10:11:36.000000 tubular-0.3.5/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 10:17:30.456595 tubular-0.3.5/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-27 10:11:36.000000 tubular-0.3.5/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14672 2023-04-27 10:11:36.000000 tubular-0.3.5/tests/test_data.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4876 2023-04-27 10:11:36.000000 tubular-0.3.5/tests/test_transformers.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 10:17:30.460595 tubular-0.3.5/tubular/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      286 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/_version.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14927 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20028 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/capping.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1985 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/comparison.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    41786 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/dates.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13464 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/imputers.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17192 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/mapping.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2002 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/misc.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42279 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/nominal.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    30363 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/numeric.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6024 2023-04-27 10:11:36.000000 tubular-0.3.5/tubular/strings.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 10:17:30.464595 tubular-0.3.5/tubular.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4335 2023-04-27 10:17:30.000000 tubular-0.3.5/tubular.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      470 2023-04-27 10:17:30.000000 tubular-0.3.5/tubular.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-27 10:17:30.000000 tubular-0.3.5/tubular.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       40 2023-04-27 10:17:30.000000 tubular-0.3.5/tubular.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       14 2023-04-27 10:17:30.000000 tubular-0.3.5/tubular.egg-info/top_level.txt
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-05-24 15:54:28.985024 tubular-0.3.6/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1550 2023-05-24 15:51:27.000000 tubular-0.3.6/LICENSE
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4335 2023-05-24 15:54:28.985024 tubular-0.3.6/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3706 2023-05-24 15:51:27.000000 tubular-0.3.6/README.md
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2023-05-24 15:54:28.985024 tubular-0.3.6/setup.cfg
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1457 2023-05-24 15:51:27.000000 tubular-0.3.6/setup.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-05-24 15:54:28.981024 tubular-0.3.6/tests/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-05-24 15:51:27.000000 tubular-0.3.6/tests/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14672 2023-05-24 15:51:27.000000 tubular-0.3.6/tests/test_data.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4876 2023-05-24 15:51:27.000000 tubular-0.3.6/tests/test_transformers.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-05-24 15:54:28.985024 tubular-0.3.6/tubular/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      286 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       22 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/_version.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14927 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/base.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    20028 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/capping.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1985 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/comparison.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    41786 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/dates.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    13464 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/imputers.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    17192 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/mapping.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2002 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/misc.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    42279 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/nominal.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    30363 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/numeric.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6024 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/strings.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-05-24 15:54:28.985024 tubular-0.3.6/tubular.egg-info/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4335 2023-05-24 15:54:28.000000 tubular-0.3.6/tubular.egg-info/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      470 2023-05-24 15:54:28.000000 tubular-0.3.6/tubular.egg-info/SOURCES.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2023-05-24 15:54:28.000000 tubular-0.3.6/tubular.egg-info/dependency_links.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       45 2023-05-24 15:54:28.000000 tubular-0.3.6/tubular.egg-info/requires.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       14 2023-05-24 15:54:28.000000 tubular-0.3.6/tubular.egg-info/top_level.txt
```

### Comparing `tubular-0.3.5/LICENSE` & `tubular-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tubular-0.3.5/PKG-INFO` & `tubular-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tubular
-Version: 0.3.5
+Version: 0.3.6
 Summary: Package to perform pre processing steps for machine learning models
 Author: LV GI Data Science Team
 Author-email: #DataSciencePackages@lv.co.uk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tubular-0.3.5/README.md` & `tubular-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `tubular-0.3.5/setup.py` & `tubular-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.5/tests/test_data.py` & `tubular-0.3.6/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.5/tests/test_transformers.py` & `tubular-0.3.6/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.5/tubular/base.py` & `tubular-0.3.6/tubular/base.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.5/tubular/capping.py` & `tubular-0.3.6/tubular/capping.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.5/tubular/comparison.py` & `tubular-0.3.6/tubular/comparison.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.5/tubular/dates.py` & `tubular-0.3.6/tubular/dates.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.5/tubular/imputers.py` & `tubular-0.3.6/tubular/imputers.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.5/tubular/mapping.py` & `tubular-0.3.6/tubular/mapping.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.5/tubular/misc.py` & `tubular-0.3.6/tubular/misc.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.5/tubular/nominal.py` & `tubular-0.3.6/tubular/nominal.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.5/tubular/numeric.py` & `tubular-0.3.6/tubular/numeric.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.5/tubular/strings.py` & `tubular-0.3.6/tubular/strings.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.5/tubular.egg-info/PKG-INFO` & `tubular-0.3.6/tubular.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tubular
-Version: 0.3.5
+Version: 0.3.6
 Summary: Package to perform pre processing steps for machine learning models
 Author: LV GI Data Science Team
 Author-email: #DataSciencePackages@lv.co.uk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

