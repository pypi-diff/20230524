# Comparing `tmp/getdaft-0.1.2.tar.gz` & `tmp/getdaft-0.1.3.tar.gz`

## Comparing `getdaft-0.1.2.tar` & `getdaft-0.1.3.tar`

### file list

```diff
@@ -1,444 +1,445 @@
--rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 getdaft-0.1.2/Cargo.toml
--rw-r--r--   0      501       20      834 2023-05-22 23:15:06.000000 getdaft-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0      501       20      595 2023-05-22 23:15:06.000000 getdaft-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0      501       20      428 2023-05-22 23:15:06.000000 getdaft-0.1.2/.github/dependabot.yml
--rw-r--r--   0      501       20     1333 2023-05-22 23:15:06.000000 getdaft-0.1.2/.github/workflows/broken-link-checker.yml
--rw-r--r--   0      501       20     3378 2023-05-22 23:15:06.000000 getdaft-0.1.2/.github/workflows/daft-profiling.yml
--rw-r--r--   0      501       20     1627 2023-05-22 23:15:06.000000 getdaft-0.1.2/.github/workflows/notebook-checker.yml
--rw-r--r--   0      501       20     2194 2023-05-22 23:15:06.000000 getdaft-0.1.2/.github/workflows/property-based-tests.yml
--rw-r--r--   0      501       20    12886 2023-05-22 23:15:06.000000 getdaft-0.1.2/.github/workflows/python-package.yml
--rw-r--r--   0      501       20     6168 2023-05-22 23:15:06.000000 getdaft-0.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0      501       20     2638 2023-05-22 23:15:06.000000 getdaft-0.1.2/.github/workflows/ray-compatibility.yml
--rw-r--r--   0      501       20      300 2023-05-22 23:15:06.000000 getdaft-0.1.2/.gitignore
--rw-r--r--   0      501       20     2126 2023-05-22 23:15:07.000000 getdaft-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0      501       20      205 2023-05-22 23:15:07.000000 getdaft-0.1.2/.readthedocs.yaml
--rw-r--r--   0      501       20     1550 2023-05-22 23:15:07.000000 getdaft-0.1.2/CONTRIBUTING.md
--rw-r--r--   0      501       20    11357 2023-05-22 23:15:07.000000 getdaft-0.1.2/LICENSE
--rw-r--r--   0      501       20     1295 2023-05-22 23:15:07.000000 getdaft-0.1.2/Makefile
--rw-r--r--   0      501       20     6126 2023-05-22 23:15:07.000000 getdaft-0.1.2/README.rst
--rw-r--r--   0      501       20        0 2023-05-22 23:15:07.000000 getdaft-0.1.2/benchmarking/__init__.py
--rw-r--r--   0      501       20        0 2023-05-22 23:15:07.000000 getdaft-0.1.2/benchmarking/tpch/__init__.py
--rw-r--r--   0      501       20     9495 2023-05-22 23:15:07.000000 getdaft-0.1.2/benchmarking/tpch/__main__.py
--rw-r--r--   0      501       20    12428 2023-05-22 23:15:07.000000 getdaft-0.1.2/benchmarking/tpch/answers.py
--rw-r--r--   0      501       20    12140 2023-05-22 23:15:07.000000 getdaft-0.1.2/benchmarking/tpch/data_generation.py
--rw-r--r--   0      501       20     4573 2023-05-22 23:15:07.000000 getdaft-0.1.2/benchmarking/tpch/pipelined_data_generation.py
--rw-r--r--   0      501       20     1436 2023-05-22 23:15:07.000000 getdaft-0.1.2/ci/upload_wheels.sh
--rw-r--r--   0      501       20      440 2023-05-22 23:15:07.000000 getdaft-0.1.2/codecov.yml
--rw-r--r--   0      501       20     2092 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/__init__.py
--rw-r--r--   0      501       20     6724 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/analytics.py
--rw-r--r--   0      501       20     3935 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/api_annotations.py
--rw-r--r--   0      501       20    10591 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/arrow_utils.py
--rw-r--r--   0      501       20     6182 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/context.py
--rw-r--r--   0      501       20     3403 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/convert.py
--rw-r--r--   0      501       20       94 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/dataframe/__init__.py
--rw-r--r--   0      501       20    49646 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/dataframe/dataframe.py
--rw-r--r--   0      501       20      306 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/dataframe/preview.py
--rw-r--r--   0      501       20      850 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/datasources.py
--rw-r--r--   0      501       20    10207 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/datatype.py
--rw-r--r--   0      501       20       84 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/errors.py
--rw-r--r--   0      501       20        0 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/execution/__init__.py
--rw-r--r--   0      501       20    24879 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/execution/execution_step.py
--rw-r--r--   0      501       20     4231 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/execution/logical_op_runners.py
--rw-r--r--   0      501       20    27790 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/execution/physical_plan.py
--rw-r--r--   0      501       20     6110 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/execution/physical_plan_factory.py
--rw-r--r--   0      501       20      170 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/expressions/__init__.py
--rw-r--r--   0      501       20    24529 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/expressions/expressions.py
--rw-r--r--   0      501       20      572 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/expressions/testing.py
--rw-r--r--   0      501       20    12728 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/filesystem.py
--rw-r--r--   0      501       20        0 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/internal/__init__.py
--rw-r--r--   0      501       20      509 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/internal/gpu.py
--rw-r--r--   0      501       20     1804 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/internal/rule.py
--rw-r--r--   0      501       20     1965 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/internal/rule_runner.py
--rw-r--r--   0      501       20     3490 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/internal/treenode.py
--rw-r--r--   0      501       20      263 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/io/__init__.py
--rw-r--r--   0      501       20     1682 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/io/_csv.py
--rw-r--r--   0      501       20     1223 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/io/_json.py
--rw-r--r--   0      501       20     2032 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/io/common.py
--rw-r--r--   0      501       20     2034 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/io/file_path.py
--rw-r--r--   0      501       20     1243 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/io/parquet.py
--rw-r--r--   0      501       20      264 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/logging.py
--rw-r--r--   0      501       20        0 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/logical/__init__.py
--rw-r--r--   0      501       20     8601 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/logical/aggregation_plan_builder.py
--rw-r--r--   0      501       20    37496 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/logical/logical_plan.py
--rw-r--r--   0      501       20     1492 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/logical/map_partition_ops.py
--rw-r--r--   0      501       20    19183 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/logical/optimizer.py
--rw-r--r--   0      501       20     3625 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/logical/schema.py
--rw-r--r--   0      501       20       99 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/pickle/__init__.py
--rw-r--r--   0      501       20    34760 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/pickle/cloudpickle.py
--rw-r--r--   0      501       20    34262 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/pickle/cloudpickle_fast.py
--rw-r--r--   0      501       20      639 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/pickle/compat.py
--rw-r--r--   0      501       20      312 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/pickle/pickle.py
--rw-r--r--   0      501       20     2036 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/resource_request.py
--rw-r--r--   0      501       20        0 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/runners/__init__.py
--rw-r--r--   0      501       20     5708 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/runners/partitioning.py
--rw-r--r--   0      501       20     1488 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/runners/profiler.py
--rw-r--r--   0      501       20    13059 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/runners/pyrunner.py
--rw-r--r--   0      501       20    25545 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/runners/ray_runner.py
--rw-r--r--   0      501       20      918 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/runners/runner.py
--rw-r--r--   0      501       20     4324 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/runners/runner_io.py
--rw-r--r--   0      501       20    18981 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/series.py
--rw-r--r--   0      501       20       82 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/table/__init__.py
--rw-r--r--   0      501       20    13420 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/table/table.py
--rw-r--r--   0      501       20     9665 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/table/table_io.py
--rw-r--r--   0      501       20     7263 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/udf.py
--rw-r--r--   0      501       20        0 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/udf_library/__init__.py
--rw-r--r--   0      501       20     3486 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/udf_library/url_udfs.py
--rw-r--r--   0      501       20     2697 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/utils.py
--rw-r--r--   0      501       20      183 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/viz/__init__.py
--rw-r--r--   0      501       20     1699 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/viz/dataframe_display.py
--rw-r--r--   0      501       20     1517 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/viz/html_viz_hooks.py
--rw-r--r--   0      501       20     5738 2023-05-22 23:15:07.000000 getdaft-0.1.2/daft/viz/repr.py
--rw-r--r--   0      501       20      148 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/CONTRIBUTING.md
--rw-r--r--   0      501       20      638 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/Makefile
--rw-r--r--   0      501       20    71692 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/10-min.ipynb
--rw-r--r--   0      501       20      389 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/_static/custom-function-signatures.css
--rw-r--r--   0      501       20      565 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/_static/daft-favicon.png
--rw-r--r--   0      501       20     7804 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/_static/daft-logo.png
--rw-r--r--   0      501       20    42148 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/_static/daft_illustration.png
--rw-r--r--   0      501       20    25200 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/_static/execution_model.png
--rw-r--r--   0      501       20     1901 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/_static/header.css
--rw-r--r--   0      501       20    32864 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/_static/high_level_architecture.png
--rw-r--r--   0      501       20      343 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/_static/icon-menu-close.svg
--rw-r--r--   0      501       20      333 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/_static/icon-menu-dots.svg
--rw-r--r--   0      501       20    18177 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/_static/in_memory_data_representation.png
--rw-r--r--   0      501       20      786 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/_static/mobile-menu.js
--rw-r--r--   0      501       20      856 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/_templates/layout.html
--rw-r--r--   0      501       20      994 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/_templates/sections/header.html
--rw-r--r--   0      501       20      957 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/_templates/sections/mobile-menu.html
--rw-r--r--   0      501       20      325 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/api_docs/context.rst
--rw-r--r--   0      501       20     2564 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/api_docs/dataframe.rst
--rw-r--r--   0      501       20     3444 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/api_docs/expressions.rst
--rw-r--r--   0      501       20      784 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/api_docs/groupby.rst
--rw-r--r--   0      501       20      124 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/api_docs/index.rst
--rw-r--r--   0      501       20     1457 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/api_docs/input_output.rst
--rw-r--r--   0      501       20       88 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/api_docs/udf.rst
--rw-r--r--   0      501       20     3547 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/conf.py
--rw-r--r--   0      501       20     4964 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/dataframe_comparison.rst
--rw-r--r--   0      501       20     1645 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/index.rst
--rw-r--r--   0      501       20     1089 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/install.rst
--rw-r--r--   0      501       20      743 2023-05-22 23:15:07.000000 getdaft-0.1.2/docs/source/learn/index.rst
--rw-r--r--   0      501       20     7586 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/learn/key_concepts.rst
--rw-r--r--   0      501       20     1398 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/learn/tutorials.rst
--rw-r--r--   0      501       20     1388 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/learn/user_guides/aggregations.rst
--rw-r--r--   0      501       20     6686 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/learn/user_guides/dataframe-operations.rst
--rw-r--r--   0      501       20     9024 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/learn/user_guides/expressions.rst
--rw-r--r--   0      501       20     7829 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/learn/user_guides/intro-dataframes.rst
--rw-r--r--   0      501       20      206 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/learn/user_guides/partitioning.rst
--rw-r--r--   0      501       20     3190 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/learn/user_guides/read-write.rst
--rw-r--r--   0      501       20     1257 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/learn/user_guides/scaling-up.rst
--rw-r--r--   0      501       20     8691 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/learn/user_guides/udf.rst
--rw-r--r--   0      501       20     1551 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/learn/user_guides.rst
--rw-r--r--   0      501       20     3575 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/release_notes/0.0.13.rst
--rw-r--r--   0      501       20     2241 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/release_notes/0.0.14.rst
--rw-r--r--   0      501       20     1913 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/release_notes/0.0.16.rst
--rw-r--r--   0      501       20     1750 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/release_notes/0.0.17.rst
--rw-r--r--   0      501       20     2100 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/release_notes/0.0.18.rst
--rw-r--r--   0      501       20     3647 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/release_notes/0.0.19.rst
--rw-r--r--   0      501       20     4240 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/release_notes/0.0.20.rst
--rw-r--r--   0      501       20     4633 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/release_notes/0.0.21.rst
--rw-r--r--   0      501       20     8016 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/release_notes/0.0.22.rst
--rw-r--r--   0      501       20     5385 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/release_notes/0.0.23.rst
--rw-r--r--   0      501       20    11759 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/release_notes/0.0.24.rst
--rw-r--r--   0      501       20     4750 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/release_notes/0.1.0.rst
--rw-r--r--   0      501       20     2411 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/release_notes/0.1.1.rst
--rw-r--r--   0      501       20     2549 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/release_notes/0.1.2.rst
--rw-r--r--   0      501       20      935 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/release_notes/_template.rst
--rw-r--r--   0      501       20      331 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/release_notes/index.rst
--rw-r--r--   0      501       20     6574 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/technical_architecture.rst
--rw-r--r--   0      501       20     1316 2023-05-22 23:15:08.000000 getdaft-0.1.2/docs/source/telemetry.rst
--rw-r--r--   0      501       20     1873 2023-05-22 23:15:08.000000 getdaft-0.1.2/pyproject.toml
--rw-r--r--   0      501       20      680 2023-05-22 23:15:08.000000 getdaft-0.1.2/requirements-dev.txt
--rw-r--r--   0      501       20       98 2023-05-22 23:15:08.000000 getdaft-0.1.2/rust-toolchain.toml
--rw-r--r--   0      501       20     4466 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/from.rs
--rw-r--r--   0      501       20      734 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/iterator.rs
--rw-r--r--   0      501       20     2945 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/mod.rs
--rw-r--r--   0      501       20      257 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/abs.rs
--rw-r--r--   0      501       20      726 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/apply.rs
--rw-r--r--   0      501       20      841 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/arange.rs
--rw-r--r--   0      501       20     6964 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/arithmetic.rs
--rw-r--r--   0      501       20     3048 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/arrow2/comparison.rs
--rw-r--r--   0      501       20       34 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/arrow2/mod.rs
--rw-r--r--   0      501       20       19 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/arrow2/sort/mod.rs
--rw-r--r--   0      501       20     3482 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/arrow2/sort/primitive/common.rs
--rw-r--r--   0      501       20      723 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/arrow2/sort/primitive/indices.rs
--rw-r--r--   0      501       20       47 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/arrow2/sort/primitive/mod.rs
--rw-r--r--   0      501       20     8075 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/arrow2/sort/primitive/sort.rs
--rw-r--r--   0      501       20     2861 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/as_arrow.rs
--rw-r--r--   0      501       20    11304 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/broadcast.rs
--rw-r--r--   0      501       20    19737 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/cast.rs
--rw-r--r--   0      501       20    11017 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/compare_agg.rs
--rw-r--r--   0      501       20    47218 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/comparison.rs
--rw-r--r--   0      501       20     1634 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/concat.rs
--rw-r--r--   0      501       20     5982 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/concat_agg.rs
--rw-r--r--   0      501       20     1433 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/count.rs
--rw-r--r--   0      501       20     1550 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/date.rs
--rw-r--r--   0      501       20     2889 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/filter.rs
--rw-r--r--   0      501       20     1264 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/float.rs
--rw-r--r--   0      501       20     1936 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/full.rs
--rw-r--r--   0      501       20     4112 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/groups.rs
--rw-r--r--   0      501       20     1515 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/hash.rs
--rw-r--r--   0      501       20    12019 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/if_else.rs
--rw-r--r--   0      501       20     1058 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/len.rs
--rw-r--r--   0      501       20     3446 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/list.rs
--rw-r--r--   0      501       20     3360 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/list_agg.rs
--rw-r--r--   0      501       20     1622 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/mean.rs
--rw-r--r--   0      501       20     2595 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/mod.rs
--rw-r--r--   0      501       20     1156 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/null.rs
--rw-r--r--   0      501       20     3819 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/pairwise.rs
--rw-r--r--   0      501       20      484 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/search_sorted.rs
--rw-r--r--   0      501       20    19071 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/sort.rs
--rw-r--r--   0      501       20     2383 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/sum.rs
--rw-r--r--   0      501       20    15006 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/take.rs
--rw-r--r--   0      501       20     5279 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/ops/utf8.rs
--rw-r--r--   0      501       20      995 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/pseudo_arrow/compute.rs
--rw-r--r--   0      501       20    13611 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/pseudo_arrow/mod.rs
--rw-r--r--   0      501       20     2502 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/array/pseudo_arrow/python.rs
--rw-r--r--   0      501       20    13119 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/datatypes/dtype.rs
--rw-r--r--   0      501       20     2012 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/datatypes/field.rs
--rw-r--r--   0      501       20     2744 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/datatypes/logical.rs
--rw-r--r--   0      501       20     8970 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/datatypes/matching.rs
--rw-r--r--   0      501       20     6650 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/datatypes/mod.rs
--rw-r--r--   0      501       20     1083 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/datatypes/time_unit.rs
--rw-r--r--   0      501       20      273 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/README.md
--rw-r--r--   0      501       20     1474 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/arithmetic.rs
--rw-r--r--   0      501       20    21828 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/expr.rs
--rw-r--r--   0      501       20     1421 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/functions/float/is_nan.rs
--rw-r--r--   0      501       20      587 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/functions/float/mod.rs
--rw-r--r--   0      501       20     1112 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/functions/list/explode.rs
--rw-r--r--   0      501       20      597 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/functions/list/mod.rs
--rw-r--r--   0      501       20     1774 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/functions/mod.rs
--rw-r--r--   0      501       20     1178 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/functions/numeric/abs.rs
--rw-r--r--   0      501       20      580 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/functions/numeric/mod.rs
--rw-r--r--   0      501       20      676 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/functions/python/mod.rs
--rw-r--r--   0      501       20     2050 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/functions/python/partial_udf.rs
--rw-r--r--   0      501       20     2769 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/functions/python/udf.rs
--rw-r--r--   0      501       20     1310 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/functions/temporal/day.rs
--rw-r--r--   0      501       20     1338 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/functions/temporal/day_of_week.rs
--rw-r--r--   0      501       20     1425 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/functions/temporal/mod.rs
--rw-r--r--   0      501       20     1320 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/functions/temporal/month.rs
--rw-r--r--   0      501       20     1314 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/functions/temporal/year.rs
--rw-r--r--   0      501       20     1617 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/functions/utf8/contains.rs
--rw-r--r--   0      501       20     1617 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/functions/utf8/endswith.rs
--rw-r--r--   0      501       20     1336 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/functions/utf8/length.rs
--rw-r--r--   0      501       20     1524 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/functions/utf8/mod.rs
--rw-r--r--   0      501       20     1627 2023-05-22 23:15:08.000000 getdaft-0.1.2/src/dsl/functions/utf8/startswith.rs
--rw-r--r--   0      501       20     4961 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/dsl/lit.rs
--rw-r--r--   0      501       20      233 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/dsl/mod.rs
--rw-r--r--   0      501       20     5298 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/dsl/optimization.rs
--rw-r--r--   0      501       20     1982 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/dsl/pyobject.rs
--rw-r--r--   0      501       20     1681 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/error.rs
--rw-r--r--   0      501       20     7867 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/ffi.rs
--rw-r--r--   0      501       20     6022 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/kernels/hashing.rs
--rw-r--r--   0      501       20       54 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/kernels/mod.rs
--rw-r--r--   0      501       20    12159 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/kernels/search_sorted.rs
--rw-r--r--   0      501       20     3917 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/kernels/utf8.rs
--rw-r--r--   0      501       20     1117 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/lib.rs
--rw-r--r--   0      501       20     5763 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/python/datatype.rs
--rw-r--r--   0      501       20      307 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/python/error.rs
--rw-r--r--   0      501       20    10188 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/python/expr.rs
--rw-r--r--   0      501       20     1644 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/python/field.rs
--rw-r--r--   0      501       20      731 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/python/mod.rs
--rw-r--r--   0      501       20     2425 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/python/schema.rs
--rw-r--r--   0      501       20     9248 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/python/series.rs
--rw-r--r--   0      501       20    10114 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/python/table.rs
--rw-r--r--   0      501       20     3016 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/schema.rs
--rw-r--r--   0      501       20    10158 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/series/array_impl/data_array.rs
--rw-r--r--   0      501       20     5346 2023-05-22 23:15:09.000000 getdaft-0.1.2/src/series/array_impl/logical_array.rs
--rw-r--r--   0      501       20      161 2023-05-22 23:15:10.000000 getdaft-0.1.2/src/series/array_impl/mod.rs
--rw-r--r--   0      501       20     2099 2023-05-22 23:15:10.000000 getdaft-0.1.2/src/series/from.rs
--rw-r--r--   0      501       20     2190 2023-05-22 23:15:10.000000 getdaft-0.1.2/src/series/mod.rs
--rw-r--r--   0      501       20      902 2023-05-22 23:15:10.000000 getdaft-0.1.2/src/series/ops/abs.rs
--rw-r--r--   0      501       20     5207 2023-05-22 23:15:10.000000 getdaft-0.1.2/src/series/ops/agg.rs
--rw-r--r--   0      501       20     6298 2023-05-22 23:15:10.000000 getdaft-0.1.2/src/series/ops/arithmetic.rs
--rw-r--r--   0      501       20     1925 2023-05-22 23:15:10.000000 getdaft-0.1.2/src/series/ops/broadcast.rs
--rw-r--r--   0      501       20      194 2023-05-22 23:15:10.000000 getdaft-0.1.2/src/series/ops/cast.rs
--rw-r--r--   0      501       20     2609 2023-05-22 23:15:10.000000 getdaft-0.1.2/src/series/ops/comparison.rs
--rw-r--r--   0      501       20     1558 2023-05-22 23:15:10.000000 getdaft-0.1.2/src/series/ops/concat.rs
--rw-r--r--   0      501       20     1822 2023-05-22 23:15:10.000000 getdaft-0.1.2/src/series/ops/date.rs
--rw-r--r--   0      501       20     3612 2023-05-22 23:15:10.000000 getdaft-0.1.2/src/series/ops/downcast.rs
--rw-r--r--   0      501       20      697 2023-05-22 23:15:10.000000 getdaft-0.1.2/src/series/ops/filter.rs
--rw-r--r--   0      501       20      399 2023-05-22 23:15:10.000000 getdaft-0.1.2/src/series/ops/float.rs
--rw-r--r--   0      501       20      432 2023-05-22 23:15:10.000000 getdaft-0.1.2/src/series/ops/groups.rs
--rw-r--r--   0      501       20      412 2023-05-22 23:15:10.000000 getdaft-0.1.2/src/series/ops/hash.rs
--rw-r--r--   0      501       20      314 2023-05-22 23:15:11.000000 getdaft-0.1.2/src/series/ops/if_else.rs
--rw-r--r--   0      501       20      229 2023-05-22 23:15:11.000000 getdaft-0.1.2/src/series/ops/len.rs
--rw-r--r--   0      501       20      934 2023-05-22 23:15:11.000000 getdaft-0.1.2/src/series/ops/list.rs
--rw-r--r--   0      501       20     2352 2023-05-22 23:15:11.000000 getdaft-0.1.2/src/series/ops/mod.rs
--rw-r--r--   0      501       20      475 2023-05-22 23:15:11.000000 getdaft-0.1.2/src/series/ops/not.rs
--rw-r--r--   0      501       20      150 2023-05-22 23:15:11.000000 getdaft-0.1.2/src/series/ops/null.rs
--rw-r--r--   0      501       20      638 2023-05-22 23:15:11.000000 getdaft-0.1.2/src/series/ops/search_sorted.rs
--rw-r--r--   0      501       20     1492 2023-05-22 23:15:11.000000 getdaft-0.1.2/src/series/ops/sort.rs
--rw-r--r--   0      501       20      557 2023-05-22 23:15:11.000000 getdaft-0.1.2/src/series/ops/take.rs
--rw-r--r--   0      501       20     1528 2023-05-22 23:15:11.000000 getdaft-0.1.2/src/series/ops/utf8.rs
--rw-r--r--   0      501       20     1351 2023-05-22 23:15:11.000000 getdaft-0.1.2/src/series/series_like.rs
--rw-r--r--   0      501       20    16667 2023-05-22 23:15:11.000000 getdaft-0.1.2/src/table/mod.rs
--rw-r--r--   0      501       20     2165 2023-05-22 23:15:11.000000 getdaft-0.1.2/src/table/ops/agg.rs
--rw-r--r--   0      501       20     3729 2023-05-22 23:15:11.000000 getdaft-0.1.2/src/table/ops/explode.rs
--rw-r--r--   0      501       20     4403 2023-05-22 23:15:11.000000 getdaft-0.1.2/src/table/ops/groups.rs
--rw-r--r--   0      501       20     2886 2023-05-22 23:15:11.000000 getdaft-0.1.2/src/table/ops/hash.rs
--rw-r--r--   0      501       20     2483 2023-05-22 23:15:11.000000 getdaft-0.1.2/src/table/ops/joins/hash_join.rs
--rw-r--r--   0      501       20     3712 2023-05-22 23:15:12.000000 getdaft-0.1.2/src/table/ops/joins/mod.rs
--rw-r--r--   0      501       20       99 2023-05-22 23:15:12.000000 getdaft-0.1.2/src/table/ops/mod.rs
--rw-r--r--   0      501       20     3468 2023-05-22 23:15:12.000000 getdaft-0.1.2/src/table/ops/partition.rs
--rw-r--r--   0      501       20     1804 2023-05-22 23:15:12.000000 getdaft-0.1.2/src/table/ops/search_sorted.rs
--rw-r--r--   0      501       20      999 2023-05-22 23:15:12.000000 getdaft-0.1.2/src/table/ops/sort.rs
--rw-r--r--   0      501       20     5371 2023-05-22 23:15:12.000000 getdaft-0.1.2/src/utils/arrow.rs
--rw-r--r--   0      501       20       34 2023-05-22 23:15:12.000000 getdaft-0.1.2/src/utils/mod.rs
--rw-r--r--   0      501       20    10065 2023-05-22 23:15:12.000000 getdaft-0.1.2/src/utils/supertype.rs
--rw-r--r--   0      501       20        0 2023-05-22 23:15:12.000000 getdaft-0.1.2/tests/__init__.py
--rw-r--r--   0      501       20      299 2023-05-22 23:15:12.000000 getdaft-0.1.2/tests/assets/__init__.py
--rw-r--r--   0      501       20      544 2023-05-22 23:15:12.000000 getdaft-0.1.2/tests/assets/tpch-sqlite-queries/1.sql
--rw-r--r--   0      501       20      542 2023-05-22 23:15:12.000000 getdaft-0.1.2/tests/assets/tpch-sqlite-queries/10.sql
--rw-r--r--   0      501       20      703 2023-05-22 23:15:12.000000 getdaft-0.1.2/tests/assets/tpch-sqlite-queries/2.sql
--rw-r--r--   0      501       20      444 2023-05-22 23:15:12.000000 getdaft-0.1.2/tests/assets/tpch-sqlite-queries/3.sql
--rw-r--r--   0      501       20      371 2023-05-22 23:15:12.000000 getdaft-0.1.2/tests/assets/tpch-sqlite-queries/4.sql
--rw-r--r--   0      501       20      504 2023-05-22 23:15:12.000000 getdaft-0.1.2/tests/assets/tpch-sqlite-queries/5.sql
--rw-r--r--   0      501       20      259 2023-05-22 23:15:12.000000 getdaft-0.1.2/tests/assets/tpch-sqlite-queries/6.sql
--rw-r--r--   0      501       20      834 2023-05-22 23:15:13.000000 getdaft-0.1.2/tests/assets/tpch-sqlite-queries/7.sql
--rw-r--r--   0      501       20      815 2023-05-22 23:15:13.000000 getdaft-0.1.2/tests/assets/tpch-sqlite-queries/8.sql
--rw-r--r--   0      501       20      627 2023-05-22 23:15:13.000000 getdaft-0.1.2/tests/assets/tpch-sqlite-queries/9.sql
--rw-r--r--   0      501       20       48 2023-05-22 23:15:13.000000 getdaft-0.1.2/tests/assets/tpch-sqlite-queries/README.md
--rw-r--r--   0      501       20      604 2023-05-22 23:15:13.000000 getdaft-0.1.2/tests/benchmarks/conftest.py
--rw-r--r--   0      501       20     1227 2023-05-22 23:15:13.000000 getdaft-0.1.2/tests/benchmarks/test_df_arithmetic.py
--rw-r--r--   0      501       20     1686 2023-05-22 23:15:13.000000 getdaft-0.1.2/tests/benchmarks/test_file_read.py
--rw-r--r--   0      501       20     5604 2023-05-22 23:15:13.000000 getdaft-0.1.2/tests/benchmarks/test_groups_and_aggs.py
--rw-r--r--   0      501       20     7292 2023-05-22 23:15:13.000000 getdaft-0.1.2/tests/benchmarks/test_join.py
--rw-r--r--   0      501       20     2603 2023-05-22 23:15:13.000000 getdaft-0.1.2/tests/benchmarks/test_repartition.py
--rw-r--r--   0      501       20     4005 2023-05-22 23:15:13.000000 getdaft-0.1.2/tests/benchmarks/test_sort.py
--rw-r--r--   0      501       20     2911 2023-05-22 23:15:13.000000 getdaft-0.1.2/tests/conftest.py
--rw-r--r--   0      501       20        0 2023-05-22 23:15:13.000000 getdaft-0.1.2/tests/cookbook/__init__.py
--rw-r--r--   0      501       20    13229 2023-05-22 23:15:13.000000 getdaft-0.1.2/tests/cookbook/assets/311-service-requests.24.csv
--rw-r--r--   0      501       20      255 2023-05-22 23:15:13.000000 getdaft-0.1.2/tests/cookbook/assets/__init__.py
--rw-r--r--   0      501       20      882 2023-05-22 23:15:13.000000 getdaft-0.1.2/tests/cookbook/conftest.py
--rw-r--r--   0      501       20     9268 2023-05-22 23:15:13.000000 getdaft-0.1.2/tests/cookbook/test_aggregations.py
--rw-r--r--   0      501       20     2979 2023-05-22 23:15:13.000000 getdaft-0.1.2/tests/cookbook/test_computations.py
--rw-r--r--   0      501       20     1798 2023-05-22 23:15:13.000000 getdaft-0.1.2/tests/cookbook/test_count_rows.py
--rw-r--r--   0      501       20     7099 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/cookbook/test_dataloading.py
--rw-r--r--   0      501       20      800 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/cookbook/test_distinct.py
--rw-r--r--   0      501       20     6049 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/cookbook/test_filter.py
--rw-r--r--   0      501       20     3810 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/cookbook/test_joins.py
--rw-r--r--   0      501       20     2878 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/cookbook/test_literals.py
--rw-r--r--   0      501       20    10311 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/cookbook/test_pandas_cookbook.py
--rw-r--r--   0      501       20     4148 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/cookbook/test_sorting.py
--rw-r--r--   0      501       20     1497 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/cookbook/test_write.py
--rw-r--r--   0      501       20        0 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/dataframe/__init__.py
--rw-r--r--   0      501       20      751 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/dataframe/conftest.py
--rw-r--r--   0      501       20      805 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/dataframe/test_accessors.py
--rw-r--r--   0      501       20    10308 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/dataframe/test_aggregations.py
--rw-r--r--   0      501       20    21893 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/dataframe/test_creation.py
--rw-r--r--   0      501       20     1824 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/dataframe/test_distinct.py
--rw-r--r--   0      501       20     1428 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/dataframe/test_explode.py
--rw-r--r--   0      501       20     1097 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/dataframe/test_filter.py
--rw-r--r--   0      501       20     2435 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/dataframe/test_getitem.py
--rw-r--r--   0      501       20     4091 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/dataframe/test_joins.py
--rw-r--r--   0      501       20      744 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/dataframe/test_logical_type.py
--rw-r--r--   0      501       20     4500 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/dataframe/test_repr.py
--rw-r--r--   0      501       20      815 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/dataframe/test_select.py
--rw-r--r--   0      501       20      656 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/dataframe/test_show.py
--rw-r--r--   0      501       20     6364 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/dataframe/test_sort.py
--rw-r--r--   0      501       20     3596 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/dataframe/test_temporals.py
--rw-r--r--   0      501       20     2385 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/dataframe/test_to_integrations.py
--rw-r--r--   0      501       20      850 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/dataframe/test_with_column.py
--rw-r--r--   0      501       20        0 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/expressions/__init__.py
--rw-r--r--   0      501       20     1417 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/expressions/test_apply.py
--rw-r--r--   0      501       20     3533 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/expressions/test_expressions.py
--rw-r--r--   0      501       20     4259 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/expressions/test_expressions_projection.py
--rw-r--r--   0      501       20     5019 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/expressions/test_udf.py
--rw-r--r--   0      501       20        0 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/expressions/typing/__init__.py
--rw-r--r--   0      501       20     6290 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/expressions/typing/conftest.py
--rw-r--r--   0      501       20     1363 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/expressions/typing/test_aggs.py
--rw-r--r--   0      501       20     2335 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/expressions/typing/test_arithmetic.py
--rw-r--r--   0      501       20      853 2023-05-22 23:15:14.000000 getdaft-0.1.2/tests/expressions/typing/test_compare.py
--rw-r--r--   0      501       20      792 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/expressions/typing/test_dt.py
--rw-r--r--   0      501       20      531 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/expressions/typing/test_float.py
--rw-r--r--   0      501       20      684 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/expressions/typing/test_if_else.py
--rw-r--r--   0      501       20      422 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/expressions/typing/test_is_null.py
--rw-r--r--   0      501       20     1176 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/expressions/typing/test_logical.py
--rw-r--r--   0      501       20     1544 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/expressions/typing/test_str.py
--rw-r--r--   0      501       20        0 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/integration/__init__.py
--rw-r--r--   0      501       20     4193 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/integration/test_tpch.py
--rw-r--r--   0      501       20        0 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/optimizer/__init__.py
--rw-r--r--   0      501       20     1116 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/optimizer/conftest.py
--rw-r--r--   0      501       20     1666 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/optimizer/test_drop_projections.py
--rw-r--r--   0      501       20     1847 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/optimizer/test_drop_repartition.py
--rw-r--r--   0      501       20     2463 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/optimizer/test_fold_projections.py
--rw-r--r--   0      501       20     7624 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/optimizer/test_prune_columns.py
--rw-r--r--   0      501       20     3597 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/optimizer/test_pushdown_clauses_into_scan.py
--rw-r--r--   0      501       20     1170 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/optimizer/test_pushdown_limit.py
--rw-r--r--   0      501       20     8453 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/optimizer/test_pushdown_predicates.py
--rw-r--r--   0      501       20        0 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/property_based_testing/__init__.py
--rw-r--r--   0      501       20     4575 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/property_based_testing/strategies.py
--rw-r--r--   0      501       20     8895 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/property_based_testing/test_sort.py
--rw-r--r--   0      501       20        0 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/ray/__init__.py
--rw-r--r--   0      501       20     5375 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/ray/test_dask.py
--rw-r--r--   0      501       20     8344 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/ray/test_datasets.py
--rw-r--r--   0      501       20      278 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/series/__init__.py
--rw-r--r--   0      501       20     9299 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/series/test_arithmetic.py
--rw-r--r--   0      501       20     5635 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/series/test_cast.py
--rw-r--r--   0      501       20    17207 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/series/test_comparisons.py
--rw-r--r--   0      501       20     7188 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/series/test_concat.py
--rw-r--r--   0      501       20      864 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/series/test_embedding.py
--rw-r--r--   0      501       20     6151 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/series/test_filter.py
--rw-r--r--   0      501       20      874 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/series/test_float.py
--rw-r--r--   0      501       20     3344 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/series/test_hash.py
--rw-r--r--   0      501       20    21522 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/series/test_if_else.py
--rw-r--r--   0      501       20      889 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/series/test_numeric_ops.py
--rw-r--r--   0      501       20     3418 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/series/test_series.py
--rw-r--r--   0      501       20     9173 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/series/test_size_bytes.py
--rw-r--r--   0      501       20     2188 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/series/test_slice.py
--rw-r--r--   0      501       20     5495 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/series/test_sort.py
--rw-r--r--   0      501       20     6111 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/series/test_take.py
--rw-r--r--   0      501       20     1934 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/series/test_temporal_ops.py
--rw-r--r--   0      501       20     4413 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/series/test_utf8_ops.py
--rw-r--r--   0      501       20      694 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/table/__init__.py
--rw-r--r--   0      501       20     1070 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/table/test_blackbox_kernels.py
--rw-r--r--   0      501       20      426 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/table/test_broadcasts.py
--rw-r--r--   0      501       20     2123 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/table/test_concat.py
--rw-r--r--   0      501       20     4900 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/table/test_eval.py
--rw-r--r--   0      501       20     3930 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/table/test_explodes.py
--rw-r--r--   0      501       20     7413 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/table/test_filter.py
--rw-r--r--   0      501       20    23407 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/table/test_from_py.py
--rw-r--r--   0      501       20      842 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/table/test_head.py
--rw-r--r--   0      501       20    10974 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/table/test_joins.py
--rw-r--r--   0      501       20     7811 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/table/test_partitioning.py
--rw-r--r--   0      501       20      654 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/table/test_size_bytes.py
--rw-r--r--   0      501       20    10955 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/table/test_sorting.py
--rw-r--r--   0      501       20    20923 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/table/test_table_aggs.py
--rw-r--r--   0      501       20    10064 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/table/test_table_io.py
--rw-r--r--   0      501       20     5061 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/table/test_take.py
--rw-r--r--   0      501       20        0 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/table/utf8/__init__.py
--rw-r--r--   0      501       20     1165 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/table/utf8/test_compares.py
--rw-r--r--   0      501       20      321 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/table/utf8/test_length.py
--rw-r--r--   0      501       20     3533 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/test_analytics.py
--rw-r--r--   0      501       20      703 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/test_datatypes.py
--rw-r--r--   0      501       20     3542 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/test_schema.py
--rw-r--r--   0      501       20        0 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/udf_library/__init__.py
--rw-r--r--   0      501       20     3989 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/udf_library/test_url_udfs.py
--rw-r--r--   0      501       20      338 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests/utils.py
--rw-r--r--   0      501       20        0 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests_legacy/__init__.py
--rw-r--r--   0      501       20     6988 2023-05-22 23:15:15.000000 getdaft-0.1.2/tests_legacy/test_resource_requests.py
--rw-r--r--   0      501       20        0 2023-05-22 23:15:15.000000 getdaft-0.1.2/tools/__init__.py
--rw-r--r--   0      501       20     1633 2023-05-22 23:15:15.000000 getdaft-0.1.2/tools/patch_package_version.py
--rw-r--r--   0      501       20        0 2023-05-22 23:15:15.000000 getdaft-0.1.2/tools/wheels/__init__.py
--rw-r--r--   0      501       20        0 2023-05-22 23:15:15.000000 getdaft-0.1.2/tools/wheels/_vendor/__init__.py
--rw-r--r--   0      501       20     1125 2023-05-22 23:15:15.000000 getdaft-0.1.2/tools/wheels/_vendor/wheel/LICENSE.txt
--rw-r--r--   0      501       20       59 2023-05-22 23:15:15.000000 getdaft-0.1.2/tools/wheels/_vendor/wheel/__init__.py
--rw-r--r--   0      501       20     2499 2023-05-22 23:15:15.000000 getdaft-0.1.2/tools/wheels/_vendor/wheel/cli/__init__.py
--rw-r--r--   0      501       20     9514 2023-05-22 23:15:15.000000 getdaft-0.1.2/tools/wheels/_vendor/wheel/cli/convert.py
--rw-r--r--   0      501       20     3113 2023-05-22 23:15:15.000000 getdaft-0.1.2/tools/wheels/_vendor/wheel/cli/pack.py
--rw-r--r--   0      501       20      662 2023-05-22 23:15:15.000000 getdaft-0.1.2/tools/wheels/_vendor/wheel/cli/unpack.py
--rw-r--r--   0      501       20     1246 2023-05-22 23:15:15.000000 getdaft-0.1.2/tools/wheels/_vendor/wheel/pkginfo.py
--rw-r--r--   0      501       20      974 2023-05-22 23:15:15.000000 getdaft-0.1.2/tools/wheels/_vendor/wheel/util.py
--rw-r--r--   0      501       20     7125 2023-05-22 23:15:15.000000 getdaft-0.1.2/tools/wheels/_vendor/wheel/wheelfile.py
--rw-r--r--   0      501       20      878 2023-05-22 23:15:15.000000 getdaft-0.1.2/tools/wheels/fix-and-copy-wheel.py
--rw-r--r--   0      501       20     2981 2023-05-22 23:15:15.000000 getdaft-0.1.2/tools/wheels/tmpdirs.py
--rw-r--r--   0      501       20     4469 2023-05-22 23:15:15.000000 getdaft-0.1.2/tools/wheels/tools.py
--rw-r--r--   0      501       20     9484 2023-05-22 23:15:15.000000 getdaft-0.1.2/tools/wheels/wheeltools.py
--rw-r--r--   0      501       20       19 2023-05-22 23:15:15.000000 getdaft-0.1.2/tutorials/.gitignore
--rw-r--r--   0      501       20    19576 2023-05-22 23:15:15.000000 getdaft-0.1.2/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb
--rw-r--r--   0      501       20    12068 2023-05-22 23:15:15.000000 getdaft-0.1.2/tutorials/image_querying/top_n_red_color.ipynb
--rw-r--r--   0      501       20    98730 2023-05-22 23:15:15.000000 getdaft-0.1.2/tutorials/mnist.ipynb
--rw-r--r--   0      501       20    11847 2023-05-22 23:15:15.000000 getdaft-0.1.2/tutorials/text_to_image/text_to_image_generation.ipynb
--rw-r--r--   0      501       20     9134 2023-05-22 23:15:15.000000 getdaft-0.1.2/tutorials/text_to_image/using_cloud_with_ray.ipynb
--rw-r--r--   0      501       20    32068 2023-05-22 23:15:07.000000 getdaft-0.1.2/Cargo.lock
--rw-r--r--   0        0        0     7325 1970-01-01 00:00:00.000000 getdaft-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 getdaft-0.1.3/Cargo.toml
+-rw-r--r--   0      501       20      834 2023-05-24 05:44:49.000000 getdaft-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0      501       20      595 2023-05-24 05:44:49.000000 getdaft-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0      501       20      428 2023-05-24 05:44:49.000000 getdaft-0.1.3/.github/dependabot.yml
+-rw-r--r--   0      501       20     1333 2023-05-24 05:44:49.000000 getdaft-0.1.3/.github/workflows/broken-link-checker.yml
+-rw-r--r--   0      501       20     3378 2023-05-24 05:44:49.000000 getdaft-0.1.3/.github/workflows/daft-profiling.yml
+-rw-r--r--   0      501       20     1627 2023-05-24 05:44:49.000000 getdaft-0.1.3/.github/workflows/notebook-checker.yml
+-rw-r--r--   0      501       20     2194 2023-05-24 05:44:49.000000 getdaft-0.1.3/.github/workflows/property-based-tests.yml
+-rw-r--r--   0      501       20    12886 2023-05-24 05:44:49.000000 getdaft-0.1.3/.github/workflows/python-package.yml
+-rw-r--r--   0      501       20     6182 2023-05-24 05:44:49.000000 getdaft-0.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0      501       20     2638 2023-05-24 05:44:49.000000 getdaft-0.1.3/.github/workflows/ray-compatibility.yml
+-rw-r--r--   0      501       20      300 2023-05-24 05:44:49.000000 getdaft-0.1.3/.gitignore
+-rw-r--r--   0      501       20     2126 2023-05-24 05:44:49.000000 getdaft-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0      501       20      205 2023-05-24 05:44:49.000000 getdaft-0.1.3/.readthedocs.yaml
+-rw-r--r--   0      501       20     1550 2023-05-24 05:44:49.000000 getdaft-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0      501       20    11357 2023-05-24 05:44:49.000000 getdaft-0.1.3/LICENSE
+-rw-r--r--   0      501       20     1295 2023-05-24 05:44:49.000000 getdaft-0.1.3/Makefile
+-rw-r--r--   0      501       20     6126 2023-05-24 05:44:49.000000 getdaft-0.1.3/README.rst
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:49.000000 getdaft-0.1.3/benchmarking/__init__.py
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:49.000000 getdaft-0.1.3/benchmarking/tpch/__init__.py
+-rw-r--r--   0      501       20     9495 2023-05-24 05:44:49.000000 getdaft-0.1.3/benchmarking/tpch/__main__.py
+-rw-r--r--   0      501       20    12428 2023-05-24 05:44:49.000000 getdaft-0.1.3/benchmarking/tpch/answers.py
+-rw-r--r--   0      501       20    12140 2023-05-24 05:44:49.000000 getdaft-0.1.3/benchmarking/tpch/data_generation.py
+-rw-r--r--   0      501       20     4573 2023-05-24 05:44:49.000000 getdaft-0.1.3/benchmarking/tpch/pipelined_data_generation.py
+-rw-r--r--   0      501       20     1436 2023-05-24 05:44:49.000000 getdaft-0.1.3/ci/upload_wheels.sh
+-rw-r--r--   0      501       20      440 2023-05-24 05:44:49.000000 getdaft-0.1.3/codecov.yml
+-rw-r--r--   0      501       20     2092 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/__init__.py
+-rw-r--r--   0      501       20     6724 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/analytics.py
+-rw-r--r--   0      501       20     3935 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/api_annotations.py
+-rw-r--r--   0      501       20    10591 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/arrow_utils.py
+-rw-r--r--   0      501       20     5395 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/context.py
+-rw-r--r--   0      501       20     3403 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/convert.py
+-rw-r--r--   0      501       20       94 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/dataframe/__init__.py
+-rw-r--r--   0      501       20    49646 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/dataframe/dataframe.py
+-rw-r--r--   0      501       20      306 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/dataframe/preview.py
+-rw-r--r--   0      501       20      850 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/datasources.py
+-rw-r--r--   0      501       20    10207 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/datatype.py
+-rw-r--r--   0      501       20       84 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/errors.py
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/execution/__init__.py
+-rw-r--r--   0      501       20    24879 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/execution/execution_step.py
+-rw-r--r--   0      501       20     4231 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/execution/logical_op_runners.py
+-rw-r--r--   0      501       20    27790 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/execution/physical_plan.py
+-rw-r--r--   0      501       20     6110 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/execution/physical_plan_factory.py
+-rw-r--r--   0      501       20      170 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/expressions/__init__.py
+-rw-r--r--   0      501       20    24529 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/expressions/expressions.py
+-rw-r--r--   0      501       20      572 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/expressions/testing.py
+-rw-r--r--   0      501       20    12728 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/filesystem.py
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/internal/__init__.py
+-rw-r--r--   0      501       20      509 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/internal/gpu.py
+-rw-r--r--   0      501       20     1804 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/internal/rule.py
+-rw-r--r--   0      501       20     1965 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/internal/rule_runner.py
+-rw-r--r--   0      501       20     3490 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/internal/treenode.py
+-rw-r--r--   0      501       20      263 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/io/__init__.py
+-rw-r--r--   0      501       20     1682 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/io/_csv.py
+-rw-r--r--   0      501       20     1223 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/io/_json.py
+-rw-r--r--   0      501       20     2032 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/io/common.py
+-rw-r--r--   0      501       20     2034 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/io/file_path.py
+-rw-r--r--   0      501       20     1243 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/io/parquet.py
+-rw-r--r--   0      501       20      264 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/logging.py
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/logical/__init__.py
+-rw-r--r--   0      501       20     8601 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/logical/aggregation_plan_builder.py
+-rw-r--r--   0      501       20    37496 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/logical/logical_plan.py
+-rw-r--r--   0      501       20     1492 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/logical/map_partition_ops.py
+-rw-r--r--   0      501       20    19183 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/logical/optimizer.py
+-rw-r--r--   0      501       20     3625 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/logical/schema.py
+-rw-r--r--   0      501       20       99 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/pickle/__init__.py
+-rw-r--r--   0      501       20    34760 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/pickle/cloudpickle.py
+-rw-r--r--   0      501       20    34262 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/pickle/cloudpickle_fast.py
+-rw-r--r--   0      501       20      639 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/pickle/compat.py
+-rw-r--r--   0      501       20      312 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/pickle/pickle.py
+-rw-r--r--   0      501       20     2036 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/resource_request.py
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/runners/__init__.py
+-rw-r--r--   0      501       20     5708 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/runners/partitioning.py
+-rw-r--r--   0      501       20     1488 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/runners/profiler.py
+-rw-r--r--   0      501       20    13059 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/runners/pyrunner.py
+-rw-r--r--   0      501       20    25296 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/runners/ray_runner.py
+-rw-r--r--   0      501       20      918 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/runners/runner.py
+-rw-r--r--   0      501       20     4324 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/runners/runner_io.py
+-rw-r--r--   0      501       20    18981 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/series.py
+-rw-r--r--   0      501       20       82 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/table/__init__.py
+-rw-r--r--   0      501       20    13420 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/table/table.py
+-rw-r--r--   0      501       20     9457 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/table/table_io.py
+-rw-r--r--   0      501       20     7263 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/udf.py
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/udf_library/__init__.py
+-rw-r--r--   0      501       20     3486 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/udf_library/url_udfs.py
+-rw-r--r--   0      501       20     2697 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/utils.py
+-rw-r--r--   0      501       20      183 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/viz/__init__.py
+-rw-r--r--   0      501       20     1699 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/viz/dataframe_display.py
+-rw-r--r--   0      501       20     1517 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/viz/html_viz_hooks.py
+-rw-r--r--   0      501       20     5738 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/viz/repr.py
+-rw-r--r--   0      501       20      148 2023-05-24 05:44:49.000000 getdaft-0.1.3/docs/CONTRIBUTING.md
+-rw-r--r--   0      501       20      638 2023-05-24 05:44:49.000000 getdaft-0.1.3/docs/Makefile
+-rw-r--r--   0      501       20    71692 2023-05-24 05:44:49.000000 getdaft-0.1.3/docs/source/10-min.ipynb
+-rw-r--r--   0      501       20      389 2023-05-24 05:44:49.000000 getdaft-0.1.3/docs/source/_static/custom-function-signatures.css
+-rw-r--r--   0      501       20      565 2023-05-24 05:44:49.000000 getdaft-0.1.3/docs/source/_static/daft-favicon.png
+-rw-r--r--   0      501       20     7804 2023-05-24 05:44:49.000000 getdaft-0.1.3/docs/source/_static/daft-logo.png
+-rw-r--r--   0      501       20    42148 2023-05-24 05:44:49.000000 getdaft-0.1.3/docs/source/_static/daft_illustration.png
+-rw-r--r--   0      501       20    25200 2023-05-24 05:44:49.000000 getdaft-0.1.3/docs/source/_static/execution_model.png
+-rw-r--r--   0      501       20     1901 2023-05-24 05:44:49.000000 getdaft-0.1.3/docs/source/_static/header.css
+-rw-r--r--   0      501       20    32864 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/_static/high_level_architecture.png
+-rw-r--r--   0      501       20      343 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/_static/icon-menu-close.svg
+-rw-r--r--   0      501       20      333 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/_static/icon-menu-dots.svg
+-rw-r--r--   0      501       20    18177 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/_static/in_memory_data_representation.png
+-rw-r--r--   0      501       20      786 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/_static/mobile-menu.js
+-rw-r--r--   0      501       20      856 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/_templates/layout.html
+-rw-r--r--   0      501       20      994 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/_templates/sections/header.html
+-rw-r--r--   0      501       20      957 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/_templates/sections/mobile-menu.html
+-rw-r--r--   0      501       20      325 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/api_docs/context.rst
+-rw-r--r--   0      501       20     2564 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/api_docs/dataframe.rst
+-rw-r--r--   0      501       20     3444 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/api_docs/expressions.rst
+-rw-r--r--   0      501       20      784 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/api_docs/groupby.rst
+-rw-r--r--   0      501       20      124 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/api_docs/index.rst
+-rw-r--r--   0      501       20     1457 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/api_docs/input_output.rst
+-rw-r--r--   0      501       20       88 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/api_docs/udf.rst
+-rw-r--r--   0      501       20     3547 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/conf.py
+-rw-r--r--   0      501       20     4964 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/dataframe_comparison.rst
+-rw-r--r--   0      501       20     1645 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/index.rst
+-rw-r--r--   0      501       20     1089 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/install.rst
+-rw-r--r--   0      501       20      743 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/index.rst
+-rw-r--r--   0      501       20     7586 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/key_concepts.rst
+-rw-r--r--   0      501       20     1398 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/tutorials.rst
+-rw-r--r--   0      501       20     1388 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/user_guides/aggregations.rst
+-rw-r--r--   0      501       20     6686 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/user_guides/dataframe-operations.rst
+-rw-r--r--   0      501       20     9024 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/user_guides/expressions.rst
+-rw-r--r--   0      501       20     7829 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/user_guides/intro-dataframes.rst
+-rw-r--r--   0      501       20      206 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/user_guides/partitioning.rst
+-rw-r--r--   0      501       20     3190 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/user_guides/read-write.rst
+-rw-r--r--   0      501       20     1257 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/user_guides/scaling-up.rst
+-rw-r--r--   0      501       20     8691 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/user_guides/udf.rst
+-rw-r--r--   0      501       20     1551 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/user_guides.rst
+-rw-r--r--   0      501       20     3575 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.13.rst
+-rw-r--r--   0      501       20     2241 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.14.rst
+-rw-r--r--   0      501       20     1913 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.16.rst
+-rw-r--r--   0      501       20     1750 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.17.rst
+-rw-r--r--   0      501       20     2100 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.18.rst
+-rw-r--r--   0      501       20     3647 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.19.rst
+-rw-r--r--   0      501       20     4240 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.20.rst
+-rw-r--r--   0      501       20     4633 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.21.rst
+-rw-r--r--   0      501       20     8016 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.22.rst
+-rw-r--r--   0      501       20     5385 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.23.rst
+-rw-r--r--   0      501       20    11759 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.24.rst
+-rw-r--r--   0      501       20     4750 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.1.0.rst
+-rw-r--r--   0      501       20     2411 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.1.1.rst
+-rw-r--r--   0      501       20     2555 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.1.2.rst
+-rw-r--r--   0      501       20      839 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.1.3.rst
+-rw-r--r--   0      501       20      935 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/_template.rst
+-rw-r--r--   0      501       20      350 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/index.rst
+-rw-r--r--   0      501       20     6574 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/technical_architecture.rst
+-rw-r--r--   0      501       20     1316 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/telemetry.rst
+-rw-r--r--   0      501       20     1873 2023-05-24 05:44:50.000000 getdaft-0.1.3/pyproject.toml
+-rw-r--r--   0      501       20      680 2023-05-24 05:44:50.000000 getdaft-0.1.3/requirements-dev.txt
+-rw-r--r--   0      501       20       98 2023-05-24 05:44:50.000000 getdaft-0.1.3/rust-toolchain.toml
+-rw-r--r--   0      501       20     4466 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/from.rs
+-rw-r--r--   0      501       20      734 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/iterator.rs
+-rw-r--r--   0      501       20     2945 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/mod.rs
+-rw-r--r--   0      501       20      257 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/abs.rs
+-rw-r--r--   0      501       20      726 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/apply.rs
+-rw-r--r--   0      501       20      841 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/arange.rs
+-rw-r--r--   0      501       20     6964 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/arithmetic.rs
+-rw-r--r--   0      501       20     3048 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/arrow2/comparison.rs
+-rw-r--r--   0      501       20       34 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/arrow2/mod.rs
+-rw-r--r--   0      501       20       19 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/arrow2/sort/mod.rs
+-rw-r--r--   0      501       20     3482 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/arrow2/sort/primitive/common.rs
+-rw-r--r--   0      501       20      723 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/arrow2/sort/primitive/indices.rs
+-rw-r--r--   0      501       20       47 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/arrow2/sort/primitive/mod.rs
+-rw-r--r--   0      501       20     8075 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/arrow2/sort/primitive/sort.rs
+-rw-r--r--   0      501       20     2861 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/as_arrow.rs
+-rw-r--r--   0      501       20    11304 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/broadcast.rs
+-rw-r--r--   0      501       20    19737 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/cast.rs
+-rw-r--r--   0      501       20    11017 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/compare_agg.rs
+-rw-r--r--   0      501       20    47218 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/comparison.rs
+-rw-r--r--   0      501       20     1634 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/concat.rs
+-rw-r--r--   0      501       20     5982 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/concat_agg.rs
+-rw-r--r--   0      501       20     1433 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/count.rs
+-rw-r--r--   0      501       20     1550 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/date.rs
+-rw-r--r--   0      501       20     2889 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/filter.rs
+-rw-r--r--   0      501       20     1264 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/float.rs
+-rw-r--r--   0      501       20     1936 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/full.rs
+-rw-r--r--   0      501       20     4112 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/groups.rs
+-rw-r--r--   0      501       20     1515 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/hash.rs
+-rw-r--r--   0      501       20    12019 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/if_else.rs
+-rw-r--r--   0      501       20     1058 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/len.rs
+-rw-r--r--   0      501       20     3446 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/list.rs
+-rw-r--r--   0      501       20     3360 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/list_agg.rs
+-rw-r--r--   0      501       20     1622 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/mean.rs
+-rw-r--r--   0      501       20     2595 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/mod.rs
+-rw-r--r--   0      501       20     1156 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/null.rs
+-rw-r--r--   0      501       20     3819 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/pairwise.rs
+-rw-r--r--   0      501       20      484 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/search_sorted.rs
+-rw-r--r--   0      501       20    19071 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/sort.rs
+-rw-r--r--   0      501       20     2383 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/sum.rs
+-rw-r--r--   0      501       20    15006 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/take.rs
+-rw-r--r--   0      501       20     5279 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/utf8.rs
+-rw-r--r--   0      501       20      995 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/pseudo_arrow/compute.rs
+-rw-r--r--   0      501       20    13611 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/pseudo_arrow/mod.rs
+-rw-r--r--   0      501       20     2502 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/pseudo_arrow/python.rs
+-rw-r--r--   0      501       20    13119 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/datatypes/dtype.rs
+-rw-r--r--   0      501       20     2012 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/datatypes/field.rs
+-rw-r--r--   0      501       20     2744 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/datatypes/logical.rs
+-rw-r--r--   0      501       20     8970 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/datatypes/matching.rs
+-rw-r--r--   0      501       20     6650 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/datatypes/mod.rs
+-rw-r--r--   0      501       20     1083 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/datatypes/time_unit.rs
+-rw-r--r--   0      501       20      273 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/README.md
+-rw-r--r--   0      501       20     1474 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/arithmetic.rs
+-rw-r--r--   0      501       20    21828 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/expr.rs
+-rw-r--r--   0      501       20     1421 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/float/is_nan.rs
+-rw-r--r--   0      501       20      587 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/float/mod.rs
+-rw-r--r--   0      501       20     1112 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/list/explode.rs
+-rw-r--r--   0      501       20      597 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/list/mod.rs
+-rw-r--r--   0      501       20     1774 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/mod.rs
+-rw-r--r--   0      501       20     1178 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/numeric/abs.rs
+-rw-r--r--   0      501       20      580 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/numeric/mod.rs
+-rw-r--r--   0      501       20      676 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/python/mod.rs
+-rw-r--r--   0      501       20     2050 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/python/partial_udf.rs
+-rw-r--r--   0      501       20     2769 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/python/udf.rs
+-rw-r--r--   0      501       20     1310 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/temporal/day.rs
+-rw-r--r--   0      501       20     1338 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/temporal/day_of_week.rs
+-rw-r--r--   0      501       20     1425 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/temporal/mod.rs
+-rw-r--r--   0      501       20     1320 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/temporal/month.rs
+-rw-r--r--   0      501       20     1314 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/temporal/year.rs
+-rw-r--r--   0      501       20     1617 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/utf8/contains.rs
+-rw-r--r--   0      501       20     1617 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/utf8/endswith.rs
+-rw-r--r--   0      501       20     1336 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/utf8/length.rs
+-rw-r--r--   0      501       20     1524 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/utf8/mod.rs
+-rw-r--r--   0      501       20     1627 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/utf8/startswith.rs
+-rw-r--r--   0      501       20     4961 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/lit.rs
+-rw-r--r--   0      501       20      233 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/mod.rs
+-rw-r--r--   0      501       20     5298 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/optimization.rs
+-rw-r--r--   0      501       20     1982 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/pyobject.rs
+-rw-r--r--   0      501       20     1681 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/error.rs
+-rw-r--r--   0      501       20     7867 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/ffi.rs
+-rw-r--r--   0      501       20     6022 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/kernels/hashing.rs
+-rw-r--r--   0      501       20       54 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/kernels/mod.rs
+-rw-r--r--   0      501       20    12159 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/kernels/search_sorted.rs
+-rw-r--r--   0      501       20     3917 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/kernels/utf8.rs
+-rw-r--r--   0      501       20     1117 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/lib.rs
+-rw-r--r--   0      501       20     5763 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/python/datatype.rs
+-rw-r--r--   0      501       20      307 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/python/error.rs
+-rw-r--r--   0      501       20    10188 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/python/expr.rs
+-rw-r--r--   0      501       20     1644 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/python/field.rs
+-rw-r--r--   0      501       20      731 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/python/mod.rs
+-rw-r--r--   0      501       20     2425 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/python/schema.rs
+-rw-r--r--   0      501       20     9248 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/python/series.rs
+-rw-r--r--   0      501       20    10114 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/python/table.rs
+-rw-r--r--   0      501       20     3016 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/schema.rs
+-rw-r--r--   0      501       20    10158 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/array_impl/data_array.rs
+-rw-r--r--   0      501       20     5346 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/array_impl/logical_array.rs
+-rw-r--r--   0      501       20      161 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/array_impl/mod.rs
+-rw-r--r--   0      501       20     2099 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/from.rs
+-rw-r--r--   0      501       20     2190 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/mod.rs
+-rw-r--r--   0      501       20      902 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/abs.rs
+-rw-r--r--   0      501       20     5207 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/agg.rs
+-rw-r--r--   0      501       20     6298 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/arithmetic.rs
+-rw-r--r--   0      501       20     1925 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/broadcast.rs
+-rw-r--r--   0      501       20      194 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/cast.rs
+-rw-r--r--   0      501       20     2609 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/comparison.rs
+-rw-r--r--   0      501       20     1558 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/concat.rs
+-rw-r--r--   0      501       20     1822 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/date.rs
+-rw-r--r--   0      501       20     3612 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/downcast.rs
+-rw-r--r--   0      501       20      697 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/filter.rs
+-rw-r--r--   0      501       20      399 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/float.rs
+-rw-r--r--   0      501       20      432 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/groups.rs
+-rw-r--r--   0      501       20      412 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/hash.rs
+-rw-r--r--   0      501       20      314 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/if_else.rs
+-rw-r--r--   0      501       20      229 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/len.rs
+-rw-r--r--   0      501       20      934 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/list.rs
+-rw-r--r--   0      501       20     2352 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/mod.rs
+-rw-r--r--   0      501       20      475 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/not.rs
+-rw-r--r--   0      501       20      150 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/null.rs
+-rw-r--r--   0      501       20      638 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/search_sorted.rs
+-rw-r--r--   0      501       20     1492 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/sort.rs
+-rw-r--r--   0      501       20      557 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/take.rs
+-rw-r--r--   0      501       20     1528 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/utf8.rs
+-rw-r--r--   0      501       20     1351 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/series_like.rs
+-rw-r--r--   0      501       20    16667 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/mod.rs
+-rw-r--r--   0      501       20     2165 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/ops/agg.rs
+-rw-r--r--   0      501       20     3729 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/ops/explode.rs
+-rw-r--r--   0      501       20     4403 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/ops/groups.rs
+-rw-r--r--   0      501       20     2886 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/ops/hash.rs
+-rw-r--r--   0      501       20     2483 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/ops/joins/hash_join.rs
+-rw-r--r--   0      501       20     3712 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/ops/joins/mod.rs
+-rw-r--r--   0      501       20       99 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/ops/mod.rs
+-rw-r--r--   0      501       20     3468 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/ops/partition.rs
+-rw-r--r--   0      501       20     1804 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/ops/search_sorted.rs
+-rw-r--r--   0      501       20      999 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/ops/sort.rs
+-rw-r--r--   0      501       20     5371 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/utils/arrow.rs
+-rw-r--r--   0      501       20       34 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/utils/mod.rs
+-rw-r--r--   0      501       20    10065 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/utils/supertype.rs
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/__init__.py
+-rw-r--r--   0      501       20      299 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/__init__.py
+-rw-r--r--   0      501       20      544 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/1.sql
+-rw-r--r--   0      501       20      542 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/10.sql
+-rw-r--r--   0      501       20      703 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/2.sql
+-rw-r--r--   0      501       20      444 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/3.sql
+-rw-r--r--   0      501       20      371 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/4.sql
+-rw-r--r--   0      501       20      504 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/5.sql
+-rw-r--r--   0      501       20      259 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/6.sql
+-rw-r--r--   0      501       20      834 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/7.sql
+-rw-r--r--   0      501       20      815 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/8.sql
+-rw-r--r--   0      501       20      627 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/9.sql
+-rw-r--r--   0      501       20       48 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/README.md
+-rw-r--r--   0      501       20      604 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/benchmarks/conftest.py
+-rw-r--r--   0      501       20     1227 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/benchmarks/test_df_arithmetic.py
+-rw-r--r--   0      501       20     2706 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/benchmarks/test_file_read.py
+-rw-r--r--   0      501       20     5604 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/benchmarks/test_groups_and_aggs.py
+-rw-r--r--   0      501       20     7292 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/benchmarks/test_join.py
+-rw-r--r--   0      501       20     2603 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/benchmarks/test_repartition.py
+-rw-r--r--   0      501       20     4005 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/benchmarks/test_sort.py
+-rw-r--r--   0      501       20     2911 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/conftest.py
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/__init__.py
+-rw-r--r--   0      501       20    13229 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/assets/311-service-requests.24.csv
+-rw-r--r--   0      501       20      255 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/assets/__init__.py
+-rw-r--r--   0      501       20      882 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/conftest.py
+-rw-r--r--   0      501       20     9268 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_aggregations.py
+-rw-r--r--   0      501       20     2979 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_computations.py
+-rw-r--r--   0      501       20     1798 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_count_rows.py
+-rw-r--r--   0      501       20     7099 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_dataloading.py
+-rw-r--r--   0      501       20      800 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_distinct.py
+-rw-r--r--   0      501       20     6049 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_filter.py
+-rw-r--r--   0      501       20     3810 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_joins.py
+-rw-r--r--   0      501       20     2878 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_literals.py
+-rw-r--r--   0      501       20    10311 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_pandas_cookbook.py
+-rw-r--r--   0      501       20     4148 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_sorting.py
+-rw-r--r--   0      501       20     1497 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_write.py
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/__init__.py
+-rw-r--r--   0      501       20      751 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/conftest.py
+-rw-r--r--   0      501       20      805 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_accessors.py
+-rw-r--r--   0      501       20    10308 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_aggregations.py
+-rw-r--r--   0      501       20    21893 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_creation.py
+-rw-r--r--   0      501       20     1824 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_distinct.py
+-rw-r--r--   0      501       20     1428 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_explode.py
+-rw-r--r--   0      501       20     1097 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_filter.py
+-rw-r--r--   0      501       20     2435 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_getitem.py
+-rw-r--r--   0      501       20     4091 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_joins.py
+-rw-r--r--   0      501       20      744 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_logical_type.py
+-rw-r--r--   0      501       20     4500 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_repr.py
+-rw-r--r--   0      501       20      815 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_select.py
+-rw-r--r--   0      501       20      656 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_show.py
+-rw-r--r--   0      501       20     6364 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_sort.py
+-rw-r--r--   0      501       20     3596 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_temporals.py
+-rw-r--r--   0      501       20     2385 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_to_integrations.py
+-rw-r--r--   0      501       20      850 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_with_column.py
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/__init__.py
+-rw-r--r--   0      501       20     1417 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/test_apply.py
+-rw-r--r--   0      501       20     3533 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/test_expressions.py
+-rw-r--r--   0      501       20     4259 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/test_expressions_projection.py
+-rw-r--r--   0      501       20     5019 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/test_udf.py
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/__init__.py
+-rw-r--r--   0      501       20     6290 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/conftest.py
+-rw-r--r--   0      501       20     1363 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/test_aggs.py
+-rw-r--r--   0      501       20     2335 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/test_arithmetic.py
+-rw-r--r--   0      501       20      853 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/test_compare.py
+-rw-r--r--   0      501       20      792 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/test_dt.py
+-rw-r--r--   0      501       20      531 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/test_float.py
+-rw-r--r--   0      501       20      684 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/test_if_else.py
+-rw-r--r--   0      501       20      422 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/test_is_null.py
+-rw-r--r--   0      501       20     1176 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/test_logical.py
+-rw-r--r--   0      501       20     1544 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/test_str.py
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/integration/__init__.py
+-rw-r--r--   0      501       20     4193 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/integration/test_tpch.py
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/optimizer/__init__.py
+-rw-r--r--   0      501       20     1116 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/optimizer/conftest.py
+-rw-r--r--   0      501       20     1666 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/optimizer/test_drop_projections.py
+-rw-r--r--   0      501       20     1847 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/optimizer/test_drop_repartition.py
+-rw-r--r--   0      501       20     2463 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/optimizer/test_fold_projections.py
+-rw-r--r--   0      501       20     7624 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/optimizer/test_prune_columns.py
+-rw-r--r--   0      501       20     3597 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/optimizer/test_pushdown_clauses_into_scan.py
+-rw-r--r--   0      501       20     1170 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/optimizer/test_pushdown_limit.py
+-rw-r--r--   0      501       20     8453 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/optimizer/test_pushdown_predicates.py
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/property_based_testing/__init__.py
+-rw-r--r--   0      501       20     4575 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/property_based_testing/strategies.py
+-rw-r--r--   0      501       20     8895 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/property_based_testing/test_sort.py
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/ray/__init__.py
+-rw-r--r--   0      501       20     5375 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/ray/test_dask.py
+-rw-r--r--   0      501       20     8461 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/ray/test_datasets.py
+-rw-r--r--   0      501       20      278 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/__init__.py
+-rw-r--r--   0      501       20     9299 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_arithmetic.py
+-rw-r--r--   0      501       20     5635 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_cast.py
+-rw-r--r--   0      501       20    17207 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_comparisons.py
+-rw-r--r--   0      501       20     7188 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_concat.py
+-rw-r--r--   0      501       20      864 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_embedding.py
+-rw-r--r--   0      501       20     6151 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_filter.py
+-rw-r--r--   0      501       20      874 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_float.py
+-rw-r--r--   0      501       20     3344 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_hash.py
+-rw-r--r--   0      501       20    21522 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_if_else.py
+-rw-r--r--   0      501       20      889 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_numeric_ops.py
+-rw-r--r--   0      501       20     3418 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_series.py
+-rw-r--r--   0      501       20     9173 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_size_bytes.py
+-rw-r--r--   0      501       20     2188 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_slice.py
+-rw-r--r--   0      501       20     5495 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_sort.py
+-rw-r--r--   0      501       20     6111 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_take.py
+-rw-r--r--   0      501       20     1934 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_temporal_ops.py
+-rw-r--r--   0      501       20     4413 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_utf8_ops.py
+-rw-r--r--   0      501       20      694 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/__init__.py
+-rw-r--r--   0      501       20     1070 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_blackbox_kernels.py
+-rw-r--r--   0      501       20      426 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_broadcasts.py
+-rw-r--r--   0      501       20     2123 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_concat.py
+-rw-r--r--   0      501       20     4900 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_eval.py
+-rw-r--r--   0      501       20     3930 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_explodes.py
+-rw-r--r--   0      501       20     7413 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_filter.py
+-rw-r--r--   0      501       20    23407 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_from_py.py
+-rw-r--r--   0      501       20      842 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_head.py
+-rw-r--r--   0      501       20    10974 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_joins.py
+-rw-r--r--   0      501       20     7811 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_partitioning.py
+-rw-r--r--   0      501       20      654 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_size_bytes.py
+-rw-r--r--   0      501       20    10955 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_sorting.py
+-rw-r--r--   0      501       20    20923 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_table_aggs.py
+-rw-r--r--   0      501       20    10064 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_table_io.py
+-rw-r--r--   0      501       20     5061 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_take.py
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/utf8/__init__.py
+-rw-r--r--   0      501       20     1165 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/utf8/test_compares.py
+-rw-r--r--   0      501       20      321 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/utf8/test_length.py
+-rw-r--r--   0      501       20     3533 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/test_analytics.py
+-rw-r--r--   0      501       20      703 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/test_datatypes.py
+-rw-r--r--   0      501       20     3542 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/test_schema.py
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/udf_library/__init__.py
+-rw-r--r--   0      501       20     3989 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/udf_library/test_url_udfs.py
+-rw-r--r--   0      501       20      338 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/utils.py
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests_legacy/__init__.py
+-rw-r--r--   0      501       20     6988 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests_legacy/test_resource_requests.py
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/__init__.py
+-rw-r--r--   0      501       20     1633 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/patch_package_version.py
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/__init__.py
+-rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/_vendor/__init__.py
+-rw-r--r--   0      501       20     1125 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/_vendor/wheel/LICENSE.txt
+-rw-r--r--   0      501       20       59 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/_vendor/wheel/__init__.py
+-rw-r--r--   0      501       20     2499 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/_vendor/wheel/cli/__init__.py
+-rw-r--r--   0      501       20     9514 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/_vendor/wheel/cli/convert.py
+-rw-r--r--   0      501       20     3113 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/_vendor/wheel/cli/pack.py
+-rw-r--r--   0      501       20      662 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/_vendor/wheel/cli/unpack.py
+-rw-r--r--   0      501       20     1246 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/_vendor/wheel/pkginfo.py
+-rw-r--r--   0      501       20      974 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/_vendor/wheel/util.py
+-rw-r--r--   0      501       20     7125 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/_vendor/wheel/wheelfile.py
+-rw-r--r--   0      501       20      878 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/fix-and-copy-wheel.py
+-rw-r--r--   0      501       20     2981 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/tmpdirs.py
+-rw-r--r--   0      501       20     4469 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/tools.py
+-rw-r--r--   0      501       20     9484 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/wheeltools.py
+-rw-r--r--   0      501       20       19 2023-05-24 05:44:50.000000 getdaft-0.1.3/tutorials/.gitignore
+-rw-r--r--   0      501       20    19576 2023-05-24 05:44:50.000000 getdaft-0.1.3/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb
+-rw-r--r--   0      501       20    12068 2023-05-24 05:44:50.000000 getdaft-0.1.3/tutorials/image_querying/top_n_red_color.ipynb
+-rw-r--r--   0      501       20    98730 2023-05-24 05:44:50.000000 getdaft-0.1.3/tutorials/mnist.ipynb
+-rw-r--r--   0      501       20    11847 2023-05-24 05:44:50.000000 getdaft-0.1.3/tutorials/text_to_image/text_to_image_generation.ipynb
+-rw-r--r--   0      501       20     9134 2023-05-24 05:44:50.000000 getdaft-0.1.3/tutorials/text_to_image/using_cloud_with_ray.ipynb
+-rw-r--r--   0      501       20    32068 2023-05-24 05:44:49.000000 getdaft-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0     7325 1970-01-01 00:00:00.000000 getdaft-0.1.3/PKG-INFO
```

### Comparing `getdaft-0.1.2/Cargo.toml` & `getdaft-0.1.3/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 [net]
 git-fetch-with-cli = true
 
 [package]
 edition = "2021"
 name = "daft"
-version = "0.1.2"
+version = "0.1.3"
 
 [dependencies.arrow2]
 branch = "clark/expand-casting-support"
 features = [ "compute", "io_ipc",]
 git = "https://github.com/Eventual-Inc/arrow2"
 package = "arrow2"
 version = "0.17.1"
```

### Comparing `getdaft-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md` & `getdaft-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md` & `getdaft-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/.github/workflows/broken-link-checker.yml` & `getdaft-0.1.3/.github/workflows/broken-link-checker.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/.github/workflows/daft-profiling.yml` & `getdaft-0.1.3/.github/workflows/daft-profiling.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/.github/workflows/notebook-checker.yml` & `getdaft-0.1.3/.github/workflows/notebook-checker.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/.github/workflows/property-based-tests.yml` & `getdaft-0.1.3/.github/workflows/property-based-tests.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/.github/workflows/python-package.yml` & `getdaft-0.1.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/.github/workflows/python-publish.yml` & `getdaft-0.1.3/.github/workflows/python-publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         # just the version we test with
         python-version: '3.8'
         channels: conda-forge
         channel-priority: true
 
     - name: Install anaconda client
       shell: bash -el {0}
-      run: conda install -q -y anaconda-client
+      run: conda install -q -y anaconda-client "urllib3<2.0"
 
     - name: Upload wheels to anaconda nightly
       if: ${{ success() && (env.IS_SCHEDULE_DISPATCH == 'true' || env.IS_PUSH == 'true') }}
       shell: bash -el {0}
       env:
         DAFT_STAGING_UPLOAD_TOKEN: ${{ secrets.DAFT_STAGING_UPLOAD_TOKEN }}
         DAFT_NIGHTLY_UPLOAD_TOKEN: ${{ secrets.DAFT_NIGHTLY_UPLOAD_TOKEN }}
```

### Comparing `getdaft-0.1.2/.github/workflows/ray-compatibility.yml` & `getdaft-0.1.3/.github/workflows/ray-compatibility.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/.pre-commit-config.yaml` & `getdaft-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/CONTRIBUTING.md` & `getdaft-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/LICENSE` & `getdaft-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/Makefile` & `getdaft-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/README.rst` & `getdaft-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/benchmarking/tpch/__main__.py` & `getdaft-0.1.3/benchmarking/tpch/__main__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/benchmarking/tpch/answers.py` & `getdaft-0.1.3/benchmarking/tpch/answers.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/benchmarking/tpch/data_generation.py` & `getdaft-0.1.3/benchmarking/tpch/data_generation.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/benchmarking/tpch/pipelined_data_generation.py` & `getdaft-0.1.3/benchmarking/tpch/pipelined_data_generation.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/ci/upload_wheels.sh` & `getdaft-0.1.3/ci/upload_wheels.sh`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/__init__.py` & `getdaft-0.1.3/daft/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/analytics.py` & `getdaft-0.1.3/daft/analytics.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/api_annotations.py` & `getdaft-0.1.3/daft/api_annotations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/arrow_utils.py` & `getdaft-0.1.3/daft/arrow_utils.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/context.py` & `getdaft-0.1.3/daft/context.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,37 +21,31 @@
     use_thread_pool: bool | None
 
 
 @dataclasses.dataclass(frozen=True)
 class _RayRunnerConfig(_RunnerConfig):
     name = "ray"
     address: str | None
-    max_tasks_per_core: float | None
-    max_refs_per_core: float | None
-    batch_dispatch_coeff: float | None
+    max_task_backlog: int | None
 
 
 def _get_runner_config_from_env() -> _RunnerConfig:
     """Retrieves the appropriate RunnerConfig from environment variables
 
     To use:
 
     1. PyRunner: set DAFT_RUNNER=py
     2. RayRunner: set DAFT_RUNNER=ray and optionally DAFT_RAY_ADDRESS=ray://...
     """
     runner = os.getenv("DAFT_RUNNER") or "PY"
     if runner.upper() == "RAY":
-        tasks_per_core_env = os.getenv("DAFT_DEVELOPER_RAY_MAX_TASKS_PER_CORE")
-        refs_per_core_env = os.getenv("DAFT_DEVELOPER_RAY_MAX_REFS_PER_CORE")
-        batch_dispatch_env = os.getenv("DAFT_DEVELOPER_RAY_BATCH_DISPATCH_COEFF")
+        task_backlog_env = os.getenv("DAFT_DEVELOPER_RAY_MAX_TASK_BACKLOG")
         return _RayRunnerConfig(
             address=os.getenv("DAFT_RAY_ADDRESS"),
-            max_tasks_per_core=float(tasks_per_core_env) if tasks_per_core_env else None,
-            max_refs_per_core=float(refs_per_core_env) if refs_per_core_env else None,
-            batch_dispatch_coeff=float(batch_dispatch_env) if batch_dispatch_env else None,
+            max_task_backlog=int(task_backlog_env) if task_backlog_env else None,
         )
     elif runner.upper() == "PY":
         use_thread_pool_env = os.getenv("DAFT_DEVELOPER_USE_THREAD_POOL")
         use_thread_pool = bool(int(use_thread_pool_env)) if use_thread_pool_env is not None else None
         return _PyRunnerConfig(use_thread_pool=use_thread_pool)
     raise ValueError(f"Unsupported DAFT_RUNNER variable: {runner}")
 
@@ -74,17 +68,15 @@
         if self.runner_config.name == "ray":
             from daft.runners.ray_runner import RayRunner
 
             logger.info("Using RayRunner")
             assert isinstance(self.runner_config, _RayRunnerConfig)
             _RUNNER = RayRunner(
                 address=self.runner_config.address,
-                max_tasks_per_core=self.runner_config.max_tasks_per_core,
-                max_refs_per_core=self.runner_config.max_refs_per_core,
-                batch_dispatch_coeff=self.runner_config.batch_dispatch_coeff,
+                max_task_backlog=self.runner_config.max_task_backlog,
             )
         elif self.runner_config.name == "py":
             from daft.runners.pyrunner import PyRunner
 
             logger.info("Using PyRunner")
             assert isinstance(self.runner_config, _PyRunnerConfig)
             _RUNNER = PyRunner(use_thread_pool=self.runner_config.use_thread_pool)
@@ -109,17 +101,15 @@
 def get_context() -> DaftContext:
     return _DaftContext
 
 
 def set_runner_ray(
     address: str | None = None,
     noop_if_initialized: bool = False,
-    max_tasks_per_core: float | None = None,
-    max_refs_per_core: float | None = None,
-    batch_dispatch_coeff: float | None = None,
+    max_task_backlog: int | None = None,
 ) -> DaftContext:
     """Set the runner for executing Daft dataframes to a Ray cluster
 
     Alternatively, users can set this behavior via environment variables:
 
     1. DAFT_RUNNER=ray
     2. Optionally, DAFT_RAY_ADDRESS=ray://...
@@ -143,17 +133,15 @@
             )
             return _DaftContext
         raise RuntimeError("Cannot set runner more than once")
     _DaftContext = dataclasses.replace(
         _DaftContext,
         runner_config=_RayRunnerConfig(
             address=address,
-            max_tasks_per_core=max_tasks_per_core,
-            max_refs_per_core=max_refs_per_core,
-            batch_dispatch_coeff=batch_dispatch_coeff,
+            max_task_backlog=max_task_backlog,
         ),
         disallow_set_runner=True,
     )
     return _DaftContext
 
 
 def set_runner_py(use_thread_pool: bool | None = None) -> DaftContext:
```

### Comparing `getdaft-0.1.2/daft/convert.py` & `getdaft-0.1.3/daft/convert.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/dataframe/dataframe.py` & `getdaft-0.1.3/daft/dataframe/dataframe.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/datasources.py` & `getdaft-0.1.3/daft/datasources.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/datatype.py` & `getdaft-0.1.3/daft/datatype.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/execution/execution_step.py` & `getdaft-0.1.3/daft/execution/execution_step.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/execution/logical_op_runners.py` & `getdaft-0.1.3/daft/execution/logical_op_runners.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/execution/physical_plan.py` & `getdaft-0.1.3/daft/execution/physical_plan.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/execution/physical_plan_factory.py` & `getdaft-0.1.3/daft/execution/physical_plan_factory.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/expressions/expressions.py` & `getdaft-0.1.3/daft/expressions/expressions.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/expressions/testing.py` & `getdaft-0.1.3/daft/expressions/testing.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/filesystem.py` & `getdaft-0.1.3/daft/filesystem.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/internal/rule.py` & `getdaft-0.1.3/daft/internal/rule.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/internal/rule_runner.py` & `getdaft-0.1.3/daft/internal/rule_runner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/internal/treenode.py` & `getdaft-0.1.3/daft/internal/treenode.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/io/_csv.py` & `getdaft-0.1.3/daft/io/_csv.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/io/_json.py` & `getdaft-0.1.3/daft/io/_json.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/io/common.py` & `getdaft-0.1.3/daft/io/common.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/io/file_path.py` & `getdaft-0.1.3/daft/io/file_path.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/io/parquet.py` & `getdaft-0.1.3/daft/io/parquet.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/logical/aggregation_plan_builder.py` & `getdaft-0.1.3/daft/logical/aggregation_plan_builder.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/logical/logical_plan.py` & `getdaft-0.1.3/daft/logical/logical_plan.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/logical/map_partition_ops.py` & `getdaft-0.1.3/daft/logical/map_partition_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/logical/optimizer.py` & `getdaft-0.1.3/daft/logical/optimizer.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/logical/schema.py` & `getdaft-0.1.3/daft/logical/schema.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/pickle/cloudpickle.py` & `getdaft-0.1.3/daft/pickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/pickle/cloudpickle_fast.py` & `getdaft-0.1.3/daft/pickle/cloudpickle_fast.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/pickle/compat.py` & `getdaft-0.1.3/daft/pickle/compat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/resource_request.py` & `getdaft-0.1.3/daft/resource_request.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/runners/partitioning.py` & `getdaft-0.1.3/daft/runners/partitioning.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/runners/profiler.py` & `getdaft-0.1.3/daft/runners/profiler.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/runners/pyrunner.py` & `getdaft-0.1.3/daft/runners/pyrunner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/runners/ray_runner.py` & `getdaft-0.1.3/daft/runners/ray_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,61 +356,47 @@
 
 @ray.remote
 def fanout_pipeline(instruction_stack: list[Instruction], *inputs: Table) -> list[list[PartitionMetadata] | Table]:
     return build_partitions(instruction_stack, *inputs)
 
 
 @ray.remote(scheduling_strategy="SPREAD")
-def reduce_pipeline(instruction_stack: list[Instruction], *inputs: Table) -> list[list[PartitionMetadata] | Table]:
-    return build_partitions(instruction_stack, *inputs)
+def reduce_pipeline(instruction_stack: list[Instruction], inputs: list) -> list[list[PartitionMetadata] | Table]:
+    import ray
+
+    return build_partitions(instruction_stack, *ray.get(inputs))
 
 
 @ray.remote(scheduling_strategy="SPREAD")
-def reduce_and_fanout(instruction_stack: list[Instruction], *inputs: Table) -> list[list[PartitionMetadata] | Table]:
-    return build_partitions(instruction_stack, *inputs)
+def reduce_and_fanout(instruction_stack: list[Instruction], inputs: list) -> list[list[PartitionMetadata] | Table]:
+    import ray
+
+    return build_partitions(instruction_stack, *ray.get(inputs))
 
 
 @ray.remote
 def get_meta(partition: Table) -> PartitionMetadata:
     return PartitionMetadata.from_table(partition)
 
 
 class Scheduler:
-    def __init__(
-        self,
-        max_tasks_per_core: float | None,
-        max_refs_per_core: float | None,
-        batch_dispatch_coeff: float | None,
-    ) -> None:
+    def __init__(self, max_task_backlog: int | None) -> None:
         """
-        max_tasks_per_core:
-            Maximum allowed inflight tasks per core.
-        max_refs_per_core:
-            Maximum allowed inflight objectrefs per core.
-        batch_dispatch_coeff:
-            When dispatching or awaiting tasks, do it in batches of size coeff * number of cores.
-            If 0, batching is disabled (i.e. batch size is set to 1).
+        max_task_backlog: Max number of inflight tasks waiting for cores.
         """
-        # The default values set below were determined in empirical benchmarking to deliver the best performance
-        # (runtime, data locality, memory pressure) across different configurations.
-        # They differ from the original intended values of the scheduler; the original values are discussed in comments.
-
-        # Theoretically, this should be around 2;
-        # higher values increase the likelihood of dispatching redundant tasks,
-        # and lower values reduce the cluster's ability to pipeline tasks and introduces worker idling during scheduling.
-        self.max_tasks_per_core = max_tasks_per_core if max_tasks_per_core is not None else 4.0
-
-        # This default is a vacuous limit for now.
-        # The option exists because Ray clusters anecdotally sometimes choke when there are too many object refs in flight.
-        self.max_refs_per_core = max_refs_per_core if max_refs_per_core is not None else 10000.0
-
-        # Theoretically, this should be 1.0: we should batch enough tasks for all the cores in a single dispatch;
-        # otherwise, we begin dispatching downstream dependencies (that are not immediately executable)
-        # before saturating all the cores (and their pipelines).
-        self.batch_dispatch_coeff = batch_dispatch_coeff if batch_dispatch_coeff is not None else 1.0
+
+        # As of writing, Ray does not seem to be guaranteed to support
+        # more than this number of pending scheduling tasks.
+        # Ray has an internal proto that reports backlogged tasks [1],
+        # and each task proto can be up to 10 MiB [2],
+        # and protobufs have a max size of 2GB (from errors empirically encountered).
+        #
+        # https://github.com/ray-project/ray/blob/8427de2776717b30086c277e5e8e140316dbd193/src/ray/protobuf/node_manager.proto#L32
+        # https://github.com/ray-project/ray/blob/fb95f03f05981f232aa7a9073dd2c2512729e99a/src/ray/common/ray_config_def.h#LL513C1-L513C1
+        self.max_task_backlog = max_task_backlog if max_task_backlog is not None else 180
 
         self.reserved_cores = 0
 
     def run_plan(
         self,
         plan: logical_plan.LogicalPlan,
         psets: dict[str, ray.ObjectRef],
@@ -418,35 +404,38 @@
         from loguru import logger
 
         phys_plan = physical_plan_factory.get_materializing_physical_plan(plan, psets)
 
         # Note: For autoscaling clusters, we will probably want to query cores dynamically.
         # Keep in mind this call takes about 0.3ms.
         cores = int(ray.cluster_resources()["CPU"]) - self.reserved_cores
-        batch_dispatch_size = int(cores * self.batch_dispatch_coeff) or 1
+
+        max_inflight_tasks = cores + self.max_task_backlog
 
         inflight_tasks: dict[str, PartitionTask[ray.ObjectRef]] = dict()
         inflight_ref_to_task: dict[ray.ObjectRef, str] = dict()
 
         result_partitions = None
         start = datetime.now()
         profile_filename = (
             f"profile_RayRunner.run()_"
             f"{datetime.replace(datetime.now(), second=0, microsecond=0).isoformat()[:-3]}.json"
         )
         with profiler(profile_filename):
-            while True:
-                while (
-                    len(inflight_tasks) < self.max_tasks_per_core * cores
-                    and len(inflight_ref_to_task) < self.max_refs_per_core * cores
-                ):
+            while True:  # Loop: Dispatch -> await.
+
+                while True:  # Loop: Dispatch (in batches).
+                    dispatches_allowed = max_inflight_tasks - len(inflight_tasks)
+                    if dispatches_allowed <= 0:
+                        break
+
                     # Get the next batch of tasks to dispatch.
                     tasks_to_dispatch = []
                     try:
-                        for _ in range(batch_dispatch_size):
+                        for _ in range(min(cores, dispatches_allowed)):
                             next_step = next(phys_plan)
 
                             # If this task is a no-op, just run it locally immediately.
                             while next_step is not None and len(next_step.instructions) == 0:
                                 logger.debug(
                                     "Running task synchronously in main thread: {next_step}", next_step=next_step
                                 )
@@ -476,29 +465,50 @@
                             inflight_ref_to_task[result] = task.id()
 
                     # Exit if the plan is complete and the result references are available.
                     if result_partitions is not None:
                         return result_partitions
 
                 # Await a batch of tasks.
-                for i in range(min(batch_dispatch_size, len(inflight_tasks))):
-                    dispatch = datetime.now()
-                    [ready], _ = ray.wait(list(inflight_ref_to_task.keys()), fetch_local=False)
-                    task_id = inflight_ref_to_task[ready]
-                    logger.debug(f"+{(datetime.now() - dispatch).total_seconds()}s to await a result from {task_id}")
-
-                    # Mark the entire task associated with the result as done.
-                    task = inflight_tasks[task_id]
-                    if isinstance(task, SingleOutputPartitionTask):
-                        del inflight_ref_to_task[ready]
-                    elif isinstance(task, MultiOutputPartitionTask):
-                        for partition in task.partitions():
-                            del inflight_ref_to_task[partition]
+                # (Awaits the next task, and then the next batch of tasks within 10ms.)
+
+                dispatch = datetime.now()
+                completed_task_ids = []
+                for wait_for in ("next_one", "next_batch"):
+                    if wait_for == "next_one":
+                        num_returns = 1
+                        timeout = None
+                    elif wait_for == "next_batch":
+                        num_returns = len(inflight_ref_to_task)
+                        timeout = 0.01  # 10ms
 
-                    del inflight_tasks[task_id]
+                    if num_returns == 0:
+                        break
+
+                    readies, _ = ray.wait(
+                        list(inflight_ref_to_task.keys()), num_returns=num_returns, timeout=timeout, fetch_local=False
+                    )
+
+                    for ready in readies:
+                        if ready in inflight_ref_to_task:
+                            task_id = inflight_ref_to_task[ready]
+                            completed_task_ids.append(task_id)
+                            # Mark the entire task associated with the result as done.
+                            task = inflight_tasks[task_id]
+                            if isinstance(task, SingleOutputPartitionTask):
+                                del inflight_ref_to_task[ready]
+                            elif isinstance(task, MultiOutputPartitionTask):
+                                for partition in task.partitions():
+                                    del inflight_ref_to_task[partition]
+
+                            del inflight_tasks[task_id]
+
+                logger.debug(
+                    f"+{(datetime.now() - dispatch).total_seconds()}s to await results from {completed_task_ids}"
+                )
 
 
 @ray.remote(num_cpus=1)
 class SchedulerActor(Scheduler):
     def __init__(self, *n, **kw) -> None:
         super().__init__(*n, **kw)
         self.reserved_cores = 1
@@ -511,34 +521,35 @@
     }
 
     if task.resource_request is not None:
         ray_options = {**ray_options, **_get_ray_task_options(task.resource_request)}
 
     if isinstance(task.instructions[0], ReduceInstruction):
         build_remote = reduce_and_fanout if isinstance(task.instructions[-1], FanoutInstruction) else reduce_pipeline
+        build_remote = build_remote.options(**ray_options)
+        [metadatas_ref, *partitions] = build_remote.remote(task.instructions, task.inputs)
+
     else:
         build_remote = (
             fanout_pipeline if isinstance(task.instructions[-1], FanoutInstruction) else single_partition_pipeline
         )
+        build_remote = build_remote.options(**ray_options)
+        [metadatas_ref, *partitions] = build_remote.remote(task.instructions, *task.inputs)
 
-    build_remote = build_remote.options(**ray_options)
-    [metadatas_ref, *partitions] = build_remote.remote(task.instructions, *task.inputs)
     metadatas_accessor = PartitionMetadataAccessor(metadatas_ref)
     task.set_result([RayMaterializedResult(partition, metadatas_accessor, i) for i, partition in enumerate(partitions)])
 
     return partitions
 
 
 class RayRunner(Runner):
     def __init__(
         self,
         address: str | None,
-        max_tasks_per_core: float | None,
-        max_refs_per_core: float | None,
-        batch_dispatch_coeff: float | None,
+        max_task_backlog: int | None,
     ) -> None:
         super().__init__()
         if ray.is_initialized():
             logger.warning(f"Ray has already been initialized, Daft will reuse the existing Ray context.")
         self.ray_context = ray.init(address=address, ignore_reinit_error=True)
         self._optimizer = RuleRunner(
             [
@@ -560,23 +571,19 @@
                 ),
             ]
         )
 
         if isinstance(self.ray_context, ray.client_builder.ClientContext):
             # Run scheduler remotely if the cluster is connected remotely.
             self.scheduler_actor = SchedulerActor.remote(  # type: ignore
-                max_tasks_per_core=max_tasks_per_core,
-                max_refs_per_core=max_refs_per_core,
-                batch_dispatch_coeff=batch_dispatch_coeff,
+                max_task_backlog=max_task_backlog,
             )
         else:
             self.scheduler = Scheduler(
-                max_tasks_per_core=max_tasks_per_core,
-                max_refs_per_core=max_refs_per_core,
-                batch_dispatch_coeff=batch_dispatch_coeff,
+                max_task_backlog=max_task_backlog,
             )
 
     def run(self, plan: logical_plan.LogicalPlan) -> PartitionCacheEntry:
         result_pset = RayPartitionSet({})
 
         plan = self.optimize(plan)
```

### Comparing `getdaft-0.1.2/daft/runners/runner.py` & `getdaft-0.1.3/daft/runners/runner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/runners/runner_io.py` & `getdaft-0.1.3/daft/runners/runner_io.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/series.py` & `getdaft-0.1.3/daft/series.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/table/table.py` & `getdaft-0.1.3/daft/table/table.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/table/table_io.py` & `getdaft-0.1.3/daft/table/table_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,14 @@
     vPartitionSchemaInferenceOptions,
 )
 from daft.table import Table
 
 FileInput = Union[pathlib.Path, str, IO[bytes]]
 
 
-# The number of rows to read per batch. This is sized to generate 10MiB batches
-# for rows about 1KiB in size.
-_PARQUET_FRAGMENT_BATCH_SIZE = 100000
-
-
 @contextlib.contextmanager
 def _open_stream(
     file: FileInput,
     fs: FileSystem | fsspec.AbstractFileSystem | None,
 ) -> Generator[pa.NativeFile, None, None]:
     """Opens the provided file for reading, yield a pyarrow file handle."""
     if isinstance(file, (pathlib.Path, str)):
@@ -95,36 +90,37 @@
     if not isinstance(file, (str, pathlib.Path)):
         # BytesIO path.
         return Table.from_arrow(papq.read_table(file, columns=read_options.column_names))
 
     paths, fs = _resolve_paths_and_filesystem(file, fs)
     assert len(paths) == 1
     path = paths[0]
-    fragment = pads.ParquetFileFormat().make_fragment(path, filesystem=fs)
-    schema = fragment.metadata.schema.to_arrow_schema()
+    f = fs.open_input_file(path)
+    pqf = papq.ParquetFile(f)
     # If no rows required, we manually construct an empty table with the right schema
     if read_options.num_rows == 0:
-        table = pa.Table.from_arrays([pa.array([], type=field.type) for field in schema], schema=schema)
+        arrow_schema = pqf.metadata.schema.to_arrow_schema()
+        table = pa.Table.from_arrays([pa.array([], type=field.type) for field in arrow_schema], schema=arrow_schema)
     elif read_options.num_rows is not None:
-        # Read the file by row group.
-        frags = fragment.split_by_row_group()
-        tables = []
-        rows_read = 0
-        for frag in frags:
-            for batch in frag.to_batches(columns=read_options.column_names, batch_size=_PARQUET_FRAGMENT_BATCH_SIZE):
-                tables.append(pa.Table.from_batches([batch], schema=schema))
-                rows_read += len(batch)
-                if rows_read >= read_options.num_rows:
-                    break
-            if rows_read >= read_options.num_rows:
+        # Only read the required row groups.
+        rows_needed = read_options.num_rows
+        for i in range(pqf.metadata.num_row_groups):
+            row_group_meta = pqf.metadata.row_group(i)
+            rows_needed -= row_group_meta.num_rows
+            if rows_needed <= 0:
                 break
-        table = pa.concat_tables(tables)
-        table = table.slice(length=read_options.num_rows)
+        table = pqf.read_row_groups(list(range(i + 1)), columns=read_options.column_names)
+        if rows_needed < 0:
+            # Need to truncate the table to the row limit.
+            table = table.slice(length=read_options.num_rows)
     else:
-        table = fragment.to_table(columns=read_options.column_names)
+        table = papq.read_table(
+            f,
+            columns=read_options.column_names,
+        )
 
     return Table.from_arrow(table)
 
 
 def read_csv(
     file: FileInput,
     fs: fsspec.AbstractFileSystem | None = None,
```

### Comparing `getdaft-0.1.2/daft/udf.py` & `getdaft-0.1.3/daft/udf.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/udf_library/url_udfs.py` & `getdaft-0.1.3/daft/udf_library/url_udfs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/utils.py` & `getdaft-0.1.3/daft/utils.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/viz/dataframe_display.py` & `getdaft-0.1.3/daft/viz/dataframe_display.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/viz/html_viz_hooks.py` & `getdaft-0.1.3/daft/viz/html_viz_hooks.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/daft/viz/repr.py` & `getdaft-0.1.3/daft/viz/repr.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/Makefile` & `getdaft-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/10-min.ipynb` & `getdaft-0.1.3/docs/source/10-min.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/_static/daft-favicon.png` & `getdaft-0.1.3/docs/source/_static/daft-favicon.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/_static/daft-logo.png` & `getdaft-0.1.3/docs/source/_static/daft-logo.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/_static/daft_illustration.png` & `getdaft-0.1.3/docs/source/_static/daft_illustration.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/_static/execution_model.png` & `getdaft-0.1.3/docs/source/_static/execution_model.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/_static/header.css` & `getdaft-0.1.3/docs/source/_static/header.css`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/_static/high_level_architecture.png` & `getdaft-0.1.3/docs/source/_static/high_level_architecture.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/_static/in_memory_data_representation.png` & `getdaft-0.1.3/docs/source/_static/in_memory_data_representation.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/_static/mobile-menu.js` & `getdaft-0.1.3/docs/source/_static/mobile-menu.js`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/_templates/layout.html` & `getdaft-0.1.3/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/_templates/sections/header.html` & `getdaft-0.1.3/docs/source/_templates/sections/header.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/_templates/sections/mobile-menu.html` & `getdaft-0.1.3/docs/source/_templates/sections/mobile-menu.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/api_docs/dataframe.rst` & `getdaft-0.1.3/docs/source/api_docs/dataframe.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/api_docs/expressions.rst` & `getdaft-0.1.3/docs/source/api_docs/expressions.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/api_docs/groupby.rst` & `getdaft-0.1.3/docs/source/api_docs/groupby.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/api_docs/input_output.rst` & `getdaft-0.1.3/docs/source/api_docs/input_output.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/conf.py` & `getdaft-0.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/dataframe_comparison.rst` & `getdaft-0.1.3/docs/source/dataframe_comparison.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/index.rst` & `getdaft-0.1.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/install.rst` & `getdaft-0.1.3/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/learn/index.rst` & `getdaft-0.1.3/docs/source/learn/index.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/learn/key_concepts.rst` & `getdaft-0.1.3/docs/source/learn/key_concepts.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/learn/tutorials.rst` & `getdaft-0.1.3/docs/source/learn/tutorials.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/learn/user_guides/aggregations.rst` & `getdaft-0.1.3/docs/source/learn/user_guides/aggregations.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/learn/user_guides/dataframe-operations.rst` & `getdaft-0.1.3/docs/source/learn/user_guides/dataframe-operations.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/learn/user_guides/expressions.rst` & `getdaft-0.1.3/docs/source/learn/user_guides/expressions.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/learn/user_guides/intro-dataframes.rst` & `getdaft-0.1.3/docs/source/learn/user_guides/intro-dataframes.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/learn/user_guides/read-write.rst` & `getdaft-0.1.3/docs/source/learn/user_guides/read-write.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/learn/user_guides/scaling-up.rst` & `getdaft-0.1.3/docs/source/learn/user_guides/scaling-up.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/learn/user_guides/udf.rst` & `getdaft-0.1.3/docs/source/learn/user_guides/udf.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/learn/user_guides.rst` & `getdaft-0.1.3/docs/source/learn/user_guides.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/release_notes/0.0.13.rst` & `getdaft-0.1.3/docs/source/release_notes/0.0.13.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/release_notes/0.0.14.rst` & `getdaft-0.1.3/docs/source/release_notes/0.0.14.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/release_notes/0.0.16.rst` & `getdaft-0.1.3/docs/source/release_notes/0.0.16.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/release_notes/0.0.17.rst` & `getdaft-0.1.3/docs/source/release_notes/0.0.17.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/release_notes/0.0.18.rst` & `getdaft-0.1.3/docs/source/release_notes/0.0.18.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/release_notes/0.0.19.rst` & `getdaft-0.1.3/docs/source/release_notes/0.0.19.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/release_notes/0.0.20.rst` & `getdaft-0.1.3/docs/source/release_notes/0.0.20.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/release_notes/0.0.21.rst` & `getdaft-0.1.3/docs/source/release_notes/0.0.21.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/release_notes/0.0.22.rst` & `getdaft-0.1.3/docs/source/release_notes/0.0.22.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/release_notes/0.0.23.rst` & `getdaft-0.1.3/docs/source/release_notes/0.0.23.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/release_notes/0.0.24.rst` & `getdaft-0.1.3/docs/source/release_notes/0.0.24.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/release_notes/0.1.0.rst` & `getdaft-0.1.3/docs/source/release_notes/0.1.0.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/release_notes/0.1.1.rst` & `getdaft-0.1.3/docs/source/release_notes/0.1.1.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/release_notes/0.1.2.rst` & `getdaft-0.1.3/docs/source/release_notes/0.1.2.rst`

 * *Files 5% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 -------------
 
 * \[ci\] enable pyrunner for 310 `#946 <https://github.com/Eventual-Inc/Daft/pull/946>`_
 * Add Pyarrow 6.0 in matrix for CI testing `#945 <https://github.com/Eventual-Inc/Daft/pull/945>`_
 * Update requirement of tabulate to \>=0.9.0 `#940 <https://github.com/Eventual-Inc/Daft/pull/940>`_
 * unpin numpy for 3.7 to get dependabot to stop complaining `#938 <https://github.com/Eventual-Inc/Daft/pull/938>`_
 * Bump slackapi/slack-github-action from 1.23.0 to 1.24.0 `#936 <https:github.com/Eventual-Inc/Daft/pull/936>`_
-* Bump hypothesis from 6.75.2 to 6.75.3 `#928 <https:github.com/Eventual-Inc/Daft/pull/928>`_
-* Bump dask from 2023.4.1 to 2023.5.0 `#927 <https:github.com/Eventual-Inc/Daft/pull/927>`_
-* Bump serde from 1.0.162 to 1.0.163 `#921 <https:github.com/Eventual-Inc/Daft/pull/921>`_
+* Bump hypothesis from 6.75.2 to 6.75.3 `#928 <https://github.com/Eventual-Inc/Daft/pull/928>`_
+* Bump dask from 2023.4.1 to 2023.5.0 `#927 <https://github.com/Eventual-Inc/Daft/pull/927>`_
+* Bump serde from 1.0.162 to 1.0.163 `#921 <https://github.com/Eventual-Inc/Daft/pull/921>`_
 
 
 Documentation
 -------------
 
 * Add comment to explain \_\_future\_\_ annotations isort rule in dataframe.py `#947 <https://github.com/Eventual-Inc/Daft/pull/947>`_
 * \[Embedding tutorial\] Suggest running on GPU cluster `#932 <https://github.com/Eventual-Inc/Daft/pull/932>`_
```

### Comparing `getdaft-0.1.2/docs/source/release_notes/_template.rst` & `getdaft-0.1.3/docs/source/release_notes/_template.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/technical_architecture.rst` & `getdaft-0.1.3/docs/source/technical_architecture.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/docs/source/telemetry.rst` & `getdaft-0.1.3/docs/source/telemetry.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/pyproject.toml` & `getdaft-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/requirements-dev.txt` & `getdaft-0.1.3/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/from.rs` & `getdaft-0.1.3/src/array/from.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/iterator.rs` & `getdaft-0.1.3/src/array/iterator.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/mod.rs` & `getdaft-0.1.3/src/array/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/apply.rs` & `getdaft-0.1.3/src/array/ops/apply.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/arange.rs` & `getdaft-0.1.3/src/array/ops/arange.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/arithmetic.rs` & `getdaft-0.1.3/src/array/ops/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/arrow2/comparison.rs` & `getdaft-0.1.3/src/array/ops/arrow2/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/arrow2/sort/primitive/common.rs` & `getdaft-0.1.3/src/array/ops/arrow2/sort/primitive/common.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/arrow2/sort/primitive/indices.rs` & `getdaft-0.1.3/src/array/ops/arrow2/sort/primitive/indices.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/arrow2/sort/primitive/sort.rs` & `getdaft-0.1.3/src/array/ops/arrow2/sort/primitive/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/as_arrow.rs` & `getdaft-0.1.3/src/array/ops/as_arrow.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/broadcast.rs` & `getdaft-0.1.3/src/array/ops/broadcast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/cast.rs` & `getdaft-0.1.3/src/array/ops/cast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/compare_agg.rs` & `getdaft-0.1.3/src/array/ops/compare_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/comparison.rs` & `getdaft-0.1.3/src/array/ops/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/concat.rs` & `getdaft-0.1.3/src/array/ops/concat.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/concat_agg.rs` & `getdaft-0.1.3/src/array/ops/concat_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/count.rs` & `getdaft-0.1.3/src/array/ops/count.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/date.rs` & `getdaft-0.1.3/src/array/ops/date.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/filter.rs` & `getdaft-0.1.3/src/array/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/float.rs` & `getdaft-0.1.3/src/array/ops/float.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/full.rs` & `getdaft-0.1.3/src/array/ops/full.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/groups.rs` & `getdaft-0.1.3/src/array/ops/groups.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/hash.rs` & `getdaft-0.1.3/src/array/ops/hash.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/if_else.rs` & `getdaft-0.1.3/src/array/ops/if_else.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/len.rs` & `getdaft-0.1.3/src/array/ops/len.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/list.rs` & `getdaft-0.1.3/src/array/ops/list.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/list_agg.rs` & `getdaft-0.1.3/src/array/ops/list_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/mean.rs` & `getdaft-0.1.3/src/array/ops/mean.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/mod.rs` & `getdaft-0.1.3/src/array/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/null.rs` & `getdaft-0.1.3/src/array/ops/null.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/pairwise.rs` & `getdaft-0.1.3/src/array/ops/pairwise.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/sort.rs` & `getdaft-0.1.3/src/array/ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/sum.rs` & `getdaft-0.1.3/src/array/ops/sum.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/take.rs` & `getdaft-0.1.3/src/array/ops/take.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/ops/utf8.rs` & `getdaft-0.1.3/src/array/ops/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/pseudo_arrow/compute.rs` & `getdaft-0.1.3/src/array/pseudo_arrow/compute.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/pseudo_arrow/mod.rs` & `getdaft-0.1.3/src/array/pseudo_arrow/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/array/pseudo_arrow/python.rs` & `getdaft-0.1.3/src/array/pseudo_arrow/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/datatypes/dtype.rs` & `getdaft-0.1.3/src/datatypes/dtype.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/datatypes/field.rs` & `getdaft-0.1.3/src/datatypes/field.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/datatypes/logical.rs` & `getdaft-0.1.3/src/datatypes/logical.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/datatypes/matching.rs` & `getdaft-0.1.3/src/datatypes/matching.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/datatypes/mod.rs` & `getdaft-0.1.3/src/datatypes/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/datatypes/time_unit.rs` & `getdaft-0.1.3/src/datatypes/time_unit.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/arithmetic.rs` & `getdaft-0.1.3/src/dsl/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/expr.rs` & `getdaft-0.1.3/src/dsl/expr.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/functions/float/is_nan.rs` & `getdaft-0.1.3/src/dsl/functions/float/is_nan.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/functions/float/mod.rs` & `getdaft-0.1.3/src/dsl/functions/float/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/functions/list/explode.rs` & `getdaft-0.1.3/src/dsl/functions/list/explode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/functions/list/mod.rs` & `getdaft-0.1.3/src/dsl/functions/list/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/functions/mod.rs` & `getdaft-0.1.3/src/dsl/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/functions/numeric/abs.rs` & `getdaft-0.1.3/src/dsl/functions/numeric/abs.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/functions/numeric/mod.rs` & `getdaft-0.1.3/src/dsl/functions/numeric/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/functions/python/mod.rs` & `getdaft-0.1.3/src/dsl/functions/python/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/functions/python/partial_udf.rs` & `getdaft-0.1.3/src/dsl/functions/python/partial_udf.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/functions/python/udf.rs` & `getdaft-0.1.3/src/dsl/functions/python/udf.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/functions/temporal/day.rs` & `getdaft-0.1.3/src/dsl/functions/temporal/day.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/functions/temporal/day_of_week.rs` & `getdaft-0.1.3/src/dsl/functions/temporal/day_of_week.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/functions/temporal/mod.rs` & `getdaft-0.1.3/src/dsl/functions/temporal/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/functions/temporal/month.rs` & `getdaft-0.1.3/src/dsl/functions/temporal/month.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/functions/temporal/year.rs` & `getdaft-0.1.3/src/dsl/functions/temporal/year.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/functions/utf8/contains.rs` & `getdaft-0.1.3/src/dsl/functions/utf8/contains.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/functions/utf8/endswith.rs` & `getdaft-0.1.3/src/dsl/functions/utf8/endswith.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/functions/utf8/length.rs` & `getdaft-0.1.3/src/dsl/functions/utf8/length.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/functions/utf8/mod.rs` & `getdaft-0.1.3/src/dsl/functions/utf8/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/functions/utf8/startswith.rs` & `getdaft-0.1.3/src/dsl/functions/utf8/startswith.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/lit.rs` & `getdaft-0.1.3/src/dsl/lit.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/optimization.rs` & `getdaft-0.1.3/src/dsl/optimization.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/dsl/pyobject.rs` & `getdaft-0.1.3/src/dsl/pyobject.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/error.rs` & `getdaft-0.1.3/src/error.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/ffi.rs` & `getdaft-0.1.3/src/ffi.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/kernels/hashing.rs` & `getdaft-0.1.3/src/kernels/hashing.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/kernels/search_sorted.rs` & `getdaft-0.1.3/src/kernels/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/kernels/utf8.rs` & `getdaft-0.1.3/src/kernels/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/lib.rs` & `getdaft-0.1.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/python/datatype.rs` & `getdaft-0.1.3/src/python/datatype.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/python/expr.rs` & `getdaft-0.1.3/src/python/expr.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/python/field.rs` & `getdaft-0.1.3/src/python/field.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/python/mod.rs` & `getdaft-0.1.3/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/python/schema.rs` & `getdaft-0.1.3/src/python/schema.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/python/series.rs` & `getdaft-0.1.3/src/python/series.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/python/table.rs` & `getdaft-0.1.3/src/python/table.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/schema.rs` & `getdaft-0.1.3/src/schema.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/series/array_impl/data_array.rs` & `getdaft-0.1.3/src/series/array_impl/data_array.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/series/array_impl/logical_array.rs` & `getdaft-0.1.3/src/series/array_impl/logical_array.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/series/from.rs` & `getdaft-0.1.3/src/series/from.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/series/mod.rs` & `getdaft-0.1.3/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/series/ops/abs.rs` & `getdaft-0.1.3/src/series/ops/abs.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/series/ops/agg.rs` & `getdaft-0.1.3/src/series/ops/agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/series/ops/arithmetic.rs` & `getdaft-0.1.3/src/series/ops/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/series/ops/broadcast.rs` & `getdaft-0.1.3/src/series/ops/broadcast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/series/ops/comparison.rs` & `getdaft-0.1.3/src/series/ops/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/series/ops/concat.rs` & `getdaft-0.1.3/src/series/ops/concat.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/series/ops/date.rs` & `getdaft-0.1.3/src/series/ops/date.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/series/ops/downcast.rs` & `getdaft-0.1.3/src/series/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/series/ops/filter.rs` & `getdaft-0.1.3/src/series/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/series/ops/list.rs` & `getdaft-0.1.3/src/series/ops/list.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/series/ops/mod.rs` & `getdaft-0.1.3/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/series/ops/search_sorted.rs` & `getdaft-0.1.3/src/series/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/series/ops/sort.rs` & `getdaft-0.1.3/src/series/ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/series/ops/take.rs` & `getdaft-0.1.3/src/series/ops/take.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/series/ops/utf8.rs` & `getdaft-0.1.3/src/series/ops/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/series/series_like.rs` & `getdaft-0.1.3/src/series/series_like.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/table/mod.rs` & `getdaft-0.1.3/src/table/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/table/ops/agg.rs` & `getdaft-0.1.3/src/table/ops/agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/table/ops/explode.rs` & `getdaft-0.1.3/src/table/ops/explode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/table/ops/groups.rs` & `getdaft-0.1.3/src/table/ops/groups.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/table/ops/hash.rs` & `getdaft-0.1.3/src/table/ops/hash.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/table/ops/joins/hash_join.rs` & `getdaft-0.1.3/src/table/ops/joins/hash_join.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/table/ops/joins/mod.rs` & `getdaft-0.1.3/src/table/ops/joins/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/table/ops/partition.rs` & `getdaft-0.1.3/src/table/ops/partition.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/table/ops/search_sorted.rs` & `getdaft-0.1.3/src/table/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/table/ops/sort.rs` & `getdaft-0.1.3/src/table/ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/utils/arrow.rs` & `getdaft-0.1.3/src/utils/arrow.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/src/utils/supertype.rs` & `getdaft-0.1.3/src/utils/supertype.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/assets/tpch-sqlite-queries/1.sql` & `getdaft-0.1.3/tests/assets/tpch-sqlite-queries/1.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/assets/tpch-sqlite-queries/10.sql` & `getdaft-0.1.3/tests/assets/tpch-sqlite-queries/10.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/assets/tpch-sqlite-queries/2.sql` & `getdaft-0.1.3/tests/assets/tpch-sqlite-queries/2.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/assets/tpch-sqlite-queries/7.sql` & `getdaft-0.1.3/tests/assets/tpch-sqlite-queries/7.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/assets/tpch-sqlite-queries/8.sql` & `getdaft-0.1.3/tests/assets/tpch-sqlite-queries/8.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/assets/tpch-sqlite-queries/9.sql` & `getdaft-0.1.3/tests/assets/tpch-sqlite-queries/9.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/benchmarks/conftest.py` & `getdaft-0.1.3/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/benchmarks/test_df_arithmetic.py` & `getdaft-0.1.3/tests/benchmarks/test_df_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/benchmarks/test_groups_and_aggs.py` & `getdaft-0.1.3/tests/benchmarks/test_groups_and_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/benchmarks/test_join.py` & `getdaft-0.1.3/tests/benchmarks/test_join.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/benchmarks/test_repartition.py` & `getdaft-0.1.3/tests/benchmarks/test_repartition.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/benchmarks/test_sort.py` & `getdaft-0.1.3/tests/benchmarks/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/conftest.py` & `getdaft-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/cookbook/assets/311-service-requests.24.csv` & `getdaft-0.1.3/tests/cookbook/assets/311-service-requests.24.csv`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/cookbook/conftest.py` & `getdaft-0.1.3/tests/cookbook/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/cookbook/test_aggregations.py` & `getdaft-0.1.3/tests/cookbook/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/cookbook/test_computations.py` & `getdaft-0.1.3/tests/cookbook/test_computations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/cookbook/test_count_rows.py` & `getdaft-0.1.3/tests/cookbook/test_count_rows.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/cookbook/test_dataloading.py` & `getdaft-0.1.3/tests/cookbook/test_dataloading.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/cookbook/test_distinct.py` & `getdaft-0.1.3/tests/cookbook/test_distinct.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/cookbook/test_filter.py` & `getdaft-0.1.3/tests/cookbook/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/cookbook/test_joins.py` & `getdaft-0.1.3/tests/cookbook/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/cookbook/test_literals.py` & `getdaft-0.1.3/tests/cookbook/test_literals.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/cookbook/test_pandas_cookbook.py` & `getdaft-0.1.3/tests/cookbook/test_pandas_cookbook.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/cookbook/test_sorting.py` & `getdaft-0.1.3/tests/cookbook/test_sorting.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/cookbook/test_write.py` & `getdaft-0.1.3/tests/cookbook/test_write.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/dataframe/conftest.py` & `getdaft-0.1.3/tests/dataframe/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/dataframe/test_accessors.py` & `getdaft-0.1.3/tests/dataframe/test_accessors.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/dataframe/test_aggregations.py` & `getdaft-0.1.3/tests/dataframe/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/dataframe/test_creation.py` & `getdaft-0.1.3/tests/dataframe/test_creation.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/dataframe/test_distinct.py` & `getdaft-0.1.3/tests/dataframe/test_distinct.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/dataframe/test_explode.py` & `getdaft-0.1.3/tests/dataframe/test_explode.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/dataframe/test_filter.py` & `getdaft-0.1.3/tests/dataframe/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/dataframe/test_getitem.py` & `getdaft-0.1.3/tests/dataframe/test_getitem.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/dataframe/test_joins.py` & `getdaft-0.1.3/tests/dataframe/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/dataframe/test_logical_type.py` & `getdaft-0.1.3/tests/dataframe/test_logical_type.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/dataframe/test_repr.py` & `getdaft-0.1.3/tests/dataframe/test_repr.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/dataframe/test_select.py` & `getdaft-0.1.3/tests/dataframe/test_select.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/dataframe/test_show.py` & `getdaft-0.1.3/tests/dataframe/test_show.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/dataframe/test_sort.py` & `getdaft-0.1.3/tests/dataframe/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/dataframe/test_temporals.py` & `getdaft-0.1.3/tests/dataframe/test_temporals.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/dataframe/test_to_integrations.py` & `getdaft-0.1.3/tests/dataframe/test_to_integrations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/dataframe/test_with_column.py` & `getdaft-0.1.3/tests/dataframe/test_with_column.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/expressions/test_apply.py` & `getdaft-0.1.3/tests/expressions/test_apply.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/expressions/test_expressions.py` & `getdaft-0.1.3/tests/expressions/test_expressions.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/expressions/test_expressions_projection.py` & `getdaft-0.1.3/tests/expressions/test_expressions_projection.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/expressions/test_udf.py` & `getdaft-0.1.3/tests/expressions/test_udf.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/expressions/typing/conftest.py` & `getdaft-0.1.3/tests/expressions/typing/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/expressions/typing/test_aggs.py` & `getdaft-0.1.3/tests/expressions/typing/test_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/expressions/typing/test_arithmetic.py` & `getdaft-0.1.3/tests/expressions/typing/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/expressions/typing/test_compare.py` & `getdaft-0.1.3/tests/expressions/typing/test_compare.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/expressions/typing/test_dt.py` & `getdaft-0.1.3/tests/expressions/typing/test_dt.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/expressions/typing/test_float.py` & `getdaft-0.1.3/tests/expressions/typing/test_float.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/expressions/typing/test_if_else.py` & `getdaft-0.1.3/tests/expressions/typing/test_if_else.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/expressions/typing/test_logical.py` & `getdaft-0.1.3/tests/expressions/typing/test_logical.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/expressions/typing/test_str.py` & `getdaft-0.1.3/tests/expressions/typing/test_str.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/integration/test_tpch.py` & `getdaft-0.1.3/tests/integration/test_tpch.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/optimizer/conftest.py` & `getdaft-0.1.3/tests/optimizer/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/optimizer/test_drop_projections.py` & `getdaft-0.1.3/tests/optimizer/test_drop_projections.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/optimizer/test_drop_repartition.py` & `getdaft-0.1.3/tests/optimizer/test_drop_repartition.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/optimizer/test_fold_projections.py` & `getdaft-0.1.3/tests/optimizer/test_fold_projections.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/optimizer/test_prune_columns.py` & `getdaft-0.1.3/tests/optimizer/test_prune_columns.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/optimizer/test_pushdown_clauses_into_scan.py` & `getdaft-0.1.3/tests/optimizer/test_pushdown_clauses_into_scan.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/optimizer/test_pushdown_limit.py` & `getdaft-0.1.3/tests/optimizer/test_pushdown_limit.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/optimizer/test_pushdown_predicates.py` & `getdaft-0.1.3/tests/optimizer/test_pushdown_predicates.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/property_based_testing/strategies.py` & `getdaft-0.1.3/tests/property_based_testing/strategies.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/property_based_testing/test_sort.py` & `getdaft-0.1.3/tests/property_based_testing/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/ray/test_dask.py` & `getdaft-0.1.3/tests/ray/test_dask.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/ray/test_datasets.py` & `getdaft-0.1.3/tests/ray/test_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,21 +183,22 @@
 @pytest.mark.skipif(get_context().runner_config.name != "ray", reason="Needs to run on Ray runner")
 @pytest.mark.parametrize("n_partitions", [1, 2])
 def test_from_ray_dataset_tensor(n_partitions: int):
     ds = ray.data.range(8)
     ds = ds.map(lambda i: {"int": i, "np": np.ones((3, 3))}).repartition(n_partitions)
 
     df = daft.from_ray_dataset(ds)
-    np.testing.assert_equal(
-        df.to_pydict(),
-        {
-            "int": list(range(8)),
-            "np": [np.ones((3, 3)) for i in range(8)],
-        },
-    )
+    out = df.to_pydict()
+    out["np"] = [arr.tolist() for arr in out["np"]]
+    expected = {
+        "int": list(range(8)),
+        "np": [np.ones((3, 3)) for i in range(8)],
+    }
+    expected["np"] = [arr.tolist() for arr in expected["np"]]
+    assert freeze(out) == freeze(expected)
 
 
 @pytest.mark.skipif(get_context().runner_config.name != "ray", reason="Needs to run on Ray runner")
 @pytest.mark.parametrize("n_partitions", [1, 2])
 def test_from_ray_dataset_pandas(n_partitions: int):
     def add_float(df: pd.DataFrame) -> pd.DataFrame:
         df["floatcol"] = df["intcol"].astype(float)
```

### Comparing `getdaft-0.1.2/tests/series/test_arithmetic.py` & `getdaft-0.1.3/tests/series/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/series/test_cast.py` & `getdaft-0.1.3/tests/series/test_cast.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/series/test_comparisons.py` & `getdaft-0.1.3/tests/series/test_comparisons.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/series/test_concat.py` & `getdaft-0.1.3/tests/series/test_concat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/series/test_embedding.py` & `getdaft-0.1.3/tests/series/test_embedding.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/series/test_filter.py` & `getdaft-0.1.3/tests/series/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/series/test_float.py` & `getdaft-0.1.3/tests/series/test_float.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/series/test_hash.py` & `getdaft-0.1.3/tests/series/test_hash.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/series/test_if_else.py` & `getdaft-0.1.3/tests/series/test_if_else.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/series/test_numeric_ops.py` & `getdaft-0.1.3/tests/series/test_numeric_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/series/test_series.py` & `getdaft-0.1.3/tests/series/test_series.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/series/test_size_bytes.py` & `getdaft-0.1.3/tests/series/test_size_bytes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/series/test_slice.py` & `getdaft-0.1.3/tests/series/test_slice.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/series/test_sort.py` & `getdaft-0.1.3/tests/series/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/series/test_take.py` & `getdaft-0.1.3/tests/series/test_take.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/series/test_temporal_ops.py` & `getdaft-0.1.3/tests/series/test_temporal_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/series/test_utf8_ops.py` & `getdaft-0.1.3/tests/series/test_utf8_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/table/__init__.py` & `getdaft-0.1.3/tests/table/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/table/test_blackbox_kernels.py` & `getdaft-0.1.3/tests/table/test_blackbox_kernels.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/table/test_concat.py` & `getdaft-0.1.3/tests/table/test_concat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/table/test_eval.py` & `getdaft-0.1.3/tests/table/test_eval.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/table/test_explodes.py` & `getdaft-0.1.3/tests/table/test_explodes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/table/test_filter.py` & `getdaft-0.1.3/tests/table/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/table/test_from_py.py` & `getdaft-0.1.3/tests/table/test_from_py.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/table/test_head.py` & `getdaft-0.1.3/tests/table/test_head.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/table/test_joins.py` & `getdaft-0.1.3/tests/table/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/table/test_partitioning.py` & `getdaft-0.1.3/tests/table/test_partitioning.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/table/test_size_bytes.py` & `getdaft-0.1.3/tests/table/test_size_bytes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/table/test_sorting.py` & `getdaft-0.1.3/tests/table/test_sorting.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/table/test_table_aggs.py` & `getdaft-0.1.3/tests/table/test_table_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/table/test_table_io.py` & `getdaft-0.1.3/tests/table/test_table_io.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/table/test_take.py` & `getdaft-0.1.3/tests/table/test_take.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/table/utf8/test_compares.py` & `getdaft-0.1.3/tests/table/utf8/test_compares.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/test_analytics.py` & `getdaft-0.1.3/tests/test_analytics.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/test_datatypes.py` & `getdaft-0.1.3/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/test_schema.py` & `getdaft-0.1.3/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests/udf_library/test_url_udfs.py` & `getdaft-0.1.3/tests/udf_library/test_url_udfs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tests_legacy/test_resource_requests.py` & `getdaft-0.1.3/tests_legacy/test_resource_requests.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tools/patch_package_version.py` & `getdaft-0.1.3/tools/patch_package_version.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tools/wheels/_vendor/wheel/LICENSE.txt` & `getdaft-0.1.3/tools/wheels/_vendor/wheel/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tools/wheels/_vendor/wheel/cli/__init__.py` & `getdaft-0.1.3/tools/wheels/_vendor/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tools/wheels/_vendor/wheel/cli/convert.py` & `getdaft-0.1.3/tools/wheels/_vendor/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tools/wheels/_vendor/wheel/cli/pack.py` & `getdaft-0.1.3/tools/wheels/_vendor/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tools/wheels/_vendor/wheel/cli/unpack.py` & `getdaft-0.1.3/tools/wheels/_vendor/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tools/wheels/_vendor/wheel/pkginfo.py` & `getdaft-0.1.3/tools/wheels/_vendor/wheel/pkginfo.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tools/wheels/_vendor/wheel/util.py` & `getdaft-0.1.3/tools/wheels/_vendor/wheel/util.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tools/wheels/_vendor/wheel/wheelfile.py` & `getdaft-0.1.3/tools/wheels/_vendor/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tools/wheels/fix-and-copy-wheel.py` & `getdaft-0.1.3/tools/wheels/fix-and-copy-wheel.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tools/wheels/tmpdirs.py` & `getdaft-0.1.3/tools/wheels/tmpdirs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tools/wheels/tools.py` & `getdaft-0.1.3/tools/wheels/tools.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tools/wheels/wheeltools.py` & `getdaft-0.1.3/tools/wheels/wheeltools.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb` & `getdaft-0.1.3/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tutorials/image_querying/top_n_red_color.ipynb` & `getdaft-0.1.3/tutorials/image_querying/top_n_red_color.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tutorials/mnist.ipynb` & `getdaft-0.1.3/tutorials/mnist.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tutorials/text_to_image/text_to_image_generation.ipynb` & `getdaft-0.1.3/tutorials/text_to_image/text_to_image_generation.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/tutorials/text_to_image/using_cloud_with_ray.ipynb` & `getdaft-0.1.3/tutorials/text_to_image/using_cloud_with_ray.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.2/Cargo.lock` & `getdaft-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "daft"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "arrow2",
  "bincode",
  "dyn-clone",
  "fnv",
  "indexmap",
  "lazy_static",
```

### Comparing `getdaft-0.1.2/PKG-INFO` & `getdaft-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: getdaft
-Version: 0.1.2
+Version: 0.1.3
 Requires-Dist: pyarrow >= 6.0.1
 Requires-Dist: fsspec[http]
 Requires-Dist: loguru
 Requires-Dist: tabulate >= 0.9.0
 Requires-Dist: psutil
 Requires-Dist: typing-extensions >= 4.0.0; python_version < '3.8'
 Requires-Dist: pickle5 >= 0.0.12; python_version < '3.8'
-Requires-Dist: numpy; extra == 'numpy'
 Requires-Dist: ray[data, default]>=2.0.0; extra == 'ray'
 Requires-Dist: packaging; extra == 'ray'
-Requires-Dist: pandas; extra == 'pandas'
 Requires-Dist: getdaft[aws, ray, pandas, numpy, viz]; extra == 'all'
 Requires-Dist: pydot; extra == 'viz'
+Requires-Dist: numpy; extra == 'numpy'
+Requires-Dist: pandas; extra == 'pandas'
 Requires-Dist: s3fs; extra == 'aws'
-Provides-Extra: numpy
 Provides-Extra: ray
-Provides-Extra: pandas
 Provides-Extra: all
 Provides-Extra: viz
+Provides-Extra: numpy
+Provides-Extra: pandas
 Provides-Extra: aws
 License-File: LICENSE
 Summary: A Distributed DataFrame library for large scale complex data processing.
 Author-email: Eventual Inc <daft@eventualcomputing.com>
 Maintainer-email: Sammy Sidhu <sammy@eventualcomputing.com>, Jay Chia <jay@eventualcomputing.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
-Project-URL: repository, https://github.com/Eventual-Inc/Daft
 Project-URL: homepage, https://www.getdaft.io
+Project-URL: repository, https://github.com/Eventual-Inc/Daft
 
 |Banner|
 
 |CI| |PyPI| |Latest Tag| |Coverage| |Slack|
 
 `Website <https://www.getdaft.io>`_ • `Docs <https://www.getdaft.io/projects/docs/>`_ • `Installation`_ • `10-minute tour of Daft <https://www.getdaft.io/projects/docs/en/latest/learn/10-min.html>`_ • `Community and Support <https://github.com/Eventual-Inc/Daft/discussions>`_
```

