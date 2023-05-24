# Comparing `tmp/django_encryption-0.3.3.tar.gz` & `tmp/django_encryption-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_encryption-0.3.3.tar", max compression
+gzip compressed data, was "django_encryption-0.3.4.tar", max compression
```

## Comparing `django_encryption-0.3.3.tar` & `django_encryption-0.3.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6293 2023-04-30 10:22:53.745396 django_encryption-0.3.3/README.md
--rw-r--r--   0        0        0       22 2023-04-30 10:22:53.745396 django_encryption-0.3.3/django_encryption/__init__.py
--rw-r--r--   0        0        0    15879 2023-04-30 10:22:53.745396 django_encryption-0.3.3/django_encryption/fields.py
--rw-r--r--   0        0        0        0 2023-04-30 10:22:53.745396 django_encryption-0.3.3/django_encryption/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 10:22:53.745396 django_encryption-0.3.3/django_encryption/management/commands/__init__.py
--rw-r--r--   0        0        0     3278 2023-04-30 10:22:53.745396 django_encryption-0.3.3/django_encryption/management/commands/generate_vault_migration.py
--rw-r--r--   0        0        0        0 2023-04-30 10:22:53.745396 django_encryption-0.3.3/django_encryption/py.typed
--rw-r--r--   0        0        0    11063 2023-04-30 10:22:53.745396 django_encryption-0.3.3/django_encryption/vault_wrapper.py
--rw-r--r--   0        0        0     2160 2023-04-30 10:23:25.470050 django_encryption-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     8085 1970-01-01 00:00:00.000000 django_encryption-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     6293 2023-05-22 13:08:52.313357 django_encryption-0.3.4/README.md
+-rw-r--r--   0        0        0       22 2023-05-22 13:08:52.313357 django_encryption-0.3.4/django_encryption/__init__.py
+-rw-r--r--   0        0        0    15879 2023-05-22 13:08:52.313357 django_encryption-0.3.4/django_encryption/fields.py
+-rw-r--r--   0        0        0        0 2023-05-22 13:08:52.313357 django_encryption-0.3.4/django_encryption/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 13:08:52.313357 django_encryption-0.3.4/django_encryption/management/commands/__init__.py
+-rw-r--r--   0        0        0     3278 2023-05-22 13:08:52.313357 django_encryption-0.3.4/django_encryption/management/commands/generate_vault_migration.py
+-rw-r--r--   0        0        0        0 2023-05-22 13:08:52.313357 django_encryption-0.3.4/django_encryption/py.typed
+-rw-r--r--   0        0        0    11063 2023-05-22 13:08:52.313357 django_encryption-0.3.4/django_encryption/vault_wrapper.py
+-rw-r--r--   0        0        0     2160 2023-05-22 13:09:23.529690 django_encryption-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     7835 1970-01-01 00:00:00.000000 django_encryption-0.3.4/PKG-INFO
```

### Comparing `django_encryption-0.3.3/README.md` & `django_encryption-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `django_encryption-0.3.3/django_encryption/fields.py` & `django_encryption-0.3.4/django_encryption/fields.py`

 * *Files identical despite different names*

### Comparing `django_encryption-0.3.3/django_encryption/management/commands/generate_vault_migration.py` & `django_encryption-0.3.4/django_encryption/management/commands/generate_vault_migration.py`

 * *Files identical despite different names*

### Comparing `django_encryption-0.3.3/django_encryption/vault_wrapper.py` & `django_encryption-0.3.4/django_encryption/vault_wrapper.py`

 * *Files identical despite different names*

### Comparing `django_encryption-0.3.3/pyproject.toml` & `django_encryption-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-encryption"
-version = "0.3.3"
+version = "0.3.4"
 description = "A set of fields that wrap standard Django fields with encryption provided Piiano Vault."
 authors = ["Imri Goldberg <imri.goldberg@piiano.com>"]
 license = "MIT"
 packages = [ { include = "django_encryption" } ]
 readme = "README.md"
 repository = "https://github.com/piiano/vault-python"
 keywords = [ "encryption", "django", "fields" ]
```

### Comparing `django_encryption-0.3.3/PKG-INFO` & `django_encryption-0.3.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-encryption
-Version: 0.3.3
+Version: 0.3.4
 Summary: A set of fields that wrap standard Django fields with encryption provided Piiano Vault.
 Home-page: https://github.com/piiano/vault-python
 License: MIT
 Keywords: encryption,django,fields
 Author: Imri Goldberg
 Author-email: imri.goldberg@piiano.com
 Requires-Python: >=3.8,<4.0
@@ -23,19 +23,14 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
 Requires-Dist: Django (>=2.2)
 Requires-Dist: mypy (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/piiano/vault-python
```

