# Comparing `tmp/jschemator-0.0.7.tar.gz` & `tmp/jschemator-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jschemator-0.0.7.tar", last modified: Tue May 16 14:44:54 2023, max compression
+gzip compressed data, was "jschemator-0.0.8.tar", last modified: Wed May 17 05:12:27 2023, max compression
```

## Comparing `jschemator-0.0.7.tar` & `jschemator-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:44:54.959568 jschemator-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 14:44:44.000000 jschemator-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-16 14:44:54.959568 jschemator-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 14:44:44.000000 jschemator-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:44:54.955567 jschemator-0.0.7/jschemator/
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-16 14:44:44.000000 jschemator-0.0.7/jschemator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-16 14:44:44.000000 jschemator-0.0.7/jschemator/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:44:54.959568 jschemator-0.0.7/jschemator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-16 14:44:54.000000 jschemator-0.0.7/jschemator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 14:44:54.000000 jschemator-0.0.7/jschemator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 14:44:54.000000 jschemator-0.0.7/jschemator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 14:44:54.000000 jschemator-0.0.7/jschemator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-16 14:44:54.000000 jschemator-0.0.7/jschemator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 14:44:54.959568 jschemator-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-16 14:44:44.000000 jschemator-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:44:54.959568 jschemator-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-16 14:44:44.000000 jschemator-0.0.7/tests/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-16 14:44:44.000000 jschemator-0.0.7/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-16 14:44:44.000000 jschemator-0.0.7/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:12:27.675193 jschemator-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-17 05:12:16.000000 jschemator-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-17 05:12:27.675193 jschemator-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-17 05:12:16.000000 jschemator-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:12:27.675193 jschemator-0.0.8/jschemator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-17 05:12:16.000000 jschemator-0.0.8/jschemator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-17 05:12:16.000000 jschemator-0.0.8/jschemator/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:12:27.675193 jschemator-0.0.8/jschemator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-17 05:12:27.000000 jschemator-0.0.8/jschemator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-17 05:12:27.000000 jschemator-0.0.8/jschemator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 05:12:27.000000 jschemator-0.0.8/jschemator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-17 05:12:27.000000 jschemator-0.0.8/jschemator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 05:12:27.000000 jschemator-0.0.8/jschemator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 05:12:27.675193 jschemator-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-17 05:12:16.000000 jschemator-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:12:27.675193 jschemator-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-17 05:12:16.000000 jschemator-0.0.8/tests/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-17 05:12:16.000000 jschemator-0.0.8/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-17 05:12:16.000000 jschemator-0.0.8/tests/test_schema.py
```

### Comparing `jschemator-0.0.7/LICENSE` & `jschemator-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jschemator-0.0.7/jschemator/__init__.py` & `jschemator-0.0.8/jschemator/__init__.py`

 * *Files identical despite different names*

### Comparing `jschemator-0.0.7/jschemator/fields.py` & `jschemator-0.0.8/jschemator/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,8 +113,10 @@
 
 class ObjectField(BaseField):
     def __init__(self, sub_schema, **kwargs):
         self.sub_schema = sub_schema
         super(ObjectField, self).__init__(**kwargs)
 
     def json_schema_render(self):
-        return self.sub_schema.json_schema()
+        schema = super(ObjectField, self).json_schema_render()
+        schema.update(self.sub_schema.json_schema())
+        return schema
```

### Comparing `jschemator-0.0.7/tests/test_schema.py` & `jschemator-0.0.8/tests/test_schema.py`

 * *Files identical despite different names*

