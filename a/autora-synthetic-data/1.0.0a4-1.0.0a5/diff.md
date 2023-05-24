# Comparing `tmp/autora-synthetic-data-1.0.0a4.tar.gz` & `tmp/autora-synthetic-data-1.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-synthetic-data-1.0.0a4.tar", last modified: Tue May 23 22:25:46 2023, max compression
+gzip compressed data, was "autora-synthetic-data-1.0.0a5.tar", last modified: Wed May 24 14:29:06 2023, max compression
```

## Comparing `autora-synthetic-data-1.0.0a4.tar` & `autora-synthetic-data-1.0.0a5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.577944 autora-synthetic-data-1.0.0a4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.569943 autora-synthetic-data-1.0.0a4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/.github/workflows/docs-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/.idea/autora-synthetic-data.iml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/docs/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 22:25:46.577944 autora-synthetic-data-1.0.0a4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.569943 autora-synthetic-data-1.0.0a4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.569943 autora-synthetic-data-1.0.0a4/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/src/autora/synthetic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/src/autora/synthetic/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/src/autora/synthetic/abstract/template_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/src/autora/synthetic/economics/
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/src/autora/synthetic/economics/expected_value_theory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/src/autora/synthetic/economics/prospect_theory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/src/autora/synthetic/psychophysics/
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/src/autora/synthetic/psychophysics/weber_fechner_law.py
--rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/src/autora/synthetic/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/src/autora_synthetic_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-23 22:25:46.000000 autora-synthetic-data-1.0.0a4/src/autora_synthetic_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-23 22:25:46.000000 autora-synthetic-data-1.0.0a4/src/autora_synthetic_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 22:25:46.000000 autora-synthetic-data-1.0.0a4/src/autora_synthetic_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-23 22:25:46.000000 autora-synthetic-data-1.0.0a4/src/autora_synthetic_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 22:25:46.000000 autora-synthetic-data-1.0.0a4/src/autora_synthetic_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:25:46.573943 autora-synthetic-data-1.0.0a4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/tests/test_bundled_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-23 22:25:33.000000 autora-synthetic-data-1.0.0a4/tests/test_synthetic_inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:29:06.661405 autora-synthetic-data-1.0.0a5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:29:06.653405 autora-synthetic-data-1.0.0a5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:29:06.657405 autora-synthetic-data-1.0.0a5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:29:06.657405 autora-synthetic-data-1.0.0a5/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/.idea/autora-synthetic-data.iml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-24 14:29:06.661405 autora-synthetic-data-1.0.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:29:06.661405 autora-synthetic-data-1.0.0a5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   171006 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/docs/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:29:06.661405 autora-synthetic-data-1.0.0a5/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:29:06.661405 autora-synthetic-data-1.0.0a5/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 14:29:06.661405 autora-synthetic-data-1.0.0a5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:29:06.657405 autora-synthetic-data-1.0.0a5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:29:06.653405 autora-synthetic-data-1.0.0a5/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:29:06.661405 autora-synthetic-data-1.0.0a5/src/autora/synthetic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:29:06.661405 autora-synthetic-data-1.0.0a5/src/autora/synthetic/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/src/autora/synthetic/abstract/template_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:29:06.661405 autora-synthetic-data-1.0.0a5/src/autora/synthetic/economics/
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/src/autora/synthetic/economics/expected_value_theory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/src/autora/synthetic/economics/prospect_theory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:29:06.661405 autora-synthetic-data-1.0.0a5/src/autora/synthetic/psychophysics/
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/src/autora/synthetic/psychophysics/weber_fechner_law.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/src/autora/synthetic/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:29:06.661405 autora-synthetic-data-1.0.0a5/src/autora_synthetic_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-24 14:29:06.000000 autora-synthetic-data-1.0.0a5/src/autora_synthetic_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-24 14:29:06.000000 autora-synthetic-data-1.0.0a5/src/autora_synthetic_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:29:06.000000 autora-synthetic-data-1.0.0a5/src/autora_synthetic_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-24 14:29:06.000000 autora-synthetic-data-1.0.0a5/src/autora_synthetic_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 14:29:06.000000 autora-synthetic-data-1.0.0a5/src/autora_synthetic_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:29:06.661405 autora-synthetic-data-1.0.0a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/tests/test_bundled_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-24 14:28:50.000000 autora-synthetic-data-1.0.0a5/tests/test_synthetic_inventory.py
```

### Comparing `autora-synthetic-data-1.0.0a4/.github/workflows/python-publish.yml` & `autora-synthetic-data-1.0.0a5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a4/.github/workflows/test-pytest.yml` & `autora-synthetic-data-1.0.0a5/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a4/.gitignore` & `autora-synthetic-data-1.0.0a5/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a4/.idea/autora-synthetic-data.iml` & `autora-synthetic-data-1.0.0a5/.idea/autora-synthetic-data.iml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a4/PKG-INFO` & `autora-synthetic-data-1.0.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-synthetic-data
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: AutoRA Synthetic Data
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-template
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `autora-synthetic-data-1.0.0a4/README.md` & `autora-synthetic-data-1.0.0a5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 ```shell
 pip install -U "autora[synthetic-data]" --pre
 ```
 
 > 💡We recommend using a `python` environment manager like `virtualenv`.
 
-Check your installation by running:
+Print a description of the prospect theory model by Kahneman and Tversky by running:
 ```shell
-python -c "from autora.synthetic import retrieve, describe; print(describe(retrieve('weber_fechner')))"
+python -c "from autora.synthetic.economics.prospect_theory import prospect_theory; print(prospect_theory().description)"
 ```
 
 ## Developer Guide
 
 ### Get started
 
 Clone the repository (e.g. using [GitHub desktop](https://desktop.github.com), 
@@ -57,28 +57,17 @@
 ```
 
 ### Add a new dataset
 
 New datasets should match existing examples in [`src/autora/synthetic/`](src/autora/synthetic/). 
 > 💡A good starting point might be to duplicate an existing example.
 
-Each experiment is described in a single file which includes: 
-- A "factory function" which constructs the experiment and optionally takes parameters to tune
-  aspects of the experiment. This function's docstring serves as the main documentation of the 
-  experiment.
-- A call to `autora.synthetic.register` to register the factory function under a unique name.
-
-The file should be imported in 
-  [`src/autora/synthetic/_data/__init__.py`](src/autora/synthetic/_data/__init__.py).
-
-If these requirements are met, you should be able to display the docstring of the experiment 
-using the `autora.synthetic.retrieve` function like this:
-```shell
-python -c "from autora.synthetic import retrieve, describe; describe(retrieve('new_experiment_name'))"
-```
+Each experiment is described in a single file which includes a "factory function" which:
+- constructs the experiment, and 
+- optionally takes parameters to tune aspects of the experiment.  
 
 New experiments fulfilling these requirements can be submitted as pull requests.
 
 ### Publish the package
 
-This package can be published using GitHub actions – create a new "Release" on the GitHub 
+This package is published using GitHub actions – create a new "Release" on the GitHub 
 repository, and Actions will do the rest.
```

### Comparing `autora-synthetic-data-1.0.0a4/docs/index.md` & `autora-synthetic-data-1.0.0a5/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a4/mkdocs/base.yml` & `autora-synthetic-data-1.0.0a5/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a4/pyproject.toml` & `autora-synthetic-data-1.0.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a4/src/autora/synthetic/abstract/template_experiment.py` & `autora-synthetic-data-1.0.0a5/src/autora/synthetic/abstract/template_experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 A template synthetic experiment.
 
 Examples:
     >>> from autora.synthetic.abstract.template_experiment import template_experiment
 
     We can instantiate the experiment using the imported function
     >>> s = template_experiment()
-    >>> s  # doctest: +ELLIPSIS
-    SyntheticExperimentCollection(name='Template Experiment', params={'name': ...}, ...)
+    >>> s  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
+    SyntheticExperimentCollection(name='Template Experiment', description='...',
+        params={'name': ...}, ...)
 
     >>> s.name
     'Template Experiment'
 
     >>> s.variables
     VariableCollection(...)
 
@@ -46,14 +47,19 @@
            [1.96837574],
            [2.99831988],
            [3.91469561]])
 
     >>> s.plotter()
     >>> plt.show()  # doctest: +SKIP
 
+    Generate a new version of the experiment with different parameters:
+    >>> new_params = dict(s.params, **dict(random_state=190))
+    >>> s.factory_function(**new_params)  # doctest: +ELLIPSIS
+    SyntheticExperimentCollection(..., params={..., 'random_state': 190}, ...)
+
 """
 
 
 from functools import partial
 
 import numpy as np
 from numpy.typing import ArrayLike
@@ -123,16 +129,17 @@
         plt.ylabel(variables.dependent_variables[0].name)
         plt.legend()
         plt.title(name)
 
     # The object which gets stored in the synthetic inventory
     collection = SyntheticExperimentCollection(
         name=name,
+        description=template_experiment.__doc__,
         variables=variables,
         experiment_runner=experiment_runner,
         ground_truth=ground_truth,
         domain=domain,
         plotter=plotter,
         params=params,
-        closure=template_experiment,
+        factory_function=template_experiment,
     )
     return collection
```

### Comparing `autora-synthetic-data-1.0.0a4/src/autora/synthetic/economics/expected_value_theory.py` & `autora-synthetic-data-1.0.0a5/src/autora/synthetic/economics/expected_value_theory.py`

 * *Files 6% similar despite different names*

```diff
@@ -180,16 +180,17 @@
         plt.xlabel(x_label, fontsize="large")
         plt.ylabel(y_label, fontsize="large")
         plt.legend(loc=2, fontsize="medium")
         plt.title(name, fontsize="x-large")
 
     collection = SyntheticExperimentCollection(
         name=name,
+        description=expected_value_theory.__doc__,
         variables=variables,
         experiment_runner=experiment_runner,
         ground_truth=ground_truth,
         domain=domain,
         plotter=plotter,
         params=params,
-        closure=expected_value_theory,
+        factory_function=expected_value_theory,
     )
     return collection
```

### Comparing `autora-synthetic-data-1.0.0a4/src/autora/synthetic/economics/prospect_theory.py` & `autora-synthetic-data-1.0.0a5/src/autora/synthetic/economics/prospect_theory.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,16 +178,17 @@
         plt.xlabel(x_label, fontsize="large")
         plt.ylabel(y_label, fontsize="large")
         plt.legend(loc=2, fontsize="medium")
         plt.title(name, fontsize="x-large")
 
     collection = SyntheticExperimentCollection(
         name=name,
+        description=prospect_theory.__doc__,
         params=params,
         variables=variables,
         domain=domain,
         experiment_runner=experiment_runner,
         ground_truth=ground_truth,
         plotter=plotter,
-        closure=prospect_theory,
+        factory_function=prospect_theory,
     )
     return collection
```

### Comparing `autora-synthetic-data-1.0.0a4/src/autora/synthetic/psychophysics/weber_fechner_law.py` & `autora-synthetic-data-1.0.0a5/src/autora/synthetic/psychophysics/weber_fechner_law.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,16 +141,17 @@
         plt.xlabel(x_label, fontsize="large")
         plt.ylabel(y_label, fontsize="large")
         plt.legend(loc=2, fontsize="medium")
         plt.title("Weber-Fechner Law", fontsize="x-large")
 
     collection = SyntheticExperimentCollection(
         name=name,
+        description=weber_fechner_law.__doc__,
         variables=variables,
         experiment_runner=experiment_runner,
         ground_truth=ground_truth,
         domain=domain,
         plotter=plotter,
         params=params,
-        closure=weber_fechner_law,
+        factory_function=weber_fechner_law,
     )
     return collection
```

### Comparing `autora-synthetic-data-1.0.0a4/src/autora/synthetic/utilities.py` & `autora-synthetic-data-1.0.0a5/src/autora/synthetic/utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 Module for registering and retrieving synthetic models from an inventory.
 
 Examples:
-    To add and recover a new model from the inventory, we need to define it using a function
-    (closure).
+    To add and recover a new model from the inventory, we need to define it using a factory
+    function.
     We start by importing the modules we'll need:
     >>> from functools import partial
     >>> import matplotlib.pyplot as plt
     >>> import numpy as np
     >>> from autora.synthetic.utilities import (register, retrieve, describe,
     ...     SyntheticExperimentCollection)
     >>> from autora.variable import IV, DV, VariableCollection
 
     Then we can define the function. We define all the arguments we want and add them to a
-    dictionary. The closure – in this case `sinusoid_experiment` – is the scope for all
+    dictionary. The factory_function – in this case `sinusoid_experiment` – is the scope for all
     the parameters we need.
     >>> def sinusoid_experiment(omega=np.pi/3, delta=np.pi/2., m=0.3, resolution=1000,
     ...                         rng=np.random.default_rng()):
     ...     \"\"\"Shifted sinusoid experiment, combining a sinusoid and a gradient drift.
     ...     Ground truth: y = sin((x - delta) * omega) + (x * m)
     ...     Parameters:
     ...         omega: angular speed in radians
@@ -47,20 +47,22 @@
     ...         plt.plot(domain(), ground_truth(domain()), label="Ground Truth")
     ...         if model is not None:
     ...             plt.plot(domain(), model.predict(domain()), label="Model")
     ...         plt.title(name)
     ...
     ...     collection = SyntheticExperimentCollection(
     ...         name=name,
+    ...         description=sinusoid_experiment.__doc__,
     ...         params=params,
     ...         variables=variables,
     ...         domain=domain,
     ...         experiment_runner=experiment_runner,
     ...         ground_truth=ground_truth,
     ...         plotter=plotter,
+    ...         factory_function=sinusoid_experiment,
     ...     )
     ...
     ...     return collection
 
     Then we can register the experiment. We register the function, rather than evaluating it.
     >>> register("sinusoid_experiment", sinusoid_experiment)
 
@@ -75,15 +77,15 @@
 
     ... or using its id:
     >>> print(describe("sinusoid_experiment"))  # doctest: +ELLIPSIS
     Shifted sinusoid experiment, combining a sinusoid and a gradient drift.
         Ground truth: y = sin((x - delta) * omega) + (x * m)
         ...
 
-    ... or we can look at the closure function directly:
+    ... or we can look at the factory function directly:
     >>> print(describe(sinusoid_experiment)) # doctest: +ELLIPSIS
     Shifted sinusoid experiment, combining a sinusoid and a gradient drift.
         Ground truth: y = sin((x - delta) * omega) + (x * m)
         ...
 
     The object returned includes all the used parameters as a dictionary
     >>> s.params  # doctest: +ELLIPSIS
@@ -95,35 +97,28 @@
     >>> t.params  # doctest: +ELLIPSIS
     {..., 'delta': 0.2, ...}
 """
 
 
 from __future__ import annotations
 
+from collections import abc
 from dataclasses import dataclass
 from functools import singledispatch
-from typing import Any, Callable, Dict, Optional, Protocol, runtime_checkable
+from typing import Any, Callable, Dict, Optional, Protocol
 
 from autora.variable import VariableCollection
 
 
-@runtime_checkable
-class _SyntheticExperimentClosure(Protocol):
-    """A function which returns a SyntheticExperimentCollection."""
-
-    def __call__(self, *args, **kwargs) -> SyntheticExperimentCollection:
-        ...
-
-
 class _SupportsPredict(Protocol):
     def predict(self, X) -> Any:
         ...
 
 
-@dataclass
+@dataclass(frozen=True)
 class SyntheticExperimentCollection:
     """
     Represents a synthetic experiment.
 
     Attributes:
         name: the name of the theory
         params: a dictionary with the settable parameters of the model and their respective values
@@ -134,73 +129,74 @@
         ground_truth: a function which takes X values and returns simulated y values **without any
             statistical noise**
         plotter: a function which plots the ground truth and, optionally, a model with a
             `predict` method (e.g. scikit-learn estimators)
     """
 
     name: Optional[str] = None
+    description: Optional[str] = None
     params: Optional[Dict] = None
     variables: Optional[VariableCollection] = None
     domain: Optional[Callable] = None
     experiment_runner: Optional[Callable] = None
     ground_truth: Optional[Callable] = None
     plotter: Optional[Callable[[Optional[_SupportsPredict]], None]] = None
-    closure: Optional[Callable] = None
+    factory_function: Optional[_SyntheticExperimentFactory] = None
+
 
+_SyntheticExperimentFactory = Callable[..., SyntheticExperimentCollection]
 
-Inventory: Dict[str, _SyntheticExperimentClosure] = dict()
+Inventory: Dict[str, _SyntheticExperimentFactory] = dict()
 """ The dictionary of `SyntheticExperimentCollection`. """
 
 
-def register(id_: str, closure: _SyntheticExperimentClosure) -> None:
+def register(id_: str, factory_function: _SyntheticExperimentFactory) -> None:
     """
     Add a new synthetic experiment to the Inventory.
 
     Parameters:
          id_: the unique id for the model.
-         closure: a function which returns a SyntheticExperimentCollection
+         factory_function: a function which returns a SyntheticExperimentCollection
 
     """
-    Inventory[id_] = closure
+    Inventory[id_] = factory_function
 
 
 def retrieve(id_: str, **kwargs) -> SyntheticExperimentCollection:
     """
     Retrieve a synthetic experiment from the Inventory.
 
     Parameters:
         id_: the unique id for the model
         **kwargs: keyword arguments for the synthetic experiment (variables, coefficients etc.)
     Returns:
         the synthetic experiment
     """
-    closure: _SyntheticExperimentClosure = Inventory[id_]
-    evaluated_closure = closure(**kwargs)
-    evaluated_closure.closure = closure
-    return evaluated_closure
+    result = Inventory[id_](**kwargs)
+    return result
 
 
 @singledispatch
 def describe(arg):
     """
     Print the docstring for a synthetic experiment.
 
     Args:
-        arg: the experiment's ID, an object returned from the `retrieve` function, or a closure
-            which creates a new experiment.
+        arg: the experiment's ID, an object returned from the `retrieve` function,
+            or a factory_function which creates a new experiment.
     """
     raise NotImplementedError(f"{arg=} not yet supported")
 
 
 @describe.register
-def _(closure: _SyntheticExperimentClosure):
-    return closure.__doc__
+def _(func: abc.Callable):
+    return func.__doc__
 
 
 @describe.register
 def _(collection: SyntheticExperimentCollection):
-    return describe(collection.closure)
+    return collection.description
 
 
 @describe.register
 def _(id_: str):
     return describe(retrieve(id_))
```

### Comparing `autora-synthetic-data-1.0.0a4/src/autora_synthetic_data.egg-info/PKG-INFO` & `autora-synthetic-data-1.0.0a5/src/autora_synthetic_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-synthetic-data
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: AutoRA Synthetic Data
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-template
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `autora-synthetic-data-1.0.0a4/src/autora_synthetic_data.egg-info/SOURCES.txt` & `autora-synthetic-data-1.0.0a5/src/autora_synthetic_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-synthetic-data-1.0.0a4/tests/test_bundled_models.py` & `autora-synthetic-data-1.0.0a5/tests/test_bundled_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,12 +39,12 @@
     assert isinstance(description, str)
 
 
 @given(name=st.sampled_from(all_bundled_model_names))
 def test_model_descriptions_from_name_model_closure_are_the_same(name):
     description_from_name = describe(name)
     description_from_model = describe(retrieve(name))
-    description_from_closure = describe(retrieve(name).closure)
+    description_from_closure = describe(retrieve(name).factory_function)
 
     assert description_from_name == description_from_model
     assert description_from_model == description_from_closure
     assert description_from_closure == description_from_name
```

### Comparing `autora-synthetic-data-1.0.0a4/tests/test_synthetic_inventory.py` & `autora-synthetic-data-1.0.0a5/tests/test_synthetic_inventory.py`

 * *Files identical despite different names*

