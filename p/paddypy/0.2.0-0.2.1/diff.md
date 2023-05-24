# Comparing `tmp/paddypy-0.2.0.tar.gz` & `tmp/paddypy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paddypy-0.2.0.tar", last modified: Fri May  5 08:58:21 2023, max compression
+gzip compressed data, was "paddypy-0.2.1.tar", last modified: Fri May  5 09:10:26 2023, max compression
```

## Comparing `paddypy-0.2.0.tar` & `paddypy-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 08:58:21.691841 paddypy-0.2.0/
--rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1795 2023-05-05 08:58:21.691341 paddypy-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 08:58:21.677342 paddypy-0.2.0/paddypy/
--rw-rw-rw-   0        0        0      102 2023-04-17 12:26:22.000000 paddypy-0.2.0/paddypy/__init__.py
--rw-rw-rw-   0        0        0     5772 2023-04-17 12:26:22.000000 paddypy-0.2.0/paddypy/access.py
--rw-rw-rw-   0        0        0     5020 2023-05-05 08:58:00.000000 paddypy-0.2.0/paddypy/log.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:58:21.690340 paddypy-0.2.0/paddypy.egg-info/
--rw-rw-rw-   0        0        0     1795 2023-05-05 08:58:21.000000 paddypy-0.2.0/paddypy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-05 08:58:21.000000 paddypy-0.2.0/paddypy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 08:58:21.000000 paddypy-0.2.0/paddypy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-05-05 08:58:21.000000 paddypy-0.2.0/paddypy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-05 08:58:21.000000 paddypy-0.2.0/paddypy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 08:58:21.691841 paddypy-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1480 2023-05-05 08:53:10.000000 paddypy-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:10:26.633408 paddypy-0.2.1/
+-rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     1795 2023-05-05 09:10:26.632910 paddypy-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 09:10:26.619409 paddypy-0.2.1/paddypy/
+-rw-rw-rw-   0        0        0      102 2023-04-17 12:26:22.000000 paddypy-0.2.1/paddypy/__init__.py
+-rw-rw-rw-   0        0        0     5772 2023-04-17 12:26:22.000000 paddypy-0.2.1/paddypy/access.py
+-rw-rw-rw-   0        0        0     5064 2023-05-05 09:10:04.000000 paddypy-0.2.1/paddypy/log.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:10:26.631408 paddypy-0.2.1/paddypy.egg-info/
+-rw-rw-rw-   0        0        0     1795 2023-05-05 09:10:26.000000 paddypy-0.2.1/paddypy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-05 09:10:26.000000 paddypy-0.2.1/paddypy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 09:10:26.000000 paddypy-0.2.1/paddypy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-05-05 09:10:26.000000 paddypy-0.2.1/paddypy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-05 09:10:26.000000 paddypy-0.2.1/paddypy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 09:10:26.633408 paddypy-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1480 2023-05-05 09:07:24.000000 paddypy-0.2.1/setup.py
```

### Comparing `paddypy-0.2.0/LICENSE` & `paddypy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paddypy-0.2.0/PKG-INFO` & `paddypy-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.2.0
+Version: 0.2.1
 Summary: Collection of helpfull extensions
 Author: Patrik
 Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paddypy-0.2.0/README.md` & `paddypy-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `paddypy-0.2.0/paddypy/access.py` & `paddypy-0.2.1/paddypy/access.py`

 * *Files identical despite different names*

### Comparing `paddypy-0.2.0/paddypy/log.py` & `paddypy-0.2.1/paddypy/log.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,41 +45,41 @@
         if applicationinsights_key:
             azure_handler = AzureLogHandler(connection_string=str(applicationinsights_key))
             azure_handler.setLevel(logger_level)
             logger.addHandler(azure_handler)
         return logger
 
 
-    def timeit(self, func):
-        @wraps(func)
-        def timeit_wrapper(*args, **kwargs):
-            start_time = time.perf_counter()
-            result = func(*args, **kwargs)
-            end_time = time.perf_counter()
-            total_time = end_time - start_time
-            self.logger.log(msg=f'Function {func.__name__}{args} {kwargs} Took {total_time:.4f} seconds', level=logging.INFO)
-            #logging.log(f'Function {func.__name__}{args} {kwargs} Took {total_time:.4f} seconds', level=logging.DEBUG)
-            return result
-        return timeit_wrapper
+    # def timeit(self, func):
+    #     @wraps(func)
+    #     def timeit_wrapper(*args, **kwargs):
+    #         start_time = time.perf_counter()
+    #         result = func(*args, **kwargs)
+    #         end_time = time.perf_counter()
+    #         total_time = end_time - start_time
+    #         self.logger.log(msg=f'Function {func.__name__}{args} {kwargs} Took {total_time:.4f} seconds', level=logging.INFO)
+    #         #logging.log(f'Function {func.__name__}{args} {kwargs} Took {total_time:.4f} seconds', level=logging.DEBUG)
+    #         return result
+    #     return timeit_wrapper
     
-    def timeit_silence(self, func):
-        @wraps(func)
-        def timeit_wrapper(*args, **kwargs):
-            start_time = time.perf_counter()
-            result = func(*args, **kwargs)
-            end_time = time.perf_counter()
-            total_time = end_time - start_time
-            arg_types = tuple(type(arg).__name__ for arg in args)
-            kwarg_types = {key: type(val).__name__ for key, val in kwargs.items()}
-            log_msg = f'Function {func.__name__}{arg_types} {kwarg_types} Took {total_time:.4f} seconds'
-            self.logger.log(msg=log_msg, level=logging.INFO)
-            return result
-        return timeit_wrapper
+    # def timeit_silence(self, func):
+    #     @wraps(func)
+    #     def timeit_wrapper(*args, **kwargs):
+    #         start_time = time.perf_counter()
+    #         result = func(*args, **kwargs)
+    #         end_time = time.perf_counter()
+    #         total_time = end_time - start_time
+    #         arg_types = tuple(type(arg).__name__ for arg in args)
+    #         kwarg_types = {key: type(val).__name__ for key, val in kwargs.items()}
+    #         log_msg = f'Function {func.__name__}{arg_types} {kwarg_types} Took {total_time:.4f} seconds'
+    #         self.logger.log(msg=log_msg, level=logging.INFO)
+    #         return result
+    #     return timeit_wrapper
     
-    def timeit_opt(self, silence_args=False):
+    def timeit(self, silence_args=False):
         def decorator(func):
             @wraps(func)
             def timeit_wrapper(*args, **kwargs):
                 start_time = time.perf_counter()
                 result = func(*args, **kwargs)
                 end_time = time.perf_counter()
                 total_time = end_time - start_time
```

### Comparing `paddypy-0.2.0/paddypy.egg-info/PKG-INFO` & `paddypy-0.2.1/paddypy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.2.0
+Version: 0.2.1
 Summary: Collection of helpfull extensions
 Author: Patrik
 Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paddypy-0.2.0/setup.py` & `paddypy-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.0'
+VERSION = '0.2.1'
 DESCRIPTION = 'Collection of helpfull extensions'
 LONG_DESCRIPTION = 'Collection of helpfull extensions'
 
 # Setting up
 setup(
     name="paddypy",
     version=VERSION,
```

