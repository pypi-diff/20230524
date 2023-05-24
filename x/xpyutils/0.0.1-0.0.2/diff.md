# Comparing `tmp/xpyutils-0.0.1.tar.gz` & `tmp/xpyutils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpyutils-0.0.1.tar", last modified: Tue May 23 17:22:58 2023, max compression
+gzip compressed data, was "xpyutils-0.0.2.tar", last modified: Wed May 24 04:57:42 2023, max compression
```

## Comparing `xpyutils-0.0.1.tar` & `xpyutils-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-05-23 17:22:58.944019 xpyutils-0.0.1/
--rw-r--r--   0 isaac      (501) staff       (20)     1323 2023-05-23 17:22:58.943911 xpyutils-0.0.1/PKG-INFO
--rw-r--r--   0 isaac      (501) staff       (20)      973 2023-05-23 07:17:55.000000 xpyutils-0.0.1/README.md
--rw-r--r--   0 isaac      (501) staff       (20)      601 2023-05-23 16:14:07.000000 xpyutils-0.0.1/pyproject.toml
--rw-r--r--   0 isaac      (501) staff       (20)       38 2023-05-23 17:22:58.944055 xpyutils-0.0.1/setup.cfg
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-05-23 17:22:58.942014 xpyutils-0.0.1/tests/
--rw-r--r--   0 isaac      (501) staff       (20)        0 2023-05-18 09:22:19.000000 xpyutils-0.0.1/tests/__init__.py
--rw-r--r--   0 isaac      (501) staff       (20)     3842 2023-05-23 06:31:20.000000 xpyutils-0.0.1/tests/test_lazy_property.py
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-05-23 17:22:58.942279 xpyutils-0.0.1/xpyutils/
--rw-r--r--   0 isaac      (501) staff       (20)       70 2023-05-17 11:22:49.000000 xpyutils-0.0.1/xpyutils/__init__.py
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-05-23 17:22:58.943665 xpyutils-0.0.1/xpyutils/property/
--rw-r--r--   0 isaac      (501) staff       (20)       66 2023-05-17 15:27:57.000000 xpyutils-0.0.1/xpyutils/property/__init__.py
--rw-r--r--   0 isaac      (501) staff       (20)     2177 2023-05-23 06:09:51.000000 xpyutils-0.0.1/xpyutils/property/base.py
--rw-r--r--   0 isaac      (501) staff       (20)     3633 2023-05-23 06:17:59.000000 xpyutils-0.0.1/xpyutils/property/lazy.py
--rw-r--r--   0 isaac      (501) staff       (20)     1886 2023-05-23 06:30:34.000000 xpyutils-0.0.1/xpyutils/property/presence_required.py
-drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-05-23 17:22:58.942850 xpyutils-0.0.1/xpyutils.egg-info/
--rw-r--r--   0 isaac      (501) staff       (20)     1323 2023-05-23 17:22:58.000000 xpyutils-0.0.1/xpyutils.egg-info/PKG-INFO
--rw-r--r--   0 isaac      (501) staff       (20)      340 2023-05-23 17:22:58.000000 xpyutils-0.0.1/xpyutils.egg-info/SOURCES.txt
--rw-r--r--   0 isaac      (501) staff       (20)        1 2023-05-23 17:22:58.000000 xpyutils-0.0.1/xpyutils.egg-info/dependency_links.txt
--rw-r--r--   0 isaac      (501) staff       (20)       15 2023-05-23 17:22:58.000000 xpyutils-0.0.1/xpyutils.egg-info/top_level.txt
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-05-24 04:57:42.415547 xpyutils-0.0.2/
+-rw-r--r--   0 isaac      (501) staff       (20)     1323 2023-05-24 04:57:42.415439 xpyutils-0.0.2/PKG-INFO
+-rw-r--r--   0 isaac      (501) staff       (20)      973 2023-05-24 04:54:52.000000 xpyutils-0.0.2/README.md
+-rw-r--r--   0 isaac      (501) staff       (20)      601 2023-05-24 04:57:09.000000 xpyutils-0.0.2/pyproject.toml
+-rw-r--r--   0 isaac      (501) staff       (20)       38 2023-05-24 04:57:42.415591 xpyutils-0.0.2/setup.cfg
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-05-24 04:57:42.414305 xpyutils-0.0.2/tests/
+-rw-r--r--   0 isaac      (501) staff       (20)        0 2023-05-18 09:22:19.000000 xpyutils-0.0.2/tests/__init__.py
+-rw-r--r--   0 isaac      (501) staff       (20)     3842 2023-05-24 04:54:52.000000 xpyutils-0.0.2/tests/test_lazy_property.py
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-05-24 04:57:42.414423 xpyutils-0.0.2/xpyutils/
+-rw-r--r--   0 isaac      (501) staff       (20)       70 2023-05-17 11:22:49.000000 xpyutils-0.0.2/xpyutils/__init__.py
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-05-24 04:57:42.415290 xpyutils-0.0.2/xpyutils/property/
+-rw-r--r--   0 isaac      (501) staff       (20)       66 2023-05-17 15:27:57.000000 xpyutils-0.0.2/xpyutils/property/__init__.py
+-rw-r--r--   0 isaac      (501) staff       (20)     2177 2023-05-23 06:09:51.000000 xpyutils-0.0.2/xpyutils/property/base.py
+-rw-r--r--   0 isaac      (501) staff       (20)     3633 2023-05-24 04:57:05.000000 xpyutils-0.0.2/xpyutils/property/lazy.py
+-rw-r--r--   0 isaac      (501) staff       (20)     1886 2023-05-23 06:30:34.000000 xpyutils-0.0.2/xpyutils/property/presence_required.py
+drwxr-xr-x   0 isaac      (501) staff       (20)        0 2023-05-24 04:57:42.414840 xpyutils-0.0.2/xpyutils.egg-info/
+-rw-r--r--   0 isaac      (501) staff       (20)     1323 2023-05-24 04:57:42.000000 xpyutils-0.0.2/xpyutils.egg-info/PKG-INFO
+-rw-r--r--   0 isaac      (501) staff       (20)      340 2023-05-24 04:57:42.000000 xpyutils-0.0.2/xpyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 isaac      (501) staff       (20)        1 2023-05-24 04:57:42.000000 xpyutils-0.0.2/xpyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 isaac      (501) staff       (20)       15 2023-05-24 04:57:42.000000 xpyutils-0.0.2/xpyutils.egg-info/top_level.txt
```

### Comparing `xpyutils-0.0.1/PKG-INFO` & `xpyutils-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: xpyutils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Ongoing project of extra Python utilities including implementations of lazy property, regular expression, ...
 Author-email: Isaac Fei <isaac.omega.fei@gmail.com>
 Project-URL: Homepage, https://github.com/Isaac-Fate/xpyutils
-Requires-Python: >=3.8
+Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 
 # Extra Python Utilities
 
 🛠️ Ongoing project of extra Python utilities including implementation of lazy property, 
 collections of common regular expressions, ...
 
@@ -35,15 +35,15 @@
     
     @lazy_property
     def lucky_number(self) -> int:
         """Lucky number.
         """
         return random.randint(0, 100)
     
-    @lazy_property.require_presense()
+    @lazy_property.require_presence()
     def age(self) -> int:
         """Age.
         """
         return random.randint(20, 30)
     
 person = Person('Isaac')
```

### Comparing `xpyutils-0.0.1/README.md` & `xpyutils-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     
     @lazy_property
     def lucky_number(self) -> int:
         """Lucky number.
         """
         return random.randint(0, 100)
     
-    @lazy_property.require_presense()
+    @lazy_property.require_presence()
     def age(self) -> int:
         """Age.
         """
         return random.randint(20, 30)
     
 person = Person('Isaac')
```

### Comparing `xpyutils-0.0.1/pyproject.toml` & `xpyutils-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 [tool.setuptools.packages.find]
 where = ['.']
 exclude = ['playground']  # empty by default
 namespaces = false  # true by default
 
 [project]
 name = 'xpyutils'
-version = '0.0.1'
+version = '0.0.2'
 authors = [
     {name = 'Isaac Fei', email = 'isaac.omega.fei@gmail.com'},
 ]
 description = 'Ongoing project of extra Python utilities including implementations of lazy property, regular expression, ...'
 readme = 'README.md'
-requires-python = '>=3.8'
+requires-python = '>=3.0'
 dependencies = []
 
 [project.urls]
 Homepage = 'https://github.com/Isaac-Fate/xpyutils'
```

### Comparing `xpyutils-0.0.1/tests/test_lazy_property.py` & `xpyutils-0.0.2/tests/test_lazy_property.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,66 +33,66 @@
         
         random.seed(42)
         self.assertEqual(p.lucky_number, 81)
         
         p.lucky_number = 100
         self.assertEqual(p.lucky_number, 100)
 
-    def test_get_presense_required_lazy_property(self):
+    def test_get_presence_required_lazy_property(self):
         
         class Person(BasePerson):
             
             def __init__(self, name: str) -> None:
                 super().__init__(name)
                 
-            @lazy_property.require_presense()
+            @lazy_property.require_presence()
             def lucky_number(self) -> int:
                 return random.randint(0, 100)
         
         p = Person("Isaac")
         self.assertEqual(p.name, "Isaac")
         
         try:
             p.lucky_number
         except Exception as e:
             self.assertEqual(
                 str(e), 
                 "property 'lucky_number' is not present yet"
             )
 
-    def test_cannot_set_presense_required_lazy_property(self):
+    def test_cannot_set_presence_required_lazy_property(self):
         
         class Person(BasePerson):
             
             def __init__(self, name: str) -> None:
                 super().__init__(name)
                 
-            @lazy_property.require_presense()
+            @lazy_property.require_presence()
             def name(self) -> str:
                 return self._name
         
         p = Person('Isaac')
         self.assertEqual(p.name, 'Isaac')
         
         try:
             p.name = 'Albert'
         except Exception as e:
             self.assertEqual(
                 str(e), 
                 "setting 'name' is not allowed"
             )
 
-    def test_can_set_presense_required_lazy_property(self):
+    def test_can_set_presence_required_lazy_property(self):
         
         class Person(BasePerson):
             
             def __init__(self, name: str) -> None:
                 super().__init__(name)
                 
-            @lazy_property.require_presense()
+            @lazy_property.require_presence()
             def name(self) -> str:
                 return self._name
             
             @name.setter
             def name(self, new_name: str) -> None:
                 self._name = new_name
         
@@ -104,15 +104,15 @@
         self.assertDictEqual(
             p.__dict__,
             dict(
                 _name='Albert'
             )
         )
     
-    def test_get_presense_required_lazy_property_with_warning(self):
+    def test_get_presence_required_lazy_property_with_warning(self):
         
         class Person(BasePerson):
             
             def __init__(self, name: str) -> None:
                 super().__init__(name)
             
             @lazy_property.with_default_value_when_missing(
```

### Comparing `xpyutils-0.0.1/xpyutils/property/base.py` & `xpyutils-0.0.2/xpyutils/property/base.py`

 * *Files identical despite different names*

### Comparing `xpyutils-0.0.1/xpyutils/property/lazy.py` & `xpyutils-0.0.2/xpyutils/property/lazy.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             get_property, 
             set_property, 
             delete_property, 
             doc
         )
     
     @classmethod
-    def require_presense(
+    def require_presence(
             cls, 
             error_message: str | None = None
         ) -> partial[presence_required_property]:
         """The property is required to be present when accessed.
         Otherwise, an exception will be raised.
 
         Parameters
```

### Comparing `xpyutils-0.0.1/xpyutils/property/presence_required.py` & `xpyutils-0.0.2/xpyutils/property/presence_required.py`

 * *Files identical despite different names*

### Comparing `xpyutils-0.0.1/xpyutils.egg-info/PKG-INFO` & `xpyutils-0.0.2/xpyutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: xpyutils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Ongoing project of extra Python utilities including implementations of lazy property, regular expression, ...
 Author-email: Isaac Fei <isaac.omega.fei@gmail.com>
 Project-URL: Homepage, https://github.com/Isaac-Fate/xpyutils
-Requires-Python: >=3.8
+Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 
 # Extra Python Utilities
 
 🛠️ Ongoing project of extra Python utilities including implementation of lazy property, 
 collections of common regular expressions, ...
 
@@ -35,15 +35,15 @@
     
     @lazy_property
     def lucky_number(self) -> int:
         """Lucky number.
         """
         return random.randint(0, 100)
     
-    @lazy_property.require_presense()
+    @lazy_property.require_presence()
     def age(self) -> int:
         """Age.
         """
         return random.randint(20, 30)
     
 person = Person('Isaac')
```

