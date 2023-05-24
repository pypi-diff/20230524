# Comparing `tmp/envoy.code.check-0.5.1.tar.gz` & `tmp/envoy.code.check-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envoy.code.check-0.5.1.tar", last modified: Wed May 24 11:58:22 2023, max compression
+gzip compressed data, was "envoy.code.check-0.5.3.tar", last modified: Wed May 24 17:33:35 2023, max compression
```

## Comparing `envoy.code.check-0.5.1.tar` & `envoy.code.check-0.5.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:58:22.449051 envoy.code.check-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-24 11:58:22.449051 envoy.code.check-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:58:22.445051 envoy.code.check-0.5.1/envoy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:58:22.445051 envoy.code.check-0.5.1/envoy/code/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:58:22.445051 envoy.code.check-0.5.1/envoy/code/check/
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:58:22.449051 envoy.code.check-0.5.1/envoy/code/check/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/flake8.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/glint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/gofmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/runtime_guards.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/shellcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/yamllint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/abstract/yapf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy/code/check/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:58:22.445051 envoy.code.check-0.5.1/envoy.code.check.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy.code.check.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy.code.check.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy.code.check.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy.code.check.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy.code.check.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy.code.check.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/envoy.code.check.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 11:58:22.449051 envoy.code.check-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-24 11:58:22.000000 envoy.code.check-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:33:35.604314 envoy.code.check-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-24 17:33:35.604314 envoy.code.check-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:33:35.600314 envoy.code.check-0.5.3/envoy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:33:35.600314 envoy.code.check-0.5.3/envoy/code/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:33:35.604314 envoy.code.check-0.5.3/envoy/code/check/
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy/code/check/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:33:35.604314 envoy.code.check-0.5.3/envoy/code/check/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy/code/check/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy/code/check/abstract/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy/code/check/abstract/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy/code/check/abstract/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy/code/check/abstract/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy/code/check/abstract/flake8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy/code/check/abstract/glint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy/code/check/abstract/gofmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy/code/check/abstract/rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy/code/check/abstract/runtime_guards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy/code/check/abstract/shellcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy/code/check/abstract/yamllint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy/code/check/abstract/yapf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy/code/check/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy/code/check/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy/code/check/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy/code/check/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy/code/check/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy/code/check/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:33:35.600314 envoy.code.check-0.5.3/envoy.code.check.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy.code.check.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy.code.check.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy.code.check.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy.code.check.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy.code.check.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy.code.check.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/envoy.code.check.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 17:33:35.604314 envoy.code.check-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-24 17:33:35.000000 envoy.code.check-0.5.3/setup.py
```

### Comparing `envoy.code.check-0.5.1/backend_shim.py` & `envoy.code.check-0.5.3/backend_shim.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.1/envoy/code/check/__init__.py` & `envoy.code.check-0.5.3/envoy/code/check/__init__.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.1/envoy/code/check/abstract/__init__.py` & `envoy.code.check-0.5.3/envoy/code/check/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.1/envoy/code/check/abstract/base.py` & `envoy.code.check-0.5.3/envoy/code/check/abstract/base.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.1/envoy/code/check/abstract/changelog.py` & `envoy.code.check-0.5.3/envoy/code/check/abstract/changelog.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.1/envoy/code/check/abstract/checker.py` & `envoy.code.check-0.5.3/envoy/code/check/abstract/checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,15 @@
 
     @cached_property
     def extensions(self) -> "interface.IExtensionsCheck":
         """Extensions checker."""
         return self.extensions_class(
             self.directory,
             extensions_build_config=self.args.extensions_build_config,
+            extensions_fuzzed_count=self.args.extensions_fuzzed_count,
             **self.check_kwargs)
 
     @property  # type:ignore
     @abstracts.interfacemethod
     def extensions_class(self) -> Type["interface.IExtensionsCheck"]:
         raise NotImplementedError
```

### Comparing `envoy.code.check-0.5.1/envoy/code/check/abstract/extensions.py` & `envoy.code.check-0.5.3/envoy/code/check/abstract/extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from envoy.code.check import abstract, exceptions, interface, typing
 
 
 logger = logging.getLogger(__name__)
 
 FUZZ_TEST_PATH = (
-    "test/extensions/filters/network/common/fuzz/BUILD")
+    "test/extensions/filters/network/common/fuzz/config.bzl")
 METADATA_PATH = "source/extensions/extensions_metadata.yaml"
 METADATA_ONLY_EXTENSIONS = (
     "envoy.filters.network.envoy_mobile_http_connection_manager", )
 CONTRIB_METADATA_PATH = "contrib/extensions_metadata.yaml"
 EXTENSIONS_SCHEMA = "tools/extensions/extensions_schema.yaml"
```

### Comparing `envoy.code.check-0.5.1/envoy/code/check/abstract/flake8.py` & `envoy.code.check-0.5.3/envoy/code/check/abstract/flake8.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.1/envoy/code/check/abstract/glint.py` & `envoy.code.check-0.5.3/envoy/code/check/abstract/glint.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.1/envoy/code/check/abstract/gofmt.py` & `envoy.code.check-0.5.3/envoy/code/check/abstract/gofmt.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.1/envoy/code/check/abstract/rst.py` & `envoy.code.check-0.5.3/envoy/code/check/abstract/rst.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.1/envoy/code/check/abstract/runtime_guards.py` & `envoy.code.check-0.5.3/envoy/code/check/abstract/runtime_guards.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.1/envoy/code/check/abstract/shellcheck.py` & `envoy.code.check-0.5.3/envoy/code/check/abstract/shellcheck.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.1/envoy/code/check/abstract/yamllint.py` & `envoy.code.check-0.5.3/envoy/code/check/abstract/yamllint.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.1/envoy/code/check/abstract/yapf.py` & `envoy.code.check-0.5.3/envoy/code/check/abstract/yapf.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.1/envoy/code/check/checker.py` & `envoy.code.check-0.5.3/envoy/code/check/checker.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.1/envoy/code/check/interface.py` & `envoy.code.check-0.5.3/envoy/code/check/interface.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.1/envoy/code/check/typing.py` & `envoy.code.check-0.5.3/envoy/code/check/typing.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.1/envoy.code.check.egg-info/SOURCES.txt` & `envoy.code.check-0.5.3/envoy.code.check.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.5.1/setup.py` & `envoy.code.check-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,9 +42,9 @@
     },
     'packages': (
         'envoy.code.check',
         'envoy.code.check.abstract',
     ),
     'python_requires': '>=3.10.0',
     'url': 'https://github.com/envoyproxy/toolshed/tree/main/envoy.code.check',
-    'version': '0.5.1',
+    'version': '0.5.3',
 })
```

