# Comparing `tmp/Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0.tar.gz` & `tmp/autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0.tar", last modified: Wed May 17 19:38:33 2023, max compression
+gzip compressed data, was "autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0.tar", last modified: Wed May 24 16:11:06 2023, max compression
```

## Comparing `Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0.tar` & `autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:38:33.820925 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-17 19:38:22.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:38:33.816925 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:38:33.816925 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-17 19:38:22.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-17 19:38:22.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-17 19:38:22.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-17 19:38:33.820925 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-17 19:38:22.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:38:33.816925 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    35702 2023-05-17 19:38:22.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/docs/basic-usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-17 19:38:22.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:38:33.816925 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-17 19:38:22.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-17 19:38:22.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:38:33.816925 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-17 19:38:22.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-17 19:38:22.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-17 19:38:22.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:38:33.820925 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:38:33.816925 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:38:33.816925 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/src/Autora_Experimentalist_Sampler_Nearest_Value_Sampler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-17 19:38:33.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/src/Autora_Experimentalist_Sampler_Nearest_Value_Sampler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-17 19:38:33.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/src/Autora_Experimentalist_Sampler_Nearest_Value_Sampler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:38:33.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/src/Autora_Experimentalist_Sampler_Nearest_Value_Sampler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 19:38:33.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/src/Autora_Experimentalist_Sampler_Nearest_Value_Sampler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 19:38:33.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/src/Autora_Experimentalist_Sampler_Nearest_Value_Sampler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:38:33.816925 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:38:33.816925 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/src/autora/experimentalist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:38:33.816925 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/src/autora/experimentalist/sampler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:38:33.816925 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/src/autora/experimentalist/sampler/nearest_value_sampler/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-17 19:38:22.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/src/autora/experimentalist/sampler/nearest_value_sampler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:38:33.820925 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-17 19:38:22.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:38:22.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-17 19:38:22.000000 Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/tests/test_nearest_value_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:06.673470 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-24 16:10:54.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:06.669470 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:06.673470 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-24 16:10:54.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-24 16:10:54.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-24 16:10:54.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-24 16:11:06.673470 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-24 16:10:54.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:06.673470 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    35702 2023-05-24 16:10:54.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/docs/basic-usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-24 16:10:54.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:06.673470 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-24 16:10:54.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-24 16:10:54.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:06.673470 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-24 16:10:54.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-24 16:10:54.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-24 16:10:54.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:11:06.673470 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:06.669470 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:06.669470 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:06.669470 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/src/autora/experimentalist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:06.669470 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/src/autora/experimentalist/sampler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:06.673470 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/src/autora/experimentalist/sampler/nearest_value_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-24 16:10:54.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/src/autora/experimentalist/sampler/nearest_value_sampler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:06.673470 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/src/autora_experimentalist_sampler_nearest_value_sampler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-24 16:11:06.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/src/autora_experimentalist_sampler_nearest_value_sampler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-24 16:11:06.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/src/autora_experimentalist_sampler_nearest_value_sampler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:11:06.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/src/autora_experimentalist_sampler_nearest_value_sampler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-24 16:11:06.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/src/autora_experimentalist_sampler_nearest_value_sampler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 16:11:06.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/src/autora_experimentalist_sampler_nearest_value_sampler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:06.673470 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-24 16:10:54.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:10:54.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-24 16:10:54.000000 autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/tests/test_nearest_value_sampler.py
```

### Comparing `Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/.github/workflows/python-publish.yml` & `autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/.gitignore` & `autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/.gitignore`

 * *Files identical despite different names*

### Comparing `Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/.pre-commit-config.yaml` & `autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/PKG-INFO` & `autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Autora-Experimentalist-Sampler-Nearest-Value-Sampler
-Version: 1.0.0a0
+Name: autora-experimentalist-sampler-nearest-value-sampler
+Version: 1.0.0b0
 Summary: A sampler which returns the nearest values between the input samples and the allowed values, without replacement.
 Author-email: "Built by Sebastian Musslick, restructured by Chad Williams" <sebastian_musslick@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-sampler-nearest-value-sampler
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/docs/basic-usage.ipynb` & `autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/docs/basic-usage.ipynb`

 * *Files identical despite different names*

### Comparing `Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/mkdocs/base.yml` & `autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/pyproject.toml` & `autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 # UPDATE THIS BEFORE PUBLISHING
-name = "Autora-Experimentalist-Sampler-Nearest-Value-Sampler"
+name = "autora-experimentalist-sampler-nearest-value-sampler"
 description = "A sampler which returns the nearest values between the input samples and the allowed values, without replacement."
 authors = [{ name = "Built by Sebastian Musslick, restructured by Chad Williams", email = "sebastian_musslick@brown.edu" }]
 dynamic = ["version"]
 
 readme = "README.md"
 license = { text = "MIT license" }
 requires-python = ">=3.8,<4"
```

### Comparing `Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/src/Autora_Experimentalist_Sampler_Nearest_Value_Sampler.egg-info/PKG-INFO` & `autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/src/autora_experimentalist_sampler_nearest_value_sampler.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Autora-Experimentalist-Sampler-Nearest-Value-Sampler
-Version: 1.0.0a0
+Name: autora-experimentalist-sampler-nearest-value-sampler
+Version: 1.0.0b0
 Summary: A sampler which returns the nearest values between the input samples and the allowed values, without replacement.
 Author-email: "Built by Sebastian Musslick, restructured by Chad Williams" <sebastian_musslick@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-sampler-nearest-value-sampler
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/src/autora/experimentalist/sampler/nearest_value_sampler/__init__.py` & `autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/src/autora/experimentalist/sampler/nearest_value_sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `Autora-Experimentalist-Sampler-Nearest-Value-Sampler-1.0.0a0/tests/README.md` & `autora-experimentalist-sampler-nearest-value-sampler-1.0.0b0/tests/README.md`

 * *Files identical despite different names*

