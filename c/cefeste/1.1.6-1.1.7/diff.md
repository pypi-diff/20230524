# Comparing `tmp/cefeste-1.1.6.tar.gz` & `tmp/cefeste-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefeste-1.1.6.tar", last modified: Mon May 22 21:02:53 2023, max compression
+gzip compressed data, was "cefeste-1.1.7.tar", last modified: Mon May 22 21:11:03 2023, max compression
```

## Comparing `cefeste-1.1.6.tar` & `cefeste-1.1.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:02:53.452531 cefeste-1.1.6/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-05-05 08:25:33.000000 cefeste-1.1.6/LICENCE
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2821 2023-05-22 21:02:53.452531 cefeste-1.1.6/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2321 2023-05-22 20:53:27.000000 cefeste-1.1.6/README.md
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      754 2023-05-22 21:01:54.000000 cefeste-1.1.6/pyproject.toml
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-05-22 21:02:53.452531 cefeste-1.1.6/setup.cfg
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      999 2023-05-22 21:01:53.000000 cefeste-1.1.6/setup.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:02:53.440530 cefeste-1.1.6/src/
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:02:53.448531 cefeste-1.1.6/src/cefeste/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3364 2023-05-05 08:25:33.000000 cefeste-1.1.6/src/cefeste/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      444 2023-05-05 08:25:33.000000 cefeste-1.1.6/src/cefeste/config.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:02:53.452531 cefeste-1.1.6/src/cefeste/elimination/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    15386 2023-05-22 20:53:27.000000 cefeste-1.1.6/src/cefeste/elimination/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    25817 2023-05-10 10:23:33.000000 cefeste-1.1.6/src/cefeste/elimination/shap_rfe.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:02:53.452531 cefeste-1.1.6/src/cefeste/selection/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27726 2023-05-05 08:25:33.000000 cefeste-1.1.6/src/cefeste/selection/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10558 2023-05-05 08:25:33.000000 cefeste-1.1.6/src/cefeste/selection/explanatory.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    21561 2023-05-05 08:25:33.000000 cefeste-1.1.6/src/cefeste/selection/multivariate.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10122 2023-05-05 08:25:33.000000 cefeste-1.1.6/src/cefeste/selection/univariate.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:02:53.452531 cefeste-1.1.6/src/cefeste/transform/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2811 2023-05-22 21:01:13.000000 cefeste-1.1.6/src/cefeste/transform/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2434 2023-05-10 10:23:33.000000 cefeste-1.1.6/src/cefeste/utils.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:02:53.448531 cefeste-1.1.6/src/cefeste.egg-info/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2821 2023-05-22 21:02:53.000000 cefeste-1.1.6/src/cefeste.egg-info/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      533 2023-05-22 21:02:53.000000 cefeste-1.1.6/src/cefeste.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-05-22 21:02:53.000000 cefeste-1.1.6/src/cefeste.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      131 2023-05-22 21:02:53.000000 cefeste-1.1.6/src/cefeste.egg-info/requires.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        8 2023-05-22 21:02:53.000000 cefeste-1.1.6/src/cefeste.egg-info/top_level.txt
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:11:03.780634 cefeste-1.1.7/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-05-05 08:25:33.000000 cefeste-1.1.7/LICENCE
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2821 2023-05-22 21:11:03.780634 cefeste-1.1.7/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2321 2023-05-22 20:53:27.000000 cefeste-1.1.7/README.md
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      754 2023-05-22 21:09:34.000000 cefeste-1.1.7/pyproject.toml
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-05-22 21:11:03.780634 cefeste-1.1.7/setup.cfg
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      999 2023-05-22 21:09:36.000000 cefeste-1.1.7/setup.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:11:03.760632 cefeste-1.1.7/src/
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:11:03.768633 cefeste-1.1.7/src/cefeste/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3364 2023-05-05 08:25:33.000000 cefeste-1.1.7/src/cefeste/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      444 2023-05-05 08:25:33.000000 cefeste-1.1.7/src/cefeste/config.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:11:03.776633 cefeste-1.1.7/src/cefeste/elimination/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    15386 2023-05-22 20:53:27.000000 cefeste-1.1.7/src/cefeste/elimination/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    25817 2023-05-10 10:23:33.000000 cefeste-1.1.7/src/cefeste/elimination/shap_rfe.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:11:03.776633 cefeste-1.1.7/src/cefeste/selection/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27726 2023-05-05 08:25:33.000000 cefeste-1.1.7/src/cefeste/selection/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10558 2023-05-05 08:25:33.000000 cefeste-1.1.7/src/cefeste/selection/explanatory.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    21561 2023-05-05 08:25:33.000000 cefeste-1.1.7/src/cefeste/selection/multivariate.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10122 2023-05-05 08:25:33.000000 cefeste-1.1.7/src/cefeste/selection/univariate.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:11:03.776633 cefeste-1.1.7/src/cefeste/transform/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2801 2023-05-22 21:09:54.000000 cefeste-1.1.7/src/cefeste/transform/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2434 2023-05-10 10:23:33.000000 cefeste-1.1.7/src/cefeste/utils.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-22 21:11:03.772633 cefeste-1.1.7/src/cefeste.egg-info/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2821 2023-05-22 21:11:03.000000 cefeste-1.1.7/src/cefeste.egg-info/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      533 2023-05-22 21:11:03.000000 cefeste-1.1.7/src/cefeste.egg-info/SOURCES.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-05-22 21:11:03.000000 cefeste-1.1.7/src/cefeste.egg-info/dependency_links.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      131 2023-05-22 21:11:03.000000 cefeste-1.1.7/src/cefeste.egg-info/requires.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        8 2023-05-22 21:11:03.000000 cefeste-1.1.7/src/cefeste.egg-info/top_level.txt
```

### Comparing `cefeste-1.1.6/LICENCE` & `cefeste-1.1.7/LICENCE`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.6/PKG-INFO` & `cefeste-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefeste
-Version: 1.1.6
+Version: 1.1.7
 Summary: Feature Selection and Elimination
 Home-page: https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Author: DAT/Mattia Centurelli
 Author-email: DAT - Mattia Centurelli <mcenturelli@credem.it>
 Project-URL: Homepage, https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cefeste-1.1.6/README.md` & `cefeste-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.6/pyproject.toml` & `cefeste-1.1.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cefeste"
-version = "1.1.6"
+version = "1.1.7"
 authors = [
   { name="DAT - Mattia Centurelli", email="mcenturelli@credem.it" },
 ]
 description = "Feature Selection and Elimination"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cefeste-1.1.6/setup.py` & `cefeste-1.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ce-feste",
-    version="1.1.6",
+    version="1.1.7",
     description="Package for Feature Selection, Transformation, Elimination",
     author="DAT/Mattia Centurelli",
     author_email="mcenturelli@credem.it",
     url="https://dev.azure.com/credem-data/DAT/_git/ce-feste",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
```

### Comparing `cefeste-1.1.6/src/cefeste/__init__.py` & `cefeste-1.1.7/src/cefeste/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.6/src/cefeste/elimination/__init__.py` & `cefeste-1.1.7/src/cefeste/elimination/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.6/src/cefeste/elimination/shap_rfe.py` & `cefeste-1.1.7/src/cefeste/elimination/shap_rfe.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.6/src/cefeste/selection/__init__.py` & `cefeste-1.1.7/src/cefeste/selection/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.6/src/cefeste/selection/explanatory.py` & `cefeste-1.1.7/src/cefeste/selection/explanatory.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.6/src/cefeste/selection/multivariate.py` & `cefeste-1.1.7/src/cefeste/selection/multivariate.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.6/src/cefeste/selection/univariate.py` & `cefeste-1.1.7/src/cefeste/selection/univariate.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.6/src/cefeste/transform/__init__.py` & `cefeste-1.1.7/src/cefeste/transform/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,13 +82,13 @@
     def fit_transform(self, X, y=None):
         """Identify and trasform the columns with dtypes object to category for the input pd.DataFrame."""
         self._fitted = True
 
         if self.feat_to_check is None:
             self.feat_to_check = X.columns
 
-        self._cols_to_categorize = [x for x in self.X[self.feat_to_check].columns if self.X[x].dtype == "O"]
+        self._cols_to_categorize = [x for x in X[self.feat_to_check].columns if X[x].dtype == "O"]
 
         for x in self._cols_to_categorize:
             X[x] = X[x].astype("category")
 
         return X
```

### Comparing `cefeste-1.1.6/src/cefeste/utils.py` & `cefeste-1.1.7/src/cefeste/utils.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.6/src/cefeste.egg-info/PKG-INFO` & `cefeste-1.1.7/src/cefeste.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefeste
-Version: 1.1.6
+Version: 1.1.7
 Summary: Feature Selection and Elimination
 Home-page: https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Author: DAT/Mattia Centurelli
 Author-email: DAT - Mattia Centurelli <mcenturelli@credem.it>
 Project-URL: Homepage, https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cefeste-1.1.6/src/cefeste.egg-info/SOURCES.txt` & `cefeste-1.1.7/src/cefeste.egg-info/SOURCES.txt`

 * *Files identical despite different names*

