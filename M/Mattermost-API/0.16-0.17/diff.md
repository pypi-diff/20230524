# Comparing `tmp/Mattermost-API-0.16.tar.gz` & `tmp/Mattermost-API-0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mattermost-API-0.16.tar", last modified: Wed May 17 17:24:47 2023, max compression
+gzip compressed data, was "Mattermost-API-0.17.tar", last modified: Wed May 24 16:18:24 2023, max compression
```

## Comparing `Mattermost-API-0.16.tar` & `Mattermost-API-0.17.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:24:47.961953 Mattermost-API-0.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-17 17:24:33.000000 Mattermost-API-0.16/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:24:47.961953 Mattermost-API-0.16/Mattermost-API/
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-05-17 17:24:33.000000 Mattermost-API-0.16/Mattermost-API/Mattermost_Base.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-17 17:24:33.000000 Mattermost-API-0.16/Mattermost-API/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-17 17:24:33.000000 Mattermost-API-0.16/Mattermost-API/mattermost.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-17 17:24:33.000000 Mattermost-API-0.16/Mattermost-API/mm_bleve_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-17 17:24:33.000000 Mattermost-API-0.16/Mattermost-API/mm_compliance_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-17 17:24:33.000000 Mattermost-API-0.16/Mattermost-API/mm_elasticsearch_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-17 17:24:33.000000 Mattermost-API-0.16/Mattermost-API/mm_exports_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-17 17:24:33.000000 Mattermost-API-0.16/Mattermost-API/mm_imports_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-17 17:24:33.000000 Mattermost-API-0.16/Mattermost-API/mm_int_actions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-17 17:24:33.000000 Mattermost-API-0.16/Mattermost-API/mm_opengraph_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-17 17:24:33.000000 Mattermost-API-0.16/Mattermost-API/mm_permissions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-17 17:24:33.000000 Mattermost-API-0.16/Mattermost-API/mm_terms_of_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-17 17:24:33.000000 Mattermost-API-0.16/Mattermost-API/mm_uploads_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-17 17:24:33.000000 Mattermost-API-0.16/Mattermost-API/mm_usage_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:24:47.961953 Mattermost-API-0.16/Mattermost_API.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-17 17:24:47.000000 Mattermost-API-0.16/Mattermost_API.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-17 17:24:47.000000 Mattermost-API-0.16/Mattermost_API.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:24:47.000000 Mattermost-API-0.16/Mattermost_API.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 17:24:47.000000 Mattermost-API-0.16/Mattermost_API.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-17 17:24:47.000000 Mattermost-API-0.16/Mattermost_API.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-17 17:24:47.961953 Mattermost-API-0.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 17:24:33.000000 Mattermost-API-0.16/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-17 17:24:33.000000 Mattermost-API-0.16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 17:24:47.961953 Mattermost-API-0.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-17 17:24:33.000000 Mattermost-API-0.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:18:24.325783 Mattermost-API-0.17/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-24 16:18:10.000000 Mattermost-API-0.17/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:18:24.325783 Mattermost-API-0.17/Mattermost-API/
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-24 16:18:10.000000 Mattermost-API-0.17/Mattermost-API/Mattermost_Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-24 16:18:10.000000 Mattermost-API-0.17/Mattermost-API/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-24 16:18:10.000000 Mattermost-API-0.17/Mattermost-API/mattermost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-24 16:18:10.000000 Mattermost-API-0.17/Mattermost-API/mm_bleve_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-24 16:18:10.000000 Mattermost-API-0.17/Mattermost-API/mm_compliance_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-24 16:18:10.000000 Mattermost-API-0.17/Mattermost-API/mm_elasticsearch_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-24 16:18:10.000000 Mattermost-API-0.17/Mattermost-API/mm_exports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-24 16:18:10.000000 Mattermost-API-0.17/Mattermost-API/mm_imports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-24 16:18:10.000000 Mattermost-API-0.17/Mattermost-API/mm_int_actions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-24 16:18:10.000000 Mattermost-API-0.17/Mattermost-API/mm_opengraph_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-24 16:18:10.000000 Mattermost-API-0.17/Mattermost-API/mm_permissions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-24 16:18:10.000000 Mattermost-API-0.17/Mattermost-API/mm_terms_of_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-24 16:18:10.000000 Mattermost-API-0.17/Mattermost-API/mm_uploads_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-24 16:18:10.000000 Mattermost-API-0.17/Mattermost-API/mm_usage_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:18:24.325783 Mattermost-API-0.17/Mattermost_API.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-24 16:18:24.000000 Mattermost-API-0.17/Mattermost_API.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-24 16:18:24.000000 Mattermost-API-0.17/Mattermost_API.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:18:24.000000 Mattermost-API-0.17/Mattermost_API.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 16:18:24.000000 Mattermost-API-0.17/Mattermost_API.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 16:18:24.000000 Mattermost-API-0.17/Mattermost_API.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-24 16:18:24.325783 Mattermost-API-0.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-24 16:18:10.000000 Mattermost-API-0.17/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-24 16:18:10.000000 Mattermost-API-0.17/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:18:24.325783 Mattermost-API-0.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-24 16:18:10.000000 Mattermost-API-0.17/setup.py
```

### Comparing `Mattermost-API-0.16/LICENSE` & `Mattermost-API-0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.16/Mattermost-API/Mattermost_Base.py` & `Mattermost-API-0.17/Mattermost-API/Mattermost_Base.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,20 +52,24 @@
             self.data = {}
         self.data.update({key: value})
 
     def add_application_json_header(self) -> None:
         """
             Добавляет заголовок в запрос для отправки JSON данных.
         """
+        if self.headers is None:
+            self.headers = {}
         self.headers.update({'Content-Type': 'application/json'})
 
     def add_application_www_form_header(self) -> None:
         """
             Добавляет заголовок в запрос для отправки JSON данных.
         """
+        if self.headers is None:
+            self.headers = {}
         self.headers.update({'Content-Type': 'application/x-www-form-urlencoded'})
 
     def add_to_json(self, key: str, value: Union[str, dict, list, tuple, int, bool]) -> None:
         """
           Добавляет запись {key:value} в json Body.
 
           :param key: Ключ для добавления в json Body.
```

### Comparing `Mattermost-API-0.16/Mattermost-API/__init__.py` & `Mattermost-API-0.17/Mattermost-API/__init__.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.16/Mattermost-API/mattermost.py` & `Mattermost-API-0.17/Mattermost-API/mattermost.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.16/Mattermost-API/mm_bleve_api.py` & `Mattermost-API-0.17/Mattermost-API/mm_bleve_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.16/Mattermost-API/mm_compliance_api.py` & `Mattermost-API-0.17/Mattermost-API/mm_compliance_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.16/Mattermost-API/mm_elasticsearch_api.py` & `Mattermost-API-0.17/Mattermost-API/mm_elasticsearch_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.16/Mattermost-API/mm_exports_api.py` & `Mattermost-API-0.17/Mattermost-API/mm_exports_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.16/Mattermost-API/mm_imports_api.py` & `Mattermost-API-0.17/Mattermost-API/mm_imports_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.16/Mattermost-API/mm_int_actions_api.py` & `Mattermost-API-0.17/Mattermost-API/mm_int_actions_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.16/Mattermost-API/mm_opengraph_api.py` & `Mattermost-API-0.17/Mattermost-API/mm_opengraph_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.16/Mattermost-API/mm_permissions_api.py` & `Mattermost-API-0.17/Mattermost-API/mm_permissions_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.16/Mattermost-API/mm_terms_of_service_api.py` & `Mattermost-API-0.17/Mattermost-API/mm_terms_of_service_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.16/Mattermost-API/mm_uploads_api.py` & `Mattermost-API-0.17/Mattermost-API/mm_uploads_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.16/Mattermost-API/mm_usage_api.py` & `Mattermost-API-0.17/Mattermost-API/mm_usage_api.py`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.16/Mattermost_API.egg-info/PKG-INFO` & `Mattermost-API-0.17/Mattermost_API.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mattermost-API
-Version: 0.16
+Version: 0.17
 Summary: Simple Mattermost API library
 Home-page: https://github.com/izhatomic/mattermost-api
 Download-URL: https://pypi.org/project/mattermost-api/
 Author: Aleksandr Kuznetsov, Aleksandr Zarin
 Author-email: Aleksandr Kuznetsov <izhatomic@yandex.ru>, Aleksandr Zarin <vector-777@yandex.ru>
 License: MIT
 Project-URL: Homepage, https://github.com/izhatomic/mattermost-api
```

### Comparing `Mattermost-API-0.16/Mattermost_API.egg-info/SOURCES.txt` & `Mattermost-API-0.17/Mattermost_API.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Mattermost-API-0.16/PKG-INFO` & `Mattermost-API-0.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mattermost-API
-Version: 0.16
+Version: 0.17
 Summary: Simple Mattermost API library
 Home-page: https://github.com/izhatomic/mattermost-api
 Download-URL: https://pypi.org/project/mattermost-api/
 Author: Aleksandr Kuznetsov, Aleksandr Zarin
 Author-email: Aleksandr Kuznetsov <izhatomic@yandex.ru>, Aleksandr Zarin <vector-777@yandex.ru>
 License: MIT
 Project-URL: Homepage, https://github.com/izhatomic/mattermost-api
```

### Comparing `Mattermost-API-0.16/pyproject.toml` & `Mattermost-API-0.17/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Mattermost-API"
-version = "0.16"
+version = "0.17"
 authors = [
     { name="Aleksandr Kuznetsov", email="izhatomic@yandex.ru" },
     { name="Aleksandr Zarin", email="vector-777@yandex.ru" },
 ]
 description = "Simple Mattermost API library"
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `Mattermost-API-0.16/setup.py` & `Mattermost-API-0.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='Mattermost-API',
-    version='0.16',
+    version='0.17',
     description='Simple Mattermost API library',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='Aleksandr Kuznetsov, Aleksandr Zarin',
     author_email='izhatomic@yandex.ru, vector-777@yandex.ru',
```

