# Comparing `tmp/cd_dynamic_versioning-0.0.2.tar.gz` & `tmp/cd_dynamic_versioning-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cd_dynamic_versioning-0.0.2.tar", max compression
+gzip compressed data, was "cd_dynamic_versioning-0.0.3.tar", max compression
```

## Comparing `cd_dynamic_versioning-0.0.2.tar` & `cd_dynamic_versioning-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0      153 2023-01-03 09:28:00.042181 cd_dynamic_versioning-0.0.2/README.md
--rw-r--r--   0        0        0       56 2023-01-03 09:28:45.277877 cd_dynamic_versioning-0.0.2/cd_dynamic_versioning/__init__.py
--rw-r--r--   0        0        0     1030 2023-01-03 09:28:45.277877 cd_dynamic_versioning-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 cd_dynamic_versioning-0.0.2/setup.py
--rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 cd_dynamic_versioning-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      554 2023-05-24 07:34:21.666597 cd_dynamic_versioning-0.0.3/README.md
+-rw-r--r--   0        0        0       56 2023-05-24 07:34:57.615394 cd_dynamic_versioning-0.0.3/cd_dynamic_versioning/__init__.py
+-rw-r--r--   0        0        0     1129 2023-05-24 07:34:57.615394 cd_dynamic_versioning-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1053 1970-01-01 00:00:00.000000 cd_dynamic_versioning-0.0.3/PKG-INFO
```

### Comparing `cd_dynamic_versioning-0.0.2/pyproject.toml` & `cd_dynamic_versioning-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 [tool.poetry]
 name = "cd-dynamic-versioning"
-version = "0.0.2"
+version = "0.0.3"
 description = "Testpackage for dynamic versioning"
 authors = ["Yngve Moe <yngve.m.moe@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "cd_dynamic_versioning"}]
 
 [tool.poetry.dependencies]
 python = ">= 3.8.1,<4.0"
 
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+sphinx = "^5.2.3"
+
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 black = "^22.12.0"
 isort = "^5.11.4"
 flake8 = "^6.0.0"
 flake8-bugbear = "^22.12.6"
 flake8-mutable = "^1.2.0"
```

