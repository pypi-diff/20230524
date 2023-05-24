# Comparing `tmp/prefeitura_rio-0.1.1.tar.gz` & `tmp/prefeitura-rio-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefeitura_rio-0.1.1.tar", max compression
+gzip compressed data, was "prefeitura-rio-0.1.1a1.tar", max compression
```

## Comparing `prefeitura_rio-0.1.1.tar` & `prefeitura-rio-0.1.1a1.tar`

### file list

```diff
@@ -1,13 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-05-24 19:33:22.496688 prefeitura_rio-0.1.1/LICENSE
--rw-r--r--   0        0        0       83 2023-05-24 19:33:22.496688 prefeitura_rio-0.1.1/README.md
--rw-r--r--   0        0        0      124 2023-05-24 19:33:22.496688 prefeitura_rio-0.1.1/prefeitura_rio/__init__.py
--rw-r--r--   0        0        0     2397 2023-05-24 19:33:22.496688 prefeitura_rio-0.1.1/prefeitura_rio/core.py
--rw-r--r--   0        0        0        0 2023-05-24 19:33:22.500688 prefeitura_rio-0.1.1/prefeitura_rio/integrations/__init__.py
--rw-r--r--   0        0        0    18392 2023-05-24 19:33:22.500688 prefeitura_rio-0.1.1/prefeitura_rio/integrations/sgrc/__init__.py
--rw-r--r--   0        0        0      455 2023-05-24 19:33:22.500688 prefeitura_rio-0.1.1/prefeitura_rio/integrations/sgrc/exceptions.py
--rw-r--r--   0        0        0    11646 2023-05-24 19:33:22.500688 prefeitura_rio-0.1.1/prefeitura_rio/integrations/sgrc/models.py
--rw-r--r--   0        0        0     2082 2023-05-24 19:33:22.500688 prefeitura_rio-0.1.1/prefeitura_rio/integrations/sgrc/utils.py
--rw-r--r--   0        0        0     1749 2023-05-24 19:33:22.500688 prefeitura_rio-0.1.1/prefeitura_rio/metrics/__init__.py
--rw-r--r--   0        0        0     7642 2023-05-24 19:33:22.500688 prefeitura_rio-0.1.1/prefeitura_rio/metrics/agnostic.py
--rw-r--r--   0        0        0      922 2023-05-24 19:33:22.500688 prefeitura_rio-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 prefeitura_rio-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-20 16:06:36.123727 prefeitura-rio-0.1.1a1/LICENSE
+-rw-r--r--   0        0        0       83 2022-09-20 16:06:36.123727 prefeitura-rio-0.1.1a1/README.md
+-rw-r--r--   0        0        0        0 2022-09-20 16:06:36.123727 prefeitura-rio-0.1.1a1/prefeitura_rio/__init__.py
+-rw-r--r--   0        0        0     1749 2022-09-20 16:06:36.123727 prefeitura-rio-0.1.1a1/prefeitura_rio/metrics/__init__.py
+-rw-r--r--   0        0        0     7642 2022-09-20 16:06:36.123727 prefeitura-rio-0.1.1a1/prefeitura_rio/metrics/agnostic.py
+-rw-r--r--   0        0        0      848 2022-09-20 16:06:36.123727 prefeitura-rio-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 prefeitura-rio-0.1.1a1/setup.py
+-rw-r--r--   0        0        0      860 1970-01-01 00:00:00.000000 prefeitura-rio-0.1.1a1/PKG-INFO
```

### Comparing `prefeitura_rio-0.1.1/LICENSE` & `prefeitura-rio-0.1.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `prefeitura_rio-0.1.1/prefeitura_rio/metrics/__init__.py` & `prefeitura-rio-0.1.1a1/prefeitura_rio/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `prefeitura_rio-0.1.1/prefeitura_rio/metrics/agnostic.py` & `prefeitura-rio-0.1.1a1/prefeitura_rio/metrics/agnostic.py`

 * *Files identical despite different names*

### Comparing `prefeitura_rio-0.1.1/pyproject.toml` & `prefeitura-rio-0.1.1a1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 [tool.poetry]
 name = "prefeitura-rio"
-version = "0.1.1"
+version = "0.1.1a1"
 description = "Pacote Python que implementa utilidades para nossos projetos!"
 authors = ["Gabriel Gazola Milan <gabriel.gazola@poli.ufrj.br>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/prefeitura-rio/prefeitura-rio"
 repository = "https://github.com/prefeitura-rio/prefeitura-rio"
 keywords = ["python", "utilities", "government"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 numpy = "^1.23.3"
 scikit-learn = "^1.1.2"
-loguru = "^0.7.0"
-requests = "^2.31.0"
-pendulum = "^2.1.2"
-pytz = "^2023.3"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.3.0"
 pre-commit = "^2.18.1"
 pytest-cov = "^3.0.0"
 flake8 = "^4.0.1"
 pdoc3 = "^0.10.0"
```

### Comparing `prefeitura_rio-0.1.1/PKG-INFO` & `prefeitura-rio-0.1.1a1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 Metadata-Version: 2.1
 Name: prefeitura-rio
-Version: 0.1.1
+Version: 0.1.1a1
 Summary: Pacote Python que implementa utilidades para nossos projetos!
 Home-page: https://github.com/prefeitura-rio/prefeitura-rio
 License: GPL-3.0-only
 Keywords: python,utilities,government
 Author: Gabriel Gazola Milan
 Author-email: gabriel.gazola@poli.ufrj.br
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: numpy (>=1.23.3,<2.0.0)
-Requires-Dist: pendulum (>=2.1.2,<3.0.0)
-Requires-Dist: pytz (>=2023.3,<2024.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: scikit-learn (>=1.1.2,<2.0.0)
 Project-URL: Repository, https://github.com/prefeitura-rio/prefeitura-rio
 Description-Content-Type: text/markdown
 
 # prefeitura-rio
 
 Um pacote Python que implementa utilidades para nossos projetos!
```

