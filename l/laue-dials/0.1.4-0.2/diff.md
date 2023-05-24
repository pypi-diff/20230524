# Comparing `tmp/laue_dials-0.1.4.tar.gz` & `tmp/laue_dials-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laue_dials-0.1.4.tar", last modified: Wed Apr 12 05:54:53 2023, max compression
+gzip compressed data, was "laue_dials-0.2.tar", last modified: Wed May 24 18:03:38 2023, max compression
```

## Comparing `laue_dials-0.1.4.tar` & `laue_dials-0.2.tar`

### file list

```diff
@@ -1,75 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.055720 laue_dials-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-12 05:52:37.000000 laue_dials-0.1.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.039720 laue_dials-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.047720 laue_dials-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-12 05:52:37.000000 laue_dials-0.1.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-12 05:52:37.000000 laue_dials-0.1.4/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-12 05:52:37.000000 laue_dials-0.1.4/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-12 05:52:37.000000 laue_dials-0.1.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-12 05:52:37.000000 laue_dials-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-12 05:52:37.000000 laue_dials-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-12 05:52:37.000000 laue_dials-0.1.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-12 05:52:37.000000 laue_dials-0.1.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-12 05:52:37.000000 laue_dials-0.1.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-04-12 05:52:37.000000 laue_dials-0.1.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-12 05:52:37.000000 laue_dials-0.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-12 05:54:53.055720 laue_dials-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-12 05:52:37.000000 laue_dials-0.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.047720 laue_dials-0.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.047720 laue_dials-0.1.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/_static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.051720 laue_dials-0.1.4/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/api/laue_dials.algorithms.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/api/laue_dials.command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/api/laue_dials.rst
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/api/laue_dials.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-12 05:52:37.000000 laue_dials-0.1.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.051720 laue_dials-0.1.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 05:52:37.000000 laue_dials-0.1.4/examples/initial_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-12 05:52:37.000000 laue_dials-0.1.4/examples/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-12 05:52:37.000000 laue_dials-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-12 05:54:53.059721 laue_dials-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-12 05:52:37.000000 laue_dials-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.039720 laue_dials-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.051720 laue_dials-0.1.4/src/laue_dials/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.051720 laue_dials-0.1.4/src/laue_dials/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/algorithms/diffgeo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/algorithms/laue.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/algorithms/outliers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.055720 laue_dials-0.1.4/src/laue_dials/command_line/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/command_line/initial_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/command_line/integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/command_line/optimize_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/command_line/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/command_line/refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/skeleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.055720 laue_dials-0.1.4/src/laue_dials/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/utils/expt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-12 05:52:37.000000 laue_dials-0.1.4/src/laue_dials/utils/refl_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.051720 laue_dials-0.1.4/src/laue_dials.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-12 05:54:53.000000 laue_dials-0.1.4/src/laue_dials.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-12 05:54:53.000000 laue_dials-0.1.4/src/laue_dials.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 05:54:53.000000 laue_dials-0.1.4/src/laue_dials.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-12 05:54:53.000000 laue_dials-0.1.4/src/laue_dials.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 05:54:53.000000 laue_dials-0.1.4/src/laue_dials.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-12 05:54:53.000000 laue_dials-0.1.4/src/laue_dials.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 05:54:53.000000 laue_dials-0.1.4/src/laue_dials.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.055720 laue_dials-0.1.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:54:53.055720 laue_dials-0.1.4/tests/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-12 05:52:37.000000 laue_dials-0.1.4/tests/algorithms/test_diffgeo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-12 05:52:37.000000 laue_dials-0.1.4/tests/algorithms/test_laue.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-12 05:52:37.000000 laue_dials-0.1.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 05:52:37.000000 laue_dials-0.1.4/tests/test_initial_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-12 05:52:37.000000 laue_dials-0.1.4/tests/test_skeleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-12 05:52:37.000000 laue_dials-0.1.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:03:38.372285 laue_dials-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-24 18:00:48.000000 laue_dials-0.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:03:38.360285 laue_dials-0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:03:38.364285 laue_dials-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-24 18:00:48.000000 laue_dials-0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-24 18:00:48.000000 laue_dials-0.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-24 18:00:48.000000 laue_dials-0.2/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-24 18:00:48.000000 laue_dials-0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-24 18:00:48.000000 laue_dials-0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-24 18:00:48.000000 laue_dials-0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-24 18:00:48.000000 laue_dials-0.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-24 18:00:48.000000 laue_dials-0.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-24 18:00:48.000000 laue_dials-0.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-05-24 18:00:48.000000 laue_dials-0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-24 18:00:48.000000 laue_dials-0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-24 18:03:38.372285 laue_dials-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-24 18:00:48.000000 laue_dials-0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:03:38.364285 laue_dials-0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-24 18:00:48.000000 laue_dials-0.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:03:38.364285 laue_dials-0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 18:00:48.000000 laue_dials-0.2/docs/_static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:03:38.368285 laue_dials-0.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-24 18:00:48.000000 laue_dials-0.2/docs/api/laue_dials.algorithms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-24 18:00:48.000000 laue_dials-0.2/docs/api/laue_dials.command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-24 18:00:48.000000 laue_dials-0.2/docs/api/laue_dials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-24 18:00:48.000000 laue_dials-0.2/docs/api/laue_dials.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-24 18:00:48.000000 laue_dials-0.2/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-24 18:00:48.000000 laue_dials-0.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 18:00:48.000000 laue_dials-0.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-05-24 18:00:48.000000 laue_dials-0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 18:00:48.000000 laue_dials-0.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-24 18:00:48.000000 laue_dials-0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-24 18:00:48.000000 laue_dials-0.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-24 18:00:48.000000 laue_dials-0.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-24 18:00:48.000000 laue_dials-0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:03:38.368285 laue_dials-0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-24 18:00:48.000000 laue_dials-0.2/examples/pipeline.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-24 18:00:48.000000 laue_dials-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-24 18:03:38.372285 laue_dials-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-24 18:00:48.000000 laue_dials-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:03:38.360285 laue_dials-0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:03:38.368285 laue_dials-0.2/src/laue_dials/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-24 18:00:48.000000 laue_dials-0.2/src/laue_dials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:03:38.368285 laue_dials-0.2/src/laue_dials/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-05-24 18:00:48.000000 laue_dials-0.2/src/laue_dials/algorithms/diffgeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-05-24 18:00:48.000000 laue_dials-0.2/src/laue_dials/algorithms/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12955 2023-05-24 18:00:48.000000 laue_dials-0.2/src/laue_dials/algorithms/laue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-24 18:00:48.000000 laue_dials-0.2/src/laue_dials/algorithms/monochromatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-24 18:00:48.000000 laue_dials-0.2/src/laue_dials/algorithms/outliers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:03:38.368285 laue_dials-0.2/src/laue_dials/command_line/
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-24 18:00:48.000000 laue_dials-0.2/src/laue_dials/command_line/combine_mtzs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-24 18:00:48.000000 laue_dials-0.2/src/laue_dials/command_line/initial_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-05-24 18:00:48.000000 laue_dials-0.2/src/laue_dials/command_line/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-05-24 18:00:48.000000 laue_dials-0.2/src/laue_dials/command_line/optimize_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-05-24 18:00:48.000000 laue_dials-0.2/src/laue_dials/command_line/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-24 18:00:48.000000 laue_dials-0.2/src/laue_dials/command_line/refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-05-24 18:00:48.000000 laue_dials-0.2/src/laue_dials/command_line/sequence_to_stills.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-24 18:00:48.000000 laue_dials-0.2/src/laue_dials/skeleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:03:38.372285 laue_dials-0.2/src/laue_dials/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-24 18:00:48.000000 laue_dials-0.2/src/laue_dials/utils/expt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-24 18:00:48.000000 laue_dials-0.2/src/laue_dials/utils/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-24 18:00:48.000000 laue_dials-0.2/src/laue_dials/utils/refl_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:03:38.368285 laue_dials-0.2/src/laue_dials.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-24 18:03:38.000000 laue_dials-0.2/src/laue_dials.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-24 18:03:38.000000 laue_dials-0.2/src/laue_dials.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:03:38.000000 laue_dials-0.2/src/laue_dials.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-24 18:03:38.000000 laue_dials-0.2/src/laue_dials.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:03:38.000000 laue_dials-0.2/src/laue_dials.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-24 18:03:38.000000 laue_dials-0.2/src/laue_dials.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-24 18:03:38.000000 laue_dials-0.2/src/laue_dials.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:03:38.372285 laue_dials-0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:03:38.372285 laue_dials-0.2/tests/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-24 18:00:48.000000 laue_dials-0.2/tests/algorithms/test_diffgeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-24 18:00:48.000000 laue_dials-0.2/tests/algorithms/test_laue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-24 18:00:48.000000 laue_dials-0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 18:00:48.000000 laue_dials-0.2/tests/test_initial_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-24 18:00:48.000000 laue_dials-0.2/tests/test_skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-24 18:00:48.000000 laue_dials-0.2/tox.ini
```

### Comparing `laue_dials-0.1.4/.coveragerc` & `laue_dials-0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.4/.github/workflows/build.yml` & `laue_dials-0.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.4/.github/workflows/docs.yml` & `laue_dials-0.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.4/.github/workflows/format.yml` & `laue_dials-0.2/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.4/.github/workflows/publish.yml` & `laue_dials-0.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.4/.gitignore` & `laue_dials-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.4/.readthedocs.yml` & `laue_dials-0.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.4/CONTRIBUTING.rst` & `laue_dials-0.2/CONTRIBUTING.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 ============
 Contributing
 ============
 
-Welcome to ``laue_dials`` developer's guide.
+Welcome to ``laue-dials`` developer's guide.
 
 This document focuses on outlining development processes, but `other kinds of contributions`_ are also
 appreciated.
 
 Please note that all users and contributors are expected to be **open,
 considerate, reasonable, honest, and respectful** when contributing
 ideas, issues, documentation, or code.
 
 Issue Reports
 =============
 
-If you experience bugs or general issues with ``laue_dials``, please have a look
+If you experience bugs or general issues with ``laue-dials``, please have a look
 on the `issue tracker`_. If you don't see anything useful there, please feel
 free to fire an issue report.
 
 New issue reports should include information about your programming environment
 (e.g., operating system, Python version) and steps to reproduce the problem.
 Please try also to simplify the reproduction steps to a very minimal example
 that still illustrates the problem you are facing. By removing other factors,
 you help us to identify the root cause of the issue.
 
 
 Documentation Improvements
 ==========================
 
-You can help improve ``laue_dials`` docs by making them more readable and coherent, or
+You can help improve ``laue-dials`` docs by making them more readable and coherent, or
 by adding missing information and correcting mistakes.
 
-``laue_dials`` documentation uses Sphinx_ as its main documentation compiler.
+``laue-dials`` documentation uses Sphinx_ as its main documentation compiler.
 This means that the docs are kept in the same repository as the project code, and
 that any documentation update is done in the same way was a code contribution.
 When working on documentation changes in your local machine, you can
-compile them using |tox|_::
+compile them using ``tox``
 
     tox -e docs
 
 and use Python's built-in web server for a preview in your web browser
 (``http://localhost:8000``)::
 
     python3 -m http.server --directory 'docs/_build/html'
@@ -68,40 +68,40 @@
 Create an environment
 ---------------------
 
 Before you start coding, we recommend creating an isolated `virtual
 environment`_ to avoid any problems with your installed Python packages.
 This can easily be done via Miniconda_::
 
-    conda create -n laue_dials python=3 six virtualenv pytest pytest-cov
-    conda activate laue_dials
+    conda create -n laue-dials python=3 six virtualenv pytest pytest-cov
+    conda activate laue-dials
 
 Clone the repository
 --------------------
 
 #. Create an user account on |the repository service| if you do not already have one.
 #. Fork the project repository_: click on the *Fork* button near the top of the
    page. This creates a copy of the code under your account on |the repository service|.
 #. Clone this copy to your local disk::
 
-    git clone git@github.com:YourLogin/laue_dials.git
-    cd laue_dials
+    git clone git@github.com:YourLogin/laue-dials.git
+    cd laue-dials
 
 #. You should run::
 
     pip install -U pip setuptools -e .
 
    to be able to import the package under development in the Python REPL.
 
 #. Install |pre-commit|_::
 
     pip install pre-commit
     pre-commit install
 
-   ``laue_dials`` comes with a lot of hooks configured to automatically help the
+   ``laue-dials`` comes with a lot of hooks configured to automatically help the
    developer to check the code being written. Compliance with all hooks is
    necessary to contribute code to maintain code quality.
 
 Implement your changes
 ----------------------
 
 #. Create a branch to hold your changes::
@@ -140,17 +140,17 @@
 
    to look for recurring communication patterns.
 
 #. Please check that your changes don't break any unit tests with::
 
     tox
 
-   (after having installed |tox-conda|_ with ``pip install tox-conda`` or ``pipx``).
+   (after having installed ``tox-conda`` with ``pip install tox-conda`` or ``pipx``).
 
-   You can also use |tox-conda|_ to run several other pre-configured tasks in the
+   You can also use ``tox-conda`` to run several other pre-configured tasks in the
    repository. Try ``tox -av`` to see a list of the available checks.
 
 Submit your contribution
 ------------------------
 
 #. If everything works fine, push your local branch to |the repository service| with::
 
@@ -171,26 +171,26 @@
    The command ``git describe --abbrev=0 --tags`` should return the version you
    are expecting. If you are trying to run CI scripts in a fork repository,
    make sure to push all the tags.
    You can also try to remove all the egg files or the complete egg folder, i.e.,
    ``.eggs``, as well as the ``*.egg-info`` folders in the ``src`` folder or
    potentially in the root of your project.
 
-#. Sometimes |tox-conda|_ misses out when new dependencies are added, especially to
+#. Sometimes ``tox-conda`` misses out when new dependencies are added, especially to
    ``setup.cfg`` and ``docs/requirements.txt``. If you find any problems with
-   missing dependencies when running a command with |tox-conda|_, try to recreate the
+   missing dependencies when running a command with ``tox-conda``, try to recreate the
    ``tox`` environment using the ``-r`` flag. For example, instead of::
 
     tox -e docs
 
    Try running::
 
     tox -r -e docs
 
-#. Make sure to have a reliable |tox-conda|_ installation that uses the correct
+#. Make sure to have a reliable ``tox-conda`` installation that uses the correct
    Python version (e.g., 3.7+). When in doubt you can run::
 
     tox --version
     # OR
     which tox
 
 #. `Pytest can drop you`_ in an interactive session in the case an error occurs.
@@ -203,35 +203,34 @@
 ================
 
 Releases
 --------
 
 If you are part of the group of maintainers and have correct user permissions
 on PyPI_, the following steps can be used to release a new version for
-``laue_dials``:
+``laue-dials``:
 
 #. Make sure all unit tests are successful.
 #. Update ``CHANGELOG.rst`` with new features and changes for the new release.
 #. Run ``git pull``, resolve any merge conflicts, and then ``git push`` the source code.
 #. Tag the current commit on the main branch with a release tag, e.g., ``git tag -a v0.1 -m 'Version message'``.
 #. Push the new tag to the upstream repository_, e.g., ``git push origin v0.1``
 #. Navigate to ``https://github.com/rs-station/laue-dials/releases/new``.
 #. Select the appropriate tag and write a description for the release.
 #. Set as a pre-release if necessary, and then publish the release on Github.
 #. After Github Actions workflows have executed, check PyPI to ensure they worked correctly.
 
 .. <-- Documentation variables -->
-.. _repository: https://github.com/rs-station/laue_dials
-.. _issue tracker: https://github.com/rs-station/laue_dials/issues
+.. _repository: https://github.com/rs-station/laue-dials
+.. _issue tracker: https://github.com/rs-station/laue-dials/issues
 
 .. |the repository service| replace:: GitHub
 .. |contribute button| replace:: "Create pull request"
 .. |virtualenv| replace:: ``virtualenv``
 .. |pre-commit| replace:: ``pre-commit``
-.. |tox-conda| replace:: ``tox``
 
 
 .. _black: https://pypi.org/project/black/
 .. _CommonMark: https://commonmark.org/
 .. _contribution-guide.org: https://www.contribution-guide.org/
 .. _creating a PR: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request
 .. _descriptive commit message: https://chris.beams.io/posts/git-commit
@@ -247,14 +246,13 @@
 .. _PyPI: https://pypi.org/
 .. _PyScaffold's contributor's guide: https://pyscaffold.org/en/stable/contributing.html
 .. _Pytest can drop you: https://docs.pytest.org/en/stable/how-to/failures.html#using-python-library-pdb-with-pytest
 .. _Python Software Foundation's Code of Conduct: https://www.python.org/psf/conduct/
 .. _reStructuredText: https://www.sphinx-doc.org/en/master/usage/restructuredtext/
 .. _Sphinx: https://www.sphinx-doc.org/en/master/
 .. _TestPyPI: https://test.pypi.org
-.. _tox: https://tox.wiki/en/stable/
 .. _virtual environment: https://realpython.com/python-virtual-environments-a-primer/
 .. _virtualenv: https://virtualenv.pypa.io/en/stable/
 
 .. _GitHub's fork and pull request workflow: https://guides.github.com/activities/forking/
 .. _GitHub web interface: https://docs.github.com/en/repositories/working-with-files/managing-files/editing-files
 .. _GitHub's code editor: https://docs.github.com/en/repositories/working-with-files/managing-files/editing-files
```

### Comparing `laue_dials-0.1.4/LICENSE.txt` & `laue_dials-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.4/PKG-INFO` & `laue_dials-0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: laue_dials
-Version: 0.1.4
+Version: 0.2
 Summary: A package for analyzing Laue x-ray crystallography data using the DIALS framework.
 Home-page: https://github.com/rs-station/laue_dials
 Author: Rick A. Hewitt
 Author-email: rahewitt@g.harvard.edu
 License: MIT
-Platform: any
+Platform: Mac
+Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE.txt
 
@@ -27,41 +28,55 @@
    :target: https://codecov.io/gh/rs-station/laue-dials
 
 .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :alt: MIT License
    :target: https://github.com/rs-station/laue-dials/blob/main/LICENSE.txt
 
 ==========
-laue_dials
+laue-dials
 ==========
 
 Data analysis package for Laue crystallography.
 
-``laue_dials`` is an extension to the `DIALS`_ code for analyzing polychromatic crystallographic data.
+``laue-dials`` is an extension to the `DIALS`_ code for analyzing polychromatic crystallographic data.
 Building off the ``DIALS`` framework, and including modern tools like ``numpy``, ``scipy``, and
 ``reciprocalspaceship``, this package allows for analysis of X-ray crystallographic data using
 wide-bandwidth light sources. This package is intended to be used in conjunction with `DIALS`_,
 `careless`_, and `Phenix`_ in order to generate molecular models from raw data.
 
 ============
 Installation
 ============
 
-To install ``laue_dials``, the DIALS code must first be installed using
+To install ``laue-dials``, the DIALS code must first be installed using
 
 .. code:: python
 
    conda install -c conda-forge dials
 
 Then, using the DIALS python environment, run the following:
 
 .. code:: python
 
    pip install laue-dials
 
-If any issues occur either with installation or use of the software, please file an issue at `issue tracker`_.
+``laue-dials`` consists of seven command-line scripts for the processing of Laue diffraction data, which are
+
+.. code:: python
+
+   laue.initial_solution
+   laue.sequence_to_stills
+   laue.optimize_indexing
+   laue.refine
+   laue.predict
+   laue.integrate
+   laue.combine_mtzs
+
+Note that you need to import the image data using ``dials.import``. For information on how to use this command, visit https://dials.github.io/documentation/programs/dials_import.html. An example of how to analyze a full dataset lives at https://github.com/rs-station/laue-dials/blob/main/examples/pipeline.sh.
+
+If any issues occur either with installation or use of the software, please file an issue at `issue tracker`_. Any and all questions, concerns, or feature requests are welcome.
 
 .. _careless: https://github.com/rs-station/careless
 .. _DIALS: https://dials.github.io/index.html
-.. _issue tracker: https://github.com/rs-station/laue_dials/issues
+.. _issue tracker: https://github.com/rs-station/laue-dials/issues
 .. _Phenix: http://www.phenix-online.org
 .. _reciprocalspaceship: https://github.com/rs-station/reciprocalspaceship
```

### Comparing `laue_dials-0.1.4/README.rst` & `laue_dials-0.2/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -11,41 +11,55 @@
    :target: https://codecov.io/gh/rs-station/laue-dials
 
 .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :alt: MIT License
    :target: https://github.com/rs-station/laue-dials/blob/main/LICENSE.txt
 
 ==========
-laue_dials
+laue-dials
 ==========
 
 Data analysis package for Laue crystallography.
 
-``laue_dials`` is an extension to the `DIALS`_ code for analyzing polychromatic crystallographic data.
+``laue-dials`` is an extension to the `DIALS`_ code for analyzing polychromatic crystallographic data.
 Building off the ``DIALS`` framework, and including modern tools like ``numpy``, ``scipy``, and
 ``reciprocalspaceship``, this package allows for analysis of X-ray crystallographic data using
 wide-bandwidth light sources. This package is intended to be used in conjunction with `DIALS`_,
 `careless`_, and `Phenix`_ in order to generate molecular models from raw data.
 
 ============
 Installation
 ============
 
-To install ``laue_dials``, the DIALS code must first be installed using
+To install ``laue-dials``, the DIALS code must first be installed using
 
 .. code:: python
 
    conda install -c conda-forge dials
 
 Then, using the DIALS python environment, run the following:
 
 .. code:: python
 
    pip install laue-dials
 
-If any issues occur either with installation or use of the software, please file an issue at `issue tracker`_.
+``laue-dials`` consists of seven command-line scripts for the processing of Laue diffraction data, which are
+
+.. code:: python
+
+   laue.initial_solution
+   laue.sequence_to_stills
+   laue.optimize_indexing
+   laue.refine
+   laue.predict
+   laue.integrate
+   laue.combine_mtzs
+
+Note that you need to import the image data using ``dials.import``. For information on how to use this command, visit https://dials.github.io/documentation/programs/dials_import.html. An example of how to analyze a full dataset lives at https://github.com/rs-station/laue-dials/blob/main/examples/pipeline.sh.
+
+If any issues occur either with installation or use of the software, please file an issue at `issue tracker`_. Any and all questions, concerns, or feature requests are welcome.
 
 .. _careless: https://github.com/rs-station/careless
 .. _DIALS: https://dials.github.io/index.html
-.. _issue tracker: https://github.com/rs-station/laue_dials/issues
+.. _issue tracker: https://github.com/rs-station/laue-dials/issues
 .. _Phenix: http://www.phenix-online.org
 .. _reciprocalspaceship: https://github.com/rs-station/reciprocalspaceship
```

### Comparing `laue_dials-0.1.4/docs/Makefile` & `laue_dials-0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.4/docs/api/laue_dials.algorithms.rst` & `laue_dials-0.2/docs/api/laue_dials.algorithms.rst`

 * *Files 11% similar despite different names*

```diff
@@ -10,22 +10,38 @@
 -------------------------------------
 
 .. automodule:: laue_dials.algorithms.diffgeo
    :members:
    :undoc-members:
    :show-inheritance:
 
+laue\_dials.algorithms.integration module
+-----------------------------------------
+
+.. automodule:: laue_dials.algorithms.integration
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 laue\_dials.algorithms.laue module
 ----------------------------------
 
 .. automodule:: laue_dials.algorithms.laue
    :members:
    :undoc-members:
    :show-inheritance:
 
+laue\_dials.algorithms.monochromatic module
+-------------------------------------------
+
+.. automodule:: laue_dials.algorithms.monochromatic
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 laue\_dials.algorithms.outliers module
 --------------------------------------
 
 .. automodule:: laue_dials.algorithms.outliers
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `laue_dials-0.1.4/docs/api/laue_dials.command_line.rst` & `laue_dials-0.2/docs/api/laue_dials.command_line.rst`

 * *Files 11% similar despite different names*

```diff
@@ -41,7 +41,15 @@
 laue\_dials.command\_line.refine module
 ---------------------------------------
 
 .. automodule:: laue_dials.command_line.refine
    :members:
    :undoc-members:
    :show-inheritance:
+
+laue\_dials.command\_line.sequence\_to\_stills module
+-----------------------------------------------------
+
+.. automodule:: laue_dials.command_line.sequence_to_stills
+   :members:
+   :undoc-members:
+   :show-inheritance:
```

### Comparing `laue_dials-0.1.4/docs/api/laue_dials.utils.rst` & `laue_dials-0.2/docs/api/laue_dials.utils.rst`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.4/docs/conf.py` & `laue_dials-0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.4/docs/index.rst` & `laue_dials-0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.4/setup.cfg` & `laue_dials-0.2/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 author = Rick A. Hewitt
 author_email = rahewitt@g.harvard.edu
 license = MIT
 license_files = LICENSE.txt
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/rs-station/laue_dials
-platforms = any
+platforms = Mac,Linux
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
 
 [options]
 zip_safe = False
 packages = find_namespace:
@@ -40,19 +40,21 @@
 testing = 
 	setuptools
 	pytest
 	pytest-cov
 
 [options.entry_points]
 console_scripts = 
-	laue.initial_solution = laue_dials.command_line.initial_solution:dials_version
+	laue.initial_solution = laue_dials.command_line.initial_solution:run
+	laue.sequence_to_stills = laue_dials.command_line.sequence_to_stills:run
 	laue.optimize_indexing = laue_dials.command_line.optimize_indexing:run
-	laue.refine = laue_dials.command_line.refine:refine_geometry
-	laue.predict = laue_dials.command_line.predict:predict_spots
-	laue.integrate = laue_dials.command_line.integrate:integrate_dataset
+	laue.refine = laue_dials.command_line.refine:run
+	laue.predict = laue_dials.command_line.predict:run
+	laue.integrate = laue_dials.command_line.integrate:run
+	laue.combine_mtzs = laue_dials.command_line.combine_mtzs:run
 
 [tool:pytest]
 addopts = 
 	--cov laue_dials --cov-report xml
 	--verbose
 norecursedirs = 
 	dist
```

### Comparing `laue_dials-0.1.4/setup.py` & `laue_dials-0.2/setup.py`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.4/src/laue_dials/__init__.py` & `laue_dials-0.2/src/laue_dials/__init__.py`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.4/src/laue_dials/algorithms/diffgeo.py` & `laue_dials-0.2/src/laue_dials/algorithms/diffgeo.py`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.4/src/laue_dials/algorithms/laue.py` & `laue_dials-0.2/src/laue_dials/algorithms/laue.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,159 @@
 """
 Classes and functions for Laue-specific processes.
 """
 
 import gemmi
 import numpy as np
 import reciprocalspaceship as rs
+from dials.array_family import flex
+from dxtbx.model import ExperimentList
+from tqdm import tqdm, trange
 
 from laue_dials.algorithms.diffgeo import hkl2ray
 
 
+def store_wavelengths(expts, refls):
+    """
+    A function for storing wavelength data in beam objects in the reflection table
+        Parameters
+        ----------
+        expts : ExperimentList
+            ExperimentList to retrieve wavelengths from
+        refls : reflection_table
+            A reflection_table to store wavelengths in
+
+        Returns
+        -------
+        new_refls : reflection_table
+            A reflection_table with updated wavelengths
+    """
+    # Make new reflection_table
+    new_refls = refls.copy()
+
+    # Get experiment ID per reflection
+    idx = new_refls["id"].as_numpy_array()
+
+    # Initialize wavelength array
+    lams = np.zeros(len(idx))
+
+    # For each reflection, get corresponding beam wavelength
+    for i in trange(len(idx)):
+        lams[i] = expts[idx[i]].beam.get_wavelength()
+
+    # Store wavelengths into reflection_table
+    new_refls["wavelength"] = flex.double(lams)
+    return new_refls
+
+
+def remove_beam_models(expts):
+    """
+    A function for removing beam models no longer needed after refinement
+        Parameters
+        ----------
+        expts : ExperimentList
+            ExperimentList to remove beams from
+
+        Returns
+        -------
+        new_expts : ExperimentList
+            An ExperimentList with an experiment per image all sharing a beam
+    """
+    # Instantiate new ExperimentList/reflection_table
+    new_expts = ExperimentList()
+
+    # Copy first experiment per image to new ExperimentList
+    for img_num in trange(len(expts.imagesets())):
+        i = 0
+        img = expts.imagesets()[img_num]
+        expt = expts[0]
+        while True:
+            expt = expts[i]
+            if expt.imageset == img:
+                break
+            i = i + 1
+        expt = expts[i]
+        expt.identifier = str(img_num)  # Reset identifier to match image
+        new_expts.append(expt)
+    return new_expts
+
+
+def gen_beam_models(expts, refls):
+    """
+    A function for generating beam models according to wavelengths in a reflection table
+        Parameters
+        ----------
+        expts : ExperimentList
+            ExperimentList to insert beams into
+        refls : reflection_table
+            A reflection_table containing wavelengths for beam models
+
+        Returns
+        -------
+        new_expts : ExperimentList
+            ExperimentList with additional beam models and adjusted identifiers
+        new_refls : reflection_table
+            A reflection_table with updated identifiers
+    """
+    # Imports
+    from copy import deepcopy
+
+    from dials.algorithms.refinement.prediction.managed_predictors import \
+        ExperimentsPredictorFactory
+
+    # Instantiate new ExperimentList/reflection_table
+    new_expts = ExperimentList()
+    new_refls = refls.copy()
+
+    # Unassign all reflections from experiments
+    new_refls["id"] = flex.int([-1] * len(new_refls))
+
+    # Initialize data frame
+    df = rs.DataSet(
+        {
+            "wavelength": refls["wavelength"],
+            "ID": refls["id"],
+            "new_ID": [-1] * len(refls),
+        }
+    )
+
+    # Generate beams per reflection
+    exp_id = -1
+    for i, refl in tqdm(df.iterrows()):
+        try:
+            # New beam per reflection
+            expt = expts[refl["ID"][i]]
+            expt.beam.get_s0()
+            new_expt = expt
+            new_expt.beam = deepcopy(expt.beam)
+            new_expt.beam.set_wavelength(refl["wavelength"][i])
+            s0 = (
+                expt.beam.get_s0() / np.linalg.norm(expt.beam.get_s0())
+            ) / new_expt.beam.get_wavelength()
+            new_expt.beam.set_s0(s0)
+            exp_id = exp_id + 1  # Increment experiment ID
+            new_expt.identifier = str(exp_id)
+            new_expts.append(new_expt)
+
+            # Write new beam identifiers to reflections
+            df.at[i, "new_ID"] = exp_id
+        except:
+            print("Warning: Unindexed strong spot has wavelength 0.")
+            df.at[i, "new_ID"] = -1
+            continue
+
+    # Replace reflection IDs with new IDs
+    idx = flex.int(df["new_ID"])
+    new_refls["id"] = idx
+
+    # Repredict centroids
+    ExperimentsPredictorFactory.from_experiments(new_expts)
+    return new_expts, new_refls
+
+
 class LaueBase:
     """
     A base class to be extended for Laue procedures
     """
 
     def __init__(self, s0, cell, R, lam_min, lam_max, dmin, spacegroup="1"):
         """
@@ -83,17 +224,15 @@
         """
         Parameters
         ----------
         s1 : array
             n x 3 array indicating the direction of the scatterd beam wavevector.
             This can be any length, it will be unit normalized in the constructor.
         """
-        super().__init__(s0, cell, R, lam_min, lam_max, dmin, spacegroup="1")
-
-        self.ewald_offset = None
+        super().__init__(s0, cell, R, lam_min, lam_max, dmin, spacegroup)
 
         self._s1 = s1 / np.linalg.norm(s1, axis=-1)[:, None]
         self._qobs = self._s1 - self.s0
         self._qpred = np.zeros_like(self._s1)
         self._H = np.zeros_like(self._s1)
         self._wav = np.zeros(len(self._H))
         self._harmonics = np.zeros(len(self._s1), dtype=bool)
@@ -183,28 +322,31 @@
         qall = qall[idx]
 
         dmat = rs.utils.angle_between(self.qobs[..., None, :], qall[None, ..., :])
         cost = dmat
 
         from scipy.optimize import linear_sum_assignment
 
-        _, idx = linear_sum_assignment(cost)
+        ido, idx = linear_sum_assignment(cost)
+
+        # Update appropriate variables
         H = Hall[idx]
         qpred = qall[idx]
         harmonics = harmonics[idx]
 
         # Set all attributes to match the current assignment
         self.set_H(H)
         self.set_qpred(qpred)
         self.set_harmonics(harmonics)
 
         # wav_pred = -2.*(self.s0 * qpred).sum(-1) / (qpred*qpred).sum(-1)
-        wav_obs = np.linalg.norm(self.qobs, axis=-1) / np.linalg.norm(
-            self.qpred, axis=-1
-        )
+        with np.errstate(divide="ignore"):
+            wav_obs = np.linalg.norm(self.qobs, axis=-1) / np.linalg.norm(
+                self.qpred, axis=-1
+            )
         self.set_wav(wav_obs)
 
     def update_rotation(self):
         """Update the rotation matrix (self.R) based on the inlying refls"""
         from scipy.linalg import orthogonal_procrustes
 
         misset, _ = orthogonal_procrustes(
@@ -228,14 +370,15 @@
     def predict_s1(self, delete_harmonics=False):
         """
         Predicts all s1 vectors for all feasible spots given some resolution-dependent bandwidth
         This method provides:
             s1_pred -- predicted feasible s1 vectors
             lams -- the wavelengths (in Angstroms) associated with these s1 vectors
             qall -- the q vectors associated with these s1 vectors
+            Hall -- the miller indices associated with s1 vectors
         """
         # Generate the feasible set of reflections from the current geometry
         Hall = self.Hall
         qall = (self.RB @ Hall.T).T
         feasible = (
             np.linalg.norm(qall + self.s0 / self.lam_min, axis=-1) < 1 / self.lam_min
         ) & (np.linalg.norm(qall + self.s0 / self.lam_max, axis=-1) > 1 / self.lam_max)
```

### Comparing `laue_dials-0.1.4/src/laue_dials/command_line/optimize_indexing.py` & `laue_dials-0.2/src/laue_dials/command_line/optimize_indexing.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 """
 This script optimizes Miller indices and wavelengths jointly.
 """
 
 import logging
 
 import libtbx.phil
+from dials.array_family.flex import reflection_table
 from dials.util import log, show_mail_handle_errors
 from dials.util.options import (ArgumentParser,
                                 reflections_and_experiments_from_files)
+from dxtbx.model import ExperimentList
 
 logger = logging.getLogger("laue-dials.command_line.optimize_indexing")
 
 help_message = """
 
 This program takes initial monochromatic estimates of the geometry in a
 DIALS experiment list and reflection table, and optimizes the indexed
@@ -23,15 +25,15 @@
 The outputs are a pair of files (optimized.expt, optimized.refl), which
 mimic the input files but with updated Miller indices, s1 vectors, and
 wavelengths in the reflection table. Note that the experiment list is
 unchanged entirely.
 
 Examples::
 
-    laue.optimize_indexing monochromatic.expt monochromatic.refl
+    laue.optimize_indexing [options] monochromatic.expt monochromatic.refl
 """
 
 # Set the phil scope
 phil_scope = libtbx.phil.parse(
     """
 
 output {
@@ -53,15 +55,15 @@
   .help = "Number of macrocycles of index optimization to perform"
 
 wavelengths {
   lam_min = 0.95
     .type = float(value_min=0.1)
     .help = "Minimum wavelength for beam spectrum"
   lam_max = 1.15
-    .type = float
+    .type = float(value_min=0.2)
     .help = "Maximum wavelength for beam spectrum"
   }
 
 reciprocal_grid {
   d_min = 1.4
     .type = float(value_min=0.1)
     .help = "Minimum d-spacing for reflecting planes"
@@ -92,27 +94,28 @@
     # This will populate refls['s1'] & refls['rlp']
     refls.centroid_px_to_mm(expts)
     refls.map_centroids_to_reciprocal_space(expts)
 
     s0 = np.array(expts[0].beam.get_s0())
 
     # Write to reflection file
-    refls["Wavelength"] = flex.double(len(refls))
+    refls["wavelength"] = flex.double(len(refls))
     refls["miller_index"] = flex.miller_index(len(refls))
+    refls["harmonics"] = flex.bool([False] * len(refls))
 
-    for i in trange(len(expts.imagesets())):
+    for i in range(len(expts.imagesets())):
         # Get experiment data from experiment objects
         experiment = expts[i]
         cryst = experiment.crystal
         spacegroup = gemmi.SpaceGroup(
             cryst.get_space_group().type().universal_hermann_mauguin_symbol()
         )
 
         # Get reflections on this image
-        idx = refls["id"] == i
+        idx = refls["id"] == int(experiment.identifier)
         subrefls = refls.select(idx)
 
         # Get unit cell params
         cell_params = cryst.get_unit_cell().parameters()
         cell = gemmi.UnitCell(*cell_params)
 
         # Generate s vectors
@@ -131,15 +134,15 @@
             params.wavelengths.lam_max,
             params.reciprocal_grid.d_min,
             spacegroup,
         )
 
         # Optimize Miller indices
         la.assign()
-        for j in range(params.n_macrocycles):
+        for j in trange(params.n_macrocycles):
             la.reset_inliers()
             la.update_rotation()
             la.assign()
             la.reject_outliers()
             la.update_rotation()
             la.assign()
 
@@ -150,81 +153,84 @@
         cryst.set_U(la.R.flatten())
         cryst.set_A(la.RB.flatten())
         cryst.set_B(la.B.flatten())
         cryst.set_space_group(space_group(la.spacegroup.hall))
         cryst.set_unit_cell(unit_cell(la.cell.parameters))
 
         # Write data to reflections
-        refls["harmonics"] = flex.bool([False] * len(refls))
         refls["s1"].set_selected(idx, flex.vec3_double(s1))
         refls["miller_index"].set_selected(
             idx,
             flex.miller_index(la._H.astype("int").tolist()),
         )
-        refls["Wavelength"].set_selected(
+        refls["wavelength"].set_selected(
             idx,
             flex.double(la._wav.tolist()),
         )
         refls["harmonics"].set_selected(
             idx,
             flex.bool(la._harmonics.tolist()),
         )
 
     # Return reindexed expts, refls
     return expts, refls
 
 
 @show_mail_handle_errors()
-def run(args=None, *, phil=working_phil, return_results=False):
+def run(args=None, *, phil=working_phil):
     # Parse arguments
-    usage = (
-        "usage: laue.optimize_indexing [options] monochromatic.expt monochromatic.refl"
-    )
+    usage = "laue.optimize_indexing [options] monochromatic.expt monochromatic.refl"
 
     parser = ArgumentParser(
         usage=usage,
         phil=phil,
         read_reflections=True,
         read_experiments=True,
         check_format=False,
         epilog=help_message,
     )
 
-    params, options = parser.parse_args(args=args, show_diff_phil=False)
+    params, options = parser.parse_args(args=args, show_diff_phil=True)
 
     # Configure logging
     log.config(verbosity=options.verbose, logfile=params.output.log)
 
     # Log diff phil
     diff_phil = parser.diff_phil.as_str()
     if diff_phil != "":
         logger.info("The following parameters have been modified:\n")
         logger.info(diff_phil)
 
     reflections, experiments = reflections_and_experiments_from_files(
         params.input.reflections, params.input.experiments
     )
+    reflections = reflections[0]  # Get reflection table out of list
 
     # Sanity checks
     if len(experiments) == 0:
         parser.print_help()
         return
 
     # Loop over input files
+    total_experiments = ExperimentList()
+    total_reflections = reflection_table()
     for i in range(len(experiments)):
         # Reindex data
         print(f"Reindexing experiment {i}.")
+        j = int(experiments[i].identifier)
         indexed_experiments, indexed_reflections = index_image(
-            params, reflections[i], experiments[i]
+            params, reflections.select(reflections["id"] == j), experiments[i]
         )
+        total_experiments.extend(indexed_experiments)
+        total_reflections.extend(indexed_reflections)
 
-        # Save experiments
-        logger.info("Saving optimized experiments to %s", params.output.experiments)
-        indexed_experiments.as_file(params.output.experiments)
-
-        # Save reflections
-        logger.info("Saving optimized reflections to %s", params.output.reflections)
-        indexed_reflections.as_file(filename=params.output.reflections)
+    # Save experiments
+    logger.info("Saving optimized experiments to %s", params.output.experiments)
+    total_experiments.as_file(params.output.experiments)
+
+    # Save reflections
+    logger.info("Saving optimized reflections to %s", params.output.reflections)
+    total_reflections.as_file(filename=params.output.reflections)
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `laue_dials-0.1.4/src/laue_dials/skeleton.py` & `laue_dials-0.2/src/laue_dials/skeleton.py`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.4/src/laue_dials.egg-info/PKG-INFO` & `laue_dials-0.2/src/laue_dials.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: laue-dials
-Version: 0.1.4
+Version: 0.2
 Summary: A package for analyzing Laue x-ray crystallography data using the DIALS framework.
 Home-page: https://github.com/rs-station/laue_dials
 Author: Rick A. Hewitt
 Author-email: rahewitt@g.harvard.edu
 License: MIT
-Platform: any
+Platform: Mac
+Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE.txt
 
@@ -27,41 +28,55 @@
    :target: https://codecov.io/gh/rs-station/laue-dials
 
 .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :alt: MIT License
    :target: https://github.com/rs-station/laue-dials/blob/main/LICENSE.txt
 
 ==========
-laue_dials
+laue-dials
 ==========
 
 Data analysis package for Laue crystallography.
 
-``laue_dials`` is an extension to the `DIALS`_ code for analyzing polychromatic crystallographic data.
+``laue-dials`` is an extension to the `DIALS`_ code for analyzing polychromatic crystallographic data.
 Building off the ``DIALS`` framework, and including modern tools like ``numpy``, ``scipy``, and
 ``reciprocalspaceship``, this package allows for analysis of X-ray crystallographic data using
 wide-bandwidth light sources. This package is intended to be used in conjunction with `DIALS`_,
 `careless`_, and `Phenix`_ in order to generate molecular models from raw data.
 
 ============
 Installation
 ============
 
-To install ``laue_dials``, the DIALS code must first be installed using
+To install ``laue-dials``, the DIALS code must first be installed using
 
 .. code:: python
 
    conda install -c conda-forge dials
 
 Then, using the DIALS python environment, run the following:
 
 .. code:: python
 
    pip install laue-dials
 
-If any issues occur either with installation or use of the software, please file an issue at `issue tracker`_.
+``laue-dials`` consists of seven command-line scripts for the processing of Laue diffraction data, which are
+
+.. code:: python
+
+   laue.initial_solution
+   laue.sequence_to_stills
+   laue.optimize_indexing
+   laue.refine
+   laue.predict
+   laue.integrate
+   laue.combine_mtzs
+
+Note that you need to import the image data using ``dials.import``. For information on how to use this command, visit https://dials.github.io/documentation/programs/dials_import.html. An example of how to analyze a full dataset lives at https://github.com/rs-station/laue-dials/blob/main/examples/pipeline.sh.
+
+If any issues occur either with installation or use of the software, please file an issue at `issue tracker`_. Any and all questions, concerns, or feature requests are welcome.
 
 .. _careless: https://github.com/rs-station/careless
 .. _DIALS: https://dials.github.io/index.html
-.. _issue tracker: https://github.com/rs-station/laue_dials/issues
+.. _issue tracker: https://github.com/rs-station/laue-dials/issues
 .. _Phenix: http://www.phenix-online.org
 .. _reciprocalspaceship: https://github.com/rs-station/reciprocalspaceship
```

### Comparing `laue_dials-0.1.4/src/laue_dials.egg-info/SOURCES.txt` & `laue_dials-0.2/src/laue_dials.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -26,33 +26,36 @@
 docs/requirements.txt
 docs/_static/.gitignore
 docs/api/laue_dials.algorithms.rst
 docs/api/laue_dials.command_line.rst
 docs/api/laue_dials.rst
 docs/api/laue_dials.utils.rst
 docs/api/modules.rst
-examples/initial_solution.py
-examples/pipeline.py
+examples/pipeline.sh
 src/laue_dials/__init__.py
 src/laue_dials/skeleton.py
 src/laue_dials.egg-info/PKG-INFO
 src/laue_dials.egg-info/SOURCES.txt
 src/laue_dials.egg-info/dependency_links.txt
 src/laue_dials.egg-info/entry_points.txt
 src/laue_dials.egg-info/not-zip-safe
 src/laue_dials.egg-info/requires.txt
 src/laue_dials.egg-info/top_level.txt
 src/laue_dials/algorithms/diffgeo.py
+src/laue_dials/algorithms/integration.py
 src/laue_dials/algorithms/laue.py
+src/laue_dials/algorithms/monochromatic.py
 src/laue_dials/algorithms/outliers.py
+src/laue_dials/command_line/combine_mtzs.py
 src/laue_dials/command_line/initial_solution.py
 src/laue_dials/command_line/integrate.py
 src/laue_dials/command_line/optimize_indexing.py
 src/laue_dials/command_line/predict.py
 src/laue_dials/command_line/refine.py
+src/laue_dials/command_line/sequence_to_stills.py
 src/laue_dials/utils/expt_utils.py
 src/laue_dials/utils/plots.py
 src/laue_dials/utils/refl_utils.py
 tests/conftest.py
 tests/test_initial_solution.py
 tests/test_skeleton.py
 tests/algorithms/test_diffgeo.py
```

### Comparing `laue_dials-0.1.4/tests/algorithms/test_diffgeo.py` & `laue_dials-0.2/tests/algorithms/test_diffgeo.py`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.4/tests/algorithms/test_laue.py` & `laue_dials-0.2/tests/algorithms/test_laue.py`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.4/tests/test_skeleton.py` & `laue_dials-0.2/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `laue_dials-0.1.4/tox.ini` & `laue_dials-0.2/tox.ini`

 * *Files identical despite different names*

