# Comparing `tmp/scinumtools-0.3.0.tar.gz` & `tmp/scinumtools-1.0.0.tar.gz`

## Comparing `scinumtools-0.3.0.tar` & `scinumtools-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,19 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 scinumtools-0.3.0/requirements.txt
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-0.3.0/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 scinumtools-0.3.0/src/scinumtools/__init__.py
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 scinumtools-0.3.0/src/scinumtools/structs/CollectorClass.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 scinumtools-0.3.0/src/scinumtools/structs/ParameterClass.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-0.3.0/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 scinumtools-0.3.0/tests/test_struct.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 scinumtools-0.3.0/.gitignore
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-0.3.0/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 scinumtools-1.0.0/requirements.txt
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.0.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 scinumtools-1.0.0/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.0.0/src/scinumtools/data/CachingClass.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 scinumtools-1.0.0/src/scinumtools/data/__init__.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.0.0/src/scinumtools/stats/StopwatchClass.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.0.0/src/scinumtools/stats/__init__.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.0.0/src/scinumtools/structs/CollectorClass.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 scinumtools-1.0.0/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.0.0/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scinumtools-1.0.0/tests/cached_data.npy
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scinumtools-1.0.0/tests/test_data.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.0.0/tests/test_stats.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 scinumtools-1.0.0/tests/test_struct.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 scinumtools-1.0.0/.gitignore
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.0.0/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.0.0/PKG-INFO
```

### Comparing `scinumtools-0.3.0/.github/workflows/python-publish.yml` & `scinumtools-1.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scinumtools-0.3.0/src/scinumtools/structs/CollectorClass.py` & `scinumtools-1.0.0/src/scinumtools/structs/CollectorClass.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,14 +37,25 @@
     def append(self, values: list):
         """ Append a single row
 
         :param values: List of values for each column
         """
         for n, name in enumerate(self._columns):
             getattr(self,name).append(values[n])
+
+    def sort(self, name: str, reverse=False):
+        """ Sort all columns according to one
+
+        :param str name: name of the sorting column
+        :param bool reverse: reverse order
+        """
+        ids = np.argsort(getattr(self, name))
+        if reverse: ids = ids[::-1]
+        for n, name in enumerate(self._columns):
+            setattr(self,name,list(np.array(getattr(self, name))[ids]))
             
     def to_dict(self):
         """ Convert class data to a dictionary of lists/arrays
         """
         data = {}
         for name in self._columns:
             data[name] = getattr(self,name)
@@ -111,14 +122,24 @@
         :param values: List of values for each column
         """
         for n, name in enumerate(self._columns):
             data = getattr(self,name)
             new = np.array(values[n],dtype=data.dtype)
             setattr(self,name, np.append(data,new) )
             
+    def sort(self, name: str, reverse=False):
+        """ Sort all columns according to one
+
+        :param str name: name of the sorting column
+        """
+        ids = np.argsort(getattr(self, name))
+        if reverse: ids = ids[::-1]
+        for n, name in enumerate(self._columns):
+            setattr(self,name,getattr(self, name)[ids])
+            
     def to_dict(self):
         """ Convert class data to a dictionary of lists/arrays
         """
         data = {}
         for name in self._columns:
             data[name] = getattr(self,name)
         return data
```

### Comparing `scinumtools-0.3.0/src/scinumtools/structs/ParameterClass.py` & `scinumtools-1.0.0/src/scinumtools/structs/ParameterClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-0.3.0/tests/test_struct.py` & `scinumtools-1.0.0/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `scinumtools-0.3.0/.gitignore` & `scinumtools-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scinumtools-0.3.0/pyproject.toml` & `scinumtools-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scinumtools"
-version = "0.3.0"
+version = "1.0.0"
 authors = [
   { name="Ondrej Pego Jaura", email="vrtulka23@pm.me" },
 ]
 description = "Set of most frequently used tools for a rapid numerical code development in Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scinumtools-0.3.0/PKG-INFO` & `scinumtools-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinumtools
-Version: 0.3.0
+Version: 1.0.0
 Summary: Set of most frequently used tools for a rapid numerical code development in Python.
 Project-URL: Homepage, https://github.com/vrtulka23/scinumtools
 Project-URL: Bug Tracker, https://github.com/vrtulka23/scinumtools/issues
 Author-email: Ondrej Pego Jaura <vrtulka23@pm.me>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

