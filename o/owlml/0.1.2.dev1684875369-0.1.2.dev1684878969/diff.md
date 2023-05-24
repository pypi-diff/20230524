# Comparing `tmp/owlml-0.1.2.dev1684875369.tar.gz` & `tmp/owlml-0.1.2.dev1684878969.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owlml-0.1.2.dev1684875369.tar", last modified: Tue May 23 20:56:21 2023, max compression
+gzip compressed data, was "owlml-0.1.2.dev1684878969.tar", last modified: Tue May 23 21:56:20 2023, max compression
```

## Comparing `owlml-0.1.2.dev1684875369.tar` & `owlml-0.1.2.dev1684878969.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:56:21.625930 owlml-0.1.2.dev1684875369/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-23 20:55:38.000000 owlml-0.1.2.dev1684875369/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-23 20:56:21.625930 owlml-0.1.2.dev1684875369/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-23 20:55:38.000000 owlml-0.1.2.dev1684875369/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:56:21.625930 owlml-0.1.2.dev1684875369/owlml/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-23 20:55:38.000000 owlml-0.1.2.dev1684875369/owlml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 20:55:38.000000 owlml-0.1.2.dev1684875369/owlml/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-23 20:55:38.000000 owlml-0.1.2.dev1684875369/owlml/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 20:55:38.000000 owlml-0.1.2.dev1684875369/owlml/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-23 20:55:38.000000 owlml-0.1.2.dev1684875369/owlml/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-23 20:55:38.000000 owlml-0.1.2.dev1684875369/owlml/images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:56:21.625930 owlml-0.1.2.dev1684875369/owlml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-23 20:56:21.000000 owlml-0.1.2.dev1684875369/owlml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-23 20:56:21.000000 owlml-0.1.2.dev1684875369/owlml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:56:21.000000 owlml-0.1.2.dev1684875369/owlml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 20:56:21.000000 owlml-0.1.2.dev1684875369/owlml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 20:56:21.000000 owlml-0.1.2.dev1684875369/owlml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 20:56:21.000000 owlml-0.1.2.dev1684875369/owlml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-23 20:56:21.625930 owlml-0.1.2.dev1684875369/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:55:38.000000 owlml-0.1.2.dev1684875369/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:56:20.608841 owlml-0.1.2.dev1684878969/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-23 21:55:39.000000 owlml-0.1.2.dev1684878969/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-23 21:56:20.608841 owlml-0.1.2.dev1684878969/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-23 21:55:39.000000 owlml-0.1.2.dev1684878969/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:56:20.608841 owlml-0.1.2.dev1684878969/owlml/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-23 21:55:39.000000 owlml-0.1.2.dev1684878969/owlml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 21:55:39.000000 owlml-0.1.2.dev1684878969/owlml/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-23 21:55:39.000000 owlml-0.1.2.dev1684878969/owlml/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 21:55:39.000000 owlml-0.1.2.dev1684878969/owlml/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-23 21:55:39.000000 owlml-0.1.2.dev1684878969/owlml/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-23 21:55:39.000000 owlml-0.1.2.dev1684878969/owlml/images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:56:20.608841 owlml-0.1.2.dev1684878969/owlml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-23 21:56:20.000000 owlml-0.1.2.dev1684878969/owlml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-23 21:56:20.000000 owlml-0.1.2.dev1684878969/owlml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:56:20.000000 owlml-0.1.2.dev1684878969/owlml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 21:56:20.000000 owlml-0.1.2.dev1684878969/owlml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 21:56:20.000000 owlml-0.1.2.dev1684878969/owlml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 21:56:20.000000 owlml-0.1.2.dev1684878969/owlml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-23 21:56:20.608841 owlml-0.1.2.dev1684878969/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:55:39.000000 owlml-0.1.2.dev1684878969/setup.py
```

### Comparing `owlml-0.1.2.dev1684875369/LICENSE` & `owlml-0.1.2.dev1684878969/LICENSE`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684875369/README.md` & `owlml-0.1.2.dev1684878969/README.md`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684875369/owlml/__main__.py` & `owlml-0.1.2.dev1684878969/owlml/__main__.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684875369/owlml/api.py` & `owlml-0.1.2.dev1684878969/owlml/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             f"{error}\nResponse body: {response.text}"
         ) from error
 
 
 class OwlMLAPI:
     """API class for OwlML."""
 
-    base_url: str = _get_required_env_var("OWLML_API")
+    base_url: str = os.path.join(_get_required_env_var("OWLML_URL"), "api")
 
     @classmethod
     def get(cls, route: str) -> dict[str, Any]:
         """Make a GET request to the OwlML API."""
         response = requests.get(os.path.join(cls.base_url, route))
         raise_for_status(response)
         if response.status_code == 204:
```

### Comparing `owlml-0.1.2.dev1684875369/owlml/auth.py` & `owlml-0.1.2.dev1684878969/owlml/auth.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684875369/owlml/datasets.py` & `owlml-0.1.2.dev1684878969/owlml/datasets.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684875369/owlml/images.py` & `owlml-0.1.2.dev1684878969/owlml/images.py`

 * *Files identical despite different names*

