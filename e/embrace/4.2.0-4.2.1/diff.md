# Comparing `tmp/embrace-4.2.0.tar.gz` & `tmp/embrace-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embrace-4.2.0.tar", last modified: Thu Dec  8 14:23:11 2022, max compression
+gzip compressed data, was "embrace-4.2.1.tar", last modified: Wed May 24 12:03:35 2023, max compression
```

## Comparing `embrace-4.2.0.tar` & `embrace-4.2.1.tar`

### file list

```diff
@@ -1,21 +1,27 @@
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2022-12-08 14:23:11.790939 embrace-4.2.0/
--rw-r--r--   0 oliver    (1001) wheel        (0)    11358 2022-12-08 14:21:55.000000 embrace-4.2.0/LICENSE.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)    12509 2022-12-08 14:23:11.791065 embrace-4.2.0/PKG-INFO
--rw-r--r--   0 oliver    (1001) wheel        (0)    11800 2022-12-08 14:21:55.000000 embrace-4.2.0/README.rst
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2022-12-08 14:23:11.789687 embrace-4.2.0/embrace/
--rw-r--r--   0 oliver    (1001) wheel        (0)      804 2022-12-08 14:21:55.000000 embrace-4.2.0/embrace/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1938 2022-12-08 14:21:55.000000 embrace-4.2.0/embrace/exceptions.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     9891 2022-12-08 14:21:55.000000 embrace-4.2.0/embrace/module.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     8810 2022-12-08 14:21:55.000000 embrace-4.2.0/embrace/parsing.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     6244 2022-12-08 14:21:55.000000 embrace-4.2.0/embrace/pool.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1897 2022-12-08 14:21:55.000000 embrace-4.2.0/embrace/poolvalidators.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    28346 2022-12-08 14:21:55.000000 embrace-4.2.0/embrace/query.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3682 2022-12-08 14:21:55.000000 embrace-4.2.0/embrace/util.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2022-12-08 14:23:11.790748 embrace-4.2.0/embrace.egg-info/
--rw-r--r--   0 oliver    (1001) wheel        (0)    12509 2022-12-08 14:23:11.000000 embrace-4.2.0/embrace.egg-info/PKG-INFO
--rw-r--r--   0 oliver    (1001) wheel        (0)      349 2022-12-08 14:23:11.000000 embrace-4.2.0/embrace.egg-info/SOURCES.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)        1 2022-12-08 14:23:11.000000 embrace-4.2.0/embrace.egg-info/dependency_links.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)       15 2022-12-08 14:23:11.000000 embrace-4.2.0/embrace.egg-info/requires.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)        8 2022-12-08 14:23:11.000000 embrace-4.2.0/embrace.egg-info/top_level.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)      748 2022-12-08 14:23:11.791658 embrace-4.2.0/setup.cfg
--rwxr-xr-x   0 oliver    (1001) wheel        (0)      635 2022-12-08 14:21:55.000000 embrace-4.2.0/setup.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-24 12:03:35.197627 embrace-4.2.1/
+-rw-r--r--   0 oliver    (1001) wheel        (0)    11358 2023-05-24 12:02:20.000000 embrace-4.2.1/LICENSE.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)    12509 2023-05-24 12:03:35.197758 embrace-4.2.1/PKG-INFO
+-rw-r--r--   0 oliver    (1001) wheel        (0)    11800 2023-05-24 12:02:20.000000 embrace-4.2.1/README.rst
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-24 12:03:35.195308 embrace-4.2.1/embrace/
+-rw-r--r--   0 oliver    (1001) wheel        (0)      804 2023-05-24 12:02:20.000000 embrace-4.2.1/embrace/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1938 2023-05-24 12:02:20.000000 embrace-4.2.1/embrace/exceptions.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     9891 2023-05-24 12:02:20.000000 embrace-4.2.1/embrace/module.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     8810 2023-05-24 12:02:20.000000 embrace-4.2.1/embrace/parsing.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     6260 2023-05-24 12:02:20.000000 embrace-4.2.1/embrace/pool.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1897 2023-05-24 12:02:20.000000 embrace-4.2.1/embrace/poolvalidators.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    28346 2023-05-24 12:02:20.000000 embrace-4.2.1/embrace/query.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3682 2023-05-24 12:02:20.000000 embrace-4.2.1/embrace/util.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-24 12:03:35.196375 embrace-4.2.1/embrace.egg-info/
+-rw-r--r--   0 oliver    (1001) wheel        (0)    12509 2023-05-24 12:03:34.000000 embrace-4.2.1/embrace.egg-info/PKG-INFO
+-rw-r--r--   0 oliver    (1001) wheel        (0)      450 2023-05-24 12:03:34.000000 embrace-4.2.1/embrace.egg-info/SOURCES.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)        1 2023-05-24 12:03:34.000000 embrace-4.2.1/embrace.egg-info/dependency_links.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)       15 2023-05-24 12:03:34.000000 embrace-4.2.1/embrace.egg-info/requires.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)        8 2023-05-24 12:03:34.000000 embrace-4.2.1/embrace.egg-info/top_level.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)      748 2023-05-24 12:03:35.198356 embrace-4.2.1/setup.cfg
+-rwxr-xr-x   0 oliver    (1001) wheel        (0)      635 2023-05-24 12:02:20.000000 embrace-4.2.1/setup.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-24 12:03:35.197446 embrace-4.2.1/tests/
+-rw-r--r--   0 oliver    (1001) wheel        (0)     6390 2023-05-24 12:02:20.000000 embrace-4.2.1/tests/test_module.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3342 2023-05-24 12:02:20.000000 embrace-4.2.1/tests/test_parsing.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1626 2023-05-24 12:02:20.000000 embrace-4.2.1/tests/test_pool.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    19059 2023-05-24 12:02:20.000000 embrace-4.2.1/tests/test_query.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1010 2023-05-24 12:02:20.000000 embrace-4.2.1/tests/test_util.py
```

### Comparing `embrace-4.2.0/LICENSE.txt` & `embrace-4.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `embrace-4.2.0/PKG-INFO` & `embrace-4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embrace
-Version: 4.2.0
+Version: 4.2.1
 Summary: Embrace SQL keeps your SQL queries in SQL files. An anti-ORM inspired by HugSQL and PugSQL
 Home-page: https://hg.sr.ht/~olly/embrace-sql
 Author: Oliver Cope
 Author-email: oliver@redgecko.org
 License: Apache
 Keywords: sql hugsql pugsql orm anti-orm files dapper
 Classifier: Development Status :: 4 - Beta
```

### Comparing `embrace-4.2.0/README.rst` & `embrace-4.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `embrace-4.2.0/embrace/__init__.py` & `embrace-4.2.1/embrace/__init__.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.0/embrace/exceptions.py` & `embrace-4.2.1/embrace/exceptions.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.0/embrace/module.py` & `embrace-4.2.1/embrace/module.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.0/embrace/parsing.py` & `embrace-4.2.1/embrace/parsing.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.0/embrace/pool.py` & `embrace-4.2.1/embrace/pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,20 +69,28 @@
             return self._getconn()
         for retry in range(self.max_validation_retries):
             conn = self._getconn()
             if self.validate(conn):
                 return conn
             self.release(conn)
         raise Exception(
-            f"Could not validate a connection after {self.max_validation_retries} attempts"
+            f"Could not validate a connection after "
+            f"{self.max_validation_retries} attempts"
         )
 
     def release(self, conn: ConnType):
         raise NotImplementedError()
 
+    def connect(self):
+        """
+        Return a context manager that manages acquiring and releasing a
+        connection.
+        """
+        return ContextManagerWrappedConnection(self)
+
     def set_validator(self, v):
         self.validate = v.validate
         self.before_release = v.before_release
 
     def auto_validate(self, conn):
         validator = poolvalidators.ConnectionValidator()
 
@@ -113,21 +121,14 @@
 
         self._pool = self.queue_class()
         self.lock = self.lock_class()
         self.connections_created = 0
         self.reached_limit = False
         self.timeout = timeout
 
-    def connect(self):
-        """
-        Return a context manager that manages acquiring and releasing a
-        connection.
-        """
-        return ContextManagerWrappedConnection(self)
-
     def _getconn(self):
         """
         Return a connection from the pool.
         """
         try:
             return self._pool.get(block=self.reached_limit, timeout=self.timeout)
         except queue.Empty:
```

### Comparing `embrace-4.2.0/embrace/poolvalidators.py` & `embrace-4.2.1/embrace/poolvalidators.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.0/embrace/query.py` & `embrace-4.2.1/embrace/query.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.0/embrace/util.py` & `embrace-4.2.1/embrace/util.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.0/embrace.egg-info/PKG-INFO` & `embrace-4.2.1/embrace.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embrace
-Version: 4.2.0
+Version: 4.2.1
 Summary: Embrace SQL keeps your SQL queries in SQL files. An anti-ORM inspired by HugSQL and PugSQL
 Home-page: https://hg.sr.ht/~olly/embrace-sql
 Author: Oliver Cope
 Author-email: oliver@redgecko.org
 License: Apache
 Keywords: sql hugsql pugsql orm anti-orm files dapper
 Classifier: Development Status :: 4 - Beta
```

### Comparing `embrace-4.2.0/setup.cfg` & `embrace-4.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = embrace
-version = 4.2.0
+version = 4.2.1
 description = Embrace SQL keeps your SQL queries in SQL files. An anti-ORM inspired by HugSQL and PugSQL
 long_description = file: README.rst
 author = Oliver Cope
 author_email = oliver@redgecko.org
 keywords = sql hugsql pugsql orm anti-orm files dapper
 url = https://hg.sr.ht/~olly/embrace-sql
 license = Apache
```

### Comparing `embrace-4.2.0/setup.py` & `embrace-4.2.1/setup.py`

 * *Files identical despite different names*

