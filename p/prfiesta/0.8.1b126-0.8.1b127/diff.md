# Comparing `tmp/prfiesta-0.8.1b126.tar.gz` & `tmp/prfiesta-0.8.1b127.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prfiesta-0.8.1b126.tar", max compression
+gzip compressed data, was "prfiesta-0.8.1b127.tar", max compression
```

## Comparing `prfiesta-0.8.1b126.tar` & `prfiesta-0.8.1b127.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2023-05-24 05:53:29.371526 prfiesta-0.8.1b126/LICENSE
--rw-r--r--   0        0        0     7783 2023-05-24 05:53:29.371526 prfiesta-0.8.1b126/README.md
--rw-r--r--   0        0        0      487 2023-05-24 05:53:29.379526 prfiesta-0.8.1b126/prfiesta/__init__.py
--rw-r--r--   0        0        0     2763 2023-05-24 05:53:29.379526 prfiesta-0.8.1b126/prfiesta/__main__.py
--rw-r--r--   0        0        0        0 2023-05-24 05:53:29.379526 prfiesta-0.8.1b126/prfiesta/analysis/__init__.py
--rw-r--r--   0        0        0     4729 2023-05-24 05:53:29.379526 prfiesta-0.8.1b126/prfiesta/analysis/plot.py
--rw-r--r--   0        0        0     1007 2023-05-24 05:53:29.379526 prfiesta-0.8.1b126/prfiesta/analysis/view.py
--rw-r--r--   0        0        0        0 2023-05-24 05:53:29.379526 prfiesta-0.8.1b126/prfiesta/collectors/__init__.py
--rw-r--r--   0        0        0     4981 2023-05-24 05:53:29.379526 prfiesta-0.8.1b126/prfiesta/collectors/github.py
--rw-r--r--   0        0        0      571 2023-05-24 05:53:29.379526 prfiesta-0.8.1b126/prfiesta/environment.py
--rw-r--r--   0        0        0      975 2023-05-24 05:53:29.379526 prfiesta-0.8.1b126/prfiesta/output.py
--rw-r--r--   0        0        0      275 2023-05-24 05:53:29.379526 prfiesta-0.8.1b126/prfiesta/spinner.py
--rw-r--r--   0        0        0     3199 2023-05-24 05:53:39.083746 prfiesta-0.8.1b126/pyproject.toml
--rw-r--r--   0        0        0     9144 1970-01-01 00:00:00.000000 prfiesta-0.8.1b126/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-24 05:57:28.932593 prfiesta-0.8.1b127/LICENSE
+-rw-r--r--   0        0        0     7884 2023-05-24 05:57:28.932593 prfiesta-0.8.1b127/README.md
+-rw-r--r--   0        0        0      487 2023-05-24 05:57:28.944594 prfiesta-0.8.1b127/prfiesta/__init__.py
+-rw-r--r--   0        0        0     2763 2023-05-24 05:57:28.944594 prfiesta-0.8.1b127/prfiesta/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:57:28.944594 prfiesta-0.8.1b127/prfiesta/analysis/__init__.py
+-rw-r--r--   0        0        0     4729 2023-05-24 05:57:28.944594 prfiesta-0.8.1b127/prfiesta/analysis/plot.py
+-rw-r--r--   0        0        0     1007 2023-05-24 05:57:28.944594 prfiesta-0.8.1b127/prfiesta/analysis/view.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:57:28.944594 prfiesta-0.8.1b127/prfiesta/collectors/__init__.py
+-rw-r--r--   0        0        0     4981 2023-05-24 05:57:28.944594 prfiesta-0.8.1b127/prfiesta/collectors/github.py
+-rw-r--r--   0        0        0      571 2023-05-24 05:57:28.944594 prfiesta-0.8.1b127/prfiesta/environment.py
+-rw-r--r--   0        0        0      975 2023-05-24 05:57:28.944594 prfiesta-0.8.1b127/prfiesta/output.py
+-rw-r--r--   0        0        0      275 2023-05-24 05:57:28.944594 prfiesta-0.8.1b127/prfiesta/spinner.py
+-rw-r--r--   0        0        0     3199 2023-05-24 05:57:42.968933 prfiesta-0.8.1b127/pyproject.toml
+-rw-r--r--   0        0        0     9245 1970-01-01 00:00:00.000000 prfiesta-0.8.1b127/PKG-INFO
```

### Comparing `prfiesta-0.8.1b126/LICENSE` & `prfiesta-0.8.1b127/LICENSE`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.1b126/README.md` & `prfiesta-0.8.1b127/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -161,7 +161,9 @@
 - `0.8.1` = The bumped version of what is currently within the `pyproject.toml` of that pull request. We don't attempt to do any analysis to figure out if we should be bumping with a higher serverity in this context.
 - `b` = Beta; Indicates to pypi that this is a prerelease package.
 - `125` = The `github.run_number` from [GitHub Actions](https://docs.github.com/en/actions/learn-github-actions/contexts#github-context).
 
 An example prerelease package looks like this: https://pypi.org/project/prfiesta/0.8.1b125/
 
 Downstream users can then do a full end to end test with the prerelease package before the change is merged into `main`.
+
+You can find the full version history of package [here](https://pypi.org/project/prfiesta/#history)
```

### Comparing `prfiesta-0.8.1b126/prfiesta/__main__.py` & `prfiesta-0.8.1b127/prfiesta/__main__.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.1b126/prfiesta/analysis/plot.py` & `prfiesta-0.8.1b127/prfiesta/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.1b126/prfiesta/analysis/view.py` & `prfiesta-0.8.1b127/prfiesta/analysis/view.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.1b126/prfiesta/collectors/github.py` & `prfiesta-0.8.1b127/prfiesta/collectors/github.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.1b126/prfiesta/environment.py` & `prfiesta-0.8.1b127/prfiesta/environment.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.1b126/prfiesta/output.py` & `prfiesta-0.8.1b127/prfiesta/output.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.1b126/pyproject.toml` & `prfiesta-0.8.1b127/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prfiesta"
-version = "0.8.1b126"
+version = "0.8.1b127"
 description = "Collect and Analyze Individual Contributor Pull Requests"
 authors = ["kiran94"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kiran94/prfiesta"
 repository = "https://github.com/kiran94/prfiesta"
 documentation = "https://github.com/kiran94/prfiesta/blob/main/README.md"
```

### Comparing `prfiesta-0.8.1b126/PKG-INFO` & `prfiesta-0.8.1b127/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prfiesta
-Version: 0.8.1b126
+Version: 0.8.1b127
 Summary: Collect and Analyze Individual Contributor Pull Requests
 Home-page: https://github.com/kiran94/prfiesta
 License: MIT
 Keywords: pull-request,pull-request-review,performance-review
 Author: kiran94
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
@@ -195,7 +195,9 @@
 - `b` = Beta; Indicates to pypi that this is a prerelease package.
 - `125` = The `github.run_number` from [GitHub Actions](https://docs.github.com/en/actions/learn-github-actions/contexts#github-context).
 
 An example prerelease package looks like this: https://pypi.org/project/prfiesta/0.8.1b125/
 
 Downstream users can then do a full end to end test with the prerelease package before the change is merged into `main`.
 
+You can find the full version history of package [here](https://pypi.org/project/prfiesta/#history)
+
```

