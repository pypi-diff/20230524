# Comparing `tmp/rust-contracts-builder-0.2.5.tar.gz` & `tmp/rust-contracts-builder-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rust-contracts-builder-0.2.5.tar", last modified: Fri Sep 16 01:49:19 2022, max compression
+gzip compressed data, was "rust-contracts-builder-0.2.6.tar", last modified: Mon May 15 09:03:29 2023, max compression
```

## Comparing `rust-contracts-builder-0.2.5.tar` & `rust-contracts-builder-0.2.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 01:49:19.756933 rust-contracts-builder-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-09-16 01:49:08.000000 rust-contracts-builder-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      499 2022-09-16 01:49:19.756933 rust-contracts-builder-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      214 2022-09-16 01:49:08.000000 rust-contracts-builder-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 01:49:19.756933 rust-contracts-builder-0.2.5/pysrc/
--rw-r--r--   0 runner    (1001) docker     (116)     7170 2022-09-16 01:49:08.000000 rust-contracts-builder-0.2.5/pysrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       40 2022-09-16 01:49:08.000000 rust-contracts-builder-0.2.5/pysrc/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 01:49:19.752933 rust-contracts-builder-0.2.5/pysrc/templates/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 01:49:19.756933 rust-contracts-builder-0.2.5/pysrc/templates/abigen/
--rw-r--r--   0 runner    (1001) docker     (116)      288 2022-09-16 01:49:08.000000 rust-contracts-builder-0.2.5/pysrc/templates/abigen/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (116)      205 2022-09-16 01:49:08.000000 rust-contracts-builder-0.2.5/pysrc/templates/abigen/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 01:49:19.756933 rust-contracts-builder-0.2.5/pysrc/templates/init/
--rw-r--r--   0 runner    (1001) docker     (116)      285 2022-09-16 01:49:08.000000 rust-contracts-builder-0.2.5/pysrc/templates/init/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      335 2022-09-16 01:49:08.000000 rust-contracts-builder-0.2.5/pysrc/templates/init/_Cargo.toml
--rwxr-xr-x   0 runner    (1001) docker     (116)       20 2022-09-16 01:49:08.000000 rust-contracts-builder-0.2.5/pysrc/templates/init/build.sh
--rw-r--r--   0 runner    (1001) docker     (116)     3191 2022-09-16 01:49:08.000000 rust-contracts-builder-0.2.5/pysrc/templates/init/lib.rs
--rw-r--r--   0 runner    (1001) docker     (116)     2118 2022-09-16 01:49:08.000000 rust-contracts-builder-0.2.5/pysrc/templates/init/test.py
--rwxr-xr-x   0 runner    (1001) docker     (116)       48 2022-09-16 01:49:08.000000 rust-contracts-builder-0.2.5/pysrc/templates/init/test.sh
--rw-r--r--   0 runner    (1001) docker     (116)     8055 2022-09-16 01:49:08.000000 rust-contracts-builder-0.2.5/pysrc/wasm_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 01:49:19.756933 rust-contracts-builder-0.2.5/rust_contracts_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      499 2022-09-16 01:49:19.000000 rust-contracts-builder-0.2.5/rust_contracts_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      618 2022-09-16 01:49:19.000000 rust-contracts-builder-0.2.5/rust_contracts_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-09-16 01:49:19.000000 rust-contracts-builder-0.2.5/rust_contracts_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       70 2022-09-16 01:49:19.000000 rust-contracts-builder-0.2.5/rust_contracts_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2022-09-16 01:49:19.000000 rust-contracts-builder-0.2.5/rust_contracts_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       23 2022-09-16 01:49:19.000000 rust-contracts-builder-0.2.5/rust_contracts_builder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      225 2022-09-16 01:49:19.756933 rust-contracts-builder-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      974 2022-09-16 01:49:08.000000 rust-contracts-builder-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:03:29.825178 rust-contracts-builder-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 09:03:18.000000 rust-contracts-builder-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-15 09:03:29.825178 rust-contracts-builder-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-15 09:03:18.000000 rust-contracts-builder-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:03:29.825178 rust-contracts-builder-0.2.6/pysrc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-05-15 09:03:18.000000 rust-contracts-builder-0.2.6/pysrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 09:03:18.000000 rust-contracts-builder-0.2.6/pysrc/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:03:29.825178 rust-contracts-builder-0.2.6/pysrc/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:03:29.825178 rust-contracts-builder-0.2.6/pysrc/templates/abigen/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-15 09:03:18.000000 rust-contracts-builder-0.2.6/pysrc/templates/abigen/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-15 09:03:18.000000 rust-contracts-builder-0.2.6/pysrc/templates/abigen/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:03:29.825178 rust-contracts-builder-0.2.6/pysrc/templates/init/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-15 09:03:18.000000 rust-contracts-builder-0.2.6/pysrc/templates/init/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-15 09:03:18.000000 rust-contracts-builder-0.2.6/pysrc/templates/init/_Cargo.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       20 2023-05-15 09:03:18.000000 rust-contracts-builder-0.2.6/pysrc/templates/init/build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-15 09:03:18.000000 rust-contracts-builder-0.2.6/pysrc/templates/init/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-15 09:03:18.000000 rust-contracts-builder-0.2.6/pysrc/templates/init/test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-05-15 09:03:18.000000 rust-contracts-builder-0.2.6/pysrc/templates/init/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-15 09:03:18.000000 rust-contracts-builder-0.2.6/pysrc/wasm_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:03:29.825178 rust-contracts-builder-0.2.6/rust_contracts_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-15 09:03:29.000000 rust-contracts-builder-0.2.6/rust_contracts_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-15 09:03:29.000000 rust-contracts-builder-0.2.6/rust_contracts_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:03:29.000000 rust-contracts-builder-0.2.6/rust_contracts_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-15 09:03:29.000000 rust-contracts-builder-0.2.6/rust_contracts_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 09:03:29.000000 rust-contracts-builder-0.2.6/rust_contracts_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 09:03:29.000000 rust-contracts-builder-0.2.6/rust_contracts_builder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-15 09:03:29.825178 rust-contracts-builder-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-15 09:03:18.000000 rust-contracts-builder-0.2.6/setup.py
```

### Comparing `rust-contracts-builder-0.2.5/LICENSE` & `rust-contracts-builder-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rust-contracts-builder-0.2.5/pysrc/__init__.py` & `rust-contracts-builder-0.2.6/pysrc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import platform
 import tempfile
 import toml
 import shutil
 import argparse
 from .wasm_checker import check_import_section
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 
 src_dir = os.path.dirname(__file__).replace('\\', '/')
 
 
 #https://stackabuse.com/how-to-print-colored-text-in-python/
 #https://stackoverflow.com/questions/287871/how-do-i-print-colored-text-to-the-terminal
 HEADER = '\033[95m'
```

### Comparing `rust-contracts-builder-0.2.5/pysrc/templates/init/lib.rs` & `rust-contracts-builder-0.2.6/pysrc/templates/init/lib.rs`

 * *Files identical despite different names*

### Comparing `rust-contracts-builder-0.2.5/pysrc/templates/init/test.py` & `rust-contracts-builder-0.2.6/pysrc/templates/init/test.py`

 * *Files identical despite different names*

### Comparing `rust-contracts-builder-0.2.5/pysrc/wasm_checker.py` & `rust-contracts-builder-0.2.6/pysrc/wasm_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,16 @@
         "get_block_num",
         "sha3",
         "blake2_f",
         "k1_recover",
         "alt_bn128_add",
         "alt_bn128_mul",
         "alt_bn128_pair",
-        "mod_exp"
+        "mod_exp",
+        "get_code_hash",
 ]
 
 class WasmReader(object):
     def __init__(self, raw):
         self.raw = raw
         self.idx = 0
```

### Comparing `rust-contracts-builder-0.2.5/rust_contracts_builder.egg-info/SOURCES.txt` & `rust-contracts-builder-0.2.6/rust_contracts_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rust-contracts-builder-0.2.5/setup.py` & `rust-contracts-builder-0.2.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     for f in files:
         release_files.append(os.path.join(root.replace('pysrc/', ''), f))    
 
 # print(release_files)
 
 setup(
     name="rust-contracts-builder",
-    version="0.2.5",
+    version="0.2.6",
     description="Rust Contracts Builder",
     author='The UUOSIO Team',
     license="Apache 2.0",
     url="https://github.com/uuosio/rust-contracts-builder",
     packages=['rust_contracts_builder'],
     package_dir={'rust_contracts_builder': 'pysrc'},
     package_data={
```

