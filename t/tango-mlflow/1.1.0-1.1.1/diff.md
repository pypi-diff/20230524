# Comparing `tmp/tango_mlflow-1.1.0.tar.gz` & `tmp/tango_mlflow-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tango_mlflow-1.1.0.tar", max compression
+gzip compressed data, was "tango_mlflow-1.1.1.tar", max compression
```

## Comparing `tango_mlflow-1.1.0.tar` & `tango_mlflow-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1064 2023-05-18 17:12:06.213088 tango_mlflow-1.1.0/LICENSE
--rw-r--r--   0        0        0     5364 2023-05-18 17:12:06.213088 tango_mlflow-1.1.0/README.md
--rw-r--r--   0        0        0     1908 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       78 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/__init__.py
--rw-r--r--   0        0        0      129 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/__main__.py
--rw-r--r--   0        0        0      569 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/commands/__init__.py
--rw-r--r--   0        0        0     3633 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/commands/subcommand.py
--rw-r--r--   0        0        0    12913 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/commands/tune.py
--rw-r--r--   0        0        0     6306 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/flax_train_callback.py
--rw-r--r--   0        0        0        0 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/py.typed
--rw-r--r--   0        0        0     1988 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/step.py
--rw-r--r--   0        0        0     6536 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/step_cache.py
--rw-r--r--   0        0        0     7535 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/torch_train_callback.py
--rw-r--r--   0        0        0    11867 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/util.py
--rw-r--r--   0        0        0    18306 2023-05-18 17:12:06.217088 tango_mlflow-1.1.0/tango_mlflow/workspace.py
--rw-r--r--   0        0        0     6330 1970-01-01 00:00:00.000000 tango_mlflow-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-24 15:18:38.525915 tango_mlflow-1.1.1/LICENSE
+-rw-r--r--   0        0        0     5551 2023-05-24 15:18:38.525915 tango_mlflow-1.1.1/README.md
+-rw-r--r--   0        0        0     1912 2023-05-24 15:18:38.529915 tango_mlflow-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-05-24 15:18:38.529915 tango_mlflow-1.1.1/tango_mlflow/__init__.py
+-rw-r--r--   0        0        0      129 2023-05-24 15:18:38.529915 tango_mlflow-1.1.1/tango_mlflow/__main__.py
+-rw-r--r--   0        0        0      569 2023-05-24 15:18:38.529915 tango_mlflow-1.1.1/tango_mlflow/commands/__init__.py
+-rw-r--r--   0        0        0     3633 2023-05-24 15:18:38.529915 tango_mlflow-1.1.1/tango_mlflow/commands/subcommand.py
+-rw-r--r--   0        0        0    12913 2023-05-24 15:18:38.529915 tango_mlflow-1.1.1/tango_mlflow/commands/tune.py
+-rw-r--r--   0        0        0     6306 2023-05-24 15:18:38.529915 tango_mlflow-1.1.1/tango_mlflow/flax_train_callback.py
+-rw-r--r--   0        0        0        0 2023-05-24 15:18:38.529915 tango_mlflow-1.1.1/tango_mlflow/py.typed
+-rw-r--r--   0        0        0     1988 2023-05-24 15:18:38.529915 tango_mlflow-1.1.1/tango_mlflow/step.py
+-rw-r--r--   0        0        0     6536 2023-05-24 15:18:38.529915 tango_mlflow-1.1.1/tango_mlflow/step_cache.py
+-rw-r--r--   0        0        0     7535 2023-05-24 15:18:38.529915 tango_mlflow-1.1.1/tango_mlflow/torch_train_callback.py
+-rw-r--r--   0        0        0    11867 2023-05-24 15:18:38.529915 tango_mlflow-1.1.1/tango_mlflow/util.py
+-rw-r--r--   0        0        0    19850 2023-05-24 15:18:38.529915 tango_mlflow-1.1.1/tango_mlflow/workspace.py
+-rw-r--r--   0        0        0     6513 1970-01-01 00:00:00.000000 tango_mlflow-1.1.1/PKG-INFO
```

### Comparing `tango_mlflow-1.1.0/LICENSE` & `tango_mlflow-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.1.0/README.md` & `tango_mlflow-1.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 MLflow integration for [ai2-tango](https://github.com/allenai/tango)
 
 ## Introduction
 
 `tango-mlflow` is a Python library that connects the [Tango](https://github.com/allenai/tango) to [MLflow](https://mlflow.org/).
 Tango, developed by AllenAI, is a flexible pipeline library for managing experiments and caching outputs of each step.
 MLflow, on the other hand, is a platform that helps manage the Machine Learning lifecycle, including experimentation, reproducibility, and deployment.
-
 This integration enables you to store and manage complete experimental settings and artifacts of your Tango run in MLflow, thus enhancing your experiment tracking capabilities.
 
 Here's a screenshot of the MLflow interface when executing with `tango-mlflow`:
 
 ![239279085-79ca2c6b-f9a1-49aa-a301-bb502a2340d2](https://github.com/altescy/tango-mlflow/assets/16734471/d41c6d08-faec-4ea0-8b23-fbc8c6147626)
 
 - **Tango run**: The top-level run in MLflow corresponds to a single execution in Tango, and its name matches the execution name in Tango.
@@ -24,23 +23,23 @@
 - **Parameters and Metrics**: The entire settings for the execution, as well as the parameters for each step, are automatically logged in MLflow.
 - **Artifacts and Caching**: The cached outputs of each step's execution are saved as artifacts under the corresponding MLflow run. These can be reused when executing Tango, enhancing efficiency and reproducibility.
 
 ## Installation
 
 Install `tango-mlflow` by running the following command in your terminal:
 
-```bash
+```shell
 pip install tango-mlflow[all]
 ```
 
 ## Usage
 
 You can use the `MLFlowWorkspace` with command line arguments as follows:
 
-```bash
+```shell
 tango run --workspace mlflow://your_experiment_name --include-package tango_mlflow
 ```
 
 Alternatively, you can define your configuration in a `tango.yml` file:
 
 ```tango.yml
 workspace:
@@ -52,14 +51,20 @@
 ```
 
 In the above `tango.yml` configuration, `type` specifies the workspace type as MLflow, and `experiment_name` sets the name of your experiment in MLflow.
 The `include_package` field needs to include the `tango_mlflow` package to use `tango-mlflow` functionality.
 
 Remember to replace `your_experiment_name` with the name of your specific experiment.
 
+To log runs remotely, set the `MLFLOW_TRACKING_URI` environment variable to a tracking server’s URI like below:
+
+```shell
+export MLFLOW_TRACKING_URI=https://mlflow.example.com
+```
+
 ## Functionalities
 
 ### Logging metrics into MLflow
 
 The `tango-mlflow` package provides the `MLflowStep` class, which allows you to easily log the results of each step execution to MLflow.
 
 ```python
@@ -79,15 +84,15 @@
 
         # post-process...
 ```
 
 In the example above, the `TrainModel` step inherits from `MLflowStep`.
 Inside the step, you can directly record metrics to the corresponding MLflow run by invoking `self.mlflow_logger.log_metric(...)`.
 
-Please note, this functionality must be used in conjunction with MLFlowWorkspace.
+Please note, this functionality must be used in conjunction with `MLFlowWorkspace`.
 
 ### Summarizing Tango run metrics
 
 You can specify a step to record its returned metrics as representative values of the Tango run by setting the class variable `MLFLOW_SUMMARY = True`.
 This feature enables you to conveniently view metrics for each Tango run directly in the MLflow interface
 
 ```python
@@ -95,21 +100,21 @@
     MLFLOW_SUMMARY = True  # Enables MLflow summary!
 
     def run(self, ...) -> dict[str, float]:
         # compute metrics ...
         return metrics
 ```
 
-In the example above, the EvaluateModel step returns metrics that are logged as the representative values for that Tango run. These metrics are then recorded in the corresponding (top-level) MLflow run.
+In the example above, the `EvaluateModel` step returns metrics that are logged as the representative values for that Tango run. These metrics are then recorded in the corresponding (top-level) MLflow run.
 
 Please note the following requirements:
 - The return value of a step where `MLFLOW_SUMMARY = True` is set must always be `dict[str, float]`.
 - You don't necessarily need to inherit from `MLflowStep` to use `MLFLOW_SUMMARY`.
 
-### Tuning hyper-parameters with Optuna
+### Tuning hyperparameters with Optuna
 
 `tango-mlflow` also provides the `tango-mlflow tune` command for tuning hyperparameters with [Optuna](https://optuna.org/).
 For more details, please refer to the [examples/breast_cancer](https://github.com/altescy/tango-mlflow/tree/main/examples/breast_cancer) directory.
 
 ## Examples
 
 - Basic example: [examples/euler](https://github.com/altescy/tango-mlflow/tree/main/examples/euler)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tango_mlflow-1.1.0/pyproject.toml` & `tango_mlflow-1.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tango-mlflow"
-version = "1.1.0"
+version = "1.1.1"
 description = "MLflow integration for ai2-tango"
 authors = ["altescy <altescy@fastmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/altescy/tango-mlflow"
 keywords=["python", "mlflow", "machine-learning"]
 
@@ -12,15 +12,15 @@
 tango-mlflow = "tango_mlflow.__main__:run"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 ai2-tango = "^1.0.0"
 mlflow = ">=1.28,<3.0"
 optuna = {version = "^3.0.5", optional = true}
-torch = {version = "^2.0.0", optional = true}
+torch = {version = ">=1.9,<2.1", optional = true}
 flax = {version = "^0.6.8", optional = true}
 
 [tool.poetry.dev-dependencies]
 python-language-server = "^0.36.2"
 pytest = "^7.3.1"
 pysen = "^0.10.4"
 black = "^23.3.0"
```

### Comparing `tango_mlflow-1.1.0/tango_mlflow/commands/__init__.py` & `tango_mlflow-1.1.1/tango_mlflow/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.1.0/tango_mlflow/commands/subcommand.py` & `tango_mlflow-1.1.1/tango_mlflow/commands/subcommand.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.1.0/tango_mlflow/commands/tune.py` & `tango_mlflow-1.1.1/tango_mlflow/commands/tune.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.1.0/tango_mlflow/flax_train_callback.py` & `tango_mlflow-1.1.1/tango_mlflow/flax_train_callback.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.1.0/tango_mlflow/step.py` & `tango_mlflow-1.1.1/tango_mlflow/step.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.1.0/tango_mlflow/step_cache.py` & `tango_mlflow-1.1.1/tango_mlflow/step_cache.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.1.0/tango_mlflow/torch_train_callback.py` & `tango_mlflow-1.1.1/tango_mlflow/torch_train_callback.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.1.0/tango_mlflow/util.py` & `tango_mlflow-1.1.1/tango_mlflow/util.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.1.0/tango_mlflow/workspace.py` & `tango_mlflow-1.1.1/tango_mlflow/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,19 +140,47 @@
         lock_path = self.step_dir(step) / "lock"
         lock = FileLock(lock_path, read_only_ok=True)
         lock.acquire_with_updates(desc=f"acquiring lock for '{step.name}'")
         self.locks[step] = lock
 
         step_info = self._get_updated_step_info(step.unique_id) or StepInfo.new_from_step(step)
         if step_info.state not in {StepState.INCOMPLETE, StepState.FAILED, StepState.UNCACHEABLE}:
+            mlflow_run = get_mlflow_run_by_tango_step(self.mlflow_client, self.experiment_name, step_info)
+            if not mlflow_run:
+                raise RuntimeError(
+                    f"Could not find mlflow run for step {step.unique_id}. There is a possibility that"
+                    " the run was deleted or modified during the execution. Please try again."
+                )
+            if step_info.state == StepState.RUNNING:
+                raise StepStateError(
+                    step,
+                    step_info.state,
+                    context=(
+                        "This step is already running. If you are certain the step is not running somewhere else,"
+                        " it seems that this step was accidentally killed in a previous run. In this case, please"
+                        f" delete the mlflow run ({mlflow_run.info.run_id}) for this step and try again."
+                    ),
+                )
+            if step_info.state == StepState.COMPLETED:
+                raise StepStateError(
+                    step,
+                    step_info.state,
+                    context=(
+                        "This step has already been completed in a previous run. Please rerun this step, and the"
+                        " cached result will be used. If this error persists, please open an issue from here:"
+                        " https://github.com/altescy/tango-mlflow/issues/new"
+                    ),
+                )
             raise StepStateError(
                 step,
                 step_info.state,
-                context="If you are certain the step is not running somewhere else, delete the lock "
-                f"file at {lock_path}.",
+                context=(
+                    "Unknown step state is detected. Please open an issue from here:"
+                    " https://github.com/altescy/tango-mlflow/issues/new"
+                ),
             )
 
         try:
             step_info.start_time = utc_now_datetime()
             step_info.end_time = None
             step_info.error = None
             step_info.result_location = None
```

### Comparing `tango_mlflow-1.1.0/PKG-INFO` & `tango_mlflow-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tango-mlflow
-Version: 1.1.0
+Version: 1.1.1
 Summary: MLflow integration for ai2-tango
 Home-page: https://github.com/altescy/tango-mlflow
 License: MIT
 Keywords: python,mlflow,machine-learning
 Author: altescy
 Author-email: altescy@fastmail.com
 Requires-Python: >=3.8.1,<4.0
@@ -17,15 +17,15 @@
 Provides-Extra: flax
 Provides-Extra: optuna
 Provides-Extra: torch
 Requires-Dist: ai2-tango (>=1.0.0,<2.0.0)
 Requires-Dist: flax (>=0.6.8,<0.7.0) ; extra == "flax" or extra == "all"
 Requires-Dist: mlflow (>=1.28,<3.0)
 Requires-Dist: optuna (>=3.0.5,<4.0.0) ; extra == "optuna" or extra == "all"
-Requires-Dist: torch (>=2.0.0,<3.0.0) ; extra == "torch" or extra == "all"
+Requires-Dist: torch (>=1.9,<2.1) ; extra == "torch" or extra == "all"
 Description-Content-Type: text/markdown
 
 # tango-mlflow
 
 [![Actions Status](https://github.com/altescy/tango-mlflow/workflows/CI/badge.svg)](https://github.com/altescy/tango-mlflow/actions/workflows/ci.yml)
 [![Python version](https://img.shields.io/pypi/pyversions/tango-mlflow)](https://github.com/altescy/tango-mlflow)
 [![pypi version](https://img.shields.io/pypi/v/tango-mlflow)](https://pypi.org/project/tango-mlflow/)
@@ -34,15 +34,14 @@
 MLflow integration for [ai2-tango](https://github.com/allenai/tango)
 
 ## Introduction
 
 `tango-mlflow` is a Python library that connects the [Tango](https://github.com/allenai/tango) to [MLflow](https://mlflow.org/).
 Tango, developed by AllenAI, is a flexible pipeline library for managing experiments and caching outputs of each step.
 MLflow, on the other hand, is a platform that helps manage the Machine Learning lifecycle, including experimentation, reproducibility, and deployment.
-
 This integration enables you to store and manage complete experimental settings and artifacts of your Tango run in MLflow, thus enhancing your experiment tracking capabilities.
 
 Here's a screenshot of the MLflow interface when executing with `tango-mlflow`:
 
 ![239279085-79ca2c6b-f9a1-49aa-a301-bb502a2340d2](https://github.com/altescy/tango-mlflow/assets/16734471/d41c6d08-faec-4ea0-8b23-fbc8c6147626)
 
 - **Tango run**: The top-level run in MLflow corresponds to a single execution in Tango, and its name matches the execution name in Tango.
@@ -50,23 +49,23 @@
 - **Parameters and Metrics**: The entire settings for the execution, as well as the parameters for each step, are automatically logged in MLflow.
 - **Artifacts and Caching**: The cached outputs of each step's execution are saved as artifacts under the corresponding MLflow run. These can be reused when executing Tango, enhancing efficiency and reproducibility.
 
 ## Installation
 
 Install `tango-mlflow` by running the following command in your terminal:
 
-```bash
+```shell
 pip install tango-mlflow[all]
 ```
 
 ## Usage
 
 You can use the `MLFlowWorkspace` with command line arguments as follows:
 
-```bash
+```shell
 tango run --workspace mlflow://your_experiment_name --include-package tango_mlflow
 ```
 
 Alternatively, you can define your configuration in a `tango.yml` file:
 
 ```tango.yml
 workspace:
@@ -78,14 +77,20 @@
 ```
 
 In the above `tango.yml` configuration, `type` specifies the workspace type as MLflow, and `experiment_name` sets the name of your experiment in MLflow.
 The `include_package` field needs to include the `tango_mlflow` package to use `tango-mlflow` functionality.
 
 Remember to replace `your_experiment_name` with the name of your specific experiment.
 
+To log runs remotely, set the `MLFLOW_TRACKING_URI` environment variable to a tracking server’s URI like below:
+
+```shell
+export MLFLOW_TRACKING_URI=https://mlflow.example.com
+```
+
 ## Functionalities
 
 ### Logging metrics into MLflow
 
 The `tango-mlflow` package provides the `MLflowStep` class, which allows you to easily log the results of each step execution to MLflow.
 
 ```python
@@ -105,15 +110,15 @@
 
         # post-process...
 ```
 
 In the example above, the `TrainModel` step inherits from `MLflowStep`.
 Inside the step, you can directly record metrics to the corresponding MLflow run by invoking `self.mlflow_logger.log_metric(...)`.
 
-Please note, this functionality must be used in conjunction with MLFlowWorkspace.
+Please note, this functionality must be used in conjunction with `MLFlowWorkspace`.
 
 ### Summarizing Tango run metrics
 
 You can specify a step to record its returned metrics as representative values of the Tango run by setting the class variable `MLFLOW_SUMMARY = True`.
 This feature enables you to conveniently view metrics for each Tango run directly in the MLflow interface
 
 ```python
@@ -121,21 +126,21 @@
     MLFLOW_SUMMARY = True  # Enables MLflow summary!
 
     def run(self, ...) -> dict[str, float]:
         # compute metrics ...
         return metrics
 ```
 
-In the example above, the EvaluateModel step returns metrics that are logged as the representative values for that Tango run. These metrics are then recorded in the corresponding (top-level) MLflow run.
+In the example above, the `EvaluateModel` step returns metrics that are logged as the representative values for that Tango run. These metrics are then recorded in the corresponding (top-level) MLflow run.
 
 Please note the following requirements:
 - The return value of a step where `MLFLOW_SUMMARY = True` is set must always be `dict[str, float]`.
 - You don't necessarily need to inherit from `MLflowStep` to use `MLFLOW_SUMMARY`.
 
-### Tuning hyper-parameters with Optuna
+### Tuning hyperparameters with Optuna
 
 `tango-mlflow` also provides the `tango-mlflow tune` command for tuning hyperparameters with [Optuna](https://optuna.org/).
 For more details, please refer to the [examples/breast_cancer](https://github.com/altescy/tango-mlflow/tree/main/examples/breast_cancer) directory.
 
 ## Examples
 
 - Basic example: [examples/euler](https://github.com/altescy/tango-mlflow/tree/main/examples/euler)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

