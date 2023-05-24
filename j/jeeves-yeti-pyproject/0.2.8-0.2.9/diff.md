# Comparing `tmp/jeeves_yeti_pyproject-0.2.8.tar.gz` & `tmp/jeeves_yeti_pyproject-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeeves_yeti_pyproject-0.2.8.tar", max compression
+gzip compressed data, was "jeeves_yeti_pyproject-0.2.9.tar", max compression
```

## Comparing `jeeves_yeti_pyproject-0.2.8.tar` & `jeeves_yeti_pyproject-0.2.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       25 2022-12-23 16:15:52.145747 jeeves_yeti_pyproject-0.2.8/README.md
--rw-r--r--   0        0        0       48 2022-12-12 14:46:21.687115 jeeves_yeti_pyproject-0.2.8/jeeves_yeti_pyproject/__init__.py
--rw-r--r--   0        0        0      569 2022-12-27 18:46:32.164561 jeeves_yeti_pyproject-0.2.8/jeeves_yeti_pyproject/diff.py
--rw-r--r--   0        0        0      674 2022-12-23 19:52:31.790186 jeeves_yeti_pyproject-0.2.8/jeeves_yeti_pyproject/files_and_directories.py
--rw-r--r--   0        0        0     1422 2022-12-26 10:34:23.725701 jeeves_yeti_pyproject-0.2.8/jeeves_yeti_pyproject/flags.py
--rw-r--r--   0        0        0       95 2022-12-23 19:37:33.989939 jeeves_yeti_pyproject-0.2.8/jeeves_yeti_pyproject/flakeheaven/__init__.py
--rw-r--r--   0        0        0     2941 2023-01-03 16:58:25.009707 jeeves_yeti_pyproject-0.2.8/jeeves_yeti_pyproject/flakeheaven/flakeheaven.toml
--rw-r--r--   0        0        0     1392 2022-12-27 18:46:32.168561 jeeves_yeti_pyproject-0.2.8/jeeves_yeti_pyproject/flakeheaven/integration.py
--rw-r--r--   0        0        0     1746 2023-01-02 10:03:22.786527 jeeves_yeti_pyproject-0.2.8/jeeves_yeti_pyproject/jeeves.py
--rw-r--r--   0        0        0     1541 2022-12-27 18:46:32.164561 jeeves_yeti_pyproject-0.2.8/jeeves_yeti_pyproject/mypy.py
--rw-r--r--   0        0        0      873 2023-01-03 17:04:32.603391 jeeves_yeti_pyproject-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 jeeves_yeti_pyproject-0.2.8/setup.py
--rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 jeeves_yeti_pyproject-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       25 2022-12-23 16:15:52.145747 jeeves_yeti_pyproject-0.2.9/README.md
+-rw-r--r--   0        0        0       48 2022-12-12 14:46:21.687115 jeeves_yeti_pyproject-0.2.9/jeeves_yeti_pyproject/__init__.py
+-rw-r--r--   0        0        0      569 2022-12-27 18:46:32.164561 jeeves_yeti_pyproject-0.2.9/jeeves_yeti_pyproject/diff.py
+-rw-r--r--   0        0        0      674 2022-12-23 19:52:31.790186 jeeves_yeti_pyproject-0.2.9/jeeves_yeti_pyproject/files_and_directories.py
+-rw-r--r--   0        0        0     1422 2022-12-26 10:34:23.725701 jeeves_yeti_pyproject-0.2.9/jeeves_yeti_pyproject/flags.py
+-rw-r--r--   0        0        0       95 2022-12-23 19:37:33.989939 jeeves_yeti_pyproject-0.2.9/jeeves_yeti_pyproject/flakeheaven/__init__.py
+-rw-r--r--   0        0        0     2941 2023-01-03 16:58:25.009707 jeeves_yeti_pyproject-0.2.9/jeeves_yeti_pyproject/flakeheaven/flakeheaven.toml
+-rw-r--r--   0        0        0     1392 2022-12-27 18:46:32.168561 jeeves_yeti_pyproject-0.2.9/jeeves_yeti_pyproject/flakeheaven/integration.py
+-rw-r--r--   0        0        0     1746 2023-01-02 10:03:22.786527 jeeves_yeti_pyproject-0.2.9/jeeves_yeti_pyproject/jeeves.py
+-rw-r--r--   0        0        0     1541 2022-12-27 18:46:32.164561 jeeves_yeti_pyproject-0.2.9/jeeves_yeti_pyproject/mypy.py
+-rw-r--r--   0        0        0     1022 2023-01-10 16:29:49.163697 jeeves_yeti_pyproject-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 jeeves_yeti_pyproject-0.2.9/setup.py
+-rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 jeeves_yeti_pyproject-0.2.9/PKG-INFO
```

### Comparing `jeeves_yeti_pyproject-0.2.8/jeeves_yeti_pyproject/diff.py` & `jeeves_yeti_pyproject-0.2.9/jeeves_yeti_pyproject/diff.py`

 * *Files identical despite different names*

### Comparing `jeeves_yeti_pyproject-0.2.8/jeeves_yeti_pyproject/files_and_directories.py` & `jeeves_yeti_pyproject-0.2.9/jeeves_yeti_pyproject/files_and_directories.py`

 * *Files identical despite different names*

### Comparing `jeeves_yeti_pyproject-0.2.8/jeeves_yeti_pyproject/flags.py` & `jeeves_yeti_pyproject-0.2.9/jeeves_yeti_pyproject/flags.py`

 * *Files identical despite different names*

### Comparing `jeeves_yeti_pyproject-0.2.8/jeeves_yeti_pyproject/flakeheaven/flakeheaven.toml` & `jeeves_yeti_pyproject-0.2.9/jeeves_yeti_pyproject/flakeheaven/flakeheaven.toml`

 * *Files identical despite different names*

### Comparing `jeeves_yeti_pyproject-0.2.8/jeeves_yeti_pyproject/flakeheaven/integration.py` & `jeeves_yeti_pyproject-0.2.9/jeeves_yeti_pyproject/flakeheaven/integration.py`

 * *Files identical despite different names*

### Comparing `jeeves_yeti_pyproject-0.2.8/jeeves_yeti_pyproject/jeeves.py` & `jeeves_yeti_pyproject-0.2.9/jeeves_yeti_pyproject/jeeves.py`

 * *Files identical despite different names*

### Comparing `jeeves_yeti_pyproject-0.2.8/jeeves_yeti_pyproject/mypy.py` & `jeeves_yeti_pyproject-0.2.9/jeeves_yeti_pyproject/mypy.py`

 * *Files identical despite different names*

### Comparing `jeeves_yeti_pyproject-0.2.8/pyproject.toml` & `jeeves_yeti_pyproject-0.2.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "jeeves-yeti-pyproject"
-version = "0.2.8"
+version = "0.2.9"
 description = "Opinionated Jeeves plugin for Python projects."
 authors = ["Anatoly Scherbakov <altaisoft@gmail.com>"]
 readme = "README.md"
 packages = [{include = "jeeves_yeti_pyproject"}]
 
 [tool.poetry.plugins.jeeves]
 pyproject = "jeeves_yeti_pyproject:jeeves"
 
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.9,<4.0"
 jeeves-shell = "^2.1.0"
 
 mypy = "^0.910"
 
 safety = "^1.10"
 
 pytest = "^6.2"
@@ -24,14 +24,20 @@
 wemake-python-styleguide = "^0.17.0"
 flakeheaven = "^3.2.1"
 rich = "^12.6.0"
 tomlkit = "^0.11.6"
 sh = "^1.14.3"
 add-trailing-comma = "^2.4.0"
 
+[tool.poetry.group.dev.dependencies]
+mkdocs = "^1.4.2"
+mkdocs-material = "^9.0.3"
+mkdocs-macros-plugin = "^0.7.0"
+mkdocs-iolanta-tables = "^1.1.13"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.flakehell.exceptions."**/flags.py"]
 wemake-python-styleguide = [
```

### Comparing `jeeves_yeti_pyproject-0.2.8/setup.py` & `jeeves_yeti_pyproject-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,24 +22,24 @@
  'wemake-python-styleguide>=0.17.0,<0.18.0']
 
 entry_points = \
 {'jeeves': ['pyproject = jeeves_yeti_pyproject:jeeves']}
 
 setup_kwargs = {
     'name': 'jeeves-yeti-pyproject',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'Opinionated Jeeves plugin for Python projects.',
     'long_description': '# jeeves-yeti-pyproject\n\n',
     'author': 'Anatoly Scherbakov',
     'author_email': 'altaisoft@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `jeeves_yeti_pyproject-0.2.8/PKG-INFO` & `jeeves_yeti_pyproject-0.2.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: jeeves-yeti-pyproject
-Version: 0.2.8
+Version: 0.2.9
 Summary: Opinionated Jeeves plugin for Python projects.
 Author: Anatoly Scherbakov
 Author-email: altaisoft@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: add-trailing-comma (>=2.4.0,<3.0.0)
 Requires-Dist: flakeheaven (>=3.2.1,<4.0.0)
 Requires-Dist: jeeves-shell (>=2.1.0,<3.0.0)
 Requires-Dist: mypy (>=0.910,<0.911)
```

