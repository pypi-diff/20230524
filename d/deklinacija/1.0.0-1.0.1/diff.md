# Comparing `tmp/deklinacija-1.0.0.tar.gz` & `tmp/deklinacija-1.0.1.tar.gz`

## Comparing `deklinacija-1.0.0.tar` & `deklinacija-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.0.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deklinacija-1.0.0/deklinacija/__init__.py
--rw-r--r--   0        0        0     8885 2020-02-02 00:00:00.000000 deklinacija-1.0.0/deklinacija/module.py
--rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 deklinacija-1.0.0/deklinacija/utils.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 deklinacija-1.0.0/deklinacija/vokativ_database.csv
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.0.0/LICENSE
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 deklinacija-1.0.0/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 deklinacija-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.0.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deklinacija-1.0.1/deklinacija/__init__.py
+-rw-r--r--   0        0        0     8885 2020-02-02 00:00:00.000000 deklinacija-1.0.1/deklinacija/module.py
+-rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 deklinacija-1.0.1/deklinacija/utils.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 deklinacija-1.0.1/deklinacija/vokativ_database.csv
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 deklinacija-1.0.1/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 deklinacija-1.0.1/PKG-INFO
```

### Comparing `deklinacija-1.0.0/.github/workflows/python-package.yml` & `deklinacija-1.0.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.0/deklinacija/module.py` & `deklinacija-1.0.1/deklinacija/module.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
     if name[-1].lower() == "i":
         return "".join(name)
     
     if name[-1].lower() == "u":
         return "".join(name)
     
     if name[-1].lower() in ["a","а"]:
-        if len(nameSep) <= 4:
+        if len(nameSep) <= 5:
             try:
                 if utils.isLatin(name[-1]):
                     return utils.toLatin(utils.vokativ_db[utils.toCyrillic(name)])
                 else:
                     return utils.vokativ_db[utils.toCyrillic(name)]
             except KeyError:
                 if name[-1].islower():
```

### Comparing `deklinacija-1.0.0/deklinacija/utils.py` & `deklinacija-1.0.1/deklinacija/utils.py`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.0/deklinacija/vokativ_database.csv` & `deklinacija-1.0.1/deklinacija/vokativ_database.csv`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.0/LICENSE` & `deklinacija-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.0/README.md` & `deklinacija-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `deklinacija-1.0.0/pyproject.toml` & `deklinacija-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "deklinacija"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="urelja", email="code.relja@gmail.com" },
 ]
 description = "A Python library for declension of personal names in Serbian"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `deklinacija-1.0.0/PKG-INFO` & `deklinacija-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deklinacija
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python library for declension of personal names in Serbian
 Project-URL: Homepage, https://github.com/urelja/deklinacija
 Project-URL: Bug Tracker, https://github.com/urelja/deklinacija/issues
 Author-email: urelja <code.relja@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

