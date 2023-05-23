# Comparing `tmp/torchgfn-0.1.0.tar.gz` & `tmp/torchgfn-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchgfn-0.1.0.tar", max compression
+gzip compressed data, was "torchgfn-0.1.1.tar", max compression
```

## Comparing `torchgfn-0.1.0.tar` & `torchgfn-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    14216 2023-05-23 21:32:03.667263 torchgfn-0.1.0/README.md
--rw-r--r--   0        0        0     3012 2023-05-23 21:57:56.845827 torchgfn-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      144 2023-05-23 20:35:01.088805 torchgfn-0.1.0/src/gfn/__init__.py
--rw-r--r--   0        0        0      103 2023-05-23 20:35:01.088947 torchgfn-0.1.0/src/gfn/containers/__init__.py
--rw-r--r--   0        0        0     2153 2023-05-03 09:42:02.656970 torchgfn-0.1.0/src/gfn/containers/base.py
--rw-r--r--   0        0        0     3584 2023-05-23 20:35:01.089079 torchgfn-0.1.0/src/gfn/containers/replay_buffer.py
--rw-r--r--   0        0        0    13197 2023-05-23 20:35:01.089208 torchgfn-0.1.0/src/gfn/containers/states.py
--rw-r--r--   0        0        0    11797 2023-05-23 20:35:01.089381 torchgfn-0.1.0/src/gfn/containers/trajectories.py
--rw-r--r--   0        0        0     7389 2023-05-23 20:35:01.089531 torchgfn-0.1.0/src/gfn/containers/transitions.py
--rw-r--r--   0        0        0     3593 2023-05-23 20:35:01.089668 torchgfn-0.1.0/src/gfn/distributions.py
--rw-r--r--   0        0        0       95 2023-05-23 20:35:01.089795 torchgfn-0.1.0/src/gfn/envs/__init__.py
--rw-r--r--   0        0        0     7424 2023-05-23 20:35:01.089960 torchgfn-0.1.0/src/gfn/envs/discrete_ebm.py
--rw-r--r--   0        0        0     8212 2023-05-23 20:35:01.090104 torchgfn-0.1.0/src/gfn/envs/env.py
--rw-r--r--   0        0        0     8634 2023-05-23 20:35:01.090270 torchgfn-0.1.0/src/gfn/envs/hypergrid.py
--rw-r--r--   0        0        0      125 2022-11-08 17:34:55.632486 torchgfn-0.1.0/src/gfn/envs/preprocessors/__init__.py
--rw-r--r--   0        0        0     1852 2023-05-23 20:35:01.090410 torchgfn-0.1.0/src/gfn/envs/preprocessors/base.py
--rw-r--r--   0        0        0     2268 2023-05-23 20:35:01.090537 torchgfn-0.1.0/src/gfn/envs/preprocessors/hot.py
--rw-r--r--   0        0        0     6545 2023-05-23 20:35:01.090676 torchgfn-0.1.0/src/gfn/estimators.py
--rw-r--r--   0        0        0      481 2023-04-28 10:00:41.421203 torchgfn-0.1.0/src/gfn/losses/__init__.py
--rw-r--r--   0        0        0     9125 2023-05-23 20:35:01.090853 torchgfn-0.1.0/src/gfn/losses/base.py
--rw-r--r--   0        0        0     6150 2023-05-23 20:35:01.091029 torchgfn-0.1.0/src/gfn/losses/detailed_balance.py
--rw-r--r--   0        0        0     4939 2023-05-23 20:35:01.091493 torchgfn-0.1.0/src/gfn/losses/flow_matching.py
--rw-r--r--   0        0        0    14025 2023-05-23 20:35:01.091818 torchgfn-0.1.0/src/gfn/losses/sub_trajectory_balance.py
--rw-r--r--   0        0        0     3703 2023-05-23 20:35:01.092021 torchgfn-0.1.0/src/gfn/losses/trajectory_balance.py
--rw-r--r--   0        0        0     5330 2023-05-23 20:35:01.092125 torchgfn-0.1.0/src/gfn/modules.py
--rw-r--r--   0        0        0      172 2023-05-23 20:35:01.092258 torchgfn-0.1.0/src/gfn/samplers/__init__.py
--rw-r--r--   0        0        0     5479 2023-05-23 20:35:01.092400 torchgfn-0.1.0/src/gfn/samplers/actions_samplers.py
--rw-r--r--   0        0        0     4705 2023-05-23 20:35:01.092536 torchgfn-0.1.0/src/gfn/samplers/trajectories_sampler.py
--rw-r--r--   0        0        0     3383 2023-05-23 20:35:01.092650 torchgfn-0.1.0/src/gfn/utils.py
--rw-r--r--   0        0        0    14786 1970-01-01 00:00:00.000000 torchgfn-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    14216 2023-05-23 21:32:03.667263 torchgfn-0.1.1/README.md
+-rw-r--r--   0        0        0     2418 2023-05-23 22:11:41.728345 torchgfn-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      144 2023-05-23 20:35:01.088805 torchgfn-0.1.1/src/gfn/__init__.py
+-rw-r--r--   0        0        0      103 2023-05-23 20:35:01.088947 torchgfn-0.1.1/src/gfn/containers/__init__.py
+-rw-r--r--   0        0        0     2153 2023-05-03 09:42:02.656970 torchgfn-0.1.1/src/gfn/containers/base.py
+-rw-r--r--   0        0        0     3584 2023-05-23 20:35:01.089079 torchgfn-0.1.1/src/gfn/containers/replay_buffer.py
+-rw-r--r--   0        0        0    13197 2023-05-23 20:35:01.089208 torchgfn-0.1.1/src/gfn/containers/states.py
+-rw-r--r--   0        0        0    11797 2023-05-23 20:35:01.089381 torchgfn-0.1.1/src/gfn/containers/trajectories.py
+-rw-r--r--   0        0        0     7389 2023-05-23 20:35:01.089531 torchgfn-0.1.1/src/gfn/containers/transitions.py
+-rw-r--r--   0        0        0     3593 2023-05-23 20:35:01.089668 torchgfn-0.1.1/src/gfn/distributions.py
+-rw-r--r--   0        0        0       95 2023-05-23 20:35:01.089795 torchgfn-0.1.1/src/gfn/envs/__init__.py
+-rw-r--r--   0        0        0     7424 2023-05-23 20:35:01.089960 torchgfn-0.1.1/src/gfn/envs/discrete_ebm.py
+-rw-r--r--   0        0        0     8212 2023-05-23 20:35:01.090104 torchgfn-0.1.1/src/gfn/envs/env.py
+-rw-r--r--   0        0        0     8634 2023-05-23 20:35:01.090270 torchgfn-0.1.1/src/gfn/envs/hypergrid.py
+-rw-r--r--   0        0        0      125 2022-11-08 17:34:55.632486 torchgfn-0.1.1/src/gfn/envs/preprocessors/__init__.py
+-rw-r--r--   0        0        0     1852 2023-05-23 20:35:01.090410 torchgfn-0.1.1/src/gfn/envs/preprocessors/base.py
+-rw-r--r--   0        0        0     2268 2023-05-23 20:35:01.090537 torchgfn-0.1.1/src/gfn/envs/preprocessors/hot.py
+-rw-r--r--   0        0        0     6545 2023-05-23 20:35:01.090676 torchgfn-0.1.1/src/gfn/estimators.py
+-rw-r--r--   0        0        0      481 2023-04-28 10:00:41.421203 torchgfn-0.1.1/src/gfn/losses/__init__.py
+-rw-r--r--   0        0        0     9125 2023-05-23 20:35:01.090853 torchgfn-0.1.1/src/gfn/losses/base.py
+-rw-r--r--   0        0        0     6150 2023-05-23 20:35:01.091029 torchgfn-0.1.1/src/gfn/losses/detailed_balance.py
+-rw-r--r--   0        0        0     4939 2023-05-23 20:35:01.091493 torchgfn-0.1.1/src/gfn/losses/flow_matching.py
+-rw-r--r--   0        0        0    14025 2023-05-23 20:35:01.091818 torchgfn-0.1.1/src/gfn/losses/sub_trajectory_balance.py
+-rw-r--r--   0        0        0     3703 2023-05-23 20:35:01.092021 torchgfn-0.1.1/src/gfn/losses/trajectory_balance.py
+-rw-r--r--   0        0        0     5330 2023-05-23 20:35:01.092125 torchgfn-0.1.1/src/gfn/modules.py
+-rw-r--r--   0        0        0      172 2023-05-23 20:35:01.092258 torchgfn-0.1.1/src/gfn/samplers/__init__.py
+-rw-r--r--   0        0        0     5479 2023-05-23 20:35:01.092400 torchgfn-0.1.1/src/gfn/samplers/actions_samplers.py
+-rw-r--r--   0        0        0     4705 2023-05-23 20:35:01.092536 torchgfn-0.1.1/src/gfn/samplers/trajectories_sampler.py
+-rw-r--r--   0        0        0     3383 2023-05-23 20:35:01.092650 torchgfn-0.1.1/src/gfn/utils.py
+-rw-r--r--   0        0        0    14870 1970-01-01 00:00:00.000000 torchgfn-0.1.1/PKG-INFO
```

### Comparing `torchgfn-0.1.0/README.md` & `torchgfn-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/pyproject.toml` & `torchgfn-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,53 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.setuptools]
-package-dir = {"" = "src"}
-packages = [
-    "gfn",
-]
-
-[tool.setuptools.package-data]
-"*" = [
-    "*.txt"
-]
-
-[project]
-name = "gfn"
-version = "0.1.0"
-
-authors = [
-  { name="Salem Lahou", email="salemlahlou9@gmail.com" },
-  { name="Joseph Viviano", email="joseph@viviano.ca" },
-  { name="Victor Schmidt", email="schmidtv@mila.quebec" },
-]
 
-description = "A Python package for GFlowNets"
+[tool.poetry]
+name = "torchgfn"
+packages = [{include = "gfn", from = "src"}]
+version = "0.1.1"
+description = "A torch inplementation of GFlowNets"
+authors = ["Salem Lahou <salemlahlou9@gmail.com>", "Joseph Viviano <joseph@viviano.ca>", "Victor Schmidt <vsch@pm.me>"]
+license = "MIT"
 readme = "README.md"
-requires-python = ">=3.10"
-
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
-dependencies = [
-    "einops",
-    "gymnasium",
-    "numpy",
-    "torch",
-    "torchtyping",
-]
+[tool.poetry.dependencies]
+python = "^3.10"
+einops = ">=0.6.1"
+gymnasium = ">=0.28.1"
+numpy = ">=1.21.2"
+torch = ">=1.9.0"
+torchtyping = ">=0.1.4"
 
 
-[project.optional-dependencies]
-scripts = [
-    "simple-parsing==0.0.20",
-    "tqdm",
-    "wandb",
-]
+[tool.poetry.group.scripts.dependencies] 
+simple-parsing = "0.0.20"
+tqdm = "*"
+wandb = "*"
+
+
+[tool.poetry.group.dev.dependencies] 
+black = "22.3.0"
+myst-parser = "0.18.1"
+pre-commit = "*"
+pytest = "*"
+renku-sphinx-theme = "*"
+sphinx_rtd_theme = "1.1.1"
+sphinx-autoapi = "2.0.0"
+sphinx-math-dollar = "1.2.1"
+sphinx = "5.3.0"
+tox = "*"
 
-dev = [
-    "black==22.3.0",
-    "myst-parser==0.18.1",
-    "pre-commit",
-    "pytest",
-    "renku-sphinx-theme",
-    "sphinx_rtd_theme==1.1.1",
-    "sphinx-autoapi==2.0.0",
-    "sphinx-math-dollar==1.2.1",
-    "sphinx==5.3.0",
-    "tox",
-]
 
 [project.urls]
 "Homepage" = "https://gfn.readthedocs.io/en/latest/"
 "Bug Tracker" = "https://github.com/saleml/gfn/issues"
 
 
 # TODO: Could use for examples? Or something else?
@@ -117,33 +100,14 @@
 reportUntypedFunctionDecorator = "none"
 reportMissingTypeStubs = false
 reportUnboundVariable = "warning"
 reportGeneralTypeIssues = "none"
 
 [tool.pytest.ini_options]
 
-[tool.poetry]
-name = "torchgfn"
-packages = [{include = "gfn", from = "src"}]
-version = "0.1.0"
-description = "A torch inplementation of GFlowNets"
-authors = ["Salem Lahou <salemlahlou9@gmail.com>", "Joseph Viviano <joseph@viviano.ca>", "Victor Schmidt <vsch@pm.me>"]
-license = "MIT"
-readme = "README.md"
-
-[tool.poetry.dependencies]
-python = "^3.10"
-einops = ">=0.6.1"
-gymnasium = ">=0.28.1"
-numpy = ">=1.21.2"
-torch = ">=1.9.0"
-
-[tool.poetry.group.dev.dependencies]
-torchtyping = ">=0.1.4"
-
 
 # Black-compatibility enforced.
 [tool.isort]
 line_length = 89
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
```

### Comparing `torchgfn-0.1.0/src/gfn/containers/base.py` & `torchgfn-0.1.1/src/gfn/containers/base.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/src/gfn/containers/replay_buffer.py` & `torchgfn-0.1.1/src/gfn/containers/replay_buffer.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/src/gfn/containers/states.py` & `torchgfn-0.1.1/src/gfn/containers/states.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/src/gfn/containers/trajectories.py` & `torchgfn-0.1.1/src/gfn/containers/trajectories.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/src/gfn/containers/transitions.py` & `torchgfn-0.1.1/src/gfn/containers/transitions.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/src/gfn/distributions.py` & `torchgfn-0.1.1/src/gfn/distributions.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/src/gfn/envs/discrete_ebm.py` & `torchgfn-0.1.1/src/gfn/envs/discrete_ebm.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/src/gfn/envs/env.py` & `torchgfn-0.1.1/src/gfn/envs/env.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/src/gfn/envs/hypergrid.py` & `torchgfn-0.1.1/src/gfn/envs/hypergrid.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/src/gfn/envs/preprocessors/base.py` & `torchgfn-0.1.1/src/gfn/envs/preprocessors/base.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/src/gfn/envs/preprocessors/hot.py` & `torchgfn-0.1.1/src/gfn/envs/preprocessors/hot.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/src/gfn/estimators.py` & `torchgfn-0.1.1/src/gfn/estimators.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/src/gfn/losses/base.py` & `torchgfn-0.1.1/src/gfn/losses/base.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/src/gfn/losses/detailed_balance.py` & `torchgfn-0.1.1/src/gfn/losses/detailed_balance.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/src/gfn/losses/flow_matching.py` & `torchgfn-0.1.1/src/gfn/losses/flow_matching.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/src/gfn/losses/sub_trajectory_balance.py` & `torchgfn-0.1.1/src/gfn/losses/sub_trajectory_balance.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/src/gfn/losses/trajectory_balance.py` & `torchgfn-0.1.1/src/gfn/losses/trajectory_balance.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/src/gfn/modules.py` & `torchgfn-0.1.1/src/gfn/modules.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/src/gfn/samplers/actions_samplers.py` & `torchgfn-0.1.1/src/gfn/samplers/actions_samplers.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/src/gfn/samplers/trajectories_sampler.py` & `torchgfn-0.1.1/src/gfn/samplers/trajectories_sampler.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/src/gfn/utils.py` & `torchgfn-0.1.1/src/gfn/utils.py`

 * *Files identical despite different names*

### Comparing `torchgfn-0.1.0/PKG-INFO` & `torchgfn-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: torchgfn
-Version: 0.1.0
+Version: 0.1.1
 Summary: A torch inplementation of GFlowNets
 License: MIT
 Author: Salem Lahou
 Author-email: salemlahlou9@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: einops (>=0.6.1)
 Requires-Dist: gymnasium (>=0.28.1)
 Requires-Dist: numpy (>=1.21.2)
 Requires-Dist: torch (>=1.9.0)
+Requires-Dist: torchtyping (>=0.1.4)
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a>
 	    <img src='https://img.shields.io/badge/python-3.10%2B-blueviolet' alt='Python' />
 	</a>
 	<a href='https://gfn.readthedocs.io/en/latest/?badge=latest'>
```

