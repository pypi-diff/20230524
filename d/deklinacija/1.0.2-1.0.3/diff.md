# Comparing `tmp/deklinacija-1.0.2.tar.gz` & `tmp/deklinacija-1.0.3.tar.gz`

## Comparing `deklinacija-1.0.2.tar` & `deklinacija-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 deklinacija-1.0.2/main.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.0.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deklinacija-1.0.2/deklinacija/__init__.py
--rw-r--r--   0        0        0     8885 2020-02-02 00:00:00.000000 deklinacija-1.0.2/deklinacija/module.py
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 deklinacija-1.0.2/deklinacija/utils.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 deklinacija-1.0.2/deklinacija/vokativ_database.csv
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.0.2/LICENSE
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 deklinacija-1.0.2/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 deklinacija-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 deklinacija-1.0.3/main.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.0.3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deklinacija-1.0.3/deklinacija/__init__.py
+-rw-r--r--   0        0        0     8885 2020-02-02 00:00:00.000000 deklinacija-1.0.3/deklinacija/module.py
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 deklinacija-1.0.3/deklinacija/utils.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 deklinacija-1.0.3/deklinacija/vokativ_database.csv
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 deklinacija-1.0.3/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 deklinacija-1.0.3/PKG-INFO
```

### Comparing `deklinacija-1.0.2/.github/workflows/python-package.yml` & `deklinacija-1.0.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.2/deklinacija/module.py` & `deklinacija-1.0.3/deklinacija/module.py`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.2/deklinacija/utils.py` & `deklinacija-1.0.3/deklinacija/utils.py`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.2/deklinacija/vokativ_database.csv` & `deklinacija-1.0.3/deklinacija/vokativ_database.csv`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.2/LICENSE` & `deklinacija-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.2/README.md` & `deklinacija-1.0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -49,7 +49,10 @@
 #Translation: You have given a gift to Nikola
 ```
 
 ## Todo
 The following features are on the roadmap:
 - Support for both Latin and Cyrillic scripts
 - Declension of last names
+
+## Attribution
+[Vokativi](https://github.com/startitrs/vokativi) by [Startit](https://github.com/startitrs) is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) / Modifications: converted to Cyrillic and filtered out names longer than 4 characters
```

### Comparing `deklinacija-1.0.2/pyproject.toml` & `deklinacija-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "deklinacija"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="urelja", email="code.relja@gmail.com" },
 ]
 description = "A Python library for declension of personal names in Serbian"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `deklinacija-1.0.2/PKG-INFO` & `deklinacija-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deklinacija
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python library for declension of personal names in Serbian
 Project-URL: Homepage, https://github.com/urelja/deklinacija
 Project-URL: Bug Tracker, https://github.com/urelja/deklinacija/issues
 Author-email: urelja <code.relja@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -63,7 +63,10 @@
 #Translation: You have given a gift to Nikola
 ```
 
 ## Todo
 The following features are on the roadmap:
 - Support for both Latin and Cyrillic scripts
 - Declension of last names
+
+## Attribution
+[Vokativi](https://github.com/startitrs/vokativi) by [Startit](https://github.com/startitrs) is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) / Modifications: converted to Cyrillic and filtered out names longer than 4 characters
```

