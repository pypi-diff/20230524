# Comparing `tmp/predictionguard-0.2.5.tar.gz` & `tmp/predictionguard-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predictionguard-0.2.5.tar", last modified: Thu May 11 18:19:31 2023, max compression
+gzip compressed data, was "predictionguard-1.0.0.tar", last modified: Wed May 24 17:27:02 2023, max compression
```

## Comparing `predictionguard-0.2.5.tar` & `predictionguard-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1083 2022-12-30 13:34:31.843283 predictionguard-0.2.5/LICENSE
--rw-r--r--   0        0        0     1878 2023-02-17 23:59:20.007675 predictionguard-0.2.5/README.md
--rw-r--r--   0        0        0     3256 2023-02-19 21:56:15.644765 predictionguard-0.2.5/examples/sentiment.ipynb
--rw-r--r--   0        0        0      104 2023-05-11 18:16:21.004867 predictionguard-0.2.5/predictionguard/__init__.py
--rw-r--r--   0        0        0    10823 2023-04-16 20:40:10.523874 predictionguard-0.2.5/predictionguard/client.py
--rw-r--r--   0        0        0      483 2023-05-11 18:10:58.709630 predictionguard-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2257 1970-01-01 00:00:00.000000 predictionguard-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-12-30 13:34:31.843283 predictionguard-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1878 2023-02-17 23:59:20.007675 predictionguard-1.0.0/README.md
+-rw-r--r--   0        0        0     3256 2023-02-19 21:56:15.644765 predictionguard-1.0.0/examples/sentiment.ipynb
+-rw-r--r--   0        0        0      133 2023-05-24 17:26:35.257335 predictionguard-1.0.0/predictionguard/__init__.py
+-rw-r--r--   0        0        0    16341 2023-05-24 16:40:32.162550 predictionguard-1.0.0/predictionguard/client.py
+-rw-r--r--   0        0        0      483 2023-05-11 18:10:58.709630 predictionguard-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2274 1970-01-01 00:00:00.000000 predictionguard-1.0.0/PKG-INFO
```

### Comparing `predictionguard-0.2.5/LICENSE` & `predictionguard-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `predictionguard-0.2.5/README.md` & `predictionguard-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `predictionguard-0.2.5/examples/sentiment.ipynb` & `predictionguard-1.0.0/examples/sentiment.ipynb`

 * *Files identical despite different names*

### Comparing `predictionguard-0.2.5/PKG-INFO` & `predictionguard-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: predictionguard
-Version: 0.2.5
-Summary: AI models are irrelevant. Use Prediction Guard.
+Version: 1.0.0
+Summary: Create controlled and compliant AI systems with PredictionGuard.
 Author-email: Daniel Whitenack <dan@predictionguard.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: tabulate >=0.8.10
 Requires-Dist: requests >=2.27.1
 Project-URL: Home, https://predictionguard.com
```

