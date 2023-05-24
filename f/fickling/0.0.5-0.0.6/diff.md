# Comparing `tmp/fickling-0.0.5.tar.gz` & `tmp/fickling-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fickling-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fickling-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fickling-0.0.5.tar` & `fickling-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7652 2023-05-19 16:32:54.507444 fickling-0.0.5/LICENSE
--rw-r--r--   0        0        0     2885 2023-05-19 16:32:54.507444 fickling-0.0.5/README.md
--rw-r--r--   0        0        0       22 2023-05-19 16:32:54.507444 fickling-0.0.5/fickling/__init__.py
--rw-r--r--   0        0        0       67 2023-05-19 16:32:54.507444 fickling-0.0.5/fickling/__main__.py
--rw-r--r--   0        0        0     5019 2023-05-19 16:32:54.507444 fickling-0.0.5/fickling/analysis.py
--rw-r--r--   0        0        0     6152 2023-05-19 16:32:54.507444 fickling-0.0.5/fickling/cli.py
--rw-r--r--   0        0        0    45956 2023-05-19 16:32:54.507444 fickling-0.0.5/fickling/pickle.py
--rw-r--r--   0        0        0     2577 2023-05-19 16:32:54.507444 fickling-0.0.5/fickling/tracing.py
--rw-r--r--   0        0        0     1884 2023-05-19 16:32:54.507444 fickling-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4322 1970-01-01 00:00:00.000000 fickling-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-05-24 21:13:26.110072 fickling-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2885 2023-05-24 21:13:26.110072 fickling-0.0.6/README.md
+-rw-r--r--   0        0        0       22 2023-05-24 21:13:26.110072 fickling-0.0.6/fickling/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-24 21:13:26.110072 fickling-0.0.6/fickling/__main__.py
+-rw-r--r--   0        0        0    10514 2023-05-24 21:13:26.110072 fickling-0.0.6/fickling/analysis.py
+-rw-r--r--   0        0        0     6152 2023-05-24 21:13:26.110072 fickling-0.0.6/fickling/cli.py
+-rw-r--r--   0        0        0    45956 2023-05-24 21:13:26.114072 fickling-0.0.6/fickling/pickle.py
+-rw-r--r--   0        0        0     2577 2023-05-24 21:13:26.114072 fickling-0.0.6/fickling/tracing.py
+-rw-r--r--   0        0        0     1884 2023-05-24 21:13:26.114072 fickling-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4322 1970-01-01 00:00:00.000000 fickling-0.0.6/PKG-INFO
```

### Comparing `fickling-0.0.5/LICENSE` & `fickling-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fickling-0.0.5/README.md` & `fickling-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fickling-0.0.5/fickling/cli.py` & `fickling-0.0.6/fickling/cli.py`

 * *Files identical despite different names*

### Comparing `fickling-0.0.5/fickling/pickle.py` & `fickling-0.0.6/fickling/pickle.py`

 * *Files identical despite different names*

### Comparing `fickling-0.0.5/fickling/tracing.py` & `fickling-0.0.6/fickling/tracing.py`

 * *Files identical despite different names*

### Comparing `fickling-0.0.5/pyproject.toml` & `fickling-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fickling-0.0.5/PKG-INFO` & `fickling-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fickling
-Version: 0.0.5
+Version: 0.0.6
 Summary: A static analyzer and interpreter for Python pickle data
 Author-email: Trail of Bits <opensource@trailofbits.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

