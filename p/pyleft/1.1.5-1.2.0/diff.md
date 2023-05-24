# Comparing `tmp/pyleft-1.1.5.tar.gz` & `tmp/pyleft-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyleft-1.1.5.tar", max compression
+gzip compressed data, was "pyleft-1.2.0.tar", max compression
```

## Comparing `pyleft-1.1.5.tar` & `pyleft-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-05-01 22:17:15.683375 pyleft-1.1.5/LICENSE
--rw-r--r--   0        0        0     3528 2023-05-01 22:17:15.683375 pyleft-1.1.5/README.md
--rw-r--r--   0        0        0        0 2023-05-01 22:17:15.683375 pyleft-1.1.5/pyleft/__init__.py
--rw-r--r--   0        0        0       37 2023-05-01 22:17:15.683375 pyleft-1.1.5/pyleft/__main__.py
--rw-r--r--   0        0        0     8980 2023-05-01 22:17:15.683375 pyleft-1.1.5/pyleft/api.py
--rw-r--r--   0        0        0     1246 2023-05-01 22:17:15.683375 pyleft-1.1.5/pyleft/console.py
--rw-r--r--   0        0        0     1327 2023-05-01 22:17:15.683375 pyleft-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     4574 1970-01-01 00:00:00.000000 pyleft-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-24 01:15:52.545921 pyleft-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3659 2023-05-24 01:15:52.545921 pyleft-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-24 01:15:52.545921 pyleft-1.2.0/pyleft/__init__.py
+-rw-r--r--   0        0        0       37 2023-05-24 01:15:52.545921 pyleft-1.2.0/pyleft/__main__.py
+-rw-r--r--   0        0        0     6228 2023-05-24 01:15:52.545921 pyleft-1.2.0/pyleft/api.py
+-rw-r--r--   0        0        0      539 2023-05-24 01:15:52.545921 pyleft-1.2.0/pyleft/console.py
+-rw-r--r--   0        0        0      276 2023-05-24 01:15:52.545921 pyleft-1.2.0/pyleft/models.py
+-rw-r--r--   0        0        0     1860 2023-05-24 01:15:52.545921 pyleft-1.2.0/pyleft/path_utils.py
+-rw-r--r--   0        0        0      474 2023-05-24 01:15:52.545921 pyleft-1.2.0/pyleft/printing.py
+-rw-r--r--   0        0        0     8860 2023-05-24 01:15:52.545921 pyleft-1.2.0/pyleft/settings.py
+-rw-r--r--   0        0        0     1353 2023-05-24 01:15:52.545921 pyleft-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4705 1970-01-01 00:00:00.000000 pyleft-1.2.0/PKG-INFO
```

### Comparing `pyleft-1.1.5/LICENSE` & `pyleft-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyleft-1.1.5/README.md` & `pyleft-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -33,54 +33,58 @@
 The module will exit with an exit code of 0 if all type hints are present, or 1
 if there are any issues.
 
 ### Example
 
 ```bash
 > pyleft .
-- tests\files\fail_1.py
+- tests/files/fail_1.py
         Argument 'two' of function 'add:1' has no type annotation
-- tests\files\fail_2.py
+- tests/files/fail_2.py
         Function 'add:1' has no return type annotation
-- tests\files\fail_3.py
+- tests/files/fail_3.py
         Function 'drive:2' has no return type annotation
-- tests\files\fail_4.py
+- tests/files/fail_4.py
         Argument 'one' of function 'wheels:4' has no type annotation
 ```
 
 ## Options
 
-- `files`: List of filenames and/or directories to recursively check.
-- `--exclude`: (optional) List of patterns to exclude, in `.gitignore` format.
-  Takes precedence over `files`.
-- `--no-gitignore`: (optional) Don't use the exclusions from the .gitignore from
-  the current working directory.
+- `paths`: File and directory names to recursively check.
+- `--exclude`: (optional) List of pattern(s) of files/directories to exclude in
+  gitignore format. Takes precedence over `paths`.
+- `--no-gitignore`: (optional) Don't use the exclusions from the .gitignore file(s)
+  in the current working directory.
+- `--ignore-if-has-default`: (optional) Ignore a lack of annotation if a function
+  argument has a default value.
 - `--quiet`: (optional) Don't print any output to STDOUT.
 - `--verbose`: (optional) Print debugging information to STDERR.
 
 ## Configuration
 
 Configuration is done through the `pyproject.toml` file.
 
 ```toml
 [tool.pyleft]
-# "files" in the configuration file are added to the option given on the
+# "paths" in the configuration file are added to the option given on the
 # command line
 # This can either be a list, or a space separated string
-files = ["extra/directory/"]
+paths = ["extra/directory/"]
 # This can either be a list, or a space separated string
 exclude = ["*_pb2.py"]
-no-gitignore = true
+# These are all booleans
+no-gitignore = false
+ignore-if-has-default = false
+quiet = false
+verbose = false
 ```
 
-The `quiet` and `verbose` options can only be specified from the command line.
-
 ## Design Decisions
 
-Only files with a `.py` extension are checked. Currently, `.pyi` files are not checked.
+If a `.pyi` file exists alongside a `.py` file, only the `.pyi` file will be checked.
 
 The `__init__` and `__new__` methods of a class are not required to
 have return type hints. `pyright` automatically assumes this to be `None`.
 
 The first (`self`) argument of any class method is not required to have a type hint.
 
 The first (`cls`) argument of any class `@property` or `@classmethod` or `__new__`
```

### Comparing `pyleft-1.1.5/pyproject.toml` & `pyleft-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
     name = "pyleft"
-    version = "1.1.5"
+    version = "1.2.0"
     description = "Python type annotation existence checker"
     license = "MIT"
     readme = "README.md"
     homepage = "https://github.com/NathanVaughn/pyleft"
     repository = "https://github.com/NathanVaughn/pyleft.git"
     authors = ["Nathan Vaughn <nvaughn51@gmail.com>"]
     classifiers = [
@@ -22,14 +22,15 @@
     # match Black's dependencies
     # https://github.com/psf/black/blob/e712e48e06420d9240ce95c81acfcf6f11d14c83/pyproject.toml#L69-L71
     tomli    = { version = ">=1.1.0", python = "<3.11" }
     pathspec = ">=0.9.0"
 
 [tool.poetry.group.dev.dependencies]
     pytest     = "^7.2.0"
+    pytest-cov = "^4.0.0"
     pre-commit = "^2.21.0"
 
 [tool.pyright]
     typeCheckingMode = "basic"
     venvPath         = "."
     venv             = ".venv"
```

### Comparing `pyleft-1.1.5/PKG-INFO` & `pyleft-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyleft
-Version: 1.1.5
+Version: 1.2.0
 Summary: Python type annotation existence checker
 Home-page: https://github.com/NathanVaughn/pyleft
 License: MIT
 Author: Nathan Vaughn
 Author-email: nvaughn51@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
@@ -58,54 +58,58 @@
 The module will exit with an exit code of 0 if all type hints are present, or 1
 if there are any issues.
 
 ### Example
 
 ```bash
 > pyleft .
-- tests\files\fail_1.py
+- tests/files/fail_1.py
         Argument 'two' of function 'add:1' has no type annotation
-- tests\files\fail_2.py
+- tests/files/fail_2.py
         Function 'add:1' has no return type annotation
-- tests\files\fail_3.py
+- tests/files/fail_3.py
         Function 'drive:2' has no return type annotation
-- tests\files\fail_4.py
+- tests/files/fail_4.py
         Argument 'one' of function 'wheels:4' has no type annotation
 ```
 
 ## Options
 
-- `files`: List of filenames and/or directories to recursively check.
-- `--exclude`: (optional) List of patterns to exclude, in `.gitignore` format.
-  Takes precedence over `files`.
-- `--no-gitignore`: (optional) Don't use the exclusions from the .gitignore from
-  the current working directory.
+- `paths`: File and directory names to recursively check.
+- `--exclude`: (optional) List of pattern(s) of files/directories to exclude in
+  gitignore format. Takes precedence over `paths`.
+- `--no-gitignore`: (optional) Don't use the exclusions from the .gitignore file(s)
+  in the current working directory.
+- `--ignore-if-has-default`: (optional) Ignore a lack of annotation if a function
+  argument has a default value.
 - `--quiet`: (optional) Don't print any output to STDOUT.
 - `--verbose`: (optional) Print debugging information to STDERR.
 
 ## Configuration
 
 Configuration is done through the `pyproject.toml` file.
 
 ```toml
 [tool.pyleft]
-# "files" in the configuration file are added to the option given on the
+# "paths" in the configuration file are added to the option given on the
 # command line
 # This can either be a list, or a space separated string
-files = ["extra/directory/"]
+paths = ["extra/directory/"]
 # This can either be a list, or a space separated string
 exclude = ["*_pb2.py"]
-no-gitignore = true
+# These are all booleans
+no-gitignore = false
+ignore-if-has-default = false
+quiet = false
+verbose = false
 ```
 
-The `quiet` and `verbose` options can only be specified from the command line.
-
 ## Design Decisions
 
-Only files with a `.py` extension are checked. Currently, `.pyi` files are not checked.
+If a `.pyi` file exists alongside a `.py` file, only the `.pyi` file will be checked.
 
 The `__init__` and `__new__` methods of a class are not required to
 have return type hints. `pyright` automatically assumes this to be `None`.
 
 The first (`self`) argument of any class method is not required to have a type hint.
 
 The first (`cls`) argument of any class `@property` or `@classmethod` or `__new__`
```

