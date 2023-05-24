# Comparing `tmp/mizu-0.2.0a4.tar.gz` & `tmp/mizu-0.2.0a5.tar.gz`

## Comparing `mizu-0.2.0a4.tar` & `mizu-0.2.0a5.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0      345 1970-01-01 00:00:00.000000 mizu-0.2.0a4/Cargo.toml
--rw-r--r--   0     1001      123     1698 2022-12-19 06:55:11.000000 mizu-0.2.0a4/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     1083 2022-12-19 06:55:11.000000 mizu-0.2.0a4/.github/workflows/docs.yml
--rw-r--r--   0     1001      123     1372 2022-12-19 06:55:11.000000 mizu-0.2.0a4/.github/workflows/python-app.yml
--rw-r--r--   0     1001      123      685 2022-12-19 06:55:11.000000 mizu-0.2.0a4/.gitignore
--rw-r--r--   0     1001      123     1065 2022-12-19 06:55:11.000000 mizu-0.2.0a4/LICENSE
--rw-r--r--   0     1001      123      965 2022-12-19 06:55:11.000000 mizu-0.2.0a4/README.md
--rw-r--r--   0     1001      123      638 2022-12-19 06:55:11.000000 mizu-0.2.0a4/docs/Makefile
--rw-r--r--   0     1001      123      804 2022-12-19 06:55:11.000000 mizu-0.2.0a4/docs/make.bat
--rw-r--r--   0     1001      123       12 2022-12-19 06:55:11.000000 mizu-0.2.0a4/docs/requirements.txt
--rw-r--r--   0     1001      123     1016 2022-12-19 06:55:11.000000 mizu-0.2.0a4/docs/source/conf.py
--rw-r--r--   0     1001      123      447 2022-12-19 06:55:11.000000 mizu-0.2.0a4/docs/source/index.rst
--rw-r--r--   0     1001      123      157 2022-12-19 06:55:11.000000 mizu-0.2.0a4/docs/source/mizu.rst
--rw-r--r--   0     1001      123       49 2022-12-19 06:55:11.000000 mizu-0.2.0a4/docs/source/modules.rst
--rw-r--r--   0     1001      123      491 2022-12-19 06:55:11.000000 mizu-0.2.0a4/mizu/__init__.py
--rw-r--r--   0     1001      123      198 2022-12-19 06:55:11.000000 mizu-0.2.0a4/mizu/mizu.pyi
--rw-r--r--   0     1001      123     1340 2022-12-19 06:55:11.000000 mizu-0.2.0a4/mizu/options.py
--rw-r--r--   0     1001      123      429 2022-12-19 06:55:11.000000 mizu-0.2.0a4/pyproject.toml
--rwxr-xr-x   0     1001      123      767 2022-12-19 06:55:49.000000 mizu-0.2.0a4/run-maturin-action.sh
--rw-r--r--   0     1001      123     1660 2022-12-19 06:55:11.000000 mizu-0.2.0a4/src/core.rs
--rw-r--r--   0     1001      123      161 2022-12-19 06:55:11.000000 mizu-0.2.0a4/src/lib.rs
--rw-r--r--   0     1001      123      120 2022-12-19 06:55:11.000000 mizu-0.2.0a4/tests/test_md.py
--rw-r--r--   0     1001      123     8742 2022-12-19 06:58:19.000000 mizu-0.2.0a4/Cargo.lock
--rw-r--r--   0        0        0     1457 1970-01-01 00:00:00.000000 mizu-0.2.0a4/PKG-INFO
+-rw-r--r--   0        0        0      345 1970-01-01 00:00:00.000000 mizu-0.2.0a5/Cargo.toml
+-rw-r--r--   0     1001      123     1698 2022-12-19 08:34:24.000000 mizu-0.2.0a5/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     1094 2022-12-19 08:34:24.000000 mizu-0.2.0a5/.github/workflows/docs.yml
+-rw-r--r--   0     1001      123     1387 2022-12-19 08:34:24.000000 mizu-0.2.0a5/.github/workflows/python-app.yml
+-rw-r--r--   0     1001      123      685 2022-12-19 08:34:24.000000 mizu-0.2.0a5/.gitignore
+-rw-r--r--   0     1001      123     1065 2022-12-19 08:34:24.000000 mizu-0.2.0a5/LICENSE
+-rw-r--r--   0     1001      123      965 2022-12-19 08:34:24.000000 mizu-0.2.0a5/README.md
+-rw-r--r--   0     1001      123      638 2022-12-19 08:34:24.000000 mizu-0.2.0a5/docs/Makefile
+-rw-r--r--   0     1001      123      804 2022-12-19 08:34:24.000000 mizu-0.2.0a5/docs/make.bat
+-rw-r--r--   0     1001      123       12 2022-12-19 08:34:24.000000 mizu-0.2.0a5/docs/requirements.txt
+-rw-r--r--   0     1001      123     1016 2022-12-19 08:34:24.000000 mizu-0.2.0a5/docs/source/conf.py
+-rw-r--r--   0     1001      123      447 2022-12-19 08:34:24.000000 mizu-0.2.0a5/docs/source/index.rst
+-rw-r--r--   0     1001      123      157 2022-12-19 08:34:24.000000 mizu-0.2.0a5/docs/source/mizu.rst
+-rw-r--r--   0     1001      123       49 2022-12-19 08:34:24.000000 mizu-0.2.0a5/docs/source/modules.rst
+-rw-r--r--   0     1001      123      491 2022-12-19 08:34:24.000000 mizu-0.2.0a5/mizu/__init__.py
+-rw-r--r--   0     1001      123      263 2022-12-19 08:34:24.000000 mizu-0.2.0a5/mizu/mizu.pyi
+-rw-r--r--   0     1001      123     1340 2022-12-19 08:34:24.000000 mizu-0.2.0a5/mizu/options.py
+-rw-r--r--   0     1001      123      429 2022-12-19 08:34:24.000000 mizu-0.2.0a5/pyproject.toml
+-rwxr-xr-x   0     1001      123      767 2022-12-19 08:35:02.000000 mizu-0.2.0a5/run-maturin-action.sh
+-rw-r--r--   0     1001      123      415 2022-12-19 08:34:24.000000 mizu-0.2.0a5/src/asyncio.rs
+-rw-r--r--   0     1001      123     2639 2022-12-19 08:34:24.000000 mizu-0.2.0a5/src/core.rs
+-rw-r--r--   0     1001      123      174 2022-12-19 08:34:24.000000 mizu-0.2.0a5/src/lib.rs
+-rw-r--r--   0     1001      123      206 2022-12-19 08:34:24.000000 mizu-0.2.0a5/tests/test_async.py
+-rw-r--r--   0     1001      123      120 2022-12-19 08:34:24.000000 mizu-0.2.0a5/tests/test_md.py
+-rw-r--r--   0     1001      123     8742 2022-12-19 08:34:24.000000 mizu-0.2.0a5/Cargo.lock
+-rw-r--r--   0        0        0     1457 1970-01-01 00:00:00.000000 mizu-0.2.0a5/PKG-INFO
```

### Comparing `mizu-0.2.0a4/.github/workflows/CI.yml` & `mizu-0.2.0a5/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `mizu-0.2.0a4/.github/workflows/docs.yml` & `mizu-0.2.0a5/.github/workflows/docs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 name: Build document
 
 on:
   push:
-    branches: ["main"]
+    branches: ["main", "develop"]
     paths:
       - docs/**
 
 jobs:
   build:
     runs-on: ubuntu-latest
     steps:
```

### Comparing `mizu-0.2.0a4/.github/workflows/python-app.yml` & `mizu-0.2.0a5/.github/workflows/python-app.yml`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
           ~/.cargo/registry/cache/
           ~/.cargo/git/db/
           target/
         key: ${{ runner.os }}-cargo-${{ hashFiles('**/Cargo.lock') }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install flake8 pytest
+        pip install flake8 pytest pytest-asyncio
         pip install .
     - name: Lint with flake8
       run: |
         # stop the build if there are Python syntax errors or undefined names
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
         flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
```

### Comparing `mizu-0.2.0a4/.gitignore` & `mizu-0.2.0a5/.gitignore`

 * *Files identical despite different names*

### Comparing `mizu-0.2.0a4/LICENSE` & `mizu-0.2.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `mizu-0.2.0a4/README.md` & `mizu-0.2.0a5/README.md`

 * *Files identical despite different names*

### Comparing `mizu-0.2.0a4/docs/Makefile` & `mizu-0.2.0a5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mizu-0.2.0a4/docs/make.bat` & `mizu-0.2.0a5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mizu-0.2.0a4/docs/source/conf.py` & `mizu-0.2.0a5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mizu-0.2.0a4/mizu/options.py` & `mizu-0.2.0a5/mizu/options.py`

 * *Files identical despite different names*

### Comparing `mizu-0.2.0a4/run-maturin-action.sh` & `mizu-0.2.0a5/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `mizu-0.2.0a4/Cargo.lock` & `mizu-0.2.0a5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mizu"
-version = "0.2.0-alpha4"
+version = "0.2.0-alpha5"
 dependencies = [
  "pulldown-cmark",
  "pyo3",
 ]
 
 [[package]]
 name = "once_cell"
```

### Comparing `mizu-0.2.0a4/PKG-INFO` & `mizu-0.2.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mizu
-Version: 0.2.0a4
+Version: 0.2.0a5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Markdown library
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Documentation, https://tuna2134.github.io/mizu
 Project-URL: Source Code, https://github.com/tuna2134/mizu
+Project-URL: Documentation, https://tuna2134.github.io/mizu
 
 # mizu 💧
 
 **Warning:** This library is now developing. Please use stable version.
 
 [![Version](https://img.shields.io/pypi/v/mizu)](https://pypi.org/project/mizu/)
 [![Downloads](https://pepy.tech/badge/mizu)](https://pepy.tech/project/mizu)
```

