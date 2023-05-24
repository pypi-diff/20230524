# Comparing `tmp/Renate-0.2.1.tar.gz` & `tmp/Renate-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Renate-0.2.1.tar", last modified: Thu May 11 10:21:33 2023, max compression
+gzip compressed data, was "Renate-0.3.0.tar", last modified: Wed May 24 11:34:42 2023, max compression
```

## Comparing `Renate-0.2.1.tar` & `Renate-0.3.0.tar`

### file list

```diff
@@ -1,262 +1,279 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.616688 Renate-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.592688 Renate-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.592688 Renate-0.2.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.592688 Renate-0.2.1/.github/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      488 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/hooks/pre-commit
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.592688 Renate-0.2.1/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)       98 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/scripts/build_docs.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      383 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/scripts/prepend_license.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/workflows/integration_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/workflows/run_renate.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/workflows/run_unit_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-11 10:21:22.000000 Renate-0.2.1/.github/workflows/test_docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-11 10:21:22.000000 Renate-0.2.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-11 10:21:22.000000 Renate-0.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-11 10:21:22.000000 Renate-0.2.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-11 10:21:22.000000 Renate-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-11 10:21:22.000000 Renate-0.2.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-11 10:21:33.616688 Renate-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-05-11 10:21:22.000000 Renate-0.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-11 10:21:22.000000 Renate-0.2.1/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-11 10:21:22.000000 Renate-0.2.1/dev_setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/doc/_images/
--rw-r--r--   0 runner    (1001) docker     (123)    35105 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/_images/improvement_renate.svg
--rw-r--r--   0 runner    (1001) docker     (123)    34694 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/_images/improvement_tuning.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/doc/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/benchmarking/custom_benchmarks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/benchmarking/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/benchmarking/renate_benchmarks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/doc/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/examples/nlp_finetuning.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/examples/train_classifier_sagemaker.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/examples/train_mlp_locally.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/doc/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/getting_started/avalanche.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/getting_started/how_to_renate_config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/getting_started/how_to_run_training.rst
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/getting_started/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/getting_started/output.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/getting_started/supported_algorithms.rst
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-11 10:21:22.000000 Renate-0.2.1/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.588688 Renate-0.2.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/examples/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/benchmarking/class_incremental_learning_cifar10_der.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/examples/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/getting_started/renate_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/examples/nlp_finetuning/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/nlp_finetuning/renate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/nlp_finetuning/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/examples/simple_classifier_cifar10/
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/simple_classifier_cifar10/renate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/simple_classifier_cifar10/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/simple_classifier_cifar10/start_with_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/simple_classifier_cifar10/start_without_hpo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.596688 Renate-0.2.1/examples/train_mlp_locally/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/train_mlp_locally/renate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/train_mlp_locally/start_training_with_er_without_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/train_mlp_locally/start_training_with_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-11 10:21:22.000000 Renate-0.2.1/examples/train_mlp_locally/start_training_without_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-11 10:21:22.000000 Renate-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-11 10:21:22.000000 Renate-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 10:21:33.616688 Renate-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.588688 Renate-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.600688 Renate-0.2.1/src/Renate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-11 10:21:33.000000 Renate-0.2.1/src/Renate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-05-11 10:21:33.000000 Renate-0.2.1/src/Renate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 10:21:33.000000 Renate-0.2.1/src/Renate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-11 10:21:33.000000 Renate-0.2.1/src/Renate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 10:21:33.000000 Renate-0.2.1/src/Renate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.600688 Renate-0.2.1/src/renate/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.600688 Renate-0.2.1/src/renate/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.600688 Renate-0.2.1/src/renate/benchmark/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/datasets/nlp_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/datasets/vision_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/experiment_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/experimentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.600688 Renate-0.2.1/src/renate/benchmark/models/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/models/vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14995 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/benchmark/scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.600688 Renate-0.2.1/src/renate/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    37040 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/cli/parsing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/cli/run_experiment_with_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/cli/run_remote_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/cli/run_training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.600688 Renate-0.2.1/src/renate/data/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/data/data_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.600688 Renate-0.2.1/src/renate/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/evaluation/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.600688 Renate-0.2.1/src/renate/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/evaluation/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/evaluation/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/evaluation/metrics/performance_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/evaluation/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.600688 Renate-0.2.1/src/renate/memory/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14089 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/memory/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/memory/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.604688 Renate-0.2.1/src/renate/models/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.604688 Renate-0.2.1/src/renate/models/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/models/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/models/layers/cn.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/models/prediction_strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/models/renate_module.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.604688 Renate-0.2.1/src/renate/training/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25769 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/training/training.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.604688 Renate-0.2.1/src/renate/updaters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.604688 Renate-0.2.1/src/renate/updaters/avalanche/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/avalanche/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/avalanche/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    21348 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/avalanche/model_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/avalanche/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.604688 Renate-0.2.1/src/renate/updaters/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49175 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/experimental/er.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/experimental/fine_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/experimental/gdumb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/experimental/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/experimental/offline_er.py
--rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/experimental/repeated_distill.py
--rw-r--r--   0 runner    (1001) docker     (123)    19816 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.604688 Renate-0.2.1/src/renate/updaters/learner_components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/learner_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/learner_components/component.py
--rw-r--r--   0 runner    (1001) docker     (123)    19390 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/learner_components/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/learner_components/reinitialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    16056 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/updaters/model_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.604688 Renate-0.2.1/src/renate/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/utils/avalanche.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/utils/config_spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/utils/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/utils/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-11 10:21:22.000000 Renate-0.2.1/src/renate/utils/syne_tune.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.604688 Renate-0.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-05-11 10:21:22.000000 Renate-0.2.1/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-11 10:21:22.000000 Renate-0.2.1/test/dummy_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.608688 Renate-0.2.1/test/integration_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.592688 Renate-0.2.1/test/integration_tests/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.608688 Renate-0.2.1/test/integration_tests/configs/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/datasets/cifar10.json
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/datasets/cifar100.json
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/datasets/fashionmnist.json
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/datasets/mnist.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.608688 Renate-0.2.1/test/integration_tests/configs/models/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/models/mlp-200.json
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/models/resnet18-cifar.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.608688 Renate-0.2.1/test/integration_tests/configs/scenarios/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/scenarios/class-incremental-2updates.json
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/scenarios/feature-sorting-2updates.json
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/scenarios/hue-shift-2updates.json
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/scenarios/iid-2updates.json
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/scenarios/permutation-2updates.json
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/scenarios/rotation-10updates.json
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/scenarios/rotation-2updates.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.592688 Renate-0.2.1/test/integration_tests/configs/suites/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.608688 Renate-0.2.1/test/integration_tests/configs/suites/quick/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/avalanche-er.json
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/avalanche-ewc.json
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/avalanche-icarl.json
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/avalanche-lwf.json
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/cls-er.json
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/der.json
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/er.json
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/fine-tuning.json
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/gdumb.json
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/joint.json
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/offline-er.json
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/pod-er.json
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/suites/quick/super-er.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/integration_tests/configs/updaters/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/avalanche-er-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/avalanche-ewc.json
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/avalanche-icarl-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/avalanche-lwf.json
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/cls-er-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/der-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/er-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/fine-tuning.json
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/gdumb-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/joint.json
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/offline-er-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/pod-er-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/configs/updaters/super-er-buffer500.json
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/run_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-11 10:21:22.000000 Renate-0.2.1/test/integration_tests/run_quick_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/benchmark/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/benchmark/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/benchmark/models/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/benchmark/models/test_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/benchmark/models/test_vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/benchmark/test_experimentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/benchmark/test_experimentation_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/benchmark/test_scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/cli/test_parsing_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/data/test_data_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/data/test_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.592688 Renate-0.2.1/test/renate/evaluation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/evaluation/metrics/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/evaluation/metrics/test_regression_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/memory/
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/memory/test_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/memory/test_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/models/
--rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/models/test_renate_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/renate_config_files/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/renate_config_files/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/renate_config_files/config_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/test_renate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/training/
--rw-r--r--   0 runner    (1001) docker     (123)    13950 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/training/test_run_training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/updaters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/updaters/avalanche/
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/updaters/avalanche/test_avalanche_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/updaters/avalanche/test_avalanche_model_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/updaters/avalanche/test_avalanche_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.612688 Renate-0.2.1/test/renate/updaters/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/updaters/experimental/test_er.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/updaters/experimental/test_fine_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/updaters/experimental/test_joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/updaters/experimental/test_repeated_distill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/updaters/test_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/updaters/test_model_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:21:33.616688 Renate-0.2.1/test/renate/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/utils/test_avalanche.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/utils/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/utils/test_metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/utils/test_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/utils/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-11 10:21:22.000000 Renate-0.2.1/test/renate/utils/test_syne_tune.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.747138 Renate-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.707137 Renate-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.707137 Renate-0.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.707137 Renate-0.3.0/.github/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      488 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/hooks/pre-commit
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.707137 Renate-0.3.0/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       98 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/scripts/build_docs.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      383 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/scripts/prepend_license.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.707137 Renate-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/workflows/integration_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/workflows/run_renate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/workflows/run_unit_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-24 11:34:28.000000 Renate-0.3.0/.github/workflows/test_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-24 11:34:28.000000 Renate-0.3.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-24 11:34:28.000000 Renate-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-24 11:34:28.000000 Renate-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-24 11:34:28.000000 Renate-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 11:34:28.000000 Renate-0.3.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-05-24 11:34:42.747138 Renate-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-05-24 11:34:28.000000 Renate-0.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-24 11:34:28.000000 Renate-0.3.0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-24 11:34:28.000000 Renate-0.3.0/dev_setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.707137 Renate-0.3.0/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.707137 Renate-0.3.0/doc/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    35105 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/_images/improvement_renate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    34694 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/_images/improvement_tuning.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.711138 Renate-0.3.0/doc/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/benchmarking/custom_benchmarks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/benchmarking/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/benchmarking/renate_benchmarks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.711138 Renate-0.3.0/doc/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/examples/nlp_finetuning.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/examples/train_classifier_sagemaker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/examples/train_mlp_locally.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.711138 Renate-0.3.0/doc/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/getting_started/avalanche.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/getting_started/how_to_renate_config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/getting_started/how_to_run_training.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/getting_started/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/getting_started/output.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/getting_started/shift_detection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/getting_started/supported_algorithms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-24 11:34:28.000000 Renate-0.3.0/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.699138 Renate-0.3.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.711138 Renate-0.3.0/examples/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/benchmarking/class_incremental_learning_cifar10_der.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.711138 Renate-0.3.0/examples/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/getting_started/renate_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.715138 Renate-0.3.0/examples/nlp_finetuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/nlp_finetuning/renate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/nlp_finetuning/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.715138 Renate-0.3.0/examples/shift_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/shift_detection/image_shift_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.715138 Renate-0.3.0/examples/simple_classifier_cifar10/
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/simple_classifier_cifar10/renate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/simple_classifier_cifar10/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/simple_classifier_cifar10/start_with_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/simple_classifier_cifar10/start_without_hpo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.715138 Renate-0.3.0/examples/train_mlp_locally/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/train_mlp_locally/renate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/train_mlp_locally/start_training_with_er_without_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/train_mlp_locally/start_training_with_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-24 11:34:28.000000 Renate-0.3.0/examples/train_mlp_locally/start_training_without_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-24 11:34:28.000000 Renate-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-24 11:34:28.000000 Renate-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 11:34:42.747138 Renate-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.699138 Renate-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.715138 Renate-0.3.0/src/Renate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-05-24 11:34:42.000000 Renate-0.3.0/src/Renate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-05-24 11:34:42.000000 Renate-0.3.0/src/Renate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:34:42.000000 Renate-0.3.0/src/Renate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-24 11:34:42.000000 Renate-0.3.0/src/Renate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 11:34:42.000000 Renate-0.3.0/src/Renate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.715138 Renate-0.3.0/src/renate/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.719138 Renate-0.3.0/src/renate/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.719138 Renate-0.3.0/src/renate/benchmark/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/datasets/nlp_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/datasets/vision_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/datasets/wild_time_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/experiment_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/experimentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.719138 Renate-0.3.0/src/renate/benchmark/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/models/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/models/vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/benchmark/scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.719138 Renate-0.3.0/src/renate/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    37040 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/cli/parsing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/cli/run_experiment_with_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/cli/run_remote_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/cli/run_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.719138 Renate-0.3.0/src/renate/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/data/data_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.723138 Renate-0.3.0/src/renate/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/evaluation/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.723138 Renate-0.3.0/src/renate/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/evaluation/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/evaluation/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/evaluation/metrics/performance_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/evaluation/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.723138 Renate-0.3.0/src/renate/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14089 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/memory/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/memory/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.723138 Renate-0.3.0/src/renate/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.723138 Renate-0.3.0/src/renate/models/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/models/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/models/layers/cn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/models/prediction_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/models/renate_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.723138 Renate-0.3.0/src/renate/shift/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/shift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/shift/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/shift/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/shift/ks_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/shift/mmd_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/shift/mmd_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.723138 Renate-0.3.0/src/renate/training/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26107 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/training/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.727138 Renate-0.3.0/src/renate/updaters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.727138 Renate-0.3.0/src/renate/updaters/avalanche/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/avalanche/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/avalanche/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21348 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/avalanche/model_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/avalanche/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.727138 Renate-0.3.0/src/renate/updaters/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49175 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/experimental/er.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/experimental/fine_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/experimental/gdumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/experimental/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/experimental/offline_er.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/experimental/repeated_distill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19816 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.727138 Renate-0.3.0/src/renate/updaters/learner_components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/learner_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/learner_components/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19390 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/learner_components/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/learner_components/reinitialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16056 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/updaters/model_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.731138 Renate-0.3.0/src/renate/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/utils/avalanche.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/utils/config_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/utils/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/utils/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-24 11:34:28.000000 Renate-0.3.0/src/renate/utils/syne_tune.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.731138 Renate-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-05-24 11:34:28.000000 Renate-0.3.0/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-24 11:34:28.000000 Renate-0.3.0/test/dummy_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.731138 Renate-0.3.0/test/integration_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.703137 Renate-0.3.0/test/integration_tests/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.731138 Renate-0.3.0/test/integration_tests/configs/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/datasets/cifar10.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/datasets/cifar100.json
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/datasets/fashionmnist.json
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/datasets/mnist.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.731138 Renate-0.3.0/test/integration_tests/configs/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/models/mlp-200.json
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/models/resnet18-cifar.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.735138 Renate-0.3.0/test/integration_tests/configs/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/scenarios/class-incremental-2updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/scenarios/feature-sorting-2updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/scenarios/hue-shift-2updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/scenarios/iid-2updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/scenarios/permutation-2updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/scenarios/rotation-10updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/scenarios/rotation-2updates.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.703137 Renate-0.3.0/test/integration_tests/configs/suites/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.735138 Renate-0.3.0/test/integration_tests/configs/suites/quick/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/avalanche-er.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/avalanche-ewc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/avalanche-icarl.json
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/avalanche-lwf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/cls-er.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/der.json
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/er.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/fine-tuning.json
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/gdumb.json
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/joint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/offline-er.json
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/pod-er.json
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/suites/quick/super-er.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.739138 Renate-0.3.0/test/integration_tests/configs/updaters/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/avalanche-er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/avalanche-ewc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/avalanche-icarl-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/avalanche-lwf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/cls-er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/der-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/fine-tuning.json
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/gdumb-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/joint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/offline-er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/pod-er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/configs/updaters/super-er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/run_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-24 11:34:28.000000 Renate-0.3.0/test/integration_tests/run_quick_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.739138 Renate-0.3.0/test/renate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.739138 Renate-0.3.0/test/renate/benchmark/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.739138 Renate-0.3.0/test/renate/benchmark/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/benchmark/models/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/benchmark/models/test_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/benchmark/models/test_vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/benchmark/test_experimentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/benchmark/test_experimentation_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/benchmark/test_scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.739138 Renate-0.3.0/test/renate/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/cli/test_parsing_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.743138 Renate-0.3.0/test/renate/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/data/test_data_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/data/test_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.703137 Renate-0.3.0/test/renate/evaluation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.743138 Renate-0.3.0/test/renate/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/evaluation/metrics/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/evaluation/metrics/test_regression_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.743138 Renate-0.3.0/test/renate/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/memory/test_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/memory/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.743138 Renate-0.3.0/test/renate/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/models/test_renate_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.743138 Renate-0.3.0/test/renate/renate_config_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/renate_config_files/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/renate_config_files/config_scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.743138 Renate-0.3.0/test/renate/shift/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/shift/test_detector_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/shift/test_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/shift/test_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/shift/test_mmd_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/test_renate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.743138 Renate-0.3.0/test/renate/training/
+-rw-r--r--   0 runner    (1001) docker     (123)    13950 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/training/test_run_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.743138 Renate-0.3.0/test/renate/updaters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.743138 Renate-0.3.0/test/renate/updaters/avalanche/
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/updaters/avalanche/test_avalanche_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/updaters/avalanche/test_avalanche_model_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/updaters/avalanche/test_avalanche_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.747138 Renate-0.3.0/test/renate/updaters/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/updaters/experimental/test_er.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/updaters/experimental/test_fine_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/updaters/experimental/test_joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/updaters/experimental/test_repeated_distill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/updaters/test_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/updaters/test_model_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:34:42.747138 Renate-0.3.0/test/renate/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/utils/test_avalanche.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/utils/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/utils/test_metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/utils/test_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/utils/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-24 11:34:28.000000 Renate-0.3.0/test/renate/utils/test_syne_tune.py
```

### Comparing `Renate-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md` & `Renate-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md` & `Renate-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/.github/workflows/codeql.yml` & `Renate-0.3.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/.github/workflows/coverage.yml` & `Renate-0.3.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/.github/workflows/integration_tests.yml` & `Renate-0.3.0/.github/workflows/integration_tests.yml`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/.github/workflows/pypi_publish.yml` & `Renate-0.3.0/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/.github/workflows/run_renate.yml` & `Renate-0.3.0/.github/workflows/run_renate.yml`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 env:
   AWS_DEFAULT_REGION: us-west-2
   SCRIPT_PATH: ${{ inputs.script-path }}
   AWS_ROLE: ${{ secrets.PROD_AWS_END_TO_END_TEST_ROLE_ARN }}
 
 jobs:
   run:
-    runs-on: Renate_ubuntu-latest_16-core
+    runs-on: ubuntu-latest
     timeout-minutes: ${{ inputs.timeout-minutes }}
     steps:
       - name: Configure AWS Credentials (if required)
         if: ${{ inputs.requires-aws-credentials == true }}
         uses: aws-actions/configure-aws-credentials@v2
         with:
           role-to-assume: ${{ secrets.PROD_AWS_END_TO_END_TEST_ROLE_ARN }}
```

### Comparing `Renate-0.2.1/.github/workflows/run_unit_tests.yml` & `Renate-0.3.0/.github/workflows/run_unit_tests.yml`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/.github/workflows/test_docs.yml` & `Renate-0.3.0/.github/workflows/test_docs.yml`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/CONTRIBUTING.md` & `Renate-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/LICENSE` & `Renate-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/PKG-INFO` & `Renate-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: Renate
-Version: 0.2.1
+Version: 0.3.0
 Summary: Library for Continual Learning for Practitioners
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: avalanche
+Provides-Extra: benchmark
 Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
 .. image:: https://img.shields.io/pypi/status/Renate
     :target: #
     :alt: PyPI - Status
```

### Comparing `Renate-0.2.1/README.rst` & `Renate-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/doc/_images/improvement_renate.svg` & `Renate-0.3.0/doc/_images/improvement_renate.svg`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/doc/_images/improvement_tuning.svg` & `Renate-0.3.0/doc/_images/improvement_tuning.svg`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/doc/benchmarking/custom_benchmarks.rst` & `Renate-0.3.0/doc/benchmarking/custom_benchmarks.rst`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 in the last chapter.
 For example, you can combine the :py:class:`~renate.benchmark.scenarios.ClassIncrementalScenario`
 with your data module as follows.
 
 .. code-block:: python
 
     def data_module_fn(
-        data_path: Union[Path, str], chunk_id: int, seed: int, class_groupings: Tuple[Tuple[int]]
+        data_path: str, chunk_id: int, seed: int, class_groupings: Tuple[Tuple[int]]
     ):
         data_module = CustomDataModule(data_path=data_path, seed=seed)
         return ClassIncrementalScenario(
             data_module=data_module,
             class_groupings=class_groupings,
             chunk_id=chunk_id,
         )
```

### Comparing `Renate-0.2.1/doc/benchmarking/index.rst` & `Renate-0.3.0/doc/benchmarking/index.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/doc/benchmarking/renate_benchmarks.rst` & `Renate-0.3.0/doc/benchmarking/renate_benchmarks.rst`

 * *Files 12% similar despite different names*

```diff
@@ -89,14 +89,18 @@
       - * ``num_outputs``: Output dimensionality, for classification the number of classes.
     * - `~renate.benchmark.models.vision_transformer.VisionTransformerL32`
       - Large `Vision Transformer <https://arxiv.org/abs/2010.11929>`_ architecture for images of size 224x224 with patch size 32.
       - * ``num_outputs``: Output dimensionality, for classification the number of classes.
     * - `~renate.benchmark.models.vision_transformer.VisionTransformerH14`
       - Huge `Vision Transformer <https://arxiv.org/abs/2010.11929>`_ architecture for images of size 224x224 with patch size 14.
       - * ``num_outputs``: Output dimensionality, for classification the number of classes.
+    * - `~renate.benchmark.models.transformer.HuggingFaceSequenceClassificationTransformer`
+      - Wrapper around Hugging Face transformers.
+      - * ``pretrained_model_name``: Hugging Face `transformer ID <https://huggingface.co/models>`__.
+        * ``num_outputs``: The number of classes.
 
 
 .. _benchmarking-renate-benchmarks-datasets:
 
 Datasets
 ========
 
@@ -113,30 +117,50 @@
 .. list-table:: Renate Dataset Overview
     :header-rows: 1
 
     * - Dataset Name
       - Task
       - Data Summary
       - Reference
+    * - arxiv
+      - Text Classification: category recognition of arXiv papers.
+      - ~1.9M train, ~206k test, 172 classes, years 2007-2023
+      - Huaxiu Yao et al.: Wild-Time: A Benchmark of in-the-Wild Distribution Shift over Time. Conference on Neural Information Processing Systems Datasets and Benchmarks Track. 2022.
     * - CIFAR10
       - Image Classification
       - 50k train, 10k test, 10 classes, image shape 32x32x3
       - Alex Krizhevsky: Learning Multiple Layers of Features from Tiny Images. 2009.
     * - CIFAR100
       - Image Classification
       - 50k train, 10k test, 100 classes, image shape 32x32x3
       - Alex Krizhevsky: Learning Multiple Layers of Features from Tiny Images. 2009.
     * - FashionMNIST
       - Image Classification
       - 60k train, 10k test, 10 classes, image shape 28x28x1
       - Han Xiao et al.: Fashion-MNIST: a Novel Image Dataset for Benchmarking Machine Learning Algorithms. 2017.
+    * - fmow
+      - Image Classification: land use recognition from satellite images.
+      - 62 classes, image shape 32x32x3
+      - Huaxiu Yao et al.: Wild-Time: A Benchmark of in-the-Wild Distribution Shift over Time. Conference on Neural Information Processing Systems Datasets and Benchmarks Track. 2022.
+    * - huffpost
+      - Text Classification: category recognition of news paper articles.
+      - ~58k train, ~6k test, 11 classes, years 2012-2019
+      - Huaxiu Yao et al.: Wild-Time: A Benchmark of in-the-Wild Distribution Shift over Time. Conference on Neural Information Processing Systems Datasets and Benchmarks Track. 2022.
     * - MNIST
       - Image Classification
       - 60k train, 10k test, 10 classes, image shape 28x28x1
       - Li Deng: The MNIST Database of Handwritten Digit Images for Machine Learning Research. IEEE Signal Processing Magazine. 2012.
+    * - yearbook
+      - Image Classification: gender identification in yearbook photos.
+      - ~33k train, ~4k test, 2 classes, years 1930-2013, image shape 32x32x1
+      - Huaxiu Yao et al.: Wild-Time: A Benchmark of in-the-Wild Distribution Shift over Time. Conference on Neural Information Processing Systems Datasets and Benchmarks Track. 2022.
+    * - hfd-{dataset_name}
+      - multiple
+      - Any `Hugging Face dataset <https://huggingface.co/datasets>`__ can be used. Just prepend the prefix ``hfd-``, e.g., ``hfd-rotten_tomatoes``. Select input and target columns via ``config_space``, e.g., add ``"input_column": "text", "target_column": "label"`` for the `rotten_tomatoes <https://huggingface.co/datasets/rotten_tomatoes>`__ example.
+      - Please refer to `the official documentation <https://huggingface.co/datasets>`__.
 
 .. _benchmarking-renate-benchmarks-scenarios:
 
 Scenarios
 =========
 
 A scenario defines how the dataset is split into several data partitions.
@@ -159,14 +183,19 @@
 
     * - Scenario Name
       - Description
       - Settings
     * - :py:class:`~renate.benchmark.scenarios.BenchmarkScenario`
       - Used in combination only with CLEAR-10 or CLEAR-100.
       - * :code:`num_tasks`: Number of data partitions.
+    * - :py:class:`~renate.benchmark.scenarios.WildTimeScenario`
+      - Used in combination only with Wild-Time datasets. This is not the scenario used in the paper.
+        Data is presented time step by time step and the model is evaluated on test data up to the
+        current time step.
+      - * :code:`num_tasks`: Number of data partitions.
     * - :py:class:`~renate.benchmark.scenarios.ClassIncrementalScenario`
       - Creates data partitions by splitting the data according to class labels.
       - * :code:`class_groupings`: Tuple of tuples containing the class labels, e.g., ``((1, ), (2, 3, 4))``.
     * - :py:class:`~renate.benchmark.scenarios.FeatureSortingScenario`
       - Splits data into different tasks after sorting the data according to a specific feature.
         Can be used for image data as well. In that case channels are selected and we select according to
         average channel value.
```

### Comparing `Renate-0.2.1/doc/conf.py` & `Renate-0.3.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/doc/examples/nlp_finetuning.rst` & `Renate-0.3.0/doc/examples/nlp_finetuning.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/doc/examples/train_classifier_sagemaker.rst` & `Renate-0.3.0/doc/examples/train_classifier_sagemaker.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/doc/examples/train_mlp_locally.rst` & `Renate-0.3.0/doc/examples/train_mlp_locally.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/doc/getting_started/avalanche.rst` & `Renate-0.3.0/doc/getting_started/avalanche.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/doc/getting_started/how_to_renate_config.rst` & `Renate-0.3.0/doc/getting_started/how_to_renate_config.rst`

 * *Files 4% similar despite different names*

```diff
@@ -12,39 +12,39 @@
 
 This function takes a path to a model state and returns a model in the form of a
 :py:class:`~renate.models.renate_module.RenateModule`.
 Its signature is
 
 .. code-block:: python
 
-    def model_fn(model_state_url: Optional[Union[Path, str]] = None) -> RenateModule:
+    def model_fn(model_state_url: Optional[str] = None) -> RenateModule:
 
 A :py:class:`~renate.models.renate_module.RenateModule` is a :code:`torch.nn.Module` with some
 additional functionality relevant to continual learning.
 If no path is given (i.e., when we first train a model) your :code:`model_fn` should create
 the model from scratch.
 Otherwise it should be reloaded from the stored state, for which
 :py:class:`~renate.models.renate_module.RenateModule` provides a
 :py:meth:`~renate.models.renate_module.RenateModule.from_state_dict`
 method, which automatically handles model hyperparameters.
 
 .. literalinclude:: ../../examples/getting_started/renate_config.py
     :caption: Example
-    :lines: 13-39
+    :lines: 14-40
 
 If you are using a torch model with **no or fixed hyperparameters**, you can use
 :py:class:`~renate.models.renate_module.RenateWrapper`.
 In this case, do not use the
 :py:meth:`~renate.models.renate_module.RenateModule.from_state_dict`
 method, but simply reinstantiate your model and call :code:`load_state_dict`.
 
 .. code-block:: python
     :caption: Example
 
-    def model_fn(model_state_url: Optional[Union[Path, str]] = None) -> RenateModule:
+    def model_fn(model_state_url: Optional[str] = None) -> RenateModule:
         my_torch_model = torch.nn.Linear(28 * 28, 10)  # Instantiate your torch model.
         model = RenateWrapper(my_torch_model)
         if model_state_url is not None:
             state_dict = torch.load(str(model_state_url))
             model.load_state_dict(state_dict)
         return model
 
@@ -54,24 +54,24 @@
 
 This function takes a path to a data folder and returns data in the form of a
 :py:class:`~renate.data.data_module.RenateDataModule`.
 Its signature is
 
 .. code-block:: python
 
-    def data_module_fn(data_path: Union[Path, str], seed: int = defaults.SEED) -> RenateDataModule:
+    def data_module_fn(data_path: str, seed: int = defaults.SEED) -> RenateDataModule:
 
 :py:class:`~renate.data.data_module.RenateDataModule` provides a structured interface to
 download, set up, and access train/val/test datasets.
 The function also accepts a :code:`seed`, which should be used for any randomized operations,
 such as data subsampling or splitting.
 
 .. literalinclude:: ../../examples/getting_started/renate_config.py
     :caption: Example
-    :lines: 42-72
+    :lines: 43-66
 
 Transforms
 ==========
 
 Transforms for data preprocessing or augmentation are often applied as part of torch datasets.
 That is, :code:`x, y = dataset[i]` returns a fully-preprocessed and potentially augmented
 data point, ready to be passed to a torch model.
@@ -108,27 +108,27 @@
 * :code:`def buffer_target_transform() -> Callable`
 
 These are optional as well but, if omitted, Renate will use :code:`train_transform` and
 :code:`train_target_transform`, respectively.
 
 .. literalinclude:: ../../examples/getting_started/renate_config.py
     :caption: Example
-    :lines: 76-93
+    :lines: 73-90
 
 Custom Metrics
 ==============
 
 It is possible to specify a set of custom metrics to be measured during the training process.
 The metrics can be either imported from :code:`torchmetrics`, which offers a vast collection,
 or created ad-hoc by implementing the same interface
 (see this `tutorial <https://torchmetrics.readthedocs.io/en/stable/pages/implement.html>`_).
 
 .. literalinclude:: ../../examples/getting_started/renate_config.py
     :caption: Example
-    :lines: 96-
+    :lines: 93-
 
 To enable the usage of additional metrics in Renate it is sufficient to implement the
 :code:`metrics_fn` function, returning a dictionary where the key is a string containing the
 metric's name and the value is an instantiation of the metric class.
 In the example above we add a metric called :code:`my_accuracy` by instantiating the accuracy
 metric from :code:`torchmetrics`.
 
@@ -139,32 +139,32 @@
 We will demonstrate this at the example of :code:`data_module_fn` but the same rules apply to all other functions
 introduced in this chapter.
 
 Let us assume we already have a config file in which we implemented a simple linear model:
 
 .. code-block:: python
 
-    def model_fn(model_state_url: Optional[Union[Path, str]] = None) -> RenateModule:
+    def model_fn(model_state_url: Optional[str] = None) -> RenateModule:
         my_torch_model = torch.nn.Linear(28 * 28, 10)
         model = RenateWrapper(my_torch_model)
         if model_state_url is not None:
-            state_dict = torch.load(str(model_state_url))
+            state_dict = torch.load(model_state_url)
             model.load_state_dict(state_dict)
         return model
 
 However, we have different datasets and each of them has different input and output dimensions.
 The natural change would be to change it to something like
 
 .. code-block:: python
 
-    def model_fn(num_inputs: int, num_outputs: int, model_state_url: Optional[Union[Path, str]] = None) -> RenateModule:
+    def model_fn(num_inputs: int, num_outputs: int, model_state_url: Optional[str] = None) -> RenateModule:
         my_torch_model = torch.nn.Linear(num_inputs, num_outputs)
         model = RenateWrapper(my_torch_model)
         if model_state_url is not None:
-            state_dict = torch.load(str(model_state_url))
+            state_dict = torch.load(model_state_url)
             model.load_state_dict(state_dict)
         return model
 
 And in fact, this is exactly how it works. However, there are few limitations:
 
 * Typing is required.
 * Only types allowed: ``bool``, ``float``, ``int``, ``str``, ``list``, and ``tuple``.
```

### Comparing `Renate-0.2.1/doc/getting_started/how_to_run_training.rst` & `Renate-0.3.0/doc/getting_started/how_to_run_training.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/doc/getting_started/index.rst` & `Renate-0.3.0/doc/getting_started/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 ***************
 
 This section covers the usage of Renate from the installation to the training
 of a model. The content is intended to explain the basic steps to be taken when creating a new
 training pipeline based on Renate.
 
 If your goal is to test multiple Renate algorithms on your dataset or to test a specific algorithm on
-multiple datasets and scenarios, you will be better served by the benchmarking functionalities 
+multiple datasets and scenarios, you will be better served by the benchmarking functionalities
 provided in :doc:`../benchmarking/renate_benchmarks`.
 
 .. toctree::
     :maxdepth: 2
 
     install
     how_to_renate_config
     how_to_run_training
     output
     supported_algorithms
     avalanche
+    shift_detection
```

### Comparing `Renate-0.2.1/doc/getting_started/install.rst` & `Renate-0.3.0/doc/getting_started/install.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Renate is available via PyPI and can be installed using :code:`pip`:
 
 .. code-block:: bash
 
     pip install Renate
 
-If you want to use additional methods that require the Avalanche library, please use use
+If you want to use additional methods that require the Avalanche library, please use
 
 .. code-block:: bash
 
     pip install Renate[avalanche]
 
 For Renate contributors we recommend using ``dev``.
 This will install further dependencies which are required for code formatting and unit testing.
```

### Comparing `Renate-0.2.1/doc/getting_started/output.rst` & `Renate-0.3.0/doc/getting_started/output.rst`

 * *Files 18% similar despite different names*

```diff
@@ -27,31 +27,31 @@
 
 In the following, we refer with :code:`model_fn` to the function defined by the user in the
 :doc:`Renate config file <how_to_renate_config>`.
 
 Output Saved Locally
 ~~~~~~~~~~~~~~~~~~~~
 
-If :code:`next_state_url` is a path to a local folder, loading the updated model can be done as follows:
+If :code:`output_state_url` is a path to a local folder, loading the updated model can be done as follows:
 
 .. code-block:: python
 
-    from renate.defaults import current_state_folder, model_file
+    from renate.defaults import input_state_folder, model_file
 
-    my_model = model_fn(model_file(current_state_folder(next_state_url)))
+    my_model = model_fn(model_file(input_state_folder(output_state_url)))
 
 Output Saved on S3
 ~~~~~~~~~~~~~~~~~~
 
 If the Renate output was saved on S3, the model checkpoint :code:`model.ckpt` can be downloaded from
 
 .. code-block:: python
 
-    from renate.defaults import current_state_folder, model_file
+    from renate.defaults import input_state_folder, model_file
 
-    print(model_file(current_state_folder(next_state_url)))
+    print(model_file(input_state_folder(output_state_url)))
 
 and then loaded via
 
 .. code-block:: python
 
     my_model = model_fn("model.ckpt")
```

### Comparing `Renate-0.2.1/doc/getting_started/supported_algorithms.rst` & `Renate-0.3.0/doc/getting_started/supported_algorithms.rst`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/examples/benchmarking/class_incremental_learning_cifar10_der.py` & `Renate-0.3.0/examples/benchmarking/class_incremental_learning_cifar10_der.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/examples/getting_started/renate_config.py` & `Renate-0.3.0/examples/getting_started/renate_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
-from typing import Callable, Dict, Literal, Optional
+from typing import Callable, Dict, Optional
 
 import torch
 import torchvision
 from torchmetrics import Accuracy
 from torchvision.transforms import transforms
 
 from renate.data.data_module import RenateDataModule
@@ -45,32 +45,29 @@
         super().__init__(data_path, val_size=val_size, seed=seed)
 
     def prepare_data(self) -> None:
         # This is only to download the data. We separate downloading from the remaining set-up to
         # streamline data loading when using multiple training jobs during HPO.
         torchvision.datasets.MNIST(self._data_path, download=True)
 
-    def setup(self, stage: Optional[Literal["train", "val", "test"]] = None) -> None:
+    def setup(self) -> None:
         # This sets up train/val/test datasets, assuming data has already been downloaded.
-        if stage in ["train", "val"] or stage is None:
-            train_data = torchvision.datasets.MNIST(
-                self._data_path,
-                train=True,
-                transform=transforms.ToTensor(),
-                target_transform=transforms.Lambda(lambda x: torch.tensor(x, dtype=torch.long)),
-            )
-            self._train_data, self._val_data = self._split_train_val_data(train_data)
-
-        if stage == "test" or stage is None:
-            self._test_data = torchvision.datasets.MNIST(
-                self._data_path,
-                train=False,
-                transform=transforms.ToTensor(),
-                target_transform=transforms.Lambda(lambda x: torch.tensor(x, dtype=torch.long)),
-            )
+        train_data = torchvision.datasets.MNIST(
+            self._data_path,
+            train=True,
+            transform=transforms.ToTensor(),
+            target_transform=transforms.Lambda(lambda x: torch.tensor(x, dtype=torch.long)),
+        )
+        self._train_data, self._val_data = self._split_train_val_data(train_data)
+        self._test_data = torchvision.datasets.MNIST(
+            self._data_path,
+            train=False,
+            transform=transforms.ToTensor(),
+            target_transform=transforms.Lambda(lambda x: torch.tensor(x, dtype=torch.long)),
+        )
 
 
 def data_module_fn(data_path: str, seed: int) -> RenateDataModule:
     return MyMNISTDataModule(val_size=0.2, seed=seed)
 
 
 def train_transform() -> Callable:
```

### Comparing `Renate-0.2.1/examples/nlp_finetuning/renate_config.py` & `Renate-0.3.0/examples/nlp_finetuning/renate_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
-from pathlib import Path
-from typing import Optional, Union
+from typing import Optional
 
 import torch
 import transformers
 
 import renate.defaults as defaults
-from renate.benchmark.datasets.nlp_datasets import HuggingfaceTextDataModule
+from renate.benchmark.datasets.nlp_datasets import HuggingFaceTextDataModule
 from renate.data.data_module import RenateDataModule
 from renate.models import RenateModule
 from renate.models.renate_module import RenateWrapper
 
 
-def model_fn(model_state_url: Optional[Union[Path, str]] = None) -> RenateModule:
+def model_fn(model_state_url: Optional[str] = None) -> RenateModule:
     """Returns a DistilBert classification model."""
     transformer_model = transformers.DistilBertForSequenceClassification.from_pretrained(
         "distilbert-base-uncased", num_labels=2, return_dict=False
     )
     model = RenateWrapper(transformer_model, loss_fn=torch.nn.CrossEntropyLoss())
     if model_state_url is not None:
-        state_dict = torch.load(str(model_state_url))
+        state_dict = torch.load(model_state_url)
         model.load_state_dict(state_dict)
     return model
 
 
-def data_module_fn(
-    data_path: Union[Path, str], chunk_id: int, seed: int = defaults.SEED
-) -> RenateDataModule:
+def data_module_fn(data_path: str, chunk_id: int, seed: int = defaults.SEED) -> RenateDataModule:
     """Returns one of two movie review datasets depending on `chunk_id`."""
     tokenizer = transformers.DistilBertTokenizer.from_pretrained("distilbert-base-uncased")
     dataset_name = "imdb" if chunk_id else "rotten_tomatoes"
-    data_module = HuggingfaceTextDataModule(
-        str(data_path),
+    data_module = HuggingFaceTextDataModule(
+        data_path,
         dataset_name=dataset_name,
         tokenizer=tokenizer,
         val_size=0.2,
         seed=seed,
     )
     return data_module
```

### Comparing `Renate-0.2.1/examples/nlp_finetuning/start.py` & `Renate-0.3.0/examples/nlp_finetuning/start.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/examples/simple_classifier_cifar10/renate_config.py` & `Renate-0.3.0/examples/simple_classifier_cifar10/renate_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
-from pathlib import Path
-from typing import Callable, Optional, Union
+from typing import Callable, Optional
 
 import torch
 from torchvision import transforms
 
 import renate.defaults as defaults
 from renate.benchmark.datasets.vision_datasets import TorchVisionDataModule
 from renate.benchmark.models import ResNet18CIFAR
 from renate.benchmark.scenarios import ClassIncrementalScenario, Scenario
 from renate.models import RenateModule
 
 
-def model_fn(model_state_url: Optional[Union[Path, str]] = None) -> RenateModule:
+def model_fn(model_state_url: Optional[str] = None) -> RenateModule:
     """Returns a model instance."""
     if model_state_url is None:
         model = ResNet18CIFAR()
     else:
-        state_dict = torch.load(str(model_state_url))
+        state_dict = torch.load(model_state_url)
         model = ResNet18CIFAR.from_state_dict(state_dict)
     return model
 
 
 def data_module_fn(data_path: str, chunk_id: int, seed: int = defaults.SEED) -> Scenario:
     """Returns a class-incremental scenario instance.
```

### Comparing `Renate-0.2.1/examples/simple_classifier_cifar10/start_with_hpo.py` & `Renate-0.3.0/examples/simple_classifier_cifar10/start_with_hpo.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/examples/simple_classifier_cifar10/start_without_hpo.py` & `Renate-0.3.0/examples/simple_classifier_cifar10/start_without_hpo.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/examples/train_mlp_locally/renate_config.py` & `Renate-0.3.0/examples/train_mlp_locally/renate_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
-from pathlib import Path
-from typing import Callable, Optional, Union
+from typing import Callable, Optional
 
 import torch
 from torchvision.transforms import transforms
 
 from renate import defaults
 from renate.benchmark.datasets.vision_datasets import TorchVisionDataModule
 from renate.benchmark.models.mlp import MultiLayerPerceptron
@@ -30,22 +29,22 @@
         data_module=data_module,
         class_groupings=[[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]],
         chunk_id=chunk_id,
     )
     return class_incremental_scenario
 
 
-def model_fn(model_state_url: Optional[Union[Path, str]] = None) -> RenateModule:
+def model_fn(model_state_url: Optional[str] = None) -> RenateModule:
     """Returns a model instance."""
     if model_state_url is None:
         model = MultiLayerPerceptron(
             num_inputs=784, num_outputs=10, num_hidden_layers=2, hidden_size=128
         )
     else:
-        state_dict = torch.load(str(model_state_url))
+        state_dict = torch.load(model_state_url)
         model = MultiLayerPerceptron.from_state_dict(state_dict)
     return model
 
 
 def train_transform() -> Callable:
     """Returns a transform function to be used in the training."""
     return transforms.Lambda(lambda x: torch.flatten(x))
```

### Comparing `Renate-0.2.1/examples/train_mlp_locally/start_training_with_er_without_hpo.py` & `Renate-0.3.0/examples/train_mlp_locally/start_training_with_er_without_hpo.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/examples/train_mlp_locally/start_training_with_hpo.py` & `Renate-0.3.0/examples/train_mlp_locally/start_training_with_hpo.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/examples/train_mlp_locally/start_training_without_hpo.py` & `Renate-0.3.0/examples/train_mlp_locally/start_training_without_hpo.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/pyproject.toml` & `Renate-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -17,17 +17,21 @@
 dynamic = ["version", "readme", "dependencies"]
 
 [project.optional-dependencies]
 avalanche = [
     "avalanche_lib==0.3.1",
     "torch>=1.10.0, <1.12.2",
 ]
+benchmark = [
+    "wild-time-data==0.1.0",
+]
 dev = [
     "black==23.1.0",
     "avalanche_lib==0.3.1",
+    "wild-time-data==0.1.0",
     "torch>=1.10.0, <1.12.2",
     # PyTest Dependencies
     "pytest==7.2.2",
     "pytest-cov==4.0.0",
     "pytest-helpers-namespace==2021.12.29",
     ]
```

### Comparing `Renate-0.2.1/src/Renate.egg-info/PKG-INFO` & `Renate-0.3.0/src/Renate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: Renate
-Version: 0.2.1
+Version: 0.3.0
 Summary: Library for Continual Learning for Practitioners
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: avalanche
+Provides-Extra: benchmark
 Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
 .. image:: https://img.shields.io/pypi/status/Renate
     :target: #
     :alt: PyPI - Status
```

### Comparing `Renate-0.2.1/src/Renate.egg-info/SOURCES.txt` & `Renate-0.3.0/src/Renate.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -35,19 +35,21 @@
 doc/examples/train_mlp_locally.rst
 doc/getting_started/avalanche.rst
 doc/getting_started/how_to_renate_config.rst
 doc/getting_started/how_to_run_training.rst
 doc/getting_started/index.rst
 doc/getting_started/install.rst
 doc/getting_started/output.rst
+doc/getting_started/shift_detection.rst
 doc/getting_started/supported_algorithms.rst
 examples/benchmarking/class_incremental_learning_cifar10_der.py
 examples/getting_started/renate_config.py
 examples/nlp_finetuning/renate_config.py
 examples/nlp_finetuning/start.py
+examples/shift_detection/image_shift_detection.py
 examples/simple_classifier_cifar10/renate_config.py
 examples/simple_classifier_cifar10/requirements.txt
 examples/simple_classifier_cifar10/start_with_hpo.py
 examples/simple_classifier_cifar10/start_without_hpo.py
 examples/train_mlp_locally/renate_config.py
 examples/train_mlp_locally/start_training_with_er_without_hpo.py
 examples/train_mlp_locally/start_training_with_hpo.py
@@ -64,18 +66,20 @@
 src/renate/benchmark/__init__.py
 src/renate/benchmark/experiment_config.py
 src/renate/benchmark/experimentation.py
 src/renate/benchmark/scenarios.py
 src/renate/benchmark/datasets/__init__.py
 src/renate/benchmark/datasets/nlp_datasets.py
 src/renate/benchmark/datasets/vision_datasets.py
+src/renate/benchmark/datasets/wild_time_data.py
 src/renate/benchmark/models/__init__.py
 src/renate/benchmark/models/base.py
 src/renate/benchmark/models/mlp.py
 src/renate/benchmark/models/resnet.py
+src/renate/benchmark/models/transformer.py
 src/renate/benchmark/models/vision_transformer.py
 src/renate/cli/parsing_functions.py
 src/renate/cli/run_experiment_with_scenario.py
 src/renate/cli/run_remote_job.py
 src/renate/cli/run_training.py
 src/renate/data/__init__.py
 src/renate/data/data_module.py
@@ -90,14 +94,20 @@
 src/renate/memory/buffer.py
 src/renate/memory/storage.py
 src/renate/models/__init__.py
 src/renate/models/prediction_strategies.py
 src/renate/models/renate_module.py
 src/renate/models/layers/__init__.py
 src/renate/models/layers/cn.py
+src/renate/shift/__init__.py
+src/renate/shift/detector.py
+src/renate/shift/kernels.py
+src/renate/shift/ks_detector.py
+src/renate/shift/mmd_detectors.py
+src/renate/shift/mmd_helpers.py
 src/renate/training/__init__.py
 src/renate/training/training.py
 src/renate/updaters/__init__.py
 src/renate/updaters/learner.py
 src/renate/updaters/model_updater.py
 src/renate/updaters/avalanche/__init__.py
 src/renate/updaters/avalanche/learner.py
@@ -178,14 +188,18 @@
 test/renate/evaluation/metrics/test_classification.py
 test/renate/evaluation/metrics/test_regression_metrics.py
 test/renate/memory/test_buffer.py
 test/renate/memory/test_storage.py
 test/renate/models/test_renate_module.py
 test/renate/renate_config_files/config.py
 test/renate/renate_config_files/config_scenario.py
+test/renate/shift/test_detector_base.py
+test/renate/shift/test_detectors.py
+test/renate/shift/test_kernels.py
+test/renate/shift/test_mmd_helpers.py
 test/renate/training/test_run_training.py
 test/renate/updaters/test_learner.py
 test/renate/updaters/test_model_updater.py
 test/renate/updaters/avalanche/test_avalanche_learner.py
 test/renate/updaters/avalanche/test_avalanche_model_updater.py
 test/renate/updaters/avalanche/test_avalanche_plugins.py
 test/renate/updaters/experimental/test_er.py
```

### Comparing `Renate-0.2.1/src/renate/__init__.py` & `Renate-0.3.0/src/renate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
     _handler = logging.StreamHandler()
     _handler.setFormatter(
         logging.Formatter("[%(asctime)s] %(levelname)s [%(name)s:%(lineno)s] %(message)s")
     )
     _renate_logger.addHandler(_handler)
     _renate_logger.propagate = False
 
-__version__ = "0.2.1"
+__version__ = "0.3.0"
```

### Comparing `Renate-0.2.1/src/renate/benchmark/datasets/nlp_datasets.py` & `Renate-0.3.0/src/renate/benchmark/datasets/nlp_datasets.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,95 +1,107 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 import logging
-from typing import Optional
+from typing import Any, Dict, Optional
 
 import datasets
 import torch
 import transformers
 
 from renate import defaults
 from renate.data.data_module import RenateDataModule
 
 
 class _InputTargetWrapper(torch.utils.data.Dataset):
-    """Make a huggingface dataset comply with the `(input, target)` format."""
+    """Make a Hugging Face dataset comply with the `(input, target)` format."""
 
     def __init__(self, dataset, target_column: str = "label"):
         self._dataset = dataset
         self._target_column = target_column
 
     def __len__(self):
         return len(self._dataset)
 
     def __getitem__(self, idx):
         item = self._dataset[idx]
         target = item.pop(self._target_column)
         return item, target
 
 
-class HuggingfaceTextDataModule(RenateDataModule):
-    """Data module wrapping Huggingface text datasets.
+class HuggingFaceTextDataModule(RenateDataModule):
+    """Data module wrapping Hugging Face text datasets.
 
-    This is a convenience wrapper to expose a hugginface dataset as a `RenateDataModule`. Datasets
+    This is a convenience wrapper to expose a Hugging Face dataset as a `RenateDataModule`. Datasets
     will be pre-tokenized and will return `input, target = dataset[i]`, where `input` is a
     dictionary with fields `["input_ids", "attention_mask"]`, and `target` is a tensor.
 
     We expect the dataset to have a "train" and a "test" split. An additional "validation" split
     will be used if present. Otherwise, a validation set may be split off of the training data
     using the `val_size` argument.
 
     Args:
         data_path: the path to the folder containing the dataset files.
+        tokenizer: Tokenizer to apply to the dataset. See https://huggingface.co/docs/tokenizers/
+            for more information on tokenizers.
         dataset_name: Name of the dataset, see https://huggingface.co/datasets. This is a wrapper
             for text datasets only.
         input_column: Name of the column containing the input text.
         target_column: Name of the column containing the target (e.g., class label).
-        tokenizer: Tokenizer to apply to the dataset. See https://huggingface.co/docs/tokenizers/
-            for more information on tokenizers.
-        tokenize_kwargs: Keyword arguments to be passed to the tokenizer. Typical options are
-           `max_length`, `padding` and `truncation`. See https://huggingface.co/docs/tokenizers/
+        tokenizer_kwargs: Keyword arguments passed when calling the tokenizer's ``__call__``
+           function. Typical options are `max_length`, `padding` and `truncation`.
+           See https://huggingface.co/docs/tokenizers/
            for more information on tokenizers. If `None` is passed, this defaults to
            `{"padding": "max_length", max_length: 128, truncation: True}`.
         val_size: Fraction of the training data to be used for validation.
         seed: Seed used to fix random number generation.
     """
 
     def __init__(
         self,
         data_path: str,
+        tokenizer: transformers.PreTrainedTokenizer,
         dataset_name: str = "ag_news",
         input_column: str = "text",
         target_column: str = "label",
-        tokenizer: Optional[transformers.PreTrainedTokenizer] = None,
-        tokenizer_kwargs: Optional[dict] = None,
+        tokenizer_kwargs: Optional[Dict[str, Any]] = None,
         val_size: float = defaults.VALIDATION_SIZE,
         seed: int = defaults.SEED,
     ):
-        super(HuggingfaceTextDataModule, self).__init__(
+        super(HuggingFaceTextDataModule, self).__init__(
             data_path=data_path,
             val_size=val_size,
             seed=seed,
         )
         self._dataset_name = dataset_name
         self._input_column = input_column
         self._target_column = target_column
         self._tokenizer = tokenizer
         self._tokenizer_kwargs = tokenizer_kwargs or defaults.TOKENIZER_KWARGS
 
     def prepare_data(self) -> None:
         """Download data."""
         split_names = datasets.get_dataset_split_names(self._dataset_name)
-        if not "train" in split_names:
+        if "train" not in split_names:
             raise RuntimeError(f"Dataset {self._dataset_name} does not contain a 'train' split.")
-        if not "test" in split_names:
+        if "test" not in split_names:
             raise RuntimeError(f"Dataset {self._dataset_name} does not contain a 'test' split.")
         self._train_data = datasets.load_dataset(
             self._dataset_name, split="train", cache_dir=self._data_path
         )
+        available_columns = list(self._train_data.features)
+        if self._input_column not in available_columns:
+            raise ValueError(
+                f"Input column '{self._input_column}' does not exist in {self._dataset_name}. "
+                f"Available columns: {available_columns}."
+            )
+        if self._target_column not in available_columns:
+            raise ValueError(
+                f"Target column '{self._target_column}' does not exist in {self._dataset_name}. "
+                f"Available columns: {available_columns}."
+            )
         self._test_data = datasets.load_dataset(
             self._dataset_name, split="test", cache_dir=self._data_path
         )
         if "validation" in split_names:
             logging.info(f"Using 'validation' split of dataset {self._dataset_name}.")
             self._val_data = datasets.load_dataset(
                 self._dataset_name, split="validation", cache_dir=self._data_path
@@ -108,17 +120,17 @@
         def tokenize_fn(batch):
             return self._tokenizer(batch[self._input_column], **self._tokenizer_kwargs)
 
         columns = ["input_ids", "attention_mask", self._target_column]
 
         self._train_data = self._train_data.map(tokenize_fn, batched=True)
         self._train_data.set_format(type="torch", columns=columns)
-        self._train_data = _InputTargetWrapper(self._train_data)
+        self._train_data = _InputTargetWrapper(self._train_data, self._target_column)
         self._test_data = self._test_data.map(tokenize_fn, batched=True)
         self._test_data.set_format(type="torch", columns=columns)
-        self._test_data = _InputTargetWrapper(self._test_data)
+        self._test_data = _InputTargetWrapper(self._test_data, self._target_column)
         if self._val_data is not None:
             self._val_data = self._val_data.map(tokenize_fn, batched=True)
             self._val_data.set_format(type="torch", columns=columns)
-            self._val_data = _InputTargetWrapper(self._val_data)
+            self._val_data = _InputTargetWrapper(self._val_data, self._target_column)
         else:
             self._train_data, self._val_data = self._split_train_val_data(self._train_data)
```

### Comparing `Renate-0.2.1/src/renate/benchmark/datasets/vision_datasets.py` & `Renate-0.3.0/src/renate/benchmark/datasets/vision_datasets.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/benchmark/experiment_config.py` & `Renate-0.3.0/src/renate/benchmark/experiment_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 from typing import List, Optional, Tuple, Union
 
 import torch
+import wild_time_data
 from torchvision.transforms import transforms
+from transformers import AutoTokenizer
 
+from renate.benchmark.datasets.nlp_datasets import HuggingFaceTextDataModule
 from renate.benchmark.datasets.vision_datasets import CLEARDataModule, TorchVisionDataModule
+from renate.benchmark.datasets.wild_time_data import WildTimeDataModule
 from renate.benchmark.models import (
     MultiLayerPerceptron,
     ResNet18,
     ResNet18CIFAR,
     ResNet34,
     ResNet34CIFAR,
     ResNet50,
@@ -17,23 +21,25 @@
     VisionTransformerB16,
     VisionTransformerB32,
     VisionTransformerCIFAR,
     VisionTransformerH14,
     VisionTransformerL16,
     VisionTransformerL32,
 )
+from renate.benchmark.models.transformer import HuggingFaceSequenceClassificationTransformer
 from renate.benchmark.scenarios import (
     BenchmarkScenario,
     ClassIncrementalScenario,
     FeatureSortingScenario,
     HueShiftScenario,
     IIDScenario,
     ImageRotationScenario,
     PermutationScenario,
     Scenario,
+    WildTimeScenario,
 )
 from renate.data.data_module import RenateDataModule
 from renate.models import RenateModule
 from renate.models.prediction_strategies import ICaRLClassificationStrategy
 
 models = {
     "MultiLayerPerceptron": MultiLayerPerceptron,
@@ -45,58 +51,101 @@
     "ResNet50": ResNet50,
     "VisionTransformerCIFAR": VisionTransformerCIFAR,
     "VisionTransformerB16": VisionTransformerB16,
     "VisionTransformerB32": VisionTransformerB32,
     "VisionTransformerL16": VisionTransformerL16,
     "VisionTransformerL32": VisionTransformerL32,
     "VisionTransformerH14": VisionTransformerH14,
+    "HuggingFaceTransformer": HuggingFaceSequenceClassificationTransformer,
 }
 
 
 def model_fn(
     model_state_url: Optional[str] = None,
     updater: Optional[str] = None,
     model_name: Optional[str] = None,
     num_inputs: Optional[int] = None,
     num_outputs: Optional[int] = None,
     num_hidden_layers: Optional[int] = None,
     hidden_size: Optional[Tuple[int]] = None,
+    dataset_name: Optional[str] = None,
+    pretrained_model_name: Optional[str] = None,
 ) -> RenateModule:
     """Returns a model instance."""
     if model_name not in models:
         raise ValueError(f"Unknown model `{model_name}`")
     model_class = models[model_name]
     model_kwargs = {}
     if updater == "Avalanche-iCaRL":
         model_kwargs["prediction_strategy"] = ICaRLClassificationStrategy()
     if model_name == "MultiLayerPerceptron":
-        model_kwargs = {
-            "num_inputs": num_inputs,
-            "num_hidden_layers": num_hidden_layers,
-            "hidden_size": hidden_size,
-        }
+        model_kwargs.update(
+            {
+                "num_inputs": num_inputs,
+                "num_hidden_layers": num_hidden_layers,
+                "hidden_size": hidden_size,
+            }
+        )
+    elif model_name.startswith("ResNet") and dataset_name in ["FashionMNIST", "MNIST", "yearbook"]:
+        model_kwargs["gray_scale"] = True
+    elif model_name == "HuggingFaceTransformer":
+        if updater == "Avalanche-iCaRL":
+            raise ValueError("Transformers do not support iCaRL.")
+        model_kwargs["pretrained_model_name"] = pretrained_model_name
     if num_outputs is not None:
         model_kwargs["num_outputs"] = num_outputs
     if model_state_url is None:
         model = model_class(**model_kwargs)
     else:
         state_dict = torch.load(model_state_url)
         model = model_class.from_state_dict(state_dict)
     return model
 
 
 def get_data_module(
-    data_path: str, dataset_name: str, val_size: float, seed: int
+    data_path: str,
+    src_bucket: Optional[str],
+    src_object_name: Optional[str],
+    dataset_name: str,
+    val_size: float,
+    seed: int,
+    pretrained_model_name: Optional[str],
+    input_column: Optional[str],
+    target_column: Optional[str],
 ) -> RenateDataModule:
     if dataset_name in TorchVisionDataModule.dataset_dict:
         return TorchVisionDataModule(
             data_path, dataset_name=dataset_name, val_size=val_size, seed=seed
         )
     if dataset_name in ["CLEAR10", "CLEAR100"]:
         return CLEARDataModule(data_path, dataset_name=dataset_name, val_size=val_size, seed=seed)
+    if dataset_name in wild_time_data.list_datasets():
+        data_module_kwargs = {
+            "data_path": data_path,
+            "src_bucket": src_bucket,
+            "src_object_name": src_object_name,
+            "dataset_name": dataset_name,
+            "val_size": val_size,
+            "seed": seed,
+        }
+        if pretrained_model_name is not None:
+            data_module_kwargs["tokenizer"] = AutoTokenizer.from_pretrained(pretrained_model_name)
+        return WildTimeDataModule(**data_module_kwargs)
+
+    if dataset_name.startswith("hfd-"):
+        tokenizer = AutoTokenizer.from_pretrained(pretrained_model_name)
+        return HuggingFaceTextDataModule(
+            data_path=data_path,
+            dataset_name=dataset_name[4:],
+            input_column=input_column,
+            target_column=target_column,
+            tokenizer=tokenizer,
+            val_size=val_size,
+            seed=seed,
+        )
     raise ValueError(f"Unknown dataset `{dataset_name}`.")
 
 
 def get_scenario(
     scenario_name: str,
     data_module: RenateDataModule,
     chunk_id: int,
@@ -171,14 +220,18 @@
         return HueShiftScenario(
             data_module=data_module,
             num_tasks=num_tasks,
             randomness=randomness,
             chunk_id=chunk_id,
             seed=seed,
         )
+    if scenario_name == "WildTimeScenario":
+        return WildTimeScenario(
+            data_module=data_module, num_tasks=num_tasks, chunk_id=chunk_id, seed=seed
+        )
     raise ValueError(f"Unknown scenario `{scenario_name}`.")
 
 
 def data_module_fn(
     data_path: str,
     chunk_id: int,
     seed: int,
@@ -187,21 +240,33 @@
     val_size: float = 0.0,
     num_tasks: Optional[int] = None,
     class_groupings: Optional[Tuple[Tuple[int]]] = None,
     degrees: Optional[Tuple[int]] = None,
     input_dim: Optional[Tuple[int]] = None,
     feature_idx: Optional[int] = None,
     randomness: Optional[float] = None,
+    src_bucket: Optional[str] = None,
+    src_object_name: Optional[str] = None,
+    pretrained_model_name: Optional[str] = None,
+    input_column: Optional[str] = None,
+    target_column: Optional[str] = None,
 ):
     data_module = get_data_module(
         data_path=data_path,
+        src_bucket=src_bucket,
+        src_object_name=src_object_name,
         dataset_name=dataset_name,
         val_size=val_size,
         seed=seed,
+        pretrained_model_name=pretrained_model_name,
+        input_column=input_column,
+        target_column=target_column,
     )
+    if dataset_name in wild_time_data.list_datasets() and num_tasks is None:
+        num_tasks = len(wild_time_data.available_time_steps(dataset_name))
     return get_scenario(
         scenario_name=scenario_name,
         data_module=data_module,
         chunk_id=chunk_id,
         seed=seed,
         num_tasks=num_tasks,
         class_groupings=class_groupings,
@@ -218,27 +283,33 @@
             TorchVisionDataModule.dataset_stats[dataset_name]["mean"],
             TorchVisionDataModule.dataset_stats[dataset_name]["std"],
         )
 
 
 def train_transform(dataset_name: str) -> Optional[transforms.Compose]:
     """Returns a transform function to be used in the training."""
-    if dataset_name in ["MNIST", "FashionMNIST"]:
+    if dataset_name in [
+        "MNIST",
+        "FashionMNIST",
+    ] + wild_time_data.list_datasets() or dataset_name.startswith("hfd-"):
         return None
-    elif dataset_name in ["CIFAR10", "CIFAR100"]:
+    if dataset_name in ["CIFAR10", "CIFAR100"]:
         return transforms.Compose(
             [
                 transforms.RandomCrop(32, padding=4),
                 transforms.RandomHorizontalFlip(),
                 _get_normalize_transform(dataset_name),
             ]
         )
     raise ValueError(f"Unknown dataset `{dataset_name}`.")
 
 
 def test_transform(dataset_name: str) -> Optional[transforms.Normalize]:
     """Returns a transform function to be used for validation or testing."""
-    if dataset_name in ["MNIST", "FashionMNIST"]:
+    if dataset_name in [
+        "MNIST",
+        "FashionMNIST",
+    ] + wild_time_data.list_datasets() or dataset_name.startswith("hfd-"):
         return None
-    elif dataset_name in ["CIFAR10", "CIFAR100"]:
+    if dataset_name in ["CIFAR10", "CIFAR100"]:
         return _get_normalize_transform(dataset_name)
     raise ValueError(f"Unknown dataset `{dataset_name}`.")
```

### Comparing `Renate-0.2.1/src/renate/benchmark/experimentation.py` & `Renate-0.3.0/src/renate/benchmark/experimentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
     deterministic_trainer: bool,
 ) -> None:
     """Runs an experiment, combining hyperparameter tuning and model for multiple updates.
 
     See renate.benchmark.experimentation.execute_experiment_job for more details.
     """
     logger.info("Start experiment.")
-    seed_everything(seed)
+    seed_everything(seed, True)
 
     input_state_url = defaults.input_state_folder(working_directory)
     output_state_url = defaults.output_state_folder(working_directory)
     data_url = defaults.data_folder(working_directory)
     model_url = defaults.model_file(input_state_url)
     logs_url = defaults.logs_folder(working_directory)
 
@@ -373,9 +373,12 @@
 
     See renate.benchmark.experimentation.execute_experiment_job for more details.
     """
     assert is_s3_uri(
         experiment_outputs_url
     ), f"experiment_outputs_url {experiment_outputs_url} is not on S3."
     return submit_remote_job(
-        source_dir=None, experiment_outputs_url=experiment_outputs_url, **job_kwargs
+        source_dir=None,
+        experiment_outputs_url=experiment_outputs_url,
+        optional_dependencies="benchmark",
+        **job_kwargs,
     )
```

### Comparing `Renate-0.2.1/src/renate/benchmark/models/__init__.py` & `Renate-0.3.0/src/renate/benchmark/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/benchmark/models/base.py` & `Renate-0.3.0/src/renate/benchmark/models/base.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/benchmark/models/mlp.py` & `Renate-0.3.0/src/renate/benchmark/models/mlp.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/benchmark/models/resnet.py` & `Renate-0.3.0/src/renate/benchmark/models/resnet.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         zero_init_residual: Whether to set the initial weights of the residual blocks to zero
             through initializing the Batch Normalization parameters at the end of the block to zero.
         groups: The number of groups to be used for the group convolution.
         width_per_group: The width of the group convolution.
         replace_stride_with_dilation: Whether to replace the stride with a dilation to save memory.
         norm_layer: What kind of normalization layer to use, following convolutions.
         cifar_stem: Whether to use a stem for CIFAR-sized images.
+        gray_scale: Whether input images are gray-scale images, i.e. only 1 color channel.
         loss: Loss function to be used for training.
         prediction_strategy: Continual learning strategies may alter the prediction at train or test
             time.
         add_icarl_class_means: If ``True``, additional parameters used only by the
             ``ICaRLModelUpdater`` are added. Only required when using that updater.
     """
 
@@ -42,14 +43,15 @@
         num_outputs: int = 10,
         zero_init_residual: bool = False,
         groups: int = 1,
         width_per_group: int = 64,
         replace_stride_with_dilation: Optional[List[bool]] = None,
         norm_layer: Type[nn.Module] = nn.BatchNorm2d,
         cifar_stem: bool = True,
+        gray_scale: bool = False,
         loss: nn.Module = nn.CrossEntropyLoss(),
         prediction_strategy: Optional[PredictionStrategy] = None,
         add_icarl_class_means: bool = True,
     ) -> None:
         model = _ResNet(
             block=block,
             layers=layers,
@@ -68,23 +70,33 @@
                 "layers": layers,
                 "zero_init_residual": zero_init_residual,
                 "groups": groups,
                 "width_per_group": width_per_group,
                 "replace_stride_with_dilation": replace_stride_with_dilation,
                 "norm_layer": norm_layer,
                 "cifar_stem": cifar_stem,
+                "gray_scale": gray_scale,
             },
             loss_fn=loss,
             prediction_strategy=prediction_strategy,
             add_icarl_class_means=add_icarl_class_means,
         )
         self._backbone = model
         if cifar_stem:
             self._backbone.conv1 = nn.Conv2d(3, 64, kernel_size=3, stride=1, padding=1, bias=False)
             self._backbone.maxpool = nn.Identity()
+        if gray_scale:
+            self._backbone.conv1 = nn.Conv2d(
+                1,
+                self._backbone.conv1.out_channels,
+                kernel_size=self._backbone.conv1.kernel_size,
+                stride=self._backbone.conv1.stride,
+                padding=self._backbone.conv1.padding,
+                bias=self._backbone.conv1.bias is not None,
+            )
         self._backbone.fc = nn.Identity()
 
         for m in self.modules():
             if hasattr(m, "reset_parameters"):
                 m.reset_parameters()
```

### Comparing `Renate-0.2.1/src/renate/benchmark/models/vision_transformer.py` & `Renate-0.3.0/src/renate/benchmark/models/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/benchmark/scenarios.py` & `Renate-0.3.0/src/renate/benchmark/scenarios.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import numpy as np
 import torch
 from torch.utils.data import Dataset, Subset
 from torchvision.transforms import Lambda, RandomRotation, ToPILImage
 
 from renate import defaults
+from renate.benchmark.datasets.wild_time_data import WildTimeDataModule
 from renate.data.data_module import RenateDataModule
 from renate.data.datasets import _TransformedDataset
 from renate.utils.pytorch import get_generator, randomly_split_data
 
 
 class Scenario(abc.ABC):
     """Creates a continual learning scenario from a RenateDataModule.
@@ -374,7 +375,44 @@
         to_pil_image = ToPILImage()
         for image, _ in dataset:
             count, value = np.histogram(
                 np.array(to_pil_image(image).convert("HSV"))[:, :, 0].reshape(-1), bins=100
             )
             scores.append(value[np.argmax(count)])
         return scores
+
+
+class WildTimeScenario(Scenario):
+    """Creating a time-incremental scenario for the Wild-Time datasets.
+
+    In contrast to the original work, data is presented time step by time step (no grouping) and
+    the test set is all data up to the current time step.
+
+    Args:
+        data_module: The source RenateDataModule for the the user data.
+        num_tasks: The total number of expected tasks for experimentation.
+        chunk_id: The data chunk to load in for the training or validation data.
+        seed: Seed used to fix random number generation.
+    """
+
+    def __init__(
+        self,
+        data_module: RenateDataModule,
+        num_tasks: int,
+        chunk_id: int,
+        seed: int = defaults.SEED,
+    ) -> None:
+        super().__init__(data_module=data_module, num_tasks=num_tasks, chunk_id=chunk_id, seed=seed)
+        if not isinstance(data_module, WildTimeDataModule):
+            raise ValueError("This scenario is only compatible with `WildTimeDataModule`.")
+
+    def setup(self) -> None:
+        """Sets up the scenario."""
+        self._data_module.time_step = self._chunk_id
+        self._data_module.setup()
+        self._train_data = self._data_module.train_data()
+        self._val_data = self._data_module.val_data()
+        self._test_data = []
+        for i in range(self._num_tasks):
+            self._data_module.time_step = i
+            self._data_module.setup()
+            self._test_data.append(self._data_module.test_data())
```

### Comparing `Renate-0.2.1/src/renate/cli/parsing_functions.py` & `Renate-0.3.0/src/renate/cli/parsing_functions.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/cli/run_experiment_with_scenario.py` & `Renate-0.3.0/src/renate/cli/run_experiment_with_scenario.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/cli/run_remote_job.py` & `Renate-0.3.0/src/renate/cli/run_remote_job.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/cli/run_training.py` & `Renate-0.3.0/src/renate/cli/run_training.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                 "buffer_transform",
                 "metrics_fn",
                 "scheduler_fn",
             ],
             ignore_args=["data_path", "model_state_url"],
         )
 
-        seed_everything(args.seed)
+        seed_everything(args.seed, True)
         self._prepare_data_state_model(args)
 
         data_module = get_and_setup_data_module(
             config_module,
             data_path=self._data_folder,
             prepare_data=args.prepare_data,
             **get_function_kwargs(args=args, function_args=function_args["data_module_fn"]),
```

### Comparing `Renate-0.2.1/src/renate/data/data_module.py` & `Renate-0.3.0/src/renate/data/data_module.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/data/datasets.py` & `Renate-0.3.0/src/renate/data/datasets.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/defaults.py` & `Renate-0.3.0/src/renate/defaults.py`

 * *Files 8% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 # LwF
 LWF_ALPHA = 1
 LWF_TEMPERATURE = 2
 
 MEMORY_SIZE = 32
 
 # Benchmark datasets/models
-TOKENIZER_KWARGS = dict(padding="max_length", max_length=128, truncation=True)
+TOKENIZER_KWARGS = {"padding": "max_length", "max_length": 128, "truncation": True}
 
 
 def scheduler(config_space: Dict[str, Any], mode: str, metric: str):
     return FIFOScheduler(
         config_space=config_space,
         searcher="random",
         mode=mode,
@@ -115,45 +115,45 @@
     )
 
 
 def current_timestamp() -> str:
     return str(datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S-%f"))
 
 
-def data_folder(working_directory: str):
+def data_folder(working_directory: str) -> str:
     return os.path.join(working_directory, "data")
 
 
-def input_state_folder(working_directory: str):
+def input_state_folder(working_directory: str) -> str:
     return os.path.join(working_directory, "input_state")
 
 
-def output_state_folder(working_directory: str):
+def output_state_folder(working_directory: str) -> str:
     return os.path.join(working_directory, "output_state")
 
 
-def logs_folder(working_directory: str):
+def logs_folder(working_directory: str) -> str:
     return os.path.join(working_directory, "logs")
 
 
-def model_file(state_folder: str):
+def model_file(state_folder: str) -> str:
     return os.path.join(state_folder, "model.ckpt")
 
 
 LEARNER_CHECKPOINT_NAME = "learner.ckpt"
 AVALANCHE_CHECKPOINT_NAME = "avalanche.ckpt"
 
 
-def learner_state_file(state_folder: str):
+def learner_state_file(state_folder: str) -> str:
     return os.path.join(state_folder, LEARNER_CHECKPOINT_NAME)
 
 
-def avalanche_state_file(state_folder: str):
+def avalanche_state_file(state_folder: str) -> str:
     return os.path.join(state_folder, AVALANCHE_CHECKPOINT_NAME)
 
 
-def metric_summary_file(logs_folder: str, special_str: str = ""):
+def metric_summary_file(logs_folder: str, special_str: str = "") -> str:
     return os.path.join(logs_folder, f"metrics_summary{special_str}.csv")
 
 
-def hpo_file(state_folder: str):
+def hpo_file(state_folder: str) -> str:
     return os.path.join(state_folder, "hpo.csv")
```

### Comparing `Renate-0.2.1/src/renate/evaluation/evaluator.py` & `Renate-0.3.0/src/renate/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/evaluation/metrics/classification.py` & `Renate-0.3.0/src/renate/evaluation/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/evaluation/metrics/performance_regression_metrics.py` & `Renate-0.3.0/src/renate/evaluation/metrics/performance_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/evaluation/metrics/utils.py` & `Renate-0.3.0/src/renate/evaluation/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/memory/buffer.py` & `Renate-0.3.0/src/renate/memory/buffer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
-from collections import defaultdict
 import copy
+from collections import defaultdict
 from typing import Callable, Dict, Optional
 
 import torch
 from torch.utils.data import Dataset
 
 from renate import defaults
 from renate.memory.storage import MemoryMappedTensorStorage
```

### Comparing `Renate-0.2.1/src/renate/memory/storage.py` & `Renate-0.3.0/src/renate/memory/storage.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/models/layers/cn.py` & `Renate-0.3.0/src/renate/models/layers/cn.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/models/prediction_strategies.py` & `Renate-0.3.0/src/renate/models/prediction_strategies.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/models/renate_module.py` & `Renate-0.3.0/src/renate/models/renate_module.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/training/training.py` & `Renate-0.3.0/src/renate/training/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 from syne_tune.optimizer.baselines import ASHA
 from syne_tune.optimizer.scheduler import TrialScheduler
 from syne_tune.optimizer.schedulers import FIFOScheduler
 from syne_tune.optimizer.schedulers.transfer_learning import (
     RUSHScheduler,
     TransferLearningTaskEvaluations,
 )
+from syne_tune.results_callback import StoreResultsCallback
 from syne_tune.stopping_criterion import StoppingCriterion
 from syne_tune.tuner import Tuner
-from syne_tune.tuner_callback import StoreResultsCallback
 from syne_tune.util import experiment_path
 
 import renate
 from renate import defaults
-from renate.cli.parsing_functions import to_dense_str, get_data_module_fn_kwargs
+from renate.cli.parsing_functions import get_data_module_fn_kwargs, to_dense_str
 from renate.utils.file import move_to_uri
 from renate.utils.module import get_and_prepare_data_module, import_module
 from renate.utils.syne_tune import (
     TrainingLoggerCallback,
     TuningLoggerCallback,
     best_hyperparameters,
     config_space_to_dict,
@@ -201,15 +201,18 @@
         devices=devices,
         deterministic_trainer=deterministic_trainer,
         job_name=job_name,
     )
 
 
 def _prepare_remote_job(
-    tmp_dir: str, requirements_file: Optional[str], **job_kwargs: Any
+    tmp_dir: str,
+    requirements_file: Optional[str],
+    optional_dependencies: Optional[str] = None,
+    **job_kwargs: Any,
 ) -> List[str]:
     """Prepares a SageMaker job."""
     dependencies = list(renate.__path__ + [job_kwargs["config_file"]])
 
     if "input_state_url" in job_kwargs and job_kwargs["input_state_url"] is None:
         del job_kwargs["input_state_url"]
     job_kwargs["config_file"] = os.path.basename(job_kwargs["config_file"])
@@ -219,15 +222,20 @@
     with open(jobs_kwargs_file, "w") as f:
         json.dump(job_kwargs, f)
     dependencies.append(jobs_kwargs_file)
 
     if requirements_file is None:
         requirements_file = os.path.join(tmp_dir, "requirements.txt")
         with open(requirements_file, "w") as f:
-            f.write(f"renate=={renate.__version__}")
+            f.write(
+                "Renate{}=={}".format(
+                    "" if optional_dependencies is None else f"[{optional_dependencies}]",
+                    renate.__version__,
+                )
+            )
     dependencies.append(requirements_file)
     return dependencies
 
 
 def _get_transfer_learning_task_evaluations(
     tuning_results: pd.DataFrame,
     config_space: Dict[str, Any],
@@ -606,24 +614,27 @@
 def submit_remote_job(
     source_dir: Union[str, None],
     role: str,
     instance_type: str,
     instance_count: int,
     instance_max_time: float,
     job_name: str,
+    optional_dependencies: Optional[str] = None,
     **job_kwargs: Any,
 ) -> str:
     """Executes the training job on SageMaker.
 
     See renate.train.run_training_job for a description of arguments."""
     tuning_script = str(Path(renate.__path__[0]) / "cli" / "run_remote_job.py")
     job_timestamp = defaults.current_timestamp()
     job_name = f"{job_name}-{job_timestamp}"
     tmp_dir = tempfile.mkdtemp()
-    dependencies = _prepare_remote_job(tmp_dir=tmp_dir, **job_kwargs)
+    dependencies = _prepare_remote_job(
+        tmp_dir=tmp_dir, optional_dependencies=optional_dependencies, **job_kwargs
+    )
     PyTorch(
         entry_point=tuning_script,
         source_dir=None if source_dir is None else str(source_dir),
         instance_type=instance_type,
         instance_count=instance_count,
         py_version=defaults.PYTHON_VERSION,
         framework_version=defaults.FRAMEWORK_VERSION,
```

### Comparing `Renate-0.2.1/src/renate/updaters/avalanche/learner.py` & `Renate-0.3.0/src/renate/updaters/avalanche/learner.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/updaters/avalanche/model_updater.py` & `Renate-0.3.0/src/renate/updaters/avalanche/model_updater.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/updaters/avalanche/plugins.py` & `Renate-0.3.0/src/renate/updaters/avalanche/plugins.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/updaters/experimental/er.py` & `Renate-0.3.0/src/renate/updaters/experimental/er.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/updaters/experimental/fine_tuning.py` & `Renate-0.3.0/src/renate/updaters/experimental/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/updaters/experimental/gdumb.py` & `Renate-0.3.0/src/renate/updaters/experimental/gdumb.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/updaters/experimental/joint.py` & `Renate-0.3.0/src/renate/updaters/experimental/joint.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/updaters/experimental/offline_er.py` & `Renate-0.3.0/src/renate/updaters/experimental/offline_er.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/updaters/experimental/repeated_distill.py` & `Renate-0.3.0/src/renate/updaters/experimental/repeated_distill.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/updaters/learner.py` & `Renate-0.3.0/src/renate/updaters/learner.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/updaters/learner_components/component.py` & `Renate-0.3.0/src/renate/updaters/learner_components/component.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/updaters/learner_components/losses.py` & `Renate-0.3.0/src/renate/updaters/learner_components/losses.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/updaters/learner_components/reinitialization.py` & `Renate-0.3.0/src/renate/updaters/learner_components/reinitialization.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/updaters/model_updater.py` & `Renate-0.3.0/src/renate/updaters/model_updater.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/utils/avalanche.py` & `Renate-0.3.0/src/renate/utils/avalanche.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/utils/config_spaces.py` & `Renate-0.3.0/src/renate/utils/config_spaces.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/utils/file.py` & `Renate-0.3.0/src/renate/utils/file.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/utils/module.py` & `Renate-0.3.0/src/renate/utils/module.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/utils/optimizer.py` & `Renate-0.3.0/src/renate/utils/optimizer.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/utils/pytorch.py` & `Renate-0.3.0/src/renate/utils/pytorch.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/src/renate/utils/syne_tune.py` & `Renate-0.3.0/src/renate/utils/syne_tune.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/conftest.py` & `Renate-0.3.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/dummy_datasets.py` & `Renate-0.3.0/test/dummy_datasets.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/integration_tests/configs/updaters/super-er-buffer500.json` & `Renate-0.3.0/test/integration_tests/configs/updaters/super-er-buffer500.json`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/integration_tests/run_experiment.py` & `Renate-0.3.0/test/integration_tests/run_experiment.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         default=0,
         help="Seed.",
     )
     parser.add_argument(
         f"--max-time",
         type=int,
         default=12 * 3600,
-        help="Seed.",
+        help="Maximum execution time.",
     )
     args = parser.parse_args()
     config_space = load_config(
         args.scenario_file, args.model_file, args.updater_file, args.dataset_file
     )
     if args.backend == "local":
         experiment_outputs_url = (
```

### Comparing `Renate-0.2.1/test/integration_tests/run_quick_test.py` & `Renate-0.3.0/test/integration_tests/run_quick_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 import argparse
 import json
 import os
 import subprocess
 from pathlib import Path
+from sys import platform
 
 import pandas as pd
 import pytest
 
 from renate import defaults
 
 if __name__ == "__main__":
@@ -46,25 +47,23 @@
             "--job-name",
             job_name,
             "--test-suite",
             test_suite,
         ]
     )
     process.wait()
-    num_updates = len(test_config["expected_accuracy"])
+    expected_accuracy = test_config[f"expected_accuracy_{platform}"]
+    num_updates = len(test_config["expected_accuracy_darwin"][0])
     result_file = (
         Path("tmp")
         / "renate-integration-tests"
         / test_suite
         / job_name
         / "logs"
         / f"metrics_summary_update_{num_updates - 1}.csv"
     )
     if result_file.exists():
         df = pd.read_csv(result_file)
         accuracies = [float(acc) for acc in list(df.iloc[-1])[1:]]
     else:
         accuracies = []
-
-    # Noticed different accuracy scores across Mac and GitHub Actions Workflows (which run on Linux)
-    # TODO see if we can align the Mac and Linux results
-    assert pytest.approx(test_config["expected_accuracy"]) == accuracies
+    assert any([pytest.approx(acc) == accuracies for acc in expected_accuracy]), accuracies
```

### Comparing `Renate-0.2.1/test/renate/benchmark/models/test_mlp.py` & `Renate-0.3.0/test/renate/benchmark/models/test_mlp.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/benchmark/models/test_vision_transformer.py` & `Renate-0.3.0/test/renate/benchmark/models/test_vision_transformer.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/benchmark/test_experimentation.py` & `Renate-0.3.0/test/renate/benchmark/test_experimentation.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/benchmark/test_experimentation_config.py` & `Renate-0.3.0/test/renate/benchmark/test_experimentation_config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 import pytest
 from torchvision.transforms import Compose, Normalize
 
 from renate.benchmark import experiment_config
+from renate.benchmark.datasets.nlp_datasets import HuggingFaceTextDataModule
 from renate.benchmark.datasets.vision_datasets import CLEARDataModule, TorchVisionDataModule
 from renate.benchmark.experiment_config import (
     data_module_fn,
     get_data_module,
     get_scenario,
     model_fn,
     models,
@@ -17,70 +18,143 @@
     BenchmarkScenario,
     ClassIncrementalScenario,
     FeatureSortingScenario,
     HueShiftScenario,
     IIDScenario,
     ImageRotationScenario,
     PermutationScenario,
+    WildTimeScenario,
 )
+from renate.models.prediction_strategies import ICaRLClassificationStrategy
 
 
 @pytest.mark.parametrize(
     "model_name,expected_model_class",
-    [(model_name, model_class) for model_name, model_class in zip(models.keys(), models.values())],
+    [(model_name, model_class) for model_name, model_class in models.items()],
 )
 def test_model_fn(model_name, expected_model_class):
     model = model_fn(
         model_state_url=None,
         model_name=model_name,
         num_inputs=1 if model_name == "MultiLayerPerceptron" else None,
-        num_outputs=1 if model_name == "MultiLayerPerceptron" else None,
+        num_outputs=1 if model_name in ["MultiLayerPerceptron", "HuggingFaceTransformer"] else None,
         num_hidden_layers=1 if model_name == "MultiLayerPerceptron" else None,
         hidden_size=1 if model_name == "MultiLayerPerceptron" else None,
+        pretrained_model_name="distilbert-base-uncased"
+        if model_name == "HuggingFaceTransformer"
+        else None,
     )
     assert isinstance(model, expected_model_class)
 
 
+@pytest.mark.parametrize(
+    "dataset_name,expected_in_channels",
+    (
+        ("FashionMNIST", 1),
+        ("MNIST", 1),
+        ("yearbook", 1),
+        ("CIFAR10", 3),
+        ("CIFAR100", 3),
+        ("fmow", 3),
+    ),
+)
+def test_model_fn_automatic_input_channel_detection_resnet(dataset_name, expected_in_channels):
+    """Tests if ResNet architectures input channels are correctly adapted to the dataset."""
+    model = model_fn(
+        model_state_url=None,
+        model_name="ResNet18",
+        dataset_name=dataset_name,
+    )
+    assert model.get_backbone().conv1.in_channels == expected_in_channels
+
+
 def test_model_fn_fails_for_unknown_model():
     unknown_model_name = "UNKNOWN_MODEL_NAME"
     with pytest.raises(ValueError, match=f"Unknown model `{unknown_model_name}`"):
         model_fn(model_name=unknown_model_name)
 
 
 @pytest.mark.parametrize(
-    "dataset_name,data_module_class",
-    (("CIFAR10", TorchVisionDataModule), ("CLEAR10", CLEARDataModule)),
+    "dataset_name,data_module_class,pretrained_model_name,input_column,target_column",
+    (
+        ("CIFAR10", TorchVisionDataModule, None, None, None),
+        ("CLEAR10", CLEARDataModule, None, None, None),
+        (
+            "hfd-rotten-tomatoes",
+            HuggingFaceTextDataModule,
+            "distilbert-base-uncased",
+            "text",
+            "label",
+        ),
+    ),
 )
-def test_get_data_module(tmpdir, dataset_name, data_module_class):
-    data_module = get_data_module(data_path=tmpdir, dataset_name=dataset_name, val_size=0.5, seed=0)
+def test_get_data_module(
+    tmpdir, dataset_name, data_module_class, pretrained_model_name, input_column, target_column
+):
+    data_module = get_data_module(
+        data_path=tmpdir,
+        dataset_name=dataset_name,
+        val_size=0.5,
+        seed=0,
+        src_bucket=None,
+        src_object_name=None,
+        pretrained_model_name=pretrained_model_name,
+        input_column=input_column,
+        target_column=target_column,
+    )
     assert isinstance(data_module, data_module_class)
 
 
 def test_get_data_module_fails_for_unknown_dataset(tmpdir):
     unknown_dataset_name = "UNKNOWN_DATASET_NAME"
     with pytest.raises(ValueError, match=f"Unknown dataset `{unknown_dataset_name}`"):
-        get_data_module(data_path=tmpdir, dataset_name=unknown_dataset_name, val_size=0.5, seed=0)
+        get_data_module(
+            data_path=tmpdir,
+            dataset_name=unknown_dataset_name,
+            val_size=0.5,
+            seed=0,
+            src_bucket=None,
+            src_object_name=None,
+            pretrained_model_name=None,
+            input_column=None,
+            target_column=None,
+        )
 
 
 def test_get_scenario_fails_for_unknown_scenario(tmpdir):
-    data_module = get_data_module(data_path=tmpdir, dataset_name="MNIST", val_size=0.5, seed=0)
+    data_module = get_data_module(
+        data_path=tmpdir,
+        dataset_name="MNIST",
+        val_size=0.5,
+        seed=0,
+        src_bucket=None,
+        src_object_name=None,
+        pretrained_model_name=None,
+        input_column=None,
+        target_column=None,
+    )
     unknown_scenario_name = "UNKNOWN_SCENARIO_NAME"
     with pytest.raises(ValueError, match=f"Unknown scenario `{unknown_scenario_name}`"):
         get_scenario(
             scenario_name=unknown_scenario_name, data_module=data_module, chunk_id=0, seed=0
         )
 
 
 @pytest.mark.parametrize(
     "scenario_name,dataset_name,scenario_kwargs,expected_scenario_class,expected_num_tasks",
     (
         (
             "ClassIncrementalScenario",
-            "CIFAR10",
-            {"class_groupings": ((0, 1), (2, 3, 4), (5, 6))},
+            "hfd-trec",
+            {
+                "pretrained_model_name": "distilbert-base-uncased",
+                "input_column": "text",
+                "target_column": "coarse_label",
+                "class_groupings": ((0, 1), (2, 3), (4, 5)),
+            },
             ClassIncrementalScenario,
             3,
         ),
         (
             "IIDScenario",
             "MNIST",
             {"num_tasks": 3},
@@ -116,23 +190,39 @@
         (
             "HueShiftScenario",
             "CIFAR10",
             {"num_tasks": 3, "randomness": 0.5},
             HueShiftScenario,
             3,
         ),
+        (
+            "WildTimeScenario",
+            "arxiv",
+            {"num_tasks": 3, "pretrained_model_name": "distilbert-base-uncased"},
+            WildTimeScenario,
+            3,
+        ),
+        (
+            "WildTimeScenario",
+            "fmow",
+            {},
+            WildTimeScenario,
+            16,
+        ),
     ),
     ids=[
-        "class_incremental_image",
+        "class_incremental",
         "iid",
         "rotation",
         "benchmark",
         "permutation",
         "feature_sorting",
         "hue_shift",
+        "wild_time_text_with_tokenizer",
+        "wild_time_image_all_tasks",
     ],
 )
 @pytest.mark.parametrize("val_size", (0, 0.5), ids=["no_val", "val"])
 def test_data_module_fn(
     tmpdir,
     scenario_name,
     dataset_name,
@@ -150,24 +240,35 @@
         val_size=val_size,
         **scenario_kwargs,
     )
     assert isinstance(scenario, expected_scenario_class)
     if expected_scenario_class == ClassIncrementalScenario:
         assert scenario._class_groupings == scenario_kwargs["class_groupings"]
     elif expected_scenario_class == FeatureSortingScenario:
-        scenario._feature_idx = scenario_kwargs["feature_idx"]
-        scenario._randomness = scenario_kwargs["randomness"]
+        assert scenario._feature_idx == scenario_kwargs["feature_idx"]
+        assert scenario._randomness == scenario_kwargs["randomness"]
     elif expected_scenario_class == HueShiftScenario:
-        scenario._randomness = scenario_kwargs["randomness"]
+        assert scenario._randomness == scenario_kwargs["randomness"]
+    elif expected_scenario_class == WildTimeScenario:
+        if "pretrained_model_name" in scenario_kwargs:
+            assert scenario._data_module._tokenizer is not None
+        else:
+            assert scenario._data_module._tokenizer is None
     assert scenario._num_tasks == expected_num_tasks
 
 
 @pytest.mark.parametrize(
     "dataset_name,use_transforms",
-    (("MNIST", False), ("FashionMNIST", False), ("CIFAR10", True), ("CIFAR100", True)),
+    (
+        ("MNIST", False),
+        ("FashionMNIST", False),
+        ("CIFAR10", True),
+        ("CIFAR100", True),
+        ("hfd-rotten_tomatoes", False),
+    ),
 )
 def test_transforms(dataset_name, use_transforms):
     train_preprocessing = train_transform(dataset_name)
     test_preprocessing = experiment_config.test_transform(dataset_name)
     if use_transforms:
         assert isinstance(train_preprocessing, Compose)
         assert isinstance(test_preprocessing, Normalize)
@@ -177,7 +278,31 @@
 
 
 def test_transforms_fails_for_unknown_dataset():
     unknown_dataset_set = "UNKNOWN_DATASET_NAME"
     for transform_function in [train_transform, experiment_config.test_transform]:
         with pytest.raises(ValueError, match=f"Unknown dataset `{unknown_dataset_set}`"):
             transform_function(unknown_dataset_set)
+
+
+@pytest.mark.parametrize("model_name", [model_name for model_name in models])
+@pytest.mark.parametrize("updater", ("ER", "Avalanche-iCaRL"))
+def test_prediction_strategy_is_correctly_set(model_name, updater):
+    """If iCaRL is used, the model prediction strategy must be changed."""
+    model_kwargs = {
+        "model_name": model_name,
+        "updater": updater,
+        "num_outputs": 2,
+    }
+    if model_name == "MultiLayerPerceptron":
+        model_kwargs.update({"num_inputs": 10, "hidden_size": 10, "num_hidden_layers": 2})
+    elif model_name == "HuggingFaceTransformer":
+        model_kwargs["pretrained_model_name"] = "distilbert-base-uncased"
+    if model_name == "HuggingFaceTransformer" and updater == "Avalanche-iCaRL":
+        with pytest.raises(ValueError, match="Transformers do not support iCaRL."):
+            model_fn(**model_kwargs)
+    else:
+        model = model_fn(**model_kwargs)
+        if updater == "ER":
+            assert not hasattr(model, "_prediction_strategy") or model._prediction_strategy is None
+        else:
+            assert isinstance(model._prediction_strategy, ICaRLClassificationStrategy)
```

### Comparing `Renate-0.2.1/test/renate/benchmark/test_scenarios.py` & `Renate-0.3.0/test/renate/benchmark/test_scenarios.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/cli/test_parsing_functions.py` & `Renate-0.3.0/test/renate/cli/test_parsing_functions.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/data/test_data_module.py` & `Renate-0.3.0/test/renate/data/test_data_module.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 import pandas as pd
 import pytest
 import torch
 import transformers
 from torch.utils.data import Dataset, TensorDataset
 
-from renate.benchmark.datasets.nlp_datasets import HuggingfaceTextDataModule
+from renate.benchmark.datasets.nlp_datasets import HuggingFaceTextDataModule
 from renate.benchmark.datasets.vision_datasets import (
     CLEARDataModule,
     TinyImageNetDataModule,
     TorchVisionDataModule,
 )
 from renate.data import CSVDataModule
 
@@ -146,18 +146,18 @@
 @pytest.mark.parametrize(
     "tokenizer_kwargs",
     [
         None,
         dict(padding="longest", max_length=512, truncation=True),
     ],
 )
-def test_huggingface_data_module(
+def test_hugging_face_data_module(
     tmpdir, dataset_name, input_column, target_column, tokenizer, tokenizer_kwargs
 ):
-    data_module = HuggingfaceTextDataModule(
+    data_module = HuggingFaceTextDataModule(
         data_path=tmpdir,
         dataset_name=dataset_name,
         input_column=input_column,
         target_column=target_column,
         tokenizer=tokenizer,
         tokenizer_kwargs=tokenizer_kwargs,
         val_size=0.2,
@@ -173,7 +173,39 @@
     for dataset in [train_data, val_data, test_data]:
         inputs, targets = dataset[0]
         assert isinstance(targets, torch.Tensor)
         assert isinstance(inputs, dict)
         assert set(inputs.keys()) == set(["input_ids", "attention_mask"])
         assert isinstance(inputs["input_ids"], torch.Tensor)
         assert isinstance(inputs["attention_mask"], torch.Tensor)
+
+
+@pytest.mark.parametrize("column", ("input", "target"), ids=("input", "target"))
+def test_hugging_face_exception_raised_with_wrong_column(tmpdir, column):
+    input_column = "text"
+    target_column = "label"
+    if column == "input":
+        input_column = "WRONG_COLUMN"
+    elif column == "target":
+        target_column = "WRONG_COLUMN"
+    data_module = HuggingFaceTextDataModule(
+        data_path=tmpdir,
+        dataset_name="rotten_tomatoes",
+        input_column=input_column,
+        target_column=target_column,
+        tokenizer=None,
+        val_size=0.2,
+    )
+    if column == "input":
+        with pytest.raises(
+            ValueError,
+            match="Input column 'WRONG_COLUMN' does not exist in rotten_tomatoes. "
+            "Available columns: \\['text', 'label'\\].",
+        ):
+            data_module.prepare_data()
+    elif column == "target":
+        with pytest.raises(
+            ValueError,
+            match="Target column 'WRONG_COLUMN' does not exist in rotten_tomatoes. "
+            "Available columns: \\['text', 'label'\\].",
+        ):
+            data_module.prepare_data()
```

### Comparing `Renate-0.2.1/test/renate/data/test_datasets.py` & `Renate-0.3.0/test/renate/data/test_datasets.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/evaluation/metrics/test_classification.py` & `Renate-0.3.0/test/renate/evaluation/metrics/test_classification.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/evaluation/metrics/test_regression_metrics.py` & `Renate-0.3.0/test/renate/evaluation/metrics/test_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/memory/test_buffer.py` & `Renate-0.3.0/test/renate/memory/test_buffer.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/memory/test_storage.py` & `Renate-0.3.0/test/renate/memory/test_storage.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/models/test_renate_module.py` & `Renate-0.3.0/test/renate/models/test_renate_module.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/renate_config_files/config.py` & `Renate-0.3.0/test/renate/renate_config_files/config.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/renate_config_files/config_scenario.py` & `Renate-0.3.0/test/renate/renate_config_files/config_scenario.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/training/test_run_training.py` & `Renate-0.3.0/test/renate/training/test_run_training.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/updaters/avalanche/test_avalanche_learner.py` & `Renate-0.3.0/test/renate/updaters/avalanche/test_avalanche_learner.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/updaters/avalanche/test_avalanche_model_updater.py` & `Renate-0.3.0/test/renate/updaters/avalanche/test_avalanche_model_updater.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/updaters/avalanche/test_avalanche_plugins.py` & `Renate-0.3.0/test/renate/updaters/avalanche/test_avalanche_plugins.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/updaters/experimental/test_er.py` & `Renate-0.3.0/test/renate/updaters/experimental/test_er.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/updaters/experimental/test_fine_tuning.py` & `Renate-0.3.0/test/renate/updaters/experimental/test_fine_tuning.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/updaters/experimental/test_joint.py` & `Renate-0.3.0/test/renate/updaters/experimental/test_joint.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/updaters/experimental/test_repeated_distill.py` & `Renate-0.3.0/test/renate/updaters/experimental/test_repeated_distill.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/updaters/test_learner.py` & `Renate-0.3.0/test/renate/updaters/test_learner.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/updaters/test_model_updater.py` & `Renate-0.3.0/test/renate/updaters/test_model_updater.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/utils/test_avalanche.py` & `Renate-0.3.0/test/renate/utils/test_avalanche.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/utils/test_file.py` & `Renate-0.3.0/test/renate/utils/test_file.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/utils/test_metrics_utils.py` & `Renate-0.3.0/test/renate/utils/test_metrics_utils.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/utils/test_optimizer.py` & `Renate-0.3.0/test/renate/utils/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/utils/test_pytorch.py` & `Renate-0.3.0/test/renate/utils/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `Renate-0.2.1/test/renate/utils/test_syne_tune.py` & `Renate-0.3.0/test/renate/utils/test_syne_tune.py`

 * *Files identical despite different names*

