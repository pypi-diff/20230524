# Comparing `tmp/python-hcl2-4.3.1.tar.gz` & `tmp/python-hcl2-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/python-hcl2/python-hcl2/dist/.tmp-zyb9vd1n/python-hcl2-4.3.1.tar", last modified: Tue May  2 15:14:38 2023, max compression
+gzip compressed data, was "/home/runner/work/python-hcl2/python-hcl2/dist/.tmp-zqeh7olj/python-hcl2-4.3.2.tar", last modified: Wed May 24 13:47:55 2023, max compression
```

## Comparing `python-hcl2-4.3.1.tar` & `python-hcl2-4.3.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/.codacy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/.github/workflows/pr_check.yml
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/.yamllint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/bin/terraform_test
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/hcl2/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/hcl2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/hcl2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/hcl2/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/hcl2/hcl2.lark
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/hcl2/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/hcl2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/hcl2/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/hcl2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/python_hcl2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/python_hcl2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/python_hcl2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/python_hcl2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/python_hcl2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:14:27.000000 python-hcl2-4.3.1/python_hcl2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/python_hcl2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/python_hcl2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/reports/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/reports/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/test-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:47:55.000000 python-hcl2-4.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/.codacy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:47:55.000000 python-hcl2-4.3.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:47:55.000000 python-hcl2-4.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/.github/workflows/pr_check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/.yamllint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-24 13:47:55.000000 python-hcl2-4.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:47:55.000000 python-hcl2-4.3.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/bin/terraform_test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:47:55.000000 python-hcl2-4.3.2/hcl2/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/hcl2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/hcl2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/hcl2/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/hcl2/hcl2.lark
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/hcl2/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/hcl2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/hcl2/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 13:47:55.000000 python-hcl2-4.3.2/hcl2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:47:55.000000 python-hcl2-4.3.2/python_hcl2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-24 13:47:55.000000 python-hcl2-4.3.2/python_hcl2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-24 13:47:55.000000 python-hcl2-4.3.2/python_hcl2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:47:55.000000 python-hcl2-4.3.2/python_hcl2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 13:47:55.000000 python-hcl2-4.3.2/python_hcl2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:47:42.000000 python-hcl2-4.3.2/python_hcl2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-24 13:47:55.000000 python-hcl2-4.3.2/python_hcl2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 13:47:55.000000 python-hcl2-4.3.2/python_hcl2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:47:55.000000 python-hcl2-4.3.2/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/reports/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 13:47:55.000000 python-hcl2-4.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/test-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-24 13:47:31.000000 python-hcl2-4.3.2/tox.ini
```

### Comparing `python-hcl2-4.3.1/.github/workflows/codeql-analysis.yml` & `python-hcl2-4.3.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.1/.github/workflows/pr_check.yml` & `python-hcl2-4.3.2/.github/workflows/pr_check.yml`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.1/.github/workflows/publish.yml` & `python-hcl2-4.3.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.1/.gitignore` & `python-hcl2-4.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.1/.pre-commit-config.yaml` & `python-hcl2-4.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.1/CHANGELOG.md` & `python-hcl2-4.3.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## \[4.3.2\] - 2023-05-24
+
+### Added
+
+- Support for the conditional inside the nested locals without parentheses ([#138](https://github.com/amplify-education/python-hcl2/pull/129))
+
 ## \[4.3.1\] - 2023-05-02
 
 ### Added
 
 - Support for the braces in the next line. Thanks @rout39574 ([#129](https://github.com/amplify-education/python-hcl2/pull/129))
 - Support for the ternary multi-line expression. Thanks @seksham ([#128](https://github.com/amplify-education/python-hcl2/pull/128))
```

### Comparing `python-hcl2-4.3.1/LICENSE` & `python-hcl2-4.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.1/PKG-INFO` & `python-hcl2-4.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-hcl2
-Version: 4.3.1
+Version: 4.3.2
 Summary: A parser for HCL2
 Author-email: Amplify Education <github@amplify.com>
 License: MIT
 Project-URL: Homepage, https://github.com/amplify-education/python-hcl2
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
```

### Comparing `python-hcl2-4.3.1/README.md` & `python-hcl2-4.3.2/README.md`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.1/bin/terraform_test` & `python-hcl2-4.3.2/bin/terraform_test`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.1/hcl2/__main__.py` & `python-hcl2-4.3.2/hcl2/__main__.py`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.1/hcl2/api.py` & `python-hcl2-4.3.2/hcl2/api.py`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.1/hcl2/hcl2.lark` & `python-hcl2-4.3.2/hcl2/hcl2.lark`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 new_line_and_or_comma: new_line_or_comment | "," | "," new_line_or_comment
 new_line_or_comment: ( /\n/ | /#.*\n/ | /\/\/.*\n/ )+
 
 identifier : /[a-zA-Z_][a-zA-Z0-9_-]*/
 
 ?expression : expr_term | operation | conditional
 
-conditional : expression "?" new_line_or_comment? expression new_line_or_comment? ":" new_line_or_comment? expression new_line_or_comment?
+conditional : expression "?" new_line_or_comment? expression new_line_or_comment? ":" new_line_or_comment? expression
 
 ?operation : unary_op | binary_op
 !unary_op : ("-" | "!") expr_term
 binary_op : expression binary_term new_line_or_comment?
 !binary_operator : "==" | "!=" | "<" | ">" | "<=" | ">=" | "-" | "*" | "/" | "%" | "&&" | "||" | "+"
 binary_term : binary_operator new_line_or_comment? expression
```

### Comparing `python-hcl2-4.3.1/hcl2/transformer.py` & `python-hcl2-4.3.2/hcl2/transformer.py`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.1/pylintrc` & `python-hcl2-4.3.2/pylintrc`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.1/pyproject.toml` & `python-hcl2-4.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.1/python_hcl2.egg-info/PKG-INFO` & `python-hcl2-4.3.2/python_hcl2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-hcl2
-Version: 4.3.1
+Version: 4.3.2
 Summary: A parser for HCL2
 Author-email: Amplify Education <github@amplify.com>
 License: MIT
 Project-URL: Homepage, https://github.com/amplify-education/python-hcl2
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
```

### Comparing `python-hcl2-4.3.1/python_hcl2.egg-info/SOURCES.txt` & `python-hcl2-4.3.2/python_hcl2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.1/tox.ini` & `python-hcl2-4.3.2/tox.ini`

 * *Files identical despite different names*

