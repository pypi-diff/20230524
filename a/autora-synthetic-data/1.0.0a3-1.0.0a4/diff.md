# Comparing `tmp/autora-synthetic-data-1.0.0a3.tar.gz` & `tmp/autora-synthetic-data-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-synthetic-data-1.0.0a3.tar", last modified: Tue May  2 23:09:24 2023, max compression
+gzip compressed data, was "autora-synthetic-data-1.0.0a4.tar", last modified: Tue May 23 22:25:46 2023, max compression
```

## Comparing `autora-synthetic-data-1.0.0a3.tar` & `autora-synthetic-data-1.0.0a4.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:09:24.315550 autora-synthetic-data-1.0.0a3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:09:24.307550 autora-synthetic-data-1.0.0a3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:09:24.311550 autora-synthetic-data-1.0.0a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/.github/workflows/docs-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:09:24.311550 autora-synthetic-data-1.0.0a3/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/.idea/autora-synthetic-data.iml
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-02 23:09:24.315550 autora-synthetic-data-1.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:09:24.311550 autora-synthetic-data-1.0.0a3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   169964 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/docs/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:09:24.311550 autora-synthetic-data-1.0.0a3/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:09:24.311550 autora-synthetic-data-1.0.0a3/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 23:09:24.315550 autora-synthetic-data-1.0.0a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:09:24.307550 autora-synthetic-data-1.0.0a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:09:24.307550 autora-synthetic-data-1.0.0a3/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:09:24.311550 autora-synthetic-data-1.0.0a3/src/autora/synthetic/
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/src/autora/synthetic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:09:24.311550 autora-synthetic-data-1.0.0a3/src/autora/synthetic/_data/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/src/autora/synthetic/_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/src/autora/synthetic/_data/expected_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/src/autora/synthetic/_data/prospect_theory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/src/autora/synthetic/_data/template_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/src/autora/synthetic/_data/weber_fechner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/src/autora/synthetic/_inventory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:09:24.311550 autora-synthetic-data-1.0.0a3/src/autora_synthetic_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-02 23:09:24.000000 autora-synthetic-data-1.0.0a3/src/autora_synthetic_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-02 23:09:24.000000 autora-synthetic-data-1.0.0a3/src/autora_synthetic_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 23:09:24.000000 autora-synthetic-data-1.0.0a3/src/autora_synthetic_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-02 23:09:24.000000 autora-synthetic-data-1.0.0a3/src/autora_synthetic_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 23:09:24.000000 autora-synthetic-data-1.0.0a3/src/autora_synthetic_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:09:24.311550 autora-synthetic-data-1.0.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-02 23:09:12.000000 autora-synthetic-data-1.0.0a3/tests/test_synthetic_inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.577944 autora-synthetic-data-1.0.0a4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.569943 autora-synthetic-data-1.0.0a4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/.idea/autora-synthetic-data.iml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/docs/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 22:25:46.577944 autora-synthetic-data-1.0.0a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.569943 autora-synthetic-data-1.0.0a4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.569943 autora-synthetic-data-1.0.0a4/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/src/autora/synthetic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/src/autora/synthetic/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/src/autora/synthetic/abstract/template_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/src/autora/synthetic/economics/
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/src/autora/synthetic/economics/expected_value_theory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/src/autora/synthetic/economics/prospect_theory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/src/autora/synthetic/psychophysics/
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/src/autora/synthetic/psychophysics/weber_fechner_law.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/src/autora/synthetic/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/src/autora_synthetic_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-23 22:25:46.000000 autora-synthetic-data-1.0.0a4/src/autora_synthetic_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-23 22:25:46.000000 autora-synthetic-data-1.0.0a4/src/autora_synthetic_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 22:25:46.000000 autora-synthetic-data-1.0.0a4/src/autora_synthetic_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-23 22:25:46.000000 autora-synthetic-data-1.0.0a4/src/autora_synthetic_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 22:25:46.000000 autora-synthetic-data-1.0.0a4/src/autora_synthetic_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/tests/test_bundled_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/tests/test_synthetic_inventory.py
```

### Comparing `autora-synthetic-data-1.0.0a3/.github/workflows/python-publish.yml` & `autora-synthetic-data-1.0.0a4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a3/.github/workflows/test-pytest.yml` & `autora-synthetic-data-1.0.0a4/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a3/.gitignore` & `autora-synthetic-data-1.0.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a3/.idea/autora-synthetic-data.iml` & `autora-synthetic-data-1.0.0a4/.idea/autora-synthetic-data.iml`

 * *Files 24% similar despite different names*

#### Comparing `autora-synthetic-data-1.0.0a3/.idea/autora-synthetic-data.iml` & `autora-synthetic-data-1.0.0a4/.idea/autora-synthetic-data.iml`

```diff
@@ -2,15 +2,15 @@
 <module type="PYTHON_MODULE" version="4">
   <component name="NewModuleRootManager">
     <content url="file://$MODULE_DIR$">
       <sourceFolder url="file://$MODULE_DIR$/src" isTestSource="false"/>
       <sourceFolder url="file://$MODULE_DIR$/tests" isTestSource="true"/>
       <excludeFolder url="file://$MODULE_DIR$/venv"/>
     </content>
-    <orderEntry type="inheritedJdk"/>
+    <orderEntry type="jdk" jdkName="Python 3.11 (autora-synthetic-data)" jdkType="Python SDK"/>
     <orderEntry type="sourceFolder" forTests="false"/>
   </component>
   <component name="PyDocumentationSettings">
     <option name="format" value="PLAIN"/>
     <option name="myDocStringFormat" value="Plain"/>
   </component>
   <component name="PyNamespacePackagesService">
```

### Comparing `autora-synthetic-data-1.0.0a3/.pre-commit-config.yaml` & `autora-synthetic-data-1.0.0a4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a3/PKG-INFO` & `autora-synthetic-data-1.0.0a4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: autora-synthetic-data
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: AutoRA Synthetic Data
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-template
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 
-# AutoRA Synthetic Data
+# Synthetic Data
 
 Synthetic experiment data for testing AutoRA theorists and experimentalists. 
 
 ## Quickstart Guide
 
 You will need:
 
 - `python` 3.8 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 
 Install the synthetic data package:
 
 ```shell
-pip install -U "autora-synthetic-data"
+pip install -U "autora[synthetic-data]" --pre
 ```
 
 !!! success
     It is recommended to use a `python` environment manager like `virtualenv`.
 
 Check your installation by running:
 ```shell
```

### Comparing `autora-synthetic-data-1.0.0a3/README.md` & `autora-synthetic-data-1.0.0a4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# AutoRA Synthetic Experiments
+# AutoRA Synthetic Data
 
 A package with synthetic experiment data for testing AutoRA theorists and experimentalists.
 
 ## User Guide
 
 You will need:
 
 - `python` 3.8 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 
 Install the synthetic data package:
 
 ```shell
-pip install -U "autora-synthetic-data"
+pip install -U "autora[synthetic-data]" --pre
 ```
 
 > 💡We recommend using a `python` environment manager like `virtualenv`.
 
 Check your installation by running:
 ```shell
 python -c "from autora.synthetic import retrieve, describe; print(describe(retrieve('weber_fechner')))"
@@ -77,8 +77,8 @@
 ```
 
 New experiments fulfilling these requirements can be submitted as pull requests.
 
 ### Publish the package
 
 This package can be published using GitHub actions – create a new "Release" on the GitHub 
-repository, and Actions will do the rest.
+repository, and Actions will do the rest.
```

### Comparing `autora-synthetic-data-1.0.0a3/mkdocs/base.yml` & `autora-synthetic-data-1.0.0a4/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a3/pyproject.toml` & `autora-synthetic-data-1.0.0a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a3/src/autora/synthetic/_data/expected_value.py` & `autora-synthetic-data-1.0.0a4/src/autora/synthetic/economics/expected_value_theory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from functools import partial
 
 import numpy as np
 
-from autora.synthetic import SyntheticExperimentCollection, register
+from autora.synthetic.utilities import SyntheticExperimentCollection
 from autora.variable import DV, IV, ValueType, VariableCollection
 
 
 def get_variables(minimum_value, maximum_value, resolution):
     v_a = IV(
         name="V_A",
         allowed_values=np.linspace(
@@ -105,15 +105,14 @@
     rng = np.random.default_rng(random_state)
 
     variables = get_variables(
         minimum_value=minimum_value, maximum_value=maximum_value, resolution=resolution
     )
 
     def experiment_runner(X: np.ndarray, added_noise_=added_noise):
-
         Y = np.zeros((X.shape[0], 1))
         for idx, x in enumerate(X):
             value_A = value_lambda * x[0]
             value_B = value_lambda * x[2]
 
             probability_a = x[1]
             probability_b = x[3]
@@ -187,12 +186,10 @@
         name=name,
         variables=variables,
         experiment_runner=experiment_runner,
         ground_truth=ground_truth,
         domain=domain,
         plotter=plotter,
         params=params,
+        closure=expected_value_theory,
     )
     return collection
-
-
-register("expected_value", expected_value_theory)
```

### Comparing `autora-synthetic-data-1.0.0a3/src/autora/synthetic/_data/prospect_theory.py` & `autora-synthetic-data-1.0.0a4/src/autora/synthetic/economics/prospect_theory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from functools import partial
 
 import numpy as np
 
-from autora.synthetic import SyntheticExperimentCollection, register
-
-from .expected_value import get_variables
+from autora.synthetic.economics.expected_value_theory import get_variables
+from autora.synthetic.utilities import SyntheticExperimentCollection
 
 
 def prospect_theory(
     name="Prospect Theory",
     added_noise=0.01,
     choice_temperature=0.1,
     value_alpha=0.88,
@@ -58,18 +57,16 @@
     )
 
     variables = get_variables(
         minimum_value=minimum_value, maximum_value=maximum_value, resolution=resolution
     )
 
     def experiment_runner(X: np.ndarray, added_noise_=added_noise):
-
         Y = np.zeros((X.shape[0], 1))
         for idx, x in enumerate(X):
-
             # power value function according to:
 
             # A. Tversky, D. Kahneman, Advances in prospect theory: Cumulative representation of
             # uncertainty. J. Risk Uncertain. 5, 297–323 (1992). doi:10.1007/BF00122574
 
             # I. Gilboa, Expected utility with purely subjective non-additive probabilities.
             # J. Math. Econ. 16, 65–88 (1987). doi:10.1016/0304-4068(87)90022-X
@@ -187,12 +184,10 @@
         name=name,
         params=params,
         variables=variables,
         domain=domain,
         experiment_runner=experiment_runner,
         ground_truth=ground_truth,
         plotter=plotter,
+        closure=prospect_theory,
     )
     return collection
-
-
-register("prospect_theory", prospect_theory)
```

### Comparing `autora-synthetic-data-1.0.0a3/src/autora/synthetic/_data/template_experiment.py` & `autora-synthetic-data-1.0.0a4/src/autora/synthetic/abstract/template_experiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 A template synthetic experiment.
 
 Examples:
-    >>> from autora.synthetic import retrieve
+    >>> from autora.synthetic.abstract.template_experiment import template_experiment
 
-    We can retrieve the experiment using its name:
-    >>> s = retrieve("template_experiment")  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
-    >>> s
+    We can instantiate the experiment using the imported function
+    >>> s = template_experiment()
+    >>> s  # doctest: +ELLIPSIS
     SyntheticExperimentCollection(name='Template Experiment', params={'name': ...}, ...)
 
     >>> s.name
     'Template Experiment'
 
     >>> s.variables
     VariableCollection(...)
@@ -54,15 +54,15 @@
 
 
 from functools import partial
 
 import numpy as np
 from numpy.typing import ArrayLike
 
-from autora.synthetic import SyntheticExperimentCollection, register
+from autora.synthetic.utilities import SyntheticExperimentCollection
 from autora.variable import DV, IV, VariableCollection
 
 
 def template_experiment(
     # Add any configurable parameters with their defaults here:
     name: str = "Template Experiment",
     added_noise: float = 0.1,
@@ -129,12 +129,10 @@
         name=name,
         variables=variables,
         experiment_runner=experiment_runner,
         ground_truth=ground_truth,
         domain=domain,
         plotter=plotter,
         params=params,
+        closure=template_experiment,
     )
     return collection
-
-
-register("template_experiment", template_experiment)
```

### Comparing `autora-synthetic-data-1.0.0a3/src/autora/synthetic/_data/weber_fechner.py` & `autora-synthetic-data-1.0.0a4/src/autora/synthetic/psychophysics/weber_fechner_law.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 from functools import partial
+from typing import Optional
 
 import numpy as np
 
-from autora.synthetic import SyntheticExperimentCollection, register
+from autora.synthetic.utilities import SyntheticExperimentCollection
 from autora.variable import DV, IV, ValueType, VariableCollection
 
 
 def weber_fechner_law(
     name="Weber-Fechner Law",
     resolution=100,
     constant=1.0,
     maximum_stimulus_intensity=5.0,
     added_noise=0.01,
-    rng=np.random.default_rng(),
+    random_state: Optional[int] = None,
 ):
     """
     Weber-Fechner Law
 
     Args:
         name: name of the experiment
         resolution: number of allowed values for stimulus 1 and 2
         constant: constant multiplier
         maximum_stimulus_intensity: maximum value for stimulus 1 and 2
         added_noise: standard deviation of normally distributed noise added to y-values
-        rng: `np.random` random number generator to use for generating noise
+        random_state: integer used to seed the random number generator
 
     """
 
     params = dict(
         added_noise=added_noise,
         name=name,
         resolution=resolution,
         constant=constant,
         maximum_stimulus_intensity=maximum_stimulus_intensity,
-        rng=rng,
+        random_state=random_state,
     )
 
     iv1 = IV(
         name="S1",
         allowed_values=np.linspace(
             1 / resolution, maximum_stimulus_intensity, resolution
         ),
@@ -67,14 +68,16 @@
     )
 
     variables = VariableCollection(
         independent_variables=[iv1, iv2],
         dependent_variables=[dv1],
     )
 
+    rng = np.random.default_rng(random_state)
+
     def experiment_runner(
         X: np.ndarray,
         std: float = 0.01,
     ):
         Y = np.zeros((X.shape[0], 1))
         for idx, x in enumerate(X):
             # jnd =  np.min(x) * weber_constant
@@ -144,15 +147,10 @@
         name=name,
         variables=variables,
         experiment_runner=experiment_runner,
         ground_truth=ground_truth,
         domain=domain,
         plotter=plotter,
         params=params,
+        closure=weber_fechner_law,
     )
     return collection
-
-
-register(
-    "weber-fechner", weber_fechner_law
-)  # todo: make a better interface for multiple aliases
-register("weber_fechner", weber_fechner_law)
```

### Comparing `autora-synthetic-data-1.0.0a3/src/autora/synthetic/_inventory.py` & `autora-synthetic-data-1.0.0a4/src/autora/synthetic/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 Examples:
     To add and recover a new model from the inventory, we need to define it using a function
     (closure).
     We start by importing the modules we'll need:
     >>> from functools import partial
     >>> import matplotlib.pyplot as plt
     >>> import numpy as np
-    >>> from autora.synthetic import register, retrieve, describe, SyntheticExperimentCollection
+    >>> from autora.synthetic.utilities import (register, retrieve, describe,
+    ...     SyntheticExperimentCollection)
     >>> from autora.variable import IV, DV, VariableCollection
 
     Then we can define the function. We define all the arguments we want and add them to a
     dictionary. The closure – in this case `sinusoid_experiment` – is the scope for all
     the parameters we need.
     >>> def sinusoid_experiment(omega=np.pi/3, delta=np.pi/2., m=0.3, resolution=1000,
     ...                         rng=np.random.default_rng()):
```

### Comparing `autora-synthetic-data-1.0.0a3/src/autora_synthetic_data.egg-info/PKG-INFO` & `autora-synthetic-data-1.0.0a4/src/autora_synthetic_data.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: autora-synthetic-data
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: AutoRA Synthetic Data
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-template
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 
-# AutoRA Synthetic Data
+# Synthetic Data
 
 Synthetic experiment data for testing AutoRA theorists and experimentalists. 
 
 ## Quickstart Guide
 
 You will need:
 
 - `python` 3.8 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 
 Install the synthetic data package:
 
 ```shell
-pip install -U "autora-synthetic-data"
+pip install -U "autora[synthetic-data]" --pre
 ```
 
 !!! success
     It is recommended to use a `python` environment manager like `virtualenv`.
 
 Check your installation by running:
 ```shell
```

### Comparing `autora-synthetic-data-1.0.0a3/tests/test_synthetic_inventory.py` & `autora-synthetic-data-1.0.0a4/tests/test_bundled_models.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,50 @@
-from hypothesis import assume, given
+from hypothesis import given
 from hypothesis import strategies as st
 
-from autora.synthetic import (
-    Inventory,
-    SyntheticExperimentCollection,
-    describe,
-    register,
-    retrieve,
-)
-
-all_bundled_model_names = [
-    "expected_value",
-    "prospect_theory",
-    "template_experiment",
-    "weber_fechner",
+from autora.synthetic.abstract.template_experiment import template_experiment
+from autora.synthetic.economics.expected_value_theory import expected_value_theory
+from autora.synthetic.economics.prospect_theory import prospect_theory
+from autora.synthetic.psychophysics.weber_fechner_law import weber_fechner_law
+from autora.synthetic.utilities import describe, register, retrieve
+
+all_bundled_models = [
+    ("expected_value_theory", expected_value_theory),
+    ("prospect_theory", prospect_theory),
+    ("template_experiment", template_experiment),
+    ("weber_fechner_law", weber_fechner_law),
 ]
 
+all_bundled_model_names = [b[0] for b in all_bundled_models]
 
-@given(st.text())
-def test_model_registration_retrieval_allows_any_string(name):
-    model = SyntheticExperimentCollection()
-    register(name, lambda: model)
+for name, func in all_bundled_models:
+    register(name, func)
 
-    retrieved = retrieve(name)
 
-    assert retrieved is model
-
-
-@given(st.text(), st.text())
-def test_model_registration_retrieval_dont_collide_with_two_models(name1, name2):
-    # We can register a model and retrieve it
-    assume(name1 != name2)
-
-    model1 = SyntheticExperimentCollection()
-    model2 = SyntheticExperimentCollection()
-    register(name1, lambda: model1)
-    retrieved1 = retrieve(name1)
-    assert retrieved1 is model1
-
-    # We can register another model and retrieve it as well
-    register(name2, lambda: model2)
-    retrieved2 = retrieve(name2)
-    assert retrieved2 is model2
-
-    # We can still retrieve the first model, and it is equal to the first version
-    retrieved3 = retrieve(name1)
-    assert retrieved3 is model1
-
-
-@given(st.sampled_from(all_bundled_model_names))
+@given(name=st.sampled_from(all_bundled_model_names))
 def test_bundled_models_can_be_retrieved_by_name(name):
     model = retrieve(name)
     assert model is not None
 
 
-@given(st.sampled_from(all_bundled_model_names))
+@given(name=st.sampled_from(all_bundled_model_names))
 def test_bundled_models_can_be_described_by_name(name):
     description = describe(name)
     assert isinstance(description, str)
 
 
-@given(st.sampled_from(all_bundled_model_names))
+@given(name=st.sampled_from(all_bundled_model_names))
 def test_bundled_models_can_be_described_by_model(name):
     model = retrieve(name)
     description = describe(model)
     assert isinstance(description, str)
 
 
-@given(st.sampled_from(all_bundled_model_names))
+@given(name=st.sampled_from(all_bundled_model_names))
 def test_model_descriptions_from_name_model_closure_are_the_same(name):
     description_from_name = describe(name)
     description_from_model = describe(retrieve(name))
-    closure = Inventory[name]
-    description_from_closure = describe(closure)
+    description_from_closure = describe(retrieve(name).closure)
 
     assert description_from_name == description_from_model
     assert description_from_model == description_from_closure
     assert description_from_closure == description_from_name
```

