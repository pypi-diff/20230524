# Comparing `tmp/formulae-0.3.4.tar.gz` & `tmp/formulae-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/formulae-0.3.4.tar", last modified: Wed May 18 16:41:06 2022, max compression
+gzip compressed data, was "formulae-0.4.0.tar", last modified: Wed May 24 12:35:56 2023, max compression
```

## Comparing `formulae-0.3.4.tar` & `formulae-0.4.0.tar`

### file list

```diff
@@ -1,57 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 16:41:06.000000 formulae-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-05-18 16:40:58.000000 formulae-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2676 2022-05-18 16:41:06.000000 formulae-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2022-05-18 16:40:58.000000 formulae-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 16:41:06.000000 formulae-0.3.4/formulae/
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7601 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/categorical.py
--rw-r--r--   0 runner    (1001) docker     (121)     5608 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/contrasts.py
--rw-r--r--   0 runner    (1001) docker     (121)     2447 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 16:41:06.000000 formulae-0.3.4/formulae/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     8159 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/examples/Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    27959 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/examples/Features.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     5271 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/expr.py
--rw-r--r--   0 runner    (1001) docker     (121)    19524 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/matrices.py
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/model_description.py
--rw-r--r--   0 runner    (1001) docker     (121)     6723 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     3001 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)     6514 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 16:41:06.000000 formulae-0.3.4/formulae/terms/
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/terms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14091 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/terms/call.py
--rw-r--r--   0 runner    (1001) docker     (121)    10078 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/terms/call_resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/terms/call_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    47711 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/terms/terms.py
--rw-r--r--   0 runner    (1001) docker     (121)     8816 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/terms/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 16:41:06.000000 formulae-0.3.4/formulae/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 16:41:06.000000 formulae-0.3.4/formulae/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/tests/data/Pixel.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 16:41:06.000000 formulae-0.3.4/formulae/tests/data/group_specific/
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/tests/data/group_specific/dog_and_side_by_day.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/tests/data/group_specific/intercept_by_side.txt
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/tests/data/group_specific/intercept_by_side_dog.txt
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/tests/data/group_specific/slope_by_dog.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1021 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/tests/data/new.csv
--rw-r--r--   0 runner    (1001) docker     (121)     1978 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/tests/data/original.csv
--rw-r--r--   0 runner    (1001) docker     (121)    44535 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/tests/test_design_matrices.py
--rw-r--r--   0 runner    (1001) docker     (121)     2147 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/tests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)    10554 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/tests/test_eval_new_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     7459 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4746 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/tests/test_poly.py
--rw-r--r--   0 runner    (1001) docker     (121)     9108 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/tests/test_resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)     7675 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/tests/test_scanner.py
--rw-r--r--   0 runner    (1001) docker     (121)     7753 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/tests/test_spline.py
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/tests/test_terms_call.py
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/tests/test_terms_variable.py
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      899 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/token.py
--rw-r--r--   0 runner    (1001) docker     (121)    13024 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)      877 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-18 16:40:58.000000 formulae-0.3.4/formulae/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 16:41:06.000000 formulae-0.3.4/formulae.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-05-18 16:41:06.000000 formulae-0.3.4/formulae.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-05-18 16:40:58.000000 formulae-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-05-18 16:40:58.000000 formulae-0.3.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-05-18 16:40:58.000000 formulae-0.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-18 16:41:06.000000 formulae-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1227 2022-05-18 16:40:58.000000 formulae-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:35:56.183400 formulae-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-24 12:35:45.000000 formulae-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-24 12:35:56.183400 formulae-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-24 12:35:45.000000 formulae-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:35:56.179400 formulae-0.4.0/formulae/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/contrasts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19524 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/model_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:35:56.183400 formulae-0.4.0/formulae/terms/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/terms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/terms/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/terms/call_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/terms/call_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47711 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/terms/terms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/terms/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 12:35:45.000000 formulae-0.4.0/formulae/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:35:56.183400 formulae-0.4.0/formulae.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-24 12:35:56.000000 formulae-0.4.0/formulae.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-24 12:35:56.000000 formulae-0.4.0/formulae.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:35:56.000000 formulae-0.4.0/formulae.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-24 12:35:56.000000 formulae-0.4.0/formulae.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 12:35:56.000000 formulae-0.4.0/formulae.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-24 12:35:45.000000 formulae-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 12:35:56.183400 formulae-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:35:56.183400 formulae-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    45916 2023-05-24 12:35:45.000000 formulae-0.4.0/tests/test_design_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-24 12:35:45.000000 formulae-0.4.0/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-05-24 12:35:45.000000 formulae-0.4.0/tests/test_eval_new_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-05-24 12:35:45.000000 formulae-0.4.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-24 12:35:45.000000 formulae-0.4.0/tests/test_poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-24 12:35:45.000000 formulae-0.4.0/tests/test_register_stateful_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9108 2023-05-24 12:35:45.000000 formulae-0.4.0/tests/test_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-24 12:35:45.000000 formulae-0.4.0/tests/test_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-05-24 12:35:45.000000 formulae-0.4.0/tests/test_spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-24 12:35:45.000000 formulae-0.4.0/tests/test_terms_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-24 12:35:45.000000 formulae-0.4.0/tests/test_terms_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-24 12:35:45.000000 formulae-0.4.0/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `formulae-0.3.4/PKG-INFO` & `formulae-0.4.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,32 @@
-Metadata-Version: 2.1
-Name: formulae
-Version: 0.3.4
-Summary: Formulas for mixed-effects models in Python
-Home-page: https://github.com/bambinos/formulae
-Maintainer: Tomás Capretto
-Maintainer-email: tomicapretto@gmail.com
-License: MIT
-Description: <img src="docs/logo/formulae_large.png" width=250></img>
-        
-        [![PyPI version](https://badge.fury.io/py/formulae.svg)](https://badge.fury.io/py/formulae)
-        [![codecov](https://codecov.io/gh/bambinos/formulae/branch/master/graph/badge.svg)](https://codecov.io/gh/bambinos/formulae)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
-        
-        # formulae
-        
-        formulae is a Python library that implements Wilkinson's formulas for mixed-effects models. The main difference with other implementations like [Patsy](https://github.com/pydata/patsy) or [formulaic](https://github.com/matthewwardrop/formulaic) is that formulae can work with formulas describing a model with both common and group specific effects (a.k.a. fixed and random effects, respectively).
-        
-        This package has been written to make it easier to specify models with group effects in [Bambi](https://github.com/bambinos/bambi), a package that makes it easy to work with Bayesian GLMMs in Python, but it could be used independently as a backend for another library. The approach in this library is to extend classical statistical formulas in a similar way than in R package [lme4](https://CRAN.R-project.org/package=lme4).
-        
-        ## Installation
-        
-        formulae requires a working Python interpreter (3.7+) and the libraries numpy, scipy and pandas with versions specified in the [requirements.txt](https://github.com/bambinos/formulae/blob/master/requirements.txt) file.
-        
-        Assuming a standard Python environment is installed on your machine (including pip), the latest release of formulae can be installed in one line using pip:
-        
-        `pip install formulae`
-        
-        Alternatively, if you want the development version of the package you can install from GitHub:
-        
-        `pip install git+https://github.com/bambinos/formulae.git`
-        
-        ## Documentation
-        
-        The official documentation can be found [here](https://bambinos.github.io/formulae)
-        
-        ## Notes
-        
-        - The `data` argument only accepts objects of class `pandas.DataFrame`.
-        - `y ~ .` is not implemented and won't be implemented in a first version. However, it is planned to be included in the future.
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+<img src="docs/logo/formulae_large.png" width=250></img>
+
+[![PyPI version](https://badge.fury.io/py/formulae.svg)](https://badge.fury.io/py/formulae)
+[![codecov](https://codecov.io/gh/bambinos/formulae/branch/master/graph/badge.svg)](https://codecov.io/gh/bambinos/formulae)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+
+# formulae
+
+formulae is a Python library that implements Wilkinson's formulas for mixed-effects models. The main difference with other implementations like [Patsy](https://github.com/pydata/patsy) or [formulaic](https://github.com/matthewwardrop/formulaic) is that formulae can work with formulas describing a model with both common and group specific effects (a.k.a. fixed and random effects, respectively).
+
+This package has been written to make it easier to specify models with group effects in [Bambi](https://github.com/bambinos/bambi), a package that makes it easy to work with Bayesian GLMMs in Python, but it could be used independently as a backend for another library. The approach in this library is to extend classical statistical formulas in a similar way than in R package [lme4](https://CRAN.R-project.org/package=lme4).
+
+## Installation
+
+formulae requires a working Python interpreter (3.7+) and the libraries numpy, scipy and pandas with versions specified in the [requirements.txt](https://github.com/bambinos/formulae/blob/master/requirements.txt) file.
+
+Assuming a standard Python environment is installed on your machine (including pip), the latest release of formulae can be installed in one line using pip:
+
+`pip install formulae`
+
+Alternatively, if you want the development version of the package you can install from GitHub:
+
+`pip install git+https://github.com/bambinos/formulae.git`
+
+## Documentation
+
+The official documentation can be found [here](https://bambinos.github.io/formulae)
+
+## Notes
+
+- The `data` argument only accepts objects of class `pandas.DataFrame`.
+- `y ~ .` is not implemented and won't be implemented in a first version. However, it is planned to be included in the future.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `formulae-0.3.4/formulae/categorical.py` & `formulae-0.4.0/formulae/categorical.py`

 * *Files identical despite different names*

### Comparing `formulae-0.3.4/formulae/contrasts.py` & `formulae-0.4.0/formulae/contrasts.py`

 * *Files identical despite different names*

### Comparing `formulae-0.3.4/formulae/environment.py` & `formulae-0.4.0/formulae/environment.py`

 * *Files identical despite different names*

### Comparing `formulae-0.3.4/formulae/expr.py` & `formulae-0.4.0/formulae/expr.py`

 * *Files 7% similar despite different names*

```diff
@@ -161,23 +161,27 @@
         return "QuotedName(" + self.expression.lexeme + ")"
 
     def accept(self, visitor):
         return visitor.visitQuotedNameExpr(self)
 
 
 class Literal:
-    def __init__(self, value):
+    def __init__(self, value, lexeme=None):
         self.value = value
+        self.lexeme = lexeme
 
     def __eq__(self, other):
         if not isinstance(other, type(self)):
             return False
-        return self.value == other.value
+        return self.value == other.value and self.lexeme == other.lexeme
 
     def __repr__(self):  # pragma: no cover
         return self.__str__()
 
     def __str__(self):  # pragma: no cover
-        return "Literal(" + str(self.value) + ")"
+        kwargs = {"value": self.value, "lexeme": self.lexeme}
+        body_list = [f"{k}={v}" for k, v in kwargs.items() if v is not None]
+        body = ", ".join(body_list)
+        return f"Literal({body})"
 
     def accept(self, visitor):
         return visitor.visitLiteralExpr(self)
```

### Comparing `formulae-0.3.4/formulae/matrices.py` & `formulae-0.4.0/formulae/matrices.py`

 * *Files identical despite different names*

### Comparing `formulae-0.3.4/formulae/model_description.py` & `formulae-0.4.0/formulae/model_description.py`

 * *Files identical despite different names*

### Comparing `formulae-0.3.4/formulae/parser.py` & `formulae-0.4.0/formulae/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,16 @@
                 self.consume("RIGHT_BRACKET", "Expect ']' after level name.")
                 return Variable(identifier, level)
             else:
                 return Variable(self.previous())
         elif self.match("NUMBER"):
             return Literal(self.previous().literal)
         elif self.match("STRING"):
-            return Literal(self.previous().literal)
+            token = self.previous()
+            return Literal(token.literal, lexeme=token.lexeme)
         elif self.match("BQNAME"):
             return QuotedName(self.previous())
         elif self.match("LEFT_PAREN"):
             expr = self.expression()
             self.consume("RIGHT_PAREN", "Expect ')' after expression.")
             return Grouping(expr)
         elif self.match("LEFT_BRACE"):
```

### Comparing `formulae-0.3.4/formulae/resolver.py` & `formulae-0.4.0/formulae/resolver.py`

 * *Files identical despite different names*

### Comparing `formulae-0.3.4/formulae/scanner.py` & `formulae-0.4.0/formulae/scanner.py`

 * *Files identical despite different names*

### Comparing `formulae-0.3.4/formulae/terms/call.py` & `formulae-0.4.0/formulae/terms/call.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,19 +320,19 @@
         return self.eval_new_data_categoric(x.data)
 
     def eval_new_data_offset(self, data_mask):
         if self._intermediate_data.kind == "constant":
             # Return value passed as the argument
             result = np.ones(len(data_mask.index)) * self.call.args[0].value
         else:
-            # Extract name of the argument
-            name = self.call.args[0].name
-            values = data_mask[name]
+            # This works both for LazyVariable (offset(x)) and LazyCall (offset(np.log(x)))
+            offset = self.call.eval(data_mask, self.env)  # returns instance of Offset
+            values = offset.eval()
             if isinstance(values, pd.Series):
-                values = values.values
+                values = values.to_numpy()
             result = values
         return result
 
     def eval_new_data_proportion(self, data_mask):
         if self._intermediate_data.trials_type == "constant":
             # Return value passed in the second component
             result = np.ones(len(data_mask.index)) * self.call.args[1].value
```

### Comparing `formulae-0.3.4/formulae/terms/call_resolver.py` & `formulae-0.4.0/formulae/terms/call_resolver.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import operator
 
 from formulae.expr import Assign
-from formulae.transforms import STATEFUL_TRANSFORMS
 
 
 class CallResolverError(Exception):
     pass
 
 
 class LazyOperator:
@@ -52,15 +51,15 @@
 
     def __hash__(self):
         return hash((self.symbol, *self.args))
 
     def __eq__(self, other):
         if not isinstance(other, type(self)):
             return False
-        return self.symbol == other.symbol and set(self.args) == set(other.args)
+        return self.symbol == other.symbol and self.args == other.args
 
     def accept(self, visitor):
         return visitor.visitLazyOperator(self)
 
     def eval(self, data_mask, env):
         """Evaluates the operation.
 
@@ -149,24 +148,36 @@
     This object holds a value (a string or a number).
     It returns its value only when it is evaluated via ``.eval()``.
 
     Parameters
     ----------
     value: string or numeric
         The value it holds.
+    lexeme: string
+        The string that generated the value it holds
     """
 
-    def __init__(self, value):
+    def __init__(self, value, lexeme):
         self.value = value
+        self.lexeme = lexeme
 
     def __str__(self):
+        if self.lexeme is not None:
+            return self.lexeme
         return str(self.value)
 
+    def __hash__(self):
+        return hash(self.value, self.lexeme)
+
     def __eq__(self, other):
-        return isinstance(other, type(self)) and self.value == other.value
+        return (
+            isinstance(other, type(self))
+            and self.value == other.value
+            and self.lexeme == other.lexeme
+        )
 
     def accept(self, visitor):
         return visitor.visitLazyValue(self)
 
     def eval(self, *args, **kwargs):  # pylint: disable = unused-argument
         """Evaluates the value.
 
@@ -204,30 +215,25 @@
 
     def __init__(self, callee, args, kwargs):
         self.callee = callee
         self.args = args
         self.kwargs = kwargs
         self.stateful_transform = None
 
-        if self.callee in STATEFUL_TRANSFORMS:
-            self.stateful_transform = STATEFUL_TRANSFORMS[self.callee]()
-
     def __str__(self):
         args = [str(arg) for arg in self.args]
-        kwargs = [f"{name} = {str(arg)}" for name, arg in self.kwargs.items()]
+        kwargs = [f"{name}={str(arg)}" for name, arg in self.kwargs.items()]
         return f"{self.callee}({', '.join(args + kwargs)})"
 
     def __hash__(self):
         return hash((self.callee, *self.args, *self.kwargs))
 
     def __eq__(self, other):
         return (
-            self.callee == other.callee
-            and set(self.args) == set(other.args)
-            and set(self.kwargs) == set(other.kwargs)
+            self.callee == other.callee and self.args == other.args and self.kwargs == other.kwargs
         )
 
     def accept(self, visitor):
         return visitor.visitLazyCall(self)
 
     def eval(self, data_mask, env):
         """Evaluate the call.
@@ -243,18 +249,26 @@
             The environment where values and functions are taken from.
 
         Returns
         -------
         result:
             The result of the call evaluation.
         """
+        callee = get_function_from_module(self.callee, env)
+
+        # Store stateful transformation
+        if (
+            hasattr(callee, "__stateful_transform__")
+            and callee.__stateful_transform__
+            and self.stateful_transform is None
+        ):
+            self.stateful_transform = callee()
+
         if self.stateful_transform:
             callee = self.stateful_transform
-        else:
-            callee = get_function_from_module(self.callee, env)
 
         args = [arg.eval(data_mask, env) for arg in self.args]
         kwargs = {name: arg.eval(data_mask, env) for name, arg in self.kwargs.items()}
 
         return callee(*args, **kwargs)
 
 
@@ -310,15 +324,15 @@
                 args.append(arg.accept(self))
         return LazyCall(expr.callee.name.lexeme, args, kwargs)
 
     def visitVariableExpr(self, expr):
         return LazyVariable(expr.name.lexeme)
 
     def visitLiteralExpr(self, expr):
-        return LazyValue(expr.value)
+        return LazyValue(expr.value, expr.lexeme)
 
     def visitQuotedNameExpr(self, expr):
         return LazyVariable(expr.expression.lexeme[1:-1])
 
 
 def get_function_from_module(name, env):
     names = name.split(".")
```

### Comparing `formulae-0.3.4/formulae/terms/call_utils.py` & `formulae-0.4.0/formulae/terms/call_utils.py`

 * *Files identical despite different names*

### Comparing `formulae-0.3.4/formulae/terms/terms.py` & `formulae-0.4.0/formulae/terms/terms.py`

 * *Files identical despite different names*

### Comparing `formulae-0.3.4/formulae/terms/variable.py` & `formulae-0.4.0/formulae/terms/variable.py`

 * *Files identical despite different names*

### Comparing `formulae-0.3.4/formulae/tests/test_design_matrices.py` & `formulae-0.4.0/tests/test_design_matrices.py`

 * *Files 3% similar despite different names*

```diff
@@ -369,16 +369,16 @@
     assert dm.common.terms["C(x3)"].spans_intercept is True
     assert dm.common.terms["C(x3)"].levels == ["1", "2", "3", "4"]
     assert dm.common.terms["C(x3)"].labels == ["C(x3)[1]", "C(x3)[2]", "C(x3)[3]", "C(x3)[4]"]
 
     # Specify levels, different to observed
     lvls = [3, 2, 4, 1]  # noqa
     dm = design_matrices("y ~ C(x3, levels=lvls)", data)
-    assert dm.common.terms["C(x3, levels = lvls)"].kind == "categoric"
-    assert dm.common.terms["C(x3, levels = lvls)"].levels == ["2", "4", "1"]
+    assert dm.common.terms["C(x3, levels=lvls)"].kind == "categoric"
+    assert dm.common.terms["C(x3, levels=lvls)"].levels == ["2", "4", "1"]
 
     # Pass a reference not in the data
     with pytest.raises(ValueError):
         dm = design_matrices("y ~ C(x3, 5)", data)
 
     # Pass categoric, remains unchanged
     dm = design_matrices("y ~ C(f)", data)
@@ -596,15 +596,15 @@
             "y": np.random.randint(0, 5, size=size),
             "x": np.random.randint(5, 10, size=size),
             "g": np.random.choice(["a", "b", "c"], size=size),
         }
     )
 
     # String value
-    term = design_matrices("y ~ binary(g, 'c')", data).common["binary(g, c)"].squeeze()
+    term = design_matrices("y ~ binary(g, 'c')", data).common["binary(g, 'c')"].squeeze()
     assert np.array_equal(np.where(term == 1), np.where(data["g"] == "c"))
 
     # Numeric value
     term = design_matrices("y ~ binary(x, 7)", data).common["binary(x, 7)"].squeeze()
     assert np.array_equal(np.where(term == 1), np.where(data["x"] == 7))
 
     # Variable name
@@ -637,15 +637,15 @@
             "y": np.random.randint(0, 5, size=size),
             "x": np.random.randint(5, 10, size=size),
             "g": np.random.choice(["a", "b", "c"], size=size),
         }
     )
 
     # String value
-    term = design_matrices("y ~ B(g, 'c')", data).common["B(g, c)"].squeeze()
+    term = design_matrices("y ~ B(g, 'c')", data).common["B(g, 'c')"].squeeze()
     assert np.array_equal(np.where(term == 1), np.where(data["g"] == "c"))
 
     # Numeric value
     term = design_matrices("y ~ B(x, 7)", data).common["B(x, 7)"].squeeze()
     assert np.array_equal(np.where(term == 1), np.where(data["x"] == 7))
 
     # Variable name
@@ -683,21 +683,21 @@
 
     term = design_matrices("C(x)", data).common.terms["C(x)"]
     assert term.kind == "categoric"
     assert term.levels == ["6", "7", "8", "9"]
     assert term.data.shape == (100, 4)
 
     levels = [6, 8, 5, 7, 9]
-    term = design_matrices("C(x, levels=levels)", data).common.terms["C(x, levels = levels)"]
+    term = design_matrices("C(x, levels=levels)", data).common.terms["C(x, levels=levels)"]
     assert term.kind == "categoric"
     assert term.levels == [str(level) for level in levels[1:]]
     assert term.data.shape == (100, 4)
 
     levels = ["b", "c", "a"]
-    term = design_matrices("C(g, levels=levels)", data).common.terms["C(g, levels = levels)"]
+    term = design_matrices("C(g, levels=levels)", data).common.terms["C(g, levels=levels)"]
     assert term.kind == "categoric"
     assert term.levels == levels[1:]
     assert term.data.shape == (100, 2)
 
     # Treatment encoding, the default
     t1 = design_matrices("C(x, Treatment)", data).common.terms["C(x, Treatment)"]
     t2 = design_matrices("C(x, Treatment())", data).common.terms["C(x, Treatment())"]
@@ -706,15 +706,15 @@
 
     assert np.array_equal(t1.data, t2.data)
     assert np.array_equal(t1.data, t3.data)
     assert np.array_equal(t1.data, t4.data)
 
     t1 = design_matrices("C(g, Treatment)", data).common.terms["C(g, Treatment)"]
     t2 = design_matrices("C(g, Treatment())", data).common.terms["C(g, Treatment())"]
-    t3 = design_matrices("C(g, Treatment('a'))", data).common.terms["C(g, Treatment(a))"]
+    t3 = design_matrices("C(g, Treatment('a'))", data).common.terms["C(g, Treatment('a'))"]
     t4 = design_matrices("C(g)", data).common.terms["C(g)"]
 
     assert np.array_equal(t1.data, t2.data)
     assert np.array_equal(t1.data, t3.data)
     assert np.array_equal(t1.data, t4.data)
 
     # Sum encoding, not the default
@@ -723,24 +723,20 @@
     t3 = design_matrices("C(x, Sum(9))", data).common.terms["C(x, Sum(9))"]
 
     assert np.array_equal(t1.data, t2.data)
     assert np.array_equal(t1.data, t3.data)
 
     t1 = design_matrices("C(g, Sum)", data).common.terms["C(g, Sum)"]
     t2 = design_matrices("C(g, Sum())", data).common.terms["C(g, Sum())"]
-    t3 = design_matrices("C(g, Sum('c'))", data).common.terms["C(g, Sum(c))"]
+    t3 = design_matrices("C(g, Sum('c'))", data).common.terms["C(g, Sum('c'))"]
 
     assert np.array_equal(t1.data, t2.data)
     assert np.array_equal(t1.data, t3.data)
 
 
-# NOTE: B(g, 'c') is then looked up ad B(g, c).
-# From the second it is impossible to tell if c is a literal or variable
-
-
 def test_C_aliases():
     size = 100
     rng = np.random.default_rng(1234)
     data = pd.DataFrame(
         {
             "x": rng.integers(5, 10, size=size),
             "g": rng.choice(["a", "b", "c"], size=size),
@@ -772,16 +768,16 @@
     assert term.labels == ["S(x)[mean]"] + [f"S(x)[{l}]" for l in [5, 6, 7, 8]]
 
     term = design_matrices("S(x, 7)", data).common.terms["S(x, 7)"]
     assert term.labels == [f"S(x, 7)[{l}]" for l in [5, 6, 8, 9]]
 
     # It still drops last level, no matter we changed the order
     levels = [9, 8, 7, 6, 5]
-    term = design_matrices("S(x, levels = levels)", data).common.terms["S(x, levels = levels)"]
-    assert term.labels == [f"S(x, levels = levels)[{l}]" for l in levels[:-1]]
+    term = design_matrices("S(x, levels=levels)", data).common.terms["S(x, levels=levels)"]
+    assert term.labels == [f"S(x, levels=levels)[{l}]" for l in levels[:-1]]
 
     term = design_matrices("S(x, 6, levels)", data).common.terms["S(x, 6, levels)"]
     assert term.labels == [f"S(x, 6, levels)[{l}]" for l in [9, 8, 7, 5]]
 
 
 def test_T_function():
     size = 100
@@ -796,16 +792,16 @@
     assert term.labels == [f"T(x)[{l}]" for l in [5, 6, 7, 8, 9]]
 
     term = design_matrices("T(x, 7)", data).common.terms["T(x, 7)"]
     assert term.labels == [f"T(x, 7)[{l}]" for l in [5, 6, 8, 9]]
 
     # It still drops first level, no matter we changed the order
     levels = [9, 8, 7, 6, 5]
-    term = design_matrices("T(x, levels = levels)", data).common.terms["T(x, levels = levels)"]
-    assert term.labels == [f"T(x, levels = levels)[{l}]" for l in levels[1:]]
+    term = design_matrices("T(x, levels = levels)", data).common.terms["T(x, levels=levels)"]
+    assert term.labels == [f"T(x, levels=levels)[{l}]" for l in levels[1:]]
 
     term = design_matrices("T(x, 6, levels)", data).common.terms["T(x, 6, levels)"]
     assert term.labels == [f"T(x, 6, levels)[{l}]" for l in [9, 8, 7, 5]]
 
 
 def test_offset():
     size = 100
@@ -818,24 +814,35 @@
         }
     )
 
     dm = design_matrices("y ~ offset(x)", data)
     term = dm.common.terms["offset(x)"]
     assert term.kind == "offset"
     assert term.labels == ["offset(x)"]
-    assert (dm.common["offset(x)"].flatten() == data["x"].values).all()
+    assert np.allclose(dm.common["offset(x)"].flatten(), data["x"])
 
     with pytest.raises(
         ValueError, match=re.escape("offset() can only be used with numeric variables")
     ):
         design_matrices("y ~ offset(g)", data)
 
     with pytest.raises(ValueError, match=re.escape("offset() cannot be used as a response term.")):
         design_matrices("offset(y) ~ x", data)
 
+    # Creation of new design matrices using calls as arguments work
+    dm = design_matrices("y ~ offset(np.log(x))", data)
+    term = dm.common.terms["offset(np.log(x))"]
+    assert term.kind == "offset"
+    assert term.labels == ["offset(np.log(x))"]
+    assert np.allclose(dm.common["offset(np.log(x))"].flatten(), np.log(data["x"]))
+
+    new_data = pd.DataFrame({"x": [3, 4, 5]})
+    new_common = dm.common.evaluate_new_data(new_data)
+    assert np.allclose(new_common["offset(np.log(x))"].flatten(), np.log(new_data["x"]))
+
 
 def test_predict_prop(beetle):
     # If trials is a variable, new dataset must have that variable
     dm = design_matrices("prop(y, n) ~ x", beetle)
     result = dm.response.evaluate_new_data(pd.DataFrame({"n": [10, 10, 30, 30]}))
     assert (result == np.array([10, 10, 30, 30])).all()
 
@@ -1158,15 +1165,15 @@
             ),
             "time": np.repeat(np.arange(0, 5), 12),
         }
     )
 
     formula = "0 + bs(time, degree=2, df=3) : state"
     dm = design_matrices(formula, data)
-    assert dm.common.terms["bs(time, degree = 2, df = 3):state"].levels == [
+    assert dm.common.terms["bs(time, degree=2, df=3):state"].levels == [
         "0, depressed",
         "0, hopeful",
         "0, isolated",
         "0, lonely",
         "0, positive",
         "0, stressed",
         "1, depressed",
@@ -1178,7 +1185,35 @@
         "2, depressed",
         "2, hopeful",
         "2, isolated",
         "2, lonely",
         "2, positive",
         "2, stressed",
     ]
+
+
+def test_calls_with_lazy_values():
+    # https://github.com/bambinos/formulae/issues/87
+    value = np.arange(5)
+    df = pd.DataFrame({"x": value})
+    dm = design_matrices("1 + x + np.power(x, 2) + np.power(x, 3) ", df)
+
+    assert (dm.common["np.power(x, 2)"].flatten() == value**2).all()
+    assert (dm.common["np.power(x, 3)"].flatten() == value**3).all()
+
+
+def test_call_names_respect_string_lexeme():
+    # If a call has an argument which is a string literal, it's important to
+    # respect the original lexeme used to represent the string.
+    # If it was written with double-quotes, we use double-quotes in the term nmae
+    # Analougs if it was written with single-quotes
+    def f(*args, **kwargs):
+        return np.arange(5)
+
+    value = np.arange(5)
+    df = pd.DataFrame({"x": value})
+
+    dm = design_matrices("f(x, y='abcd')", df)
+    assert "f(x, y='abcd')" in dm.common.terms
+
+    dm = design_matrices('f(x, y="abcd")', df)
+    assert 'f(x, y="abcd")' in dm.common.terms
```

### Comparing `formulae-0.3.4/formulae/tests/test_environment.py` & `formulae-0.4.0/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `formulae-0.3.4/formulae/tests/test_eval_new_data.py` & `formulae-0.4.0/tests/test_eval_new_data.py`

 * *Files identical despite different names*

### Comparing `formulae-0.3.4/formulae/tests/test_parser.py` & `formulae-0.4.0/tests/test_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def parse(x, add_intercept=True):
     return Parser(Scanner(x).scan(add_intercept)).parse()
 
 
 def test_parse_literal():
     p = parse("'A'")
-    assert p == Binary(Literal(1), Token("PLUS", "+"), Literal("A"))
+    assert p == Binary(Literal(1), Token("PLUS", "+"), Literal("A", "'A'"))
 
     p = parse("1")
     assert p == Binary(Literal(1), Token("PLUS", "+"), Literal(1))
 
     p = parse("1.132")
     assert p == Binary(Literal(1), Token("PLUS", "+"), Literal(1.132))
```

### Comparing `formulae-0.3.4/formulae/tests/test_poly.py` & `formulae-0.4.0/tests/test_poly.py`

 * *Files identical despite different names*

### Comparing `formulae-0.3.4/formulae/tests/test_resolver.py` & `formulae-0.4.0/tests/test_resolver.py`

 * *Files identical despite different names*

### Comparing `formulae-0.3.4/formulae/tests/test_scanner.py` & `formulae-0.4.0/tests/test_scanner.py`

 * *Files identical despite different names*

### Comparing `formulae-0.3.4/formulae/tests/test_spline.py` & `formulae-0.4.0/tests/test_spline.py`

 * *Files identical despite different names*

### Comparing `formulae-0.3.4/formulae/tests/test_terms_call.py` & `formulae-0.4.0/tests/test_terms_call.py`

 * *Files identical despite different names*

### Comparing `formulae-0.3.4/formulae/tests/test_terms_variable.py` & `formulae-0.4.0/tests/test_terms_variable.py`

 * *Files identical despite different names*

### Comparing `formulae-0.3.4/formulae/tests/test_utils.py` & `formulae-0.4.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `formulae-0.3.4/formulae/token.py` & `formulae-0.4.0/formulae/token.py`

 * *Files identical despite different names*

### Comparing `formulae-0.3.4/formulae/transforms.py` & `formulae-0.4.0/formulae/transforms.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,57 @@
+import inspect
+
 import numpy as np
 import pandas as pd
 
 from pandas.api.types import is_numeric_dtype
 from scipy.interpolate import splev
 
 from formulae.categorical import CategoricalBox, Sum, Treatment
 
+TRANSFORMS = {}
+
+
+def is_class_callable(cls):
+    members = (member[0] for member in inspect.getmembers(cls))
+    return "__call__" in members
+
+
 # Stateful transformations.
 # These transformations have memory about the state of parameters that are
 # required to compute the transformation and are obtained as a subproduct of the
 # data that is used to compute the transform.
+def register_stateful_transform(cls):
+    assert isinstance(cls, type), "Can only decorate classes"
+    assert is_class_callable(cls), "The class must implement a __call__ method"
+    key = cls.__transform_name__ if hasattr(cls, "__transform_name__") else cls.__name__
+    cls.__stateful_transform__ = True
+    TRANSFORMS[key] = cls
+    return cls
 
 
+@register_stateful_transform
 class Center:
+    __transform_name__ = "center"
+
     def __init__(self):
         self.params_set = False
         self.mean = None
 
     def __call__(self, x):
         if not self.params_set:
             self.mean = np.mean(x)
             self.params_set = True
         return x - self.mean
 
 
+@register_stateful_transform
 class Scale:
+    __transform_name__ = "scale"
+
     def __init__(self):
         self.params_set = False
         self.mean = None
         self.std = None
 
     def __call__(self, x):
         if not self.params_set:
@@ -198,14 +221,15 @@
         self.size = size
 
 
 def offset(x):
     return Offset(x)
 
 
+@register_stateful_transform
 class BSpline:
     """B-Spline representation
 
     Generates a B-spline basis for ``x``, allowing non-linear fits. The usual
     usage is something like::
 
         y ~ 1 + bs(x, 4)
@@ -228,14 +252,16 @@
         If ``True``, an intercept is included in the basis. Default is ``False``.
     lower_bound:
         The lower exterior knot location.
     upper_bound:
         The upper exterior knot location.
     """
 
+    __transform_name__ = "bs"
+
     def __init__(self):
         self.params_set = False
         self._intercept = None
         self._degree = None
         self._knots = None
 
     def __call__(
@@ -331,14 +357,15 @@
             basis[:, i] = splev(x, (self._knots, coefs, self._degree))
 
         if not self._intercept:
             basis = basis[:, 1:]
         return basis
 
 
+@register_stateful_transform
 class Polynomial:
     """Polynomial transformation
 
     The computation of this transformation is borrowed from the implementation in the
     Formulaic library written by Matthew Wardrop.
 
     The original implementation and more documentation can be found here:
@@ -351,14 +378,16 @@
     degree: int
         The degree of the polynomial terms to compute. If degree is k, with k > 1, this
         transformation computes the polinomials x^1, x^2, ...x^k.
     raw: bool
         Whether to use raw polynomials or orthonormal ones. Defaults to False.
     """
 
+    __transform_name__ = "poly"
+
     def __init__(self):
         self.params_set = False
         self.degree = 1
         self.raw = False
         self.alpha = {}
         self.norms2 = {}
 
@@ -393,27 +422,22 @@
             if i >= 2:
                 P[:, i] -= get_beta(i - 1) * P[:, i - 2]
 
         P /= np.array([np.sqrt(get_norm(k)) for k in range(0, self.degree + 1)])
         return P[:, 1:]
 
 
-TRANSFORMS = {
-    "B": binary,
-    "binary": binary,
-    "C": C,
-    "I": I,
-    "offset": offset,
-    "p": proportion,
-    "prop": proportion,
-    "proportion": proportion,
-    "S": S,
-    "T": T,
-}
-
-STATEFUL_TRANSFORMS = {
-    "bs": BSpline,
-    "center": Center,
-    "poly": Polynomial,
-    "scale": Scale,
-    "standardize": Scale,
-}
+TRANSFORMS.update(
+    {
+        "B": binary,
+        "binary": binary,
+        "C": C,
+        "I": I,
+        "offset": offset,
+        "p": proportion,
+        "prop": proportion,
+        "proportion": proportion,
+        "S": S,
+        "standardize": Scale,
+        "T": T,
+    }
+)
```

### Comparing `formulae-0.3.4/formulae/utils.py` & `formulae-0.4.0/formulae/utils.py`

 * *Files identical despite different names*

