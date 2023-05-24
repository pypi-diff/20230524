# Comparing `tmp/Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0.tar.gz` & `tmp/autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0.tar", last modified: Wed May 17 19:55:52 2023, max compression
+gzip compressed data, was "autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0.tar", last modified: Wed May 24 15:54:29 2023, max compression
```

## Comparing `Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0.tar` & `autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:55:52.128082 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-17 19:55:40.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:55:52.120082 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:55:52.124082 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-17 19:55:40.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-17 19:55:40.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-17 19:55:40.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-17 19:55:52.128082 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-17 19:55:40.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:55:52.124082 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   141677 2023-05-17 19:55:40.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/docs/basic-usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-17 19:55:40.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:55:52.124082 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-17 19:55:40.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-17 19:55:40.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:55:52.124082 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-17 19:55:40.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-17 19:55:40.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-17 19:55:40.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:55:52.128082 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:55:52.120082 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:55:52.124082 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/src/Autora_Experimentalist_Sampler_Model_Disagreement_Sampler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-17 19:55:52.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/src/Autora_Experimentalist_Sampler_Model_Disagreement_Sampler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-17 19:55:52.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/src/Autora_Experimentalist_Sampler_Model_Disagreement_Sampler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:55:52.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/src/Autora_Experimentalist_Sampler_Model_Disagreement_Sampler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 19:55:52.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/src/Autora_Experimentalist_Sampler_Model_Disagreement_Sampler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 19:55:52.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/src/Autora_Experimentalist_Sampler_Model_Disagreement_Sampler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:55:52.120082 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:55:52.120082 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/src/autora/experimentalist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:55:52.120082 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/src/autora/experimentalist/sampler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:55:52.124082 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/src/autora/experimentalist/sampler/model_disagreement_sampler/
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-17 19:55:40.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/src/autora/experimentalist/sampler/model_disagreement_sampler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:55:52.128082 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-17 19:55:40.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:55:40.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-17 19:55:40.000000 Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/tests/test_model_disagreement_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:54:29.205730 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-24 15:54:15.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:54:29.201730 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:54:29.201730 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-24 15:54:15.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-24 15:54:15.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-24 15:54:15.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-24 15:54:29.205730 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-24 15:54:15.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:54:29.201730 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   141677 2023-05-24 15:54:15.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/docs/basic-usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-24 15:54:15.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:54:29.201730 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-24 15:54:15.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-24 15:54:15.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:54:29.201730 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-24 15:54:15.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-24 15:54:15.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-24 15:54:15.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:54:29.205730 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:54:29.201730 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:54:29.201730 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:54:29.201730 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/src/autora/experimentalist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:54:29.201730 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/src/autora/experimentalist/sampler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:54:29.201730 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/src/autora/experimentalist/sampler/model_disagreement_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-24 15:54:15.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/src/autora/experimentalist/sampler/model_disagreement_sampler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:54:29.205730 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/src/autora_experimentalist_sampler_model_disagreement_sampler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-24 15:54:29.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/src/autora_experimentalist_sampler_model_disagreement_sampler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-24 15:54:29.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/src/autora_experimentalist_sampler_model_disagreement_sampler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:54:29.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/src/autora_experimentalist_sampler_model_disagreement_sampler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-24 15:54:29.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/src/autora_experimentalist_sampler_model_disagreement_sampler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 15:54:29.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/src/autora_experimentalist_sampler_model_disagreement_sampler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:54:29.205730 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-24 15:54:15.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:54:15.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-24 15:54:15.000000 autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/tests/test_model_disagreement_sampler.py
```

### Comparing `Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/.github/workflows/python-publish.yml` & `autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/.gitignore` & `autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/.pre-commit-config.yaml` & `autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/PKG-INFO` & `autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Autora-Experimentalist-Sampler-Model-Disagreement-Sampler
-Version: 1.0.0b0
+Name: autora-experimentalist-sampler-model-disagreement-sampler
+Version: 1.0.0rc0
 Summary: Compares weaknesses in multiple models
 Author-email: "Built by Sebastian Musslick, re-factored by Chad Williams" <sebastian_musslick@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-sampler-model-disagreement-sampler.git
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/README.md` & `autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/docs/basic-usage.ipynb` & `autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/docs/basic-usage.ipynb`

 * *Files identical despite different names*

### Comparing `Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/docs/index.md` & `autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/docs/index.md`

 * *Files identical despite different names*

### Comparing `Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/mkdocs/base.yml` & `autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/pyproject.toml` & `autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 # UPDATE THIS BEFORE PUBLISHING
-name = "Autora-Experimentalist-Sampler-Model-Disagreement-Sampler"
+name = "autora-experimentalist-sampler-model-disagreement-sampler"
 description = "Compares weaknesses in multiple models"
 authors = [{ name = "Built by Sebastian Musslick, re-factored by Chad Williams", email = "sebastian_musslick@brown.edu" }]
 dynamic = ["version"]
 
 readme = "README.md"
 license = { text = "MIT license" }
 requires-python = ">=3.8,<4"
```

### Comparing `Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/src/Autora_Experimentalist_Sampler_Model_Disagreement_Sampler.egg-info/PKG-INFO` & `autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/src/autora_experimentalist_sampler_model_disagreement_sampler.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Autora-Experimentalist-Sampler-Model-Disagreement-Sampler
-Version: 1.0.0b0
+Name: autora-experimentalist-sampler-model-disagreement-sampler
+Version: 1.0.0rc0
 Summary: Compares weaknesses in multiple models
 Author-email: "Built by Sebastian Musslick, re-factored by Chad Williams" <sebastian_musslick@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-sampler-model-disagreement-sampler.git
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/src/Autora_Experimentalist_Sampler_Model_Disagreement_Sampler.egg-info/SOURCES.txt` & `autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/src/autora_experimentalist_sampler_model_disagreement_sampler.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 pyproject.toml
 .github/workflows/python-publish.yml
 docs/basic-usage.ipynb
 docs/index.md
 docs/quickstart.md
 docs/javascripts/mathjax.js
 mkdocs/base.yml
-src/Autora_Experimentalist_Sampler_Model_Disagreement_Sampler.egg-info/PKG-INFO
-src/Autora_Experimentalist_Sampler_Model_Disagreement_Sampler.egg-info/SOURCES.txt
-src/Autora_Experimentalist_Sampler_Model_Disagreement_Sampler.egg-info/dependency_links.txt
-src/Autora_Experimentalist_Sampler_Model_Disagreement_Sampler.egg-info/requires.txt
-src/Autora_Experimentalist_Sampler_Model_Disagreement_Sampler.egg-info/top_level.txt
 src/autora/experimentalist/sampler/model_disagreement_sampler/__init__.py
+src/autora_experimentalist_sampler_model_disagreement_sampler.egg-info/PKG-INFO
+src/autora_experimentalist_sampler_model_disagreement_sampler.egg-info/SOURCES.txt
+src/autora_experimentalist_sampler_model_disagreement_sampler.egg-info/dependency_links.txt
+src/autora_experimentalist_sampler_model_disagreement_sampler.egg-info/requires.txt
+src/autora_experimentalist_sampler_model_disagreement_sampler.egg-info/top_level.txt
 tests/README.md
 tests/__init__.py
 tests/test_model_disagreement_sampler.py
```

### Comparing `Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/src/autora/experimentalist/sampler/model_disagreement_sampler/__init__.py` & `autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/src/autora/experimentalist/sampler/model_disagreement_sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/tests/README.md` & `autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/tests/README.md`

 * *Files identical despite different names*

### Comparing `Autora-Experimentalist-Sampler-Model-Disagreement-Sampler-1.0.0b0/tests/test_model_disagreement_sampler.py` & `autora-experimentalist-sampler-model-disagreement-sampler-1.0.0rc0/tests/test_model_disagreement_sampler.py`

 * *Files identical despite different names*

