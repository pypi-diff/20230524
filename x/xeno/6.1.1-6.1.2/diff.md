# Comparing `tmp/xeno-6.1.1.tar.gz` & `tmp/xeno-6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeno-6.1.1.tar", last modified: Fri May  5 03:45:29 2023, max compression
+gzip compressed data, was "xeno-6.1.2.tar", last modified: Wed May 24 16:28:40 2023, max compression
```

## Comparing `xeno-6.1.1.tar` & `xeno-6.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-05 03:45:29.281481 xeno-6.1.1/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1567 2023-04-03 20:39:53.000000 xeno-6.1.1/LICENSE
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       18 2023-04-03 20:39:53.000000 xeno-6.1.1/MANIFEST.in
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9867 2023-05-05 03:45:29.281481 xeno-6.1.1/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9195 2023-04-03 20:39:53.000000 xeno-6.1.1/README.md
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-05-05 03:45:29.281481 xeno-6.1.1/setup.cfg
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1210 2023-05-05 03:45:24.000000 xeno-6.1.1/setup.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-05 03:45:29.281481 xeno-6.1.1/xeno/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1808 2023-04-18 01:18:36.000000 xeno-6.1.1/xeno/__init__.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10174 2023-04-18 01:18:36.000000 xeno-6.1.1/xeno/abstract.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    13407 2023-04-18 01:18:36.000000 xeno-6.1.1/xeno/async_injector.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7094 2023-04-18 01:18:36.000000 xeno-6.1.1/xeno/attributes.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    19364 2023-05-03 00:21:00.000000 xeno-6.1.1/xeno/build.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5004 2023-05-03 00:21:00.000000 xeno-6.1.1/xeno/color.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10293 2023-05-03 00:21:00.000000 xeno-6.1.1/xeno/cookbook.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4465 2023-04-18 01:18:36.000000 xeno-6.1.1/xeno/decorators.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2677 2023-04-14 18:38:05.000000 xeno-6.1.1/xeno/errors.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7250 2023-04-21 23:51:24.000000 xeno-6.1.1/xeno/events.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3018 2023-04-14 18:38:05.000000 xeno-6.1.1/xeno/namespaces.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1321 2023-04-14 18:38:05.000000 xeno-6.1.1/xeno/pkg_config.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    25812 2023-05-03 00:21:00.000000 xeno-6.1.1/xeno/recipe.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7140 2023-05-03 00:21:00.000000 xeno-6.1.1/xeno/shell.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2056 2023-05-03 00:21:00.000000 xeno-6.1.1/xeno/spinner.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7505 2023-04-18 01:18:36.000000 xeno-6.1.1/xeno/sync_injector.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1362 2023-04-18 01:18:36.000000 xeno-6.1.1/xeno/testing.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3258 2023-04-21 23:51:24.000000 xeno-6.1.1/xeno/utils.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-05 03:45:29.281481 xeno-6.1.1/xeno.egg-info/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9867 2023-05-05 03:45:29.000000 xeno-6.1.1/xeno.egg-info/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      455 2023-05-05 03:45:29.000000 xeno-6.1.1/xeno.egg-info/SOURCES.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-05-05 03:45:29.000000 xeno-6.1.1/xeno.egg-info/dependency_links.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        5 2023-05-05 03:45:29.000000 xeno-6.1.1/xeno.egg-info/top_level.txt
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-24 16:28:40.918533 xeno-6.1.2/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1567 2023-02-22 19:19:33.000000 xeno-6.1.2/LICENSE
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       18 2023-02-22 19:19:33.000000 xeno-6.1.2/MANIFEST.in
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-05-24 16:28:40.918533 xeno-6.1.2/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9195 2023-02-22 19:19:33.000000 xeno-6.1.2/README.md
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-05-24 16:28:40.918533 xeno-6.1.2/setup.cfg
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1160 2023-05-24 16:28:25.000000 xeno-6.1.2/setup.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-24 16:28:40.918533 xeno-6.1.2/xeno/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1808 2023-05-24 16:26:11.000000 xeno-6.1.2/xeno/__init__.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10174 2023-04-25 17:49:02.000000 xeno-6.1.2/xeno/abstract.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    13407 2023-04-25 17:49:02.000000 xeno-6.1.2/xeno/async_injector.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7094 2023-04-25 17:49:02.000000 xeno-6.1.2/xeno/attributes.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    19488 2023-05-24 16:26:03.000000 xeno-6.1.2/xeno/build.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5004 2023-05-01 08:08:44.000000 xeno-6.1.2/xeno/color.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10217 2023-05-24 16:25:54.000000 xeno-6.1.2/xeno/cookbook.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4465 2023-04-25 17:49:02.000000 xeno-6.1.2/xeno/decorators.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2677 2023-02-22 19:19:33.000000 xeno-6.1.2/xeno/errors.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7250 2023-05-01 07:35:53.000000 xeno-6.1.2/xeno/events.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3018 2023-02-22 19:19:33.000000 xeno-6.1.2/xeno/namespaces.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1321 2023-03-04 18:15:00.000000 xeno-6.1.2/xeno/pkg_config.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    25812 2023-05-24 16:14:14.000000 xeno-6.1.2/xeno/recipe.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7140 2023-05-01 08:08:44.000000 xeno-6.1.2/xeno/shell.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2056 2023-05-01 08:08:44.000000 xeno-6.1.2/xeno/spinner.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7505 2023-04-25 17:49:02.000000 xeno-6.1.2/xeno/sync_injector.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1362 2023-04-25 17:49:02.000000 xeno-6.1.2/xeno/testing.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3258 2023-04-25 17:49:02.000000 xeno-6.1.2/xeno/utils.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-24 16:28:40.918533 xeno-6.1.2/xeno.egg-info/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-05-24 16:28:40.000000 xeno-6.1.2/xeno.egg-info/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      455 2023-05-24 16:28:40.000000 xeno-6.1.2/xeno.egg-info/SOURCES.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-05-24 16:28:40.000000 xeno-6.1.2/xeno.egg-info/dependency_links.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        5 2023-05-24 16:28:40.000000 xeno-6.1.2/xeno.egg-info/top_level.txt
```

### Comparing `xeno-6.1.1/LICENSE` & `xeno-6.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xeno-6.1.1/PKG-INFO` & `xeno-6.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: xeno
-Version: 6.1.1
+Version: 6.1.2
 Summary: The Python dependency injector from outer space.
 Home-page: https://github.com/lainproliant/xeno
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: IOC dependency injector
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Xeno: The Python dependency injector from outer space. 
 [![Build Status](https://travis-ci.org/lainproliant/xeno.svg?branch=master)](https://travis-ci.org/lainproliant/xeno)
 
 Xeno is a simple Python dependency injection framework. Use it when you
```

### Comparing `xeno-6.1.1/README.md` & `xeno-6.1.2/README.md`

 * *Files identical despite different names*

### Comparing `xeno-6.1.1/setup.py` & `xeno-6.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,29 +7,28 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="xeno",
-    version="6.1.1",
+    version="6.1.2",
     description="The Python dependency injector from outer space.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lainproliant/xeno",
     author="Lain Musgrove (lainproliant)",
     author_email="lainproliant@gmail.com",
     license="BSD",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
     ],
     keywords="IOC dependency injector",
     packages=find_packages(),
     install_requires=[],
     extras_require={},
     package_data={"xeno": ["LICENSE"]},
     data_files=[],
```

### Comparing `xeno-6.1.1/xeno/__init__.py` & `xeno-6.1.2/xeno/__init__.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.1/xeno/abstract.py` & `xeno-6.1.2/xeno/abstract.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.1/xeno/async_injector.py` & `xeno-6.1.2/xeno/async_injector.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.1/xeno/attributes.py` & `xeno-6.1.2/xeno/attributes.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.1/xeno/build.py` & `xeno-6.1.2/xeno/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,14 +254,17 @@
 
     def provide(self, *args, **kwargs):
         self.injector.provide(*args, **{**kwargs, "is_singleton": True})
 
     def recipe(self, *args, **kwargs):
         return base_recipe(*args, **kwargs)
 
+    def factory(self, *args, **kwargs):
+        return base_recipe(*args, **kwargs, factory=True)
+
     def task(
         self,
         name_or_f: Optional[str | Callable] = None,
         *,
         dep: Optional[str | Iterable[str]] = None,
         default=False,
         factory=True,
@@ -569,13 +572,14 @@
 
 
 # --------------------------------------------------------------------
 engine = Engine()
 engine.add_hook(DefaultEngineHook())
 provide = engine.provide
 recipe = engine.recipe
+factory = engine.factory
 task = engine.task
 
 
 # --------------------------------------------------------------------
 def build():
     return engine.build(*sys.argv[1:], raise_errors=False)
```

### Comparing `xeno-6.1.1/xeno/color.py` & `xeno-6.1.2/xeno/color.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.1/xeno/cookbook.py` & `xeno-6.1.2/xeno/cookbook.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     docs: Optional[str] = None,
     factory=False,
     fmt: Optional[Recipe.Format] = None,
     keep=False,
     memoize=False,
     sigil: Optional[FormatF] = None,
     sync=False,
-    target: Optional[FormatF] = None,
 ):
     """
     Decorator for a function that defines a recipe template.
 
     The function is meant to be a recipe implementation method.  The
     parameters eventually passed to the method depend on whether the
     parameters are recipes or plain values.  Each recipe parameter has its
@@ -107,15 +106,14 @@
                         [*result],
                         docs=docs,
                         fmt=fmt or Recipe.Format(),
                         keep=keep,
                         memoize=memoize,
                         name=truename,
                         sync=sync,
-                        target=target
                     )
                 else:
                     result = cast(Recipe, result)
 
                     result.docs = docs
                     result.fmt = fmt or result.fmt
                     result.keep = keep
```

### Comparing `xeno-6.1.1/xeno/decorators.py` & `xeno-6.1.2/xeno/decorators.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.1/xeno/errors.py` & `xeno-6.1.2/xeno/errors.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.1/xeno/events.py` & `xeno-6.1.2/xeno/events.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.1/xeno/namespaces.py` & `xeno-6.1.2/xeno/namespaces.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.1/xeno/pkg_config.py` & `xeno-6.1.2/xeno/pkg_config.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.1/xeno/recipe.py` & `xeno-6.1.2/xeno/recipe.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.1/xeno/shell.py` & `xeno-6.1.2/xeno/shell.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.1/xeno/spinner.py` & `xeno-6.1.2/xeno/spinner.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.1/xeno/sync_injector.py` & `xeno-6.1.2/xeno/sync_injector.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.1/xeno/testing.py` & `xeno-6.1.2/xeno/testing.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.1/xeno/utils.py` & `xeno-6.1.2/xeno/utils.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.1/xeno.egg-info/PKG-INFO` & `xeno-6.1.2/xeno.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: xeno
-Version: 6.1.1
+Version: 6.1.2
 Summary: The Python dependency injector from outer space.
 Home-page: https://github.com/lainproliant/xeno
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: IOC dependency injector
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Xeno: The Python dependency injector from outer space. 
 [![Build Status](https://travis-ci.org/lainproliant/xeno.svg?branch=master)](https://travis-ci.org/lainproliant/xeno)
 
 Xeno is a simple Python dependency injection framework. Use it when you
```

