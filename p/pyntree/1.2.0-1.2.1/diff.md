# Comparing `tmp/pyntree-1.2.0.tar.gz` & `tmp/pyntree-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyntree-1.2.0.tar", last modified: Mon May  8 23:30:51 2023, max compression
+gzip compressed data, was "pyntree-1.2.1.tar", last modified: Tue May 23 22:59:12 2023, max compression
```

## Comparing `pyntree-1.2.0.tar` & `pyntree-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-05-08 23:30:51.166399 pyntree-1.2.0/
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    11357 2023-03-27 17:16:15.000000 pyntree-1.2.0/LICENSE.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    15475 2023-05-08 23:30:51.162399 pyntree-1.2.0/PKG-INFO
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1585 2023-03-29 03:58:07.000000 pyntree-1.2.0/README.md
-drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-05-08 23:30:51.162399 pyntree-1.2.0/pyntree/
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     9124 2023-05-08 23:22:16.000000 pyntree-1.2.0/pyntree/__init__.py
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1128 2023-04-17 13:39:08.000000 pyntree-1.2.0/pyntree/encryption.py
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      166 2023-04-10 21:40:01.000000 pyntree-1.2.0/pyntree/errors.py
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     6259 2023-03-29 03:58:07.000000 pyntree-1.2.0/pyntree/file.py
-drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-05-08 23:30:51.162399 pyntree-1.2.0/pyntree.egg-info/
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    15475 2023-05-08 23:30:51.000000 pyntree-1.2.0/pyntree.egg-info/PKG-INFO
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      298 2023-05-08 23:30:51.000000 pyntree-1.2.0/pyntree.egg-info/SOURCES.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)        1 2023-05-08 23:30:51.000000 pyntree-1.2.0/pyntree.egg-info/dependency_links.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      117 2023-05-08 23:30:51.000000 pyntree-1.2.0/pyntree.egg-info/requires.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)        8 2023-05-08 23:30:51.000000 pyntree-1.2.0/pyntree.egg-info/top_level.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1298 2023-05-08 23:30:41.000000 pyntree-1.2.0/pyproject.toml
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)       23 2023-03-27 16:14:00.000000 pyntree-1.2.0/requirements.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)       38 2023-05-08 23:30:51.166399 pyntree-1.2.0/setup.cfg
-drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-05-08 23:30:51.162399 pyntree-1.2.0/tests/
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    11299 2023-05-08 23:14:11.000000 pyntree-1.2.0/tests/tests.py
+drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-05-23 22:59:12.838169 pyntree-1.2.1/
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    11357 2023-03-27 17:16:15.000000 pyntree-1.2.1/LICENSE.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    15475 2023-05-23 22:59:12.838169 pyntree-1.2.1/PKG-INFO
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1585 2023-03-29 03:58:07.000000 pyntree-1.2.1/README.md
+drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-05-23 22:59:12.834169 pyntree-1.2.1/pyntree/
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     9292 2023-05-23 22:51:03.000000 pyntree-1.2.1/pyntree/__init__.py
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1128 2023-04-17 13:39:08.000000 pyntree-1.2.1/pyntree/encryption.py
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      166 2023-04-10 21:40:01.000000 pyntree-1.2.1/pyntree/errors.py
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     6436 2023-05-23 22:51:02.000000 pyntree-1.2.1/pyntree/file.py
+drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-05-23 22:59:12.834169 pyntree-1.2.1/pyntree.egg-info/
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    15475 2023-05-23 22:59:12.000000 pyntree-1.2.1/pyntree.egg-info/PKG-INFO
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      298 2023-05-23 22:59:12.000000 pyntree-1.2.1/pyntree.egg-info/SOURCES.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)        1 2023-05-23 22:59:12.000000 pyntree-1.2.1/pyntree.egg-info/dependency_links.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      126 2023-05-23 22:59:12.000000 pyntree-1.2.1/pyntree.egg-info/requires.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)        8 2023-05-23 22:59:12.000000 pyntree-1.2.1/pyntree.egg-info/top_level.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1310 2023-05-23 22:54:39.000000 pyntree-1.2.1/pyproject.toml
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)       23 2023-03-27 16:14:00.000000 pyntree-1.2.1/requirements.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)       38 2023-05-23 22:59:12.838169 pyntree-1.2.1/setup.cfg
+drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-05-23 22:59:12.838169 pyntree-1.2.1/tests/
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    11430 2023-05-23 22:52:34.000000 pyntree-1.2.1/tests/tests.py
```

### Comparing `pyntree-1.2.0/LICENSE.txt` & `pyntree-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyntree-1.2.0/PKG-INFO` & `pyntree-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyntree
-Version: 1.2.0
+Version: 1.2.1
 Summary: pyntree is a python package which allows you to easily and syntactically save your data. Not only that, it also lets you save in multiple formats, and even serialize and compress data by merely changing a few characters.
 Author-email: jvadair <dev@jvadair.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pyntree-1.2.0/README.md` & `pyntree-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyntree-1.2.0/pyntree/__init__.py` & `pyntree-1.2.1/pyntree/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -203,39 +203,39 @@
         """
         :return: The Node's value, as it would be returned by __call__
         """
         return self()
 
     # Arithmetic operations - only for child Nodes since the operations don't work on dictionaries anyways
     def __iadd__(self, other):
-        self.file.data[self.path[0]] += other
+        self.file.get_nested(*self.path[:-1])[self.path[-1]] += other
         return self()
 
     def __isub__(self, other):
-        self.file.data[self.path[0]] -= other
+        self.file.get_nested(*self.path[:-1])[self.path[-1]] -= other
         return self()
 
     def __imul__(self, other):
-        self.file.data[self.path[0]] *= other
+        self.file.get_nested(*self.path[:-1])[self.path[-1]] *= other
         return self()
 
     def __itruediv__(self, other):
-        self.file.data[self.path[0]] /= other
+        self.file.get_nested(*self.path[:-1])[self.path[-1]] /= other
         return self()
 
     def __ifloordiv__(self, other):
-        self.file.data[self.path[0]] //= other
+        self.file.get_nested(*self.path[:-1])[self.path[-1]] //= other
         return self()
 
     def __imod__(self, other):
-        self.file.data[self.path[0]] %= other
+        self.file.get_nested(*self.path[:-1])[self.path[-1]] %= other
         return self()
 
     def __ipow__(self, other):
-        self.file.data[self.path[0]] **= other
+        self.file.get_nested(*self.path[:-1])[self.path[-1]] **= other
         return self()
 
     # Comparison methods (<, >, <=, >=, ==, !=)
     def __lt__(self, other):
         return True if self() < other() else False
 
     def __le__(self, other):
```

### Comparing `pyntree-1.2.0/pyntree/encryption.py` & `pyntree-1.2.1/pyntree/encryption.py`

 * *Files identical despite different names*

### Comparing `pyntree-1.2.0/pyntree/file.py` & `pyntree-1.2.1/pyntree/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,20 @@
         
         self.file.seek(0)
         self.file.write(to_write)
         self.file.truncate()
         if filename and old_filename:  # If the old filename was None, then it can't be switched back to
             self.switch_to_file(old_filename)
 
+    def get_nested(self, *args):
+        found = self.data
+        for child in args:
+            found = found[child]  # Move 1 deeper towards the target
+        return found
+
     def __del__(self) -> None:
         """
         Garbage collector function for implementing save_on_close and properly closing the file object
         :return:
         """
         if 'file' in self.__dict__.keys():  # If file attribute was set
             if self.save_on_close:
```

### Comparing `pyntree-1.2.0/pyntree.egg-info/PKG-INFO` & `pyntree-1.2.1/pyntree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyntree
-Version: 1.2.0
+Version: 1.2.1
 Summary: pyntree is a python package which allows you to easily and syntactically save your data. Not only that, it also lets you save in multiple formats, and even serialize and compress data by merely changing a few characters.
 Author-email: jvadair <dev@jvadair.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pyntree-1.2.0/pyproject.toml` & `pyntree-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dynamic = ["dependencies"]
 name = "pyntree"
-version = "1.2.0"
+version = "1.2.1"
 description = "pyntree is a python package which allows you to easily and syntactically save your data. Not only that, it also lets you save in multiple formats, and even serialize and compress data by merely changing a few characters."
 readme = "README.md"
 authors = [{ name = "jvadair", email = "dev@jvadair.com" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
@@ -18,15 +18,15 @@
     "Topic :: Database",
 ]
 keywords = ["database", "pyntree", "pyndb", "python", "encryption", "crypto", "cryptography", "security"]
 requires-python = ">=3.7.3"
 
 [project.optional-dependencies]  # Format: pip3 install pyntree[dev]
 lz4 = ["compress_pickle[lz4]"]
-dev = ["pipreqs", "build", "twine"]
+dev = ["pipreqs", "build", "twine", "requests"]
 encryption = ["cryptography", "argon2-cffi"]
 
 [project.urls]
 Homepage = "https://github.com/jvadair/pyntree"
 Documentation = "https://pen.jvadair.com/books/pyntree"
 
 [tool.setuptools]
```

### Comparing `pyntree-1.2.0/tests/tests.py` & `pyntree-1.2.1/tests/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -358,11 +358,15 @@
         self.assertTrue(db.a < db.b)
         self.assertTrue(db.a <= db.b)
         self.assertFalse(db.a > db.b)
         self.assertFalse(db.a >= db.b)
         self.assertFalse(db.a == db.b)
         self.assertTrue(db.a != db.b)
 
+    def test_nested_operations(self):
+        db = Node({'a': {'b': 1}})
+        db.a.b += 1
+        self.assertEqual(db.a.b(), 2)
 
 
 if __name__ == '__main__':
     unittest.main()
```

