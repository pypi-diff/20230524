# Comparing `tmp/mfunc-0.1.0.tar.gz` & `tmp/mfunc-0.1.1.tar.gz`

## Comparing `mfunc-0.1.0.tar` & `mfunc-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mfunc-0.1.0/src/mfunc/__init__.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 mfunc-0.1.0/src/mfunc/mfunc.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 mfunc-0.1.0/LICENSE
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 mfunc-0.1.0/README.md
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 mfunc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 mfunc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mfunc-0.1.1/src/mfunc/__init__.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 mfunc-0.1.1/src/mfunc/mfunc.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 mfunc-0.1.1/LICENSE
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 mfunc-0.1.1/README.md
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 mfunc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 mfunc-0.1.1/PKG-INFO
```

### Comparing `mfunc-0.1.0/src/mfunc/mfunc.py` & `mfunc-0.1.1/src/mfunc/mfunc.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     def __init__(self,function):
         self.f=function
     def __getitem__(self,key):
         if isinstance(key,slice):
             return [self.f(x) for x in range(key.start or 0,key.stop,key.step or 1)]
         return self.f(key)
     def __repr__(self):
-        return self.f
+        return str(self.f)
     def __add__(self,other):
         return mfunc(lambda x:self.f(x)+other.f(x))
     def __sub__(self,other):
         return mfunc(lambda x:self.f(x)-other.f(x))
     def __mul__(self,other):
         return mfunc(lambda x:self.f(x)*other.f(x))
     def __truediv__(self,other):
```

### Comparing `mfunc-0.1.0/LICENSE` & `mfunc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mfunc-0.1.0/README.md` & `mfunc-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # `mfunc`
 This library was made so that you can get a list of points of a function by list slicing.
 ## How to Use
-First, put `from mfunc import mfunc` at the top of your code.
-Then, if you have already defined a function `f(x)`, you can initiate an instance of an `mfunc` by assigning `mfunc(f)` to a variable. Due to the behaviour of importing, you may need to do `mfunc.mfunc()` instead.
+First, put `from mfunc.mfunc import mfunc` at the top of your code.
+Then, if you have already defined a function `f(x)`, you can initiate an instance of an `mfunc` by assigning `mfunc(f)` to a variable.
 ## Supported Features
 Here is the list of supported features for an `mfunc`:<br><br>
 * Item retrieval and slicing (e.g. `mfunc(lambda x:x)[:5]` returns the values of the function from 0 to 4).<br>
 
-* The arithmetic operators `+ - * / // **`<br>
+* The arithmetic operators `+ - * / // **`.<br>
 
 * A string representation (returns actual function).
 ## Bugs
 If you hae discovered a bug or have an idea, post it [here](https://github.com/PlaceReporter99/mfunc-bug-tracker/issues).
```

### Comparing `mfunc-0.1.0/pyproject.toml` & `mfunc-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "mfunc"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="PlaceReporter99", email="sfurman35@outlook.com" },
 ]
 description = "A python library to add list slicing capabilities and equality checking to mathematical functions."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mfunc-0.1.0/PKG-INFO` & `mfunc-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: mfunc
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python library to add list slicing capabilities and equality checking to mathematical functions.
 Project-URL: Homepage, https://github.com/PlaceReporter99/mfunc-bug-tracker
 Project-URL: Bug Tracker, https://github.com/PlaceReporter99/mfunc-bug-tracker/issues
 Author-email: PlaceReporter99 <sfurman35@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # `mfunc`
 This library was made so that you can get a list of points of a function by list slicing.
 ## How to Use
-First, put `from mfunc import mfunc` at the top of your code.
-Then, if you have already defined a function `f(x)`, you can initiate an instance of an `mfunc` by assigning `mfunc(f)` to a variable. Due to the behaviour of importing, you may need to do `mfunc.mfunc()` instead.
+First, put `from mfunc.mfunc import mfunc` at the top of your code.
+Then, if you have already defined a function `f(x)`, you can initiate an instance of an `mfunc` by assigning `mfunc(f)` to a variable.
 ## Supported Features
 Here is the list of supported features for an `mfunc`:<br><br>
 * Item retrieval and slicing (e.g. `mfunc(lambda x:x)[:5]` returns the values of the function from 0 to 4).<br>
 
-* The arithmetic operators `+ - * / // **`<br>
+* The arithmetic operators `+ - * / // **`.<br>
 
 * A string representation (returns actual function).
 ## Bugs
 If you hae discovered a bug or have an idea, post it [here](https://github.com/PlaceReporter99/mfunc-bug-tracker/issues).
```

