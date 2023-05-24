# Comparing `tmp/ydata-profiling-4.1.2.tar.gz` & `tmp/ydata-profiling-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydata-profiling-4.1.2.tar", last modified: Tue Mar 28 08:05:03 2023, max compression
+gzip compressed data, was "ydata-profiling-4.2.0.tar", last modified: Wed May 24 08:07:13 2023, max compression
```

## Comparing `ydata-profiling-4.1.2.tar` & `ydata-profiling-4.2.0.tar`

### file list

```diff
@@ -1,259 +1,263 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.083026 ydata-profiling-4.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)     6240 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1133 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1206 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)    21245 2023-03-28 08:05:03.079025 ydata-profiling-4.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17965 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      978 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/requirements-spark.txt
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (122)      490 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-28 08:05:03.083026 ydata-profiling-4.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2565 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.047024 ydata-profiling-4.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.051024 ydata-profiling-4.1.2/src/pandas_profiling/
--rw-r--r--   0 runner    (1001) docker     (122)      790 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/pandas_profiling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.051024 ydata-profiling-4.1.2/src/ydata_profiling/
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12839 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/compare_reports.py
--rw-r--r--   0 runner    (1001) docker     (122)    12320 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     4479 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/config_default.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     4394 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/config_minimal.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.055024 ydata-profiling-4.1.2/src/ydata_profiling/controller/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3192 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/controller/console.py
--rw-r--r--   0 runner    (1001) docker     (122)      511 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/controller/pandas_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     4487 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/expectations_report.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.055024 ydata-profiling-4.1.2/src/ydata_profiling/model/
--rw-r--r--   0 runner    (1001) docker     (122)      114 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10891 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)     4142 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/correlations.py
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (122)     6467 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/describe.py
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (122)     3226 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/expectation_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (122)     2344 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     3520 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/missing.py
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pairwise.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.059024 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6743 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/correlations_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/dataframe_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)      985 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_boolean_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)     9285 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_categorical_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)     1844 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_counts_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_date_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)     1496 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_file_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)      968 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_generic_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)     5830 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_image_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)     5221 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_numeric_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_path_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_supported_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)     5139 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_timeseries_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_url_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)     2635 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/discretize_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)     1899 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/duplicates_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)     1762 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/imbalance_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)     1401 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/missing_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/sample_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/summary_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)     1703 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/table_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/utils_pandas.py
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.059024 ydata-profiling-4.1.2/src/ydata_profiling/model/spark/
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5141 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/spark/correlations_spark.py
--rw-r--r--   0 runner    (1001) docker     (122)     1777 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/spark/dataframe_spark.py
--rw-r--r--   0 runner    (1001) docker     (122)      788 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/spark/describe_boolean_spark.py
--rw-r--r--   0 runner    (1001) docker     (122)      777 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/spark/describe_categorical_spark.py
--rw-r--r--   0 runner    (1001) docker     (122)     1790 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/spark/describe_counts_spark.py
--rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/spark/describe_date_spark.py
--rw-r--r--   0 runner    (1001) docker     (122)      916 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/spark/describe_generic_spark.py
--rw-r--r--   0 runner    (1001) docker     (122)     4582 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/spark/describe_numeric_spark.py
--rw-r--r--   0 runner    (1001) docker     (122)     1046 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/spark/describe_supported_spark.py
--rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/spark/duplicates_spark.py
--rw-r--r--   0 runner    (1001) docker     (122)     3680 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/spark/missing_spark.py
--rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/spark/sample_spark.py
--rw-r--r--   0 runner    (1001) docker     (122)     3282 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/spark/summary_spark.py
--rw-r--r--   0 runner    (1001) docker     (122)     1858 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/spark/table_spark.py
--rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/summarizer.py
--rw-r--r--   0 runner    (1001) docker     (122)      648 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/summary.py
--rw-r--r--   0 runner    (1001) docker     (122)     4717 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/summary_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (122)      230 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/table.py
--rw-r--r--   0 runner    (1001) docker     (122)     8839 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/typeset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2889 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/model/typeset_relations.py
--rw-r--r--   0 runner    (1001) docker     (122)    19160 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/profile_report.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.059024 ydata-profiling-4.1.2/src/ydata_profiling/report/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9093 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/formatters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.059024 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.063025 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/
--rw-r--r--   0 runner    (1001) docker     (122)     1473 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      551 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)      843 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/collapse.py
--rw-r--r--   0 runner    (1001) docker     (122)     1372 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/container.py
--rw-r--r--   0 runner    (1001) docker     (122)      545 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/correlation_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (122)      420 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/frequency_table.py
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/frequency_table_small.py
--rw-r--r--   0 runner    (1001) docker     (122)      362 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/html.py
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/image.py
--rw-r--r--   0 runner    (1001) docker     (122)      460 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/item_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/renderable.py
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/root.py
--rw-r--r--   0 runner    (1001) docker     (122)      517 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/sample.py
--rw-r--r--   0 runner    (1001) docker     (122)      648 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/table.py
--rw-r--r--   0 runner    (1001) docker     (122)      381 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/toggle_button.py
--rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/variable.py
--rw-r--r--   0 runner    (1001) docker     (122)      906 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/variable_info.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.063025 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3964 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/flavours.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.067025 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/
--rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      921 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/collapse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2040 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/container.py
--rw-r--r--   0 runner    (1001) docker     (122)      582 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/correlation_table.py
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (122)      726 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/frequency_table.py
--rw-r--r--   0 runner    (1001) docker     (122)      525 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/frequency_table_small.py
--rw-r--r--   0 runner    (1001) docker     (122)      147 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/html.py
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/image.py
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/root.py
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/sample.py
--rw-r--r--   0 runner    (1001) docker     (122)      263 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/table.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.067025 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.071025 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_constant.html
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_constant_length.html
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_duplicates.html
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_empty.html
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_high_cardinality.html
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_high_correlation.html
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_imbalance.html
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_infinite.html
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_missing.html
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_non_stationary.html
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_seasonal.html
--rw-r--r--   0 runner    (1001) docker     (122)      151 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_skewed.html
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_truncated.html
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_type_date.html
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_uniform.html
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_unique.html
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_unsupported.html
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_zeros.html
--rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts.html
--rw-r--r--   0 runner    (1001) docker     (122)      371 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/collapse.html
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/correlation_table.html
--rw-r--r--   0 runner    (1001) docker     (122)      353 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/diagram.html
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/duplicate.html
--rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table.html
--rw-r--r--   0 runner    (1001) docker     (122)     1328 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table_small.html
--rw-r--r--   0 runner    (1001) docker     (122)      961 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/report.html
--rw-r--r--   0 runner    (1001) docker     (122)      205 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/sample.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.071025 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/
--rw-r--r--   0 runner    (1001) docker     (122)      769 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/batch_grid.html
--rw-r--r--   0 runner    (1001) docker     (122)      712 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/grid.html
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/list.html
--rw-r--r--   0 runner    (1001) docker     (122)      213 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/named_list.html
--rw-r--r--   0 runner    (1001) docker     (122)      533 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/sections.html
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/select.html
--rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/tabs.html
--rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/table.html
--rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/toggle_button.html
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/variable.html
--rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/variable_info.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.071025 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.075025 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/
--rw-r--r--   0 runner    (1001) docker     (122)    23409 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (122)   121200 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (122)    37045 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (122)   125618 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/cosmo.bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (122)   127321 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/flatly.bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (122)    97163 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/jquery-1.12.4.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      941 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/script.js
--rw-r--r--   0 runner    (1001) docker     (122)   127551 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/simplex.bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (122)     5946 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/style.css
--rw-r--r--   0 runner    (1001) docker     (122)   122851 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/united.bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (122)      201 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/footer.html
--rw-r--r--   0 runner    (1001) docker     (122)      896 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/javascript.html
--rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/navigation.html
--rw-r--r--   0 runner    (1001) docker     (122)     3227 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/style.html
--rw-r--r--   0 runner    (1001) docker     (122)     2377 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates.py
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/toggle_button.py
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/variable.py
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/variable_info.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.075025 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/
--rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1299 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/collapse.py
--rw-r--r--   0 runner    (1001) docker     (122)     3797 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/container.py
--rw-r--r--   0 runner    (1001) docker     (122)      460 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/correlation_table.py
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/frequency_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/frequency_table_small.py
--rw-r--r--   0 runner    (1001) docker     (122)      313 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/html.py
--rw-r--r--   0 runner    (1001) docker     (122)      898 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     2253 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/notebook.py
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/root.py
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/sample.py
--rw-r--r--   0 runner    (1001) docker     (122)      961 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/table.py
--rw-r--r--   0 runner    (1001) docker     (122)      548 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/toggle_button.py
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/variable.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/variable_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     3960 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/frequency_table_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.075025 ydata-profiling-4.1.2/src/ydata_profiling/report/structure/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3972 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/structure/correlations.py
--rw-r--r--   0 runner    (1001) docker     (122)     8837 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/structure/overview.py
--rw-r--r--   0 runner    (1001) docker     (122)    14857 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/structure/report.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.079025 ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/
--rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4375 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_boolean.py
--rw-r--r--   0 runner    (1001) docker     (122)    17888 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_categorical.py
--rw-r--r--   0 runner    (1001) docker     (122)      965 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2798 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_complex.py
--rw-r--r--   0 runner    (1001) docker     (122)     4391 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_count.py
--rw-r--r--   0 runner    (1001) docker     (122)     3452 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_date.py
--rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_file.py
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_generic.py
--rw-r--r--   0 runner    (1001) docker     (122)     6950 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_image.py
--rw-r--r--   0 runner    (1001) docker     (122)     4466 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_path.py
--rw-r--r--   0 runner    (1001) docker     (122)     9487 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_real.py
--rw-r--r--   0 runner    (1001) docker     (122)     9246 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (122)     4029 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4626 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/serialize_report.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.079025 ydata-profiling-4.1.2/src/ydata_profiling/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/utils/compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     8401 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/utils/imghdr_patch.py
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/utils/notebook.py
--rw-r--r--   0 runner    (1001) docker     (122)      972 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (122)      334 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/utils/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-03-28 08:05:02.000000 ydata-profiling-4.1.2/src/ydata_profiling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.079025 ydata-profiling-4.1.2/src/ydata_profiling/visualisation/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2803 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/visualisation/context.py
--rw-r--r--   0 runner    (1001) docker     (122)     3793 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/visualisation/missing.py
--rw-r--r--   0 runner    (1001) docker     (122)    28957 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/visualisation/plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     3206 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/src/ydata_profiling/visualisation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.051024 ydata-profiling-4.1.2/src/ydata_profiling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    21245 2023-03-28 08:05:02.000000 ydata-profiling-4.1.2/src/ydata_profiling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13947 2023-03-28 08:05:02.000000 ydata-profiling-4.1.2/src/ydata_profiling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-28 08:05:02.000000 ydata-profiling-4.1.2/src/ydata_profiling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-03-28 08:05:02.000000 ydata-profiling-4.1.2/src/ydata_profiling.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      478 2023-03-28 08:05:02.000000 ydata-profiling-4.1.2/src/ydata_profiling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-03-28 08:05:02.000000 ydata-profiling-4.1.2/src/ydata_profiling.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 08:05:03.079025 ydata-profiling-4.1.2/venv/
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-03-28 08:02:05.000000 ydata-profiling-4.1.2/venv/spark.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.900820 ydata-profiling-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    20736 2023-05-24 08:07:13.900820 ydata-profiling-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17440 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/requirements-spark.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 08:07:13.900820 ydata-profiling-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.852819 ydata-profiling-4.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.856819 ydata-profiling-4.2.0/src/pandas_profiling/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/pandas_profiling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.860819 ydata-profiling-4.2.0/src/ydata_profiling/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/compare_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/config_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/config_minimal.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.860819 ydata-profiling-4.2.0/src/ydata_profiling/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/controller/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/controller/pandas_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/expectations_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.864819 ydata-profiling-4.2.0/src/ydata_profiling/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20409 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/correlations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/describe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/expectation_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pairwise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.868819 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/correlations_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/dataframe_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_boolean_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_categorical_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_counts_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_date_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_file_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_generic_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_image_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_numeric_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_path_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_supported_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_text_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_timeseries_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_url_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/discretize_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/duplicates_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/imbalance_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/missing_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/sample_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/summary_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/table_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/utils_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.868819 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/correlations_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/dataframe_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_boolean_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_categorical_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_counts_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_date_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_generic_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_numeric_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_supported_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_text_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/duplicates_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/missing_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/sample_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/summary_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/spark/table_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/summary_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11164 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/typeset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/model/typeset_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19411 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/profile_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.868819 ydata-profiling-4.2.0/src/ydata_profiling/report/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/formatters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.868819 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.872819 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/correlation_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/frequency_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/frequency_table_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/item_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/renderable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/toggle_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/variable_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.872819 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/flavours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.876819 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/correlation_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/frequency_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/frequency_table_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.876819 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.884820 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_constant.html
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_constant_length.html
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_duplicates.html
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_empty.html
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_high_cardinality.html
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_high_correlation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_imbalance.html
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_infinite.html
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_missing.html
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_non_stationary.html
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_seasonal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_skewed.html
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_truncated.html
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_type_date.html
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_uniform.html
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_unique.html
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_unsupported.html
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_zeros.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/collapse.html
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/correlation_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/diagram.html
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/duplicate.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table_small.html
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sample.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.884820 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/batch_grid.html
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/grid.html
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/named_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/sections.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/tabs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/table.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/toggle_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/variable.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/variable_info.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.884820 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.888820 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    23409 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   121200 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    37045 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   125618 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/cosmo.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   127321 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/flatly.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    97163 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/jquery-1.12.4.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/script.js
+-rw-r--r--   0 runner    (1001) docker     (123)   127551 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/simplex.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)   122851 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/united.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/javascript.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/style.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/toggle_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/variable_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.888820 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/correlation_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/frequency_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/frequency_table_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/toggle_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/variable_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/frequency_table_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.892820 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/correlations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14934 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.892820 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/serialize_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.896820 ydata-profiling-4.2.0/src/ydata_profiling/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/utils/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/utils/imghdr_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/utils/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/utils/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 08:07:13.000000 ydata-profiling-4.2.0/src/ydata_profiling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.896820 ydata-profiling-4.2.0/src/ydata_profiling/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/visualisation/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/visualisation/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29573 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/visualisation/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/src/ydata_profiling/visualisation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.860819 ydata-profiling-4.2.0/src/ydata_profiling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20736 2023-05-24 08:07:13.000000 ydata-profiling-4.2.0/src/ydata_profiling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14162 2023-05-24 08:07:13.000000 ydata-profiling-4.2.0/src/ydata_profiling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 08:07:13.000000 ydata-profiling-4.2.0/src/ydata_profiling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-24 08:07:13.000000 ydata-profiling-4.2.0/src/ydata_profiling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-24 08:07:13.000000 ydata-profiling-4.2.0/src/ydata_profiling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 08:07:13.000000 ydata-profiling-4.2.0/src/ydata_profiling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:07:13.896820 ydata-profiling-4.2.0/venv/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-24 08:04:09.000000 ydata-profiling-4.2.0/venv/spark.yml
```

### Comparing `ydata-profiling-4.1.2/CONTRIBUTING.md` & `ydata-profiling-4.2.0/CONTRIBUTING.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-## How to contribute to Pandas-Profiling
+## How to contribute to YData-Profiling
 
-Pandas-profiling aims to ease exploratory data analysis for structured datasets, including time-series. 
+YData-profiling aims to ease exploratory data analysis for structured datasets, including time-series. 
 Our focus is to provide users with useful and robust statistics for such datasets encountered in industry, academia and elsewhere.
-Pandas-profiling is open-source and stimulates contributions from passionate community users.
+YData-profiling is open-source and stimulates contributions from passionate community users.
 
 
 #### Themes to contribute
 In line with our aim, we identify the following themes:
 
 - **Exploratory data analysis**: 
   The core of the package is a dataset summarization by its main characteristics, which is complemented with warnings on data issues and visualisations.
 
   _Suggestions for contribution_: 
   Extend the support of more data types (think of paths, location or GPS coordinates and ordinal data types),
   text data (e.g. encoding, vocabulary size, spelling errors, language detection), 
   time series analysis, 
   or even images (e.g. dimensions, EXIF).
   
-  _Related_: [#7][i7], [#129][i129], [#190][i190], [#204][i204] or [create one](https://github.com/ydataai/pandas-profiling/issues/new/choose).
+  _Related_: [#7][i7], [#129][i129], [#190][i190], [#204][i204] or [create one](https://github.com/ydataai/ydata-profiling/issues/new/choose).
 
 - **Stability, Performance and Restricted environment compatibility:** 
   Data exploration takes place in all kinds of conditions, on the latest machine learning platforms with enormous dataset to managed environments in large corporations.
-  `pandas-profiling` helps analysts, researchers and engineers alike in these cases.
+  `ydata-profiling` helps analysts, researchers and engineers alike in these cases.
   We do this by fixing bugs, improving performance on big datasets and adding environment compatibility.
   
   _Suggestions for contribution (Performance)_: 
-  Perform concurrency analysis or profile execution times and leverage the gained insights for improved performance (e.g. multiprocessing, cython, numba) or test the performance of `pandas-profiling` with [big data sets](https://www.stats.govt.nz/large-datasets/csv-files-for-download/) and corresponding commonly used data formats (such as parquet). 
+  Perform concurrency analysis or profile execution times and leverage the gained insights for improved performance (e.g. multiprocessing, cython, numba) or test the performance of `ydata-profiling` with [big data sets](https://www.stats.govt.nz/large-datasets/csv-files-for-download/) and corresponding commonly used data formats (such as parquet). 
   
   _Suggestions for contribution (Stability)_: 
-  Either review the code and add tests or watch the [issues page](https://github.com/ydataai/pandas-profiling/issues) and [Stackoverflow tag](https://stackoverflow.com/questions/tagged/pandas-profiling) to find current issues.
+  Either review the code and add tests or watch the [issues page](https://github.com/ydataai/ydata-profiling/issues) and [Stackoverflow tag](https://stackoverflow.com/questions/tagged/ydata-profiling) to find current issues.
      
-  _Related_: [#98][i98], [#122][i122] or [create one](https://github.com/ydataai/pandas-profiling/issues/new/choose).
+  _Related_: [#98][i98], [#122][i122] or [create one](https://github.com/ydataai/ydata-profiling/issues/new/choose).
 
 - **Interaction, presentation and user experience**: 
-  As `pandas-profiling` eases exploratory data analysis, working with the package should reflect that.
+  As `ydata-profiling` eases exploratory data analysis, working with the package should reflect that.
   Interaction and user experience plays a central role in working with the package.
   Working on interactive and static features is possible through the modular nature of the package: the user can configure which features to use.
 
   _Suggestions for contribution (interactivity)_:
   Interactivity allows for more user friendly applications, including but not limited to on demand analysis (don't compute what you don't want to see) and interactive histograms and correlations. 
   This is ideal for smaller datasets, where we can compute this on-the-fly. 
   `ipywidgets` would be a great place to start (e.g. [widget based view](https://ipywidgets.readthedocs.io/en/stable/examples/Widget%20List.html)).
 
   _Suggestions for contribution (presentation)_:
   Other forms of distribution than HTML (for example PDF or packaged as an GUI application via [PyQt](https://riverbankcomputing.com/software/pyqt/intro))
   Users should be able to share reports (improve size of labels in graph, add explanations to correlation matrices and allow for styling/branding).
 
-  _Related_: [#161][i161], [#175][i175], [#191][i191] or [create one](https://github.com/ydataai/pandas-profiling/issues/new/choose).
+  _Related_: [#161][i161], [#175][i175], [#191][i191] or [create one](https://github.com/ydataai/ydata-profiling/issues/new/choose).
 
 - **Community**: 
   The success of this package demonstrates the power of sharing and working together.
   You are welcome as part of this community.
   
   _Suggestions for contribution_:
   Share with us if this package is of value to you, let us know [in our community](https://discord.com/invite/mw7xjJ7b7s).
-  We are interested in how you use `pandas-profiling` in your work.
+  We are interested in how you use `ydata-profiling` in your work.
   
-  _Related_: [#87][i87] or [create one](https://github.com/ydataai/pandas-profiling/issues/new/choose).
+  _Related_: [#87][i87] or [create one](https://github.com/ydataai/ydata-profiling/issues/new/choose).
 
 - **Machine learning:** 
-  `pandas-profiling` is not a machine learning package, even though many of our users use EDA as a step prior to developing their models.
+  `ydata-profiling` is not a machine learning package, even though many of our users use EDA as a step prior to developing their models.
   Our focus lies in the exploratory data analysis.
   Any functionality that enables machine learning applications by more effective data profiling, is welcome.
 
-  _Related_: [#124][i124], [#173][i173], [#198][i198] or [create one](https://github.com/ydataai/pandas-profiling/issues/new/choose).
+  _Related_: [#124][i124], [#173][i173], [#198][i198] or [create one](https://github.com/ydataai/ydata-profiling/issues/new/choose).
 
 #### **Did you find a bug?**
 
-* **Ensure the bug was not already reported** by searching on Github under [Issues](https://github.com/ydataai/pandas-profiling/issues).
+* **Ensure the bug was not already reported** by searching on Github under [Issues](https://github.com/ydataai/ydata-profiling/issues).
 
-* If you're unable to find an open issue addressing the problem, [open a new one](https://github.com/ydataai/pandas-profiling/issues/new/choose). 
+* If you're unable to find an open issue addressing the problem, [open a new one](https://github.com/ydataai/ydata-profiling/issues/new/choose). 
 If possible, use the relevant bug report templates to create the issue. 
 
 #### **Did you write a patch that fixes a bug?**
 
 * Open a new Github pull request with the patch.
 
 * Ensure the PR description clearly describes the problem and solution. 
 Include the relevant issue number if applicable.
 
 
 #### Acknowledgements
 
 We would like to thank everyone who has helped getting us to where we are now.
 
-See the [Contributor Graph](https://github.com/ydataai/pandas-profiling/graphs/contributors)
+See the [Contributor Graph](https://github.com/ydataai/ydata-profiling/graphs/contributors)
 
-[i7]: https://github.com/ydataai/pandas-profiling/issues/7
-[i129]: https://github.com/ydataai/pandas-profiling/issues/129
-[i190]: https://github.com/ydataai/pandas-profiling/issues/190
-[i204]: https://github.com/ydataai/pandas-profiling/issues/204
-[i98]: https://github.com/ydataai/pandas-profiling/issues/98
-[i122]: https://github.com/ydataai/pandas-profiling/issues/122
-[i124]: https://github.com/ydataai/pandas-profiling/issues/24
-[i173]: https://github.com/ydataai/pandas-profiling/issues/173
-[i198]: https://github.com/ydataai/pandas-profiling/issues/198
-[i87]: https://github.com/ydataai/pandas-profiling/issues/87
-[i161]: https://github.com/ydataai/pandas-profiling/issues/161
-[i175]: https://github.com/ydataai/pandas-profiling/issues/175
-[i191]: https://github.com/ydataai/pandas-profiling/issues/191
+[i7]: https://github.com/ydataai/ydata-profiling/issues/7
+[i129]: https://github.com/ydataai/ydata-profiling/issues/129
+[i190]: https://github.com/ydataai/ydata-profiling/issues/190
+[i204]: https://github.com/ydataai/ydata-profiling/issues/204
+[i98]: https://github.com/ydataai/ydata-profiling/issues/98
+[i122]: https://github.com/ydataai/ydata-profiling/issues/122
+[i124]: https://github.com/ydataai/ydata-profiling/issues/24
+[i173]: https://github.com/ydataai/ydata-profiling/issues/173
+[i198]: https://github.com/ydataai/ydata-profiling/issues/198
+[i87]: https://github.com/ydataai/ydata-profiling/issues/87
+[i161]: https://github.com/ydataai/ydata-profiling/issues/161
+[i175]: https://github.com/ydataai/ydata-profiling/issues/175
+[i191]: https://github.com/ydataai/ydata-profiling/issues/191
```

### Comparing `ydata-profiling-4.1.2/LICENSE` & `ydata-profiling-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/MANIFEST.in` & `ydata-profiling-4.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/Makefile` & `ydata-profiling-4.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/PKG-INFO` & `ydata-profiling-4.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydata-profiling
-Version: 4.1.2
+Version: 4.2.0
 Summary: Generate profile report for pandas DataFrame
 Home-page: https://github.com/ydataai/ydata-profiling
 Author: YData Labs Inc
 Author-email: opensource@ydata.ai
 License: MIT
 Description: # ydata-profiling
         
@@ -31,24 +31,44 @@
         
         <p align="center">
           Do you like this project? Show us your love and <a href="https://engage.ydata.ai">give feedback!</a>
         </p>
         
         `ydata-profiling` primary goal is to provide a one-line Exploratory Data Analysis (EDA) experience in a consistent and fast solution. Like pandas `df.describe()` function, that is so handy, ydata-profiling delivers an extended analysis of a DataFrame while allowing the data analysis to be exported in different formats such as **html** and **json**.
         
-        The package outputs a simple and digested analysis of a dataset, including **time-series** and **text**. 
+        The package outputs a simple and digested analysis of a dataset, including **time-series** and **text**.
         
-        ### 🎊 New year, new face, more functionalities! 
         
-        Thank you for using and following ``pandas-profiling`` developments. Yet, we have a new exciting feature - we are now thrilled to announce
-        that <u>Spark</u> is now part of the Data Profiling family from version 4.0.0 onwards
-         
-        With its introduction, there was also the need for a new naming, one that will allow to decouple the concept of profiling from the Pandas Dataframes - `ydata-profiling`! 
-         
-        But fear not, `pip install pandas-profiling` will still be a valid for a while, and we will keep investing in growing the best open-source for data profiling, so you can use it for even more use cases.
+        ## ▶️ Quickstart
+        
+        ### Install
+        ```cmd
+        pip install ydata-profiling
+        ```
+        or
+        ```cmd
+        conda install -c conda-forge ydata-profiling
+        ```
+        ### Start profiling
+        
+        Start by loading your pandas `DataFrame` as you normally would, e.g. by using:
+        
+        ```python
+        import numpy as np
+        import pandas as pd
+        from ydata_profiling import ProfileReport
+        
+        df = pd.DataFrame(np.random.rand(100, 5), columns=["a", "b", "c", "d", "e"])
+        ```
+        
+        To generate the standard profiling report, merely run:
+        
+        ```python
+        profile = ProfileReport(df, title="Profiling Report")
+        ```
         
         ## Key features
         
         - **Type inference**: automatic detection of columns' data types (*Categorical*, *Numerical*, *Date*, etc.)
         - **Warnings**: A summary of the problems/challenges in the data that you might need to work on (*missing data*, *inaccuracies*, *skewness*, etc.)
         - **Univariate analysis**: including descriptive statistics (mean, median, mode, etc) and informative visualizations such as distribution histograms
         - **Multivariate analysis**: including correlations, a detailed analysis of missing data, duplicate rows, and visual support for variables pairwise interaction
@@ -83,32 +103,14 @@
         | [Comparing datasets](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/comparing_datasets.html )                        | Comparing multiple version of the same dataset                                              |
         | [Profiling a Time-Series dataset](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/time_series_datasets.html)               | Generating a report for a time-series dataset with a single line of code                    |
         |[Profiling large datasets](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/big_data.html )                            | Tips on how to prepare data and configure `ydata-profiling` for working with large datasets |
         | [Handling sensitive data](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/sensitive_data.html )                       | Generating reports which are mindful about sensitive data in the input dataset              |
         | [Dataset metadata and data dictionaries](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/metadata.html)               | Complementing the report with dataset details and column-specific data dictionaries         |
         | [Customizing the report's appearance](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/custom_report_appearance.html ) | Changing the appearance of the report's page and of the contained visualizations            |
         
-        ## ▶️ Quickstart
-        
-        Start by loading your pandas `DataFrame` as you normally would, e.g. by using:
-        
-        ```python
-        import numpy as np
-        import pandas as pd
-        from ydata_profiling import ProfileReport
-        
-        df = pd.DataFrame(np.random.rand(100, 5), columns=["a", "b", "c", "d", "e"])
-        ```
-        
-        To generate the standard profiling report, merely run:
-        
-        ```python
-        profile = ProfileReport(df, title="Profiling Report")
-        ```
-        
         ### Using inside Jupyter Notebooks
         
         There are two interfaces to consume the report inside a Jupyter notebook: through widgets and through an embedded HTML report.
         
         <img alt="Notebook Widgets" src="https://ydata-profiling.ydata.ai/docs/master/assets/widgets.gif" width="800" />
         
         The above is achieved by simply displaying the report as a set of widgets. In a Jupyter Notebook, run:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ydata-profiling Version: 4.1.2 Summary: Generate
+Metadata-Version: 2.1 Name: ydata-profiling Version: 4.2.0 Summary: Generate
 profile report for pandas DataFrame Home-page: https://github.com/ydataai/
 ydata-profiling Author: YData Labs Inc Author-email: opensource@ydata.ai
 License: MIT Description: # ydata-profiling [![Build Status](https://
 github.com/ydataai/pandas-profiling/actions/workflows/tests.yml/
 badge.svg?branch=master)](https://github.com/ydataai/pandas-profiling/actions/
 workflows/tests.yml) [![PyPI download month](https://img.shields.io/pypi/dm/
 ydata-profiling.svg)](https://pypi.python.org/pypi/ydata-profiling/) [![]
@@ -20,86 +20,79 @@
         Do you like this project? Show us your love and give_feedback!
 `ydata-profiling` primary goal is to provide a one-line Exploratory Data
 Analysis (EDA) experience in a consistent and fast solution. Like pandas
 `df.describe()` function, that is so handy, ydata-profiling delivers an
 extended analysis of a DataFrame while allowing the data analysis to be
 exported in different formats such as **html** and **json**. The package
 outputs a simple and digested analysis of a dataset, including **time-series**
-and **text**. ### ð New year, new face, more functionalities! Thank you for
-using and following ``pandas-profiling`` developments. Yet, we have a new
-exciting feature - we are now thrilled to announce that Spark is now part of
-the Data Profiling family from version 4.0.0 onwards With its introduction,
-there was also the need for a new naming, one that will allow to decouple the
-concept of profiling from the Pandas Dataframes - `ydata-profiling`! But fear
-not, `pip install pandas-profiling` will still be a valid for a while, and we
-will keep investing in growing the best open-source for data profiling, so you
-can use it for even more use cases. ## Key features - **Type inference**:
-automatic detection of columns' data types (*Categorical*, *Numerical*, *Date*,
-etc.) - **Warnings**: A summary of the problems/challenges in the data that you
-might need to work on (*missing data*, *inaccuracies*, *skewness*, etc.) -
-**Univariate analysis**: including descriptive statistics (mean, median, mode,
-etc) and informative visualizations such as distribution histograms -
-**Multivariate analysis**: including correlations, a detailed analysis of
-missing data, duplicate rows, and visual support for variables pairwise
-interaction - **Time-Series**: including different statistical information
-relative to time dependent data such as auto-correlation and seasonality, along
-ACF and PACF plots. - **Text analysis**: most common categories (uppercase,
-lowercase, separator), scripts (Latin, Cyrillic) and blocks (ASCII, Cyrilic) -
-**File and Image analysis**: file sizes, creation dates, dimensions, indication
-of truncated images and existence of EXIF metadata - **Compare datasets**: one-
-line solution to enable a fast and complete report on the comparison of
-datasets - **Flexible output formats**: all analysis can be exported to an HTML
-report that can be easily shared with different parties, as JSON for an easy
-integration in automated systems and as a widget in a Jupyter Notebook. The
-report contains three additional sections: - **Overview**: mostly global
-details about the dataset (number of records, number of variables, overall
-missigness and duplicates, memory footprint) - **Alerts**: a comprehensive and
-automatic list of potential data quality issues (high correlation, skewness,
-uniformity, zeros, missing values, constant values, between others) -
-**Reproduction**: technical details about the analysis (time, version and
-configuration) ### ð Latest features - Want to scale? Check the latest
-release with â­â¡[Spark support](https://ydata-profiling.ydata.ai/docs/
-master/pages/integrations/pypspark.html)! - Looking for how you can do an EDA
-for Time-Series ð ? Check [this blogpost](https://towardsdatascience.com/
-how-to-do-an-eda-for-time-series-cbb92b3b1913). - You want to compare 2
-datasets and get a report? Check [this blogpost](https://medium.com/towards-
-artificial-intelligence/how-to-compare-2-dataset-with-pandas-profiling-
-2ae3a9d7695e) ### â¡ Spark Spark support has been released, but we are always
-looking for an extra pair of hands ð. [Check current work in progress!]
-(https://github.com/ydataai/ydata-profiling/projects/3). ## ð Use cases
-YData-profiling can be used to deliver a variety of different use-case. The
-documentation includes guides, tips and tricks for tackling them: | Use case |
-Description | |----------|-----------------------------------------------------
-----------------------------------------| | [Comparing datasets](https://ydata-
-profiling.ydata.ai/docs/master/pages/use_cases/comparing_datasets.html ) |
-Comparing multiple version of the same dataset | | [Profiling a Time-Series
-dataset](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/
-time_series_datasets.html) | Generating a report for a time-series dataset with
-a single line of code | |[Profiling large datasets](https://ydata-
-profiling.ydata.ai/docs/master/pages/use_cases/big_data.html ) | Tips on how to
-prepare data and configure `ydata-profiling` for working with large datasets |
-| [Handling sensitive data](https://ydata-profiling.ydata.ai/docs/master/pages/
-use_cases/sensitive_data.html ) | Generating reports which are mindful about
-sensitive data in the input dataset | | [Dataset metadata and data
-dictionaries](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/
-metadata.html) | Complementing the report with dataset details and column-
-specific data dictionaries | | [Customizing the report's appearance](https://
-ydata-profiling.ydata.ai/docs/master/pages/use_cases/
+and **text**. ## â¶ï¸ Quickstart ### Install ```cmd pip install ydata-
+profiling ``` or ```cmd conda install -c conda-forge ydata-profiling ``` ###
+Start profiling Start by loading your pandas `DataFrame` as you normally would,
+e.g. by using: ```python import numpy as np import pandas as pd from
+ydata_profiling import ProfileReport df = pd.DataFrame(np.random.rand(100, 5),
+columns=["a", "b", "c", "d", "e"]) ``` To generate the standard profiling
+report, merely run: ```python profile = ProfileReport(df, title="Profiling
+Report") ``` ## Key features - **Type inference**: automatic detection of
+columns' data types (*Categorical*, *Numerical*, *Date*, etc.) - **Warnings**:
+A summary of the problems/challenges in the data that you might need to work on
+(*missing data*, *inaccuracies*, *skewness*, etc.) - **Univariate analysis**:
+including descriptive statistics (mean, median, mode, etc) and informative
+visualizations such as distribution histograms - **Multivariate analysis**:
+including correlations, a detailed analysis of missing data, duplicate rows,
+and visual support for variables pairwise interaction - **Time-Series**:
+including different statistical information relative to time dependent data
+such as auto-correlation and seasonality, along ACF and PACF plots. - **Text
+analysis**: most common categories (uppercase, lowercase, separator), scripts
+(Latin, Cyrillic) and blocks (ASCII, Cyrilic) - **File and Image analysis**:
+file sizes, creation dates, dimensions, indication of truncated images and
+existence of EXIF metadata - **Compare datasets**: one-line solution to enable
+a fast and complete report on the comparison of datasets - **Flexible output
+formats**: all analysis can be exported to an HTML report that can be easily
+shared with different parties, as JSON for an easy integration in automated
+systems and as a widget in a Jupyter Notebook. The report contains three
+additional sections: - **Overview**: mostly global details about the dataset
+(number of records, number of variables, overall missigness and duplicates,
+memory footprint) - **Alerts**: a comprehensive and automatic list of potential
+data quality issues (high correlation, skewness, uniformity, zeros, missing
+values, constant values, between others) - **Reproduction**: technical details
+about the analysis (time, version and configuration) ### ð Latest features -
+Want to scale? Check the latest release with â­â¡[Spark support](https://
+ydata-profiling.ydata.ai/docs/master/pages/integrations/pypspark.html)! -
+Looking for how you can do an EDA for Time-Series ð ? Check [this blogpost]
+(https://towardsdatascience.com/how-to-do-an-eda-for-time-series-cbb92b3b1913).
+- You want to compare 2 datasets and get a report? Check [this blogpost](https:
+//medium.com/towards-artificial-intelligence/how-to-compare-2-dataset-with-
+pandas-profiling-2ae3a9d7695e) ### â¡ Spark Spark support has been released,
+but we are always looking for an extra pair of hands ð. [Check current work
+in progress!](https://github.com/ydataai/ydata-profiling/projects/3). ## ð
+Use cases YData-profiling can be used to deliver a variety of different use-
+case. The documentation includes guides, tips and tricks for tackling them: |
+Use case | Description | |----------|------------------------------------------
+---------------------------------------------------| | [Comparing datasets]
+(https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/
+comparing_datasets.html ) | Comparing multiple version of the same dataset | |
+[Profiling a Time-Series dataset](https://ydata-profiling.ydata.ai/docs/master/
+pages/use_cases/time_series_datasets.html) | Generating a report for a time-
+series dataset with a single line of code | |[Profiling large datasets](https:/
+/ydata-profiling.ydata.ai/docs/master/pages/use_cases/big_data.html ) | Tips on
+how to prepare data and configure `ydata-profiling` for working with large
+datasets | | [Handling sensitive data](https://ydata-profiling.ydata.ai/docs/
+master/pages/use_cases/sensitive_data.html ) | Generating reports which are
+mindful about sensitive data in the input dataset | | [Dataset metadata and
+data dictionaries](https://ydata-profiling.ydata.ai/docs/master/pages/
+use_cases/metadata.html) | Complementing the report with dataset details and
+column-specific data dictionaries | | [Customizing the report's appearance]
+(https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/
 custom_report_appearance.html ) | Changing the appearance of the report's page
-and of the contained visualizations | ## â¶ï¸ Quickstart Start by loading
-your pandas `DataFrame` as you normally would, e.g. by using: ```python import
-numpy as np import pandas as pd from ydata_profiling import ProfileReport df =
-pd.DataFrame(np.random.rand(100, 5), columns=["a", "b", "c", "d", "e"]) ``` To
-generate the standard profiling report, merely run: ```python profile =
-ProfileReport(df, title="Profiling Report") ``` ### Using inside Jupyter
-Notebooks There are two interfaces to consume the report inside a Jupyter
-notebook: through widgets and through an embedded HTML report. [Notebook
-Widgets] The above is achieved by simply displaying the report as a set of
-widgets. In a Jupyter Notebook, run: ```python profile.to_widgets() ``` The
-HTML report can be directly embedded in a cell in a similar fashion: ```python
+and of the contained visualizations | ### Using inside Jupyter Notebooks There
+are two interfaces to consume the report inside a Jupyter notebook: through
+widgets and through an embedded HTML report. [Notebook Widgets] The above is
+achieved by simply displaying the report as a set of widgets. In a Jupyter
+Notebook, run: ```python profile.to_widgets() ``` The HTML report can be
+directly embedded in a cell in a similar fashion: ```python
 profile.to_notebook_iframe() ``` [HTML] ### Exporting the report to a file To
 generate a HTML report file, save the `ProfileReport` to an object and use the
 `to_file()` function: ```python profile.to_file("your_report.html") ```
 Alternatively, the report's data can be obtained as a JSON file: ```python # As
 a JSON string json_data = profile.to_json() # As a file profile.to_file
 ("your_report.json") ``` ### Using in the command line For standard formatted
 CSV files (which can be read directly by pandas without additional settings),
```

### Comparing `ydata-profiling-4.1.2/README.md` & `ydata-profiling-4.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,24 +23,44 @@
 
 <p align="center">
   Do you like this project? Show us your love and <a href="https://engage.ydata.ai">give feedback!</a>
 </p>
 
 `ydata-profiling` primary goal is to provide a one-line Exploratory Data Analysis (EDA) experience in a consistent and fast solution. Like pandas `df.describe()` function, that is so handy, ydata-profiling delivers an extended analysis of a DataFrame while allowing the data analysis to be exported in different formats such as **html** and **json**.
 
-The package outputs a simple and digested analysis of a dataset, including **time-series** and **text**. 
+The package outputs a simple and digested analysis of a dataset, including **time-series** and **text**.
 
-### 🎊 New year, new face, more functionalities! 
 
-Thank you for using and following ``pandas-profiling`` developments. Yet, we have a new exciting feature - we are now thrilled to announce
-that <u>Spark</u> is now part of the Data Profiling family from version 4.0.0 onwards
- 
-With its introduction, there was also the need for a new naming, one that will allow to decouple the concept of profiling from the Pandas Dataframes - `ydata-profiling`! 
- 
-But fear not, `pip install pandas-profiling` will still be a valid for a while, and we will keep investing in growing the best open-source for data profiling, so you can use it for even more use cases.
+## ▶️ Quickstart
+
+### Install
+```cmd
+pip install ydata-profiling
+```
+or
+```cmd
+conda install -c conda-forge ydata-profiling
+```
+### Start profiling
+
+Start by loading your pandas `DataFrame` as you normally would, e.g. by using:
+
+```python
+import numpy as np
+import pandas as pd
+from ydata_profiling import ProfileReport
+
+df = pd.DataFrame(np.random.rand(100, 5), columns=["a", "b", "c", "d", "e"])
+```
+
+To generate the standard profiling report, merely run:
+
+```python
+profile = ProfileReport(df, title="Profiling Report")
+```
 
 ## Key features
 
 - **Type inference**: automatic detection of columns' data types (*Categorical*, *Numerical*, *Date*, etc.)
 - **Warnings**: A summary of the problems/challenges in the data that you might need to work on (*missing data*, *inaccuracies*, *skewness*, etc.)
 - **Univariate analysis**: including descriptive statistics (mean, median, mode, etc) and informative visualizations such as distribution histograms
 - **Multivariate analysis**: including correlations, a detailed analysis of missing data, duplicate rows, and visual support for variables pairwise interaction
@@ -75,32 +95,14 @@
 | [Comparing datasets](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/comparing_datasets.html )                        | Comparing multiple version of the same dataset                                              |
 | [Profiling a Time-Series dataset](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/time_series_datasets.html)               | Generating a report for a time-series dataset with a single line of code                    |
 |[Profiling large datasets](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/big_data.html )                            | Tips on how to prepare data and configure `ydata-profiling` for working with large datasets |
 | [Handling sensitive data](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/sensitive_data.html )                       | Generating reports which are mindful about sensitive data in the input dataset              |
 | [Dataset metadata and data dictionaries](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/metadata.html)               | Complementing the report with dataset details and column-specific data dictionaries         |
 | [Customizing the report's appearance](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/custom_report_appearance.html ) | Changing the appearance of the report's page and of the contained visualizations            |
 
-## ▶️ Quickstart
-
-Start by loading your pandas `DataFrame` as you normally would, e.g. by using:
-
-```python
-import numpy as np
-import pandas as pd
-from ydata_profiling import ProfileReport
-
-df = pd.DataFrame(np.random.rand(100, 5), columns=["a", "b", "c", "d", "e"])
-```
-
-To generate the standard profiling report, merely run:
-
-```python
-profile = ProfileReport(df, title="Profiling Report")
-```
-
 ### Using inside Jupyter Notebooks
 
 There are two interfaces to consume the report inside a Jupyter notebook: through widgets and through an embedded HTML report.
 
 <img alt="Notebook Widgets" src="https://ydata-profiling.ydata.ai/docs/master/assets/widgets.gif" width="800" />
 
 The above is achieved by simply displaying the report as a set of widgets. In a Jupyter Notebook, run:
```

#### html2text {}

```diff
@@ -16,86 +16,79 @@
         Do you like this project? Show us your love and give_feedback!
 `ydata-profiling` primary goal is to provide a one-line Exploratory Data
 Analysis (EDA) experience in a consistent and fast solution. Like pandas
 `df.describe()` function, that is so handy, ydata-profiling delivers an
 extended analysis of a DataFrame while allowing the data analysis to be
 exported in different formats such as **html** and **json**. The package
 outputs a simple and digested analysis of a dataset, including **time-series**
-and **text**. ### ð New year, new face, more functionalities! Thank you for
-using and following ``pandas-profiling`` developments. Yet, we have a new
-exciting feature - we are now thrilled to announce that Spark is now part of
-the Data Profiling family from version 4.0.0 onwards With its introduction,
-there was also the need for a new naming, one that will allow to decouple the
-concept of profiling from the Pandas Dataframes - `ydata-profiling`! But fear
-not, `pip install pandas-profiling` will still be a valid for a while, and we
-will keep investing in growing the best open-source for data profiling, so you
-can use it for even more use cases. ## Key features - **Type inference**:
-automatic detection of columns' data types (*Categorical*, *Numerical*, *Date*,
-etc.) - **Warnings**: A summary of the problems/challenges in the data that you
-might need to work on (*missing data*, *inaccuracies*, *skewness*, etc.) -
-**Univariate analysis**: including descriptive statistics (mean, median, mode,
-etc) and informative visualizations such as distribution histograms -
-**Multivariate analysis**: including correlations, a detailed analysis of
-missing data, duplicate rows, and visual support for variables pairwise
-interaction - **Time-Series**: including different statistical information
-relative to time dependent data such as auto-correlation and seasonality, along
-ACF and PACF plots. - **Text analysis**: most common categories (uppercase,
-lowercase, separator), scripts (Latin, Cyrillic) and blocks (ASCII, Cyrilic) -
-**File and Image analysis**: file sizes, creation dates, dimensions, indication
-of truncated images and existence of EXIF metadata - **Compare datasets**: one-
-line solution to enable a fast and complete report on the comparison of
-datasets - **Flexible output formats**: all analysis can be exported to an HTML
-report that can be easily shared with different parties, as JSON for an easy
-integration in automated systems and as a widget in a Jupyter Notebook. The
-report contains three additional sections: - **Overview**: mostly global
-details about the dataset (number of records, number of variables, overall
-missigness and duplicates, memory footprint) - **Alerts**: a comprehensive and
-automatic list of potential data quality issues (high correlation, skewness,
-uniformity, zeros, missing values, constant values, between others) -
-**Reproduction**: technical details about the analysis (time, version and
-configuration) ### ð Latest features - Want to scale? Check the latest
-release with â­â¡[Spark support](https://ydata-profiling.ydata.ai/docs/
-master/pages/integrations/pypspark.html)! - Looking for how you can do an EDA
-for Time-Series ð ? Check [this blogpost](https://towardsdatascience.com/
-how-to-do-an-eda-for-time-series-cbb92b3b1913). - You want to compare 2
-datasets and get a report? Check [this blogpost](https://medium.com/towards-
-artificial-intelligence/how-to-compare-2-dataset-with-pandas-profiling-
-2ae3a9d7695e) ### â¡ Spark Spark support has been released, but we are always
-looking for an extra pair of hands ð. [Check current work in progress!]
-(https://github.com/ydataai/ydata-profiling/projects/3). ## ð Use cases
-YData-profiling can be used to deliver a variety of different use-case. The
-documentation includes guides, tips and tricks for tackling them: | Use case |
-Description | |----------|-----------------------------------------------------
-----------------------------------------| | [Comparing datasets](https://ydata-
-profiling.ydata.ai/docs/master/pages/use_cases/comparing_datasets.html ) |
-Comparing multiple version of the same dataset | | [Profiling a Time-Series
-dataset](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/
-time_series_datasets.html) | Generating a report for a time-series dataset with
-a single line of code | |[Profiling large datasets](https://ydata-
-profiling.ydata.ai/docs/master/pages/use_cases/big_data.html ) | Tips on how to
-prepare data and configure `ydata-profiling` for working with large datasets |
-| [Handling sensitive data](https://ydata-profiling.ydata.ai/docs/master/pages/
-use_cases/sensitive_data.html ) | Generating reports which are mindful about
-sensitive data in the input dataset | | [Dataset metadata and data
-dictionaries](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/
-metadata.html) | Complementing the report with dataset details and column-
-specific data dictionaries | | [Customizing the report's appearance](https://
-ydata-profiling.ydata.ai/docs/master/pages/use_cases/
+and **text**. ## â¶ï¸ Quickstart ### Install ```cmd pip install ydata-
+profiling ``` or ```cmd conda install -c conda-forge ydata-profiling ``` ###
+Start profiling Start by loading your pandas `DataFrame` as you normally would,
+e.g. by using: ```python import numpy as np import pandas as pd from
+ydata_profiling import ProfileReport df = pd.DataFrame(np.random.rand(100, 5),
+columns=["a", "b", "c", "d", "e"]) ``` To generate the standard profiling
+report, merely run: ```python profile = ProfileReport(df, title="Profiling
+Report") ``` ## Key features - **Type inference**: automatic detection of
+columns' data types (*Categorical*, *Numerical*, *Date*, etc.) - **Warnings**:
+A summary of the problems/challenges in the data that you might need to work on
+(*missing data*, *inaccuracies*, *skewness*, etc.) - **Univariate analysis**:
+including descriptive statistics (mean, median, mode, etc) and informative
+visualizations such as distribution histograms - **Multivariate analysis**:
+including correlations, a detailed analysis of missing data, duplicate rows,
+and visual support for variables pairwise interaction - **Time-Series**:
+including different statistical information relative to time dependent data
+such as auto-correlation and seasonality, along ACF and PACF plots. - **Text
+analysis**: most common categories (uppercase, lowercase, separator), scripts
+(Latin, Cyrillic) and blocks (ASCII, Cyrilic) - **File and Image analysis**:
+file sizes, creation dates, dimensions, indication of truncated images and
+existence of EXIF metadata - **Compare datasets**: one-line solution to enable
+a fast and complete report on the comparison of datasets - **Flexible output
+formats**: all analysis can be exported to an HTML report that can be easily
+shared with different parties, as JSON for an easy integration in automated
+systems and as a widget in a Jupyter Notebook. The report contains three
+additional sections: - **Overview**: mostly global details about the dataset
+(number of records, number of variables, overall missigness and duplicates,
+memory footprint) - **Alerts**: a comprehensive and automatic list of potential
+data quality issues (high correlation, skewness, uniformity, zeros, missing
+values, constant values, between others) - **Reproduction**: technical details
+about the analysis (time, version and configuration) ### ð Latest features -
+Want to scale? Check the latest release with â­â¡[Spark support](https://
+ydata-profiling.ydata.ai/docs/master/pages/integrations/pypspark.html)! -
+Looking for how you can do an EDA for Time-Series ð ? Check [this blogpost]
+(https://towardsdatascience.com/how-to-do-an-eda-for-time-series-cbb92b3b1913).
+- You want to compare 2 datasets and get a report? Check [this blogpost](https:
+//medium.com/towards-artificial-intelligence/how-to-compare-2-dataset-with-
+pandas-profiling-2ae3a9d7695e) ### â¡ Spark Spark support has been released,
+but we are always looking for an extra pair of hands ð. [Check current work
+in progress!](https://github.com/ydataai/ydata-profiling/projects/3). ## ð
+Use cases YData-profiling can be used to deliver a variety of different use-
+case. The documentation includes guides, tips and tricks for tackling them: |
+Use case | Description | |----------|------------------------------------------
+---------------------------------------------------| | [Comparing datasets]
+(https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/
+comparing_datasets.html ) | Comparing multiple version of the same dataset | |
+[Profiling a Time-Series dataset](https://ydata-profiling.ydata.ai/docs/master/
+pages/use_cases/time_series_datasets.html) | Generating a report for a time-
+series dataset with a single line of code | |[Profiling large datasets](https:/
+/ydata-profiling.ydata.ai/docs/master/pages/use_cases/big_data.html ) | Tips on
+how to prepare data and configure `ydata-profiling` for working with large
+datasets | | [Handling sensitive data](https://ydata-profiling.ydata.ai/docs/
+master/pages/use_cases/sensitive_data.html ) | Generating reports which are
+mindful about sensitive data in the input dataset | | [Dataset metadata and
+data dictionaries](https://ydata-profiling.ydata.ai/docs/master/pages/
+use_cases/metadata.html) | Complementing the report with dataset details and
+column-specific data dictionaries | | [Customizing the report's appearance]
+(https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/
 custom_report_appearance.html ) | Changing the appearance of the report's page
-and of the contained visualizations | ## â¶ï¸ Quickstart Start by loading
-your pandas `DataFrame` as you normally would, e.g. by using: ```python import
-numpy as np import pandas as pd from ydata_profiling import ProfileReport df =
-pd.DataFrame(np.random.rand(100, 5), columns=["a", "b", "c", "d", "e"]) ``` To
-generate the standard profiling report, merely run: ```python profile =
-ProfileReport(df, title="Profiling Report") ``` ### Using inside Jupyter
-Notebooks There are two interfaces to consume the report inside a Jupyter
-notebook: through widgets and through an embedded HTML report. [Notebook
-Widgets] The above is achieved by simply displaying the report as a set of
-widgets. In a Jupyter Notebook, run: ```python profile.to_widgets() ``` The
-HTML report can be directly embedded in a cell in a similar fashion: ```python
+and of the contained visualizations | ### Using inside Jupyter Notebooks There
+are two interfaces to consume the report inside a Jupyter notebook: through
+widgets and through an embedded HTML report. [Notebook Widgets] The above is
+achieved by simply displaying the report as a set of widgets. In a Jupyter
+Notebook, run: ```python profile.to_widgets() ``` The HTML report can be
+directly embedded in a cell in a similar fashion: ```python
 profile.to_notebook_iframe() ``` [HTML] ### Exporting the report to a file To
 generate a HTML report file, save the `ProfileReport` to an object and use the
 `to_file()` function: ```python profile.to_file("your_report.html") ```
 Alternatively, the report's data can be obtained as a JSON file: ```python # As
 a JSON string json_data = profile.to_json() # As a file profile.to_file
 ("your_report.json") ``` ### Using in the command line For standard formatted
 CSV files (which can be read directly by pandas without additional settings),
```

### Comparing `ydata-profiling-4.1.2/make.bat` & `ydata-profiling-4.2.0/make.bat`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/setup.py` & `ydata-profiling-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/pandas_profiling/__init__.py` & `ydata-profiling-4.2.0/src/pandas_profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/__init__.py` & `ydata-profiling-4.2.0/src/ydata_profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/compare_reports.py` & `ydata-profiling-4.2.0/src/ydata_profiling/compare_reports.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import json
 import warnings
+from dataclasses import asdict
 from typing import Any, List, Optional, Tuple, Union
 
 import pandas as pd
+from dacite import from_dict
 
 from ydata_profiling.config import Correlation, Settings
+from ydata_profiling.model import BaseDescription
 from ydata_profiling.model.alerts import Alert
 from ydata_profiling.profile_report import ProfileReport
 
 
 def _should_wrap(v1: Any, v2: Any) -> bool:
     if isinstance(v1, (list, dict)):
         return False
@@ -75,32 +78,32 @@
         raise TypeError(
             "Both arguments need to be of type dictionary (ProfileReport.description_set)"
         )
 
     return _update_merge_dict(d1, d2)
 
 
-def _placeholders(*reports: dict) -> None:
+def _placeholders(reports: List[BaseDescription]) -> None:
     """Generates placeholders in the dataset descriptions where needed"""
 
-    keys = {v for r in reports for v in r["scatter"]}
-    type_keys = {v for r in reports for v in r["table"]["types"]}
+    keys = {v for r in reports for v in r.scatter}
+    type_keys = {v for r in reports for v in r.table["types"]}
     for report in reports:
         # Interactions
         for k1 in keys:
             for k2 in keys:
-                if k1 not in report["scatter"]:
-                    report["scatter"][k1] = {}
-                if k2 not in report["scatter"][k1]:
-                    report["scatter"][k1][k2] = ""
+                if k1 not in report.scatter:
+                    report.scatter[k1] = {}
+                if k2 not in report.scatter[k1]:
+                    report.scatter[k1][k2] = ""
 
         # Types
         for type_key in type_keys:
-            if type_key not in report["table"]["types"]:
-                report["table"]["types"][type_key] = 0
+            if type_key not in report.table["types"]:
+                report.table["types"][type_key] = 0
 
 
 def _update_titles(reports: List[ProfileReport]) -> None:
     """Redefine title of reports with the default one."""
     for idx, report in enumerate(reports):
         if report.config.title == "Pandas Profiling Report":
             report.config.title = f"Dataset {chr(65 + idx)}"
@@ -113,15 +116,15 @@
         title = ", ".join(titles[:-1])
         return f"<em>Comparing</em> {title} <em>and</em> {titles[-1]}"
 
 
 def _compare_profile_report_preprocess(
     reports: List[ProfileReport],
     config: Optional[Settings] = None,
-) -> Tuple[List[str], List[dict]]:
+) -> Tuple[List[str], List[BaseDescription]]:
     # Use titles as labels
     labels = [report.config.title for report in reports]
 
     # Use color per report if not custom set
     if config is None:
         if len(reports[0].config.html.style.primary_colors) > 1:
             for idx, report in enumerate(reports):
@@ -138,28 +141,28 @@
     # enforce same types
     for report in reports[1:]:
         report._typeset = reports[0].typeset
 
     # Obtain description sets
     descriptions = [report.get_description() for report in reports]
     for label, description in zip(labels, descriptions):
-        description["analysis"]["title"] = label
+        description.analysis.title = label
 
     return labels, descriptions
 
 
 def _compare_dataset_description_preprocess(
-    reports: List[dict],
-) -> Tuple[List[str], List[dict]]:
-    labels = [report["analysis"]["title"] for report in reports]
+    reports: List[BaseDescription],
+) -> Tuple[List[str], List[BaseDescription]]:
+    labels = [report.analysis.title for report in reports]
     return labels, reports
 
 
 def validate_reports(
-    reports: Union[List[ProfileReport], List[dict]], configs: List[dict]
+    reports: Union[List[ProfileReport], List[BaseDescription]], configs: List[dict]
 ) -> None:
     """Validate if the reports are comparable.
 
     Args:
         reports: two reports to compare
                  input may either be a ProfileReport, or the summary obtained from report.get_description()
     """
@@ -182,55 +185,53 @@
         is_df_available = [r.df is not None for r in reports]  # type: ignore
         if not all(is_df_available):
             raise ValueError("Reports where not initialized with a DataFrame.")
 
     if isinstance(reports[0], ProfileReport):
         features = [set(r.df.columns) for r in reports]  # type: ignore
     else:
-        features = [set(r["variables"].keys()) for r in reports]  # type: ignore
+        features = [set(r.variables.keys()) for r in reports]  # type: ignore
 
     if not all(features[0] == x for x in features):
         warnings.warn(
             "The datasets being profiled have a different set of columns. "
             "Only the left side profile will be calculated."
         )
 
 
-def _apply_config(description: dict, config: Settings) -> dict:
+def _apply_config(description: BaseDescription, config: Settings) -> BaseDescription:
     """Apply the configuration for visualilzation purposes.
 
     This handles the cases in which the report description
     was computed prior to comparison with a different config
 
     Args:
         description: report summary
         config: the settings object for the ProfileReport
 
     Returns:
         the updated description
     """
-    description["missing"] = {
-        k: v for k, v in description["missing"].items() if config.missing_diagrams[k]
+    description.missing = {
+        k: v for k, v in description.missing.items() if config.missing_diagrams[k]
     }
 
-    description["correlations"] = {
+    description.correlations = {
         k: v
-        for k, v in description["correlations"].items()
+        for k, v in description.correlations.items()
         if config.correlations.get(k, Correlation(calculate=False).calculate)
     }
 
     samples = [config.samples.head, config.samples.tail, config.samples.random]
     samples = [s > 0 for s in samples]
-    description["sample"] = description["sample"] if any(samples) else []
-    description["duplicates"] = (
-        description["duplicates"] if config.duplicates.head > 0 else None
-    )
-    description["scatter"] = (
-        description["scatter"] if config.interactions.continuous else {}
+    description.sample = description.sample if any(samples) else []
+    description.duplicates = (
+        description.duplicates if config.duplicates.head > 0 else None
     )
+    description.scatter = description.scatter if config.interactions.continuous else {}
 
     return description
 
 
 def _is_alert_present(alert: Alert, alert_list: list) -> bool:
     return any(
         a.column_name == alert.column_name and a.alert_type == alert.alert_type
@@ -252,15 +253,15 @@
                     empty_alert = copy(alert)
                     empty_alert._is_empty = True
                     fix.append(empty_alert)
     return tuple(fixed)
 
 
 def compare(
-    reports: Union[List[ProfileReport], List[dict]],
+    reports: Union[List[ProfileReport], List[BaseDescription]],
     config: Optional[Settings] = None,
     compute: bool = False,
 ) -> ProfileReport:
     """
     Compare Profile reports
 
     Args:
@@ -280,15 +281,15 @@
             "The input must have the same data type for all reports. Comparing ProfileReport objects to summaries obtained from the get_description() method is not supported."
         )
 
     if isinstance(reports[0], ProfileReport):
         all_configs = [r.config for r in reports]  # type: ignore
     else:
         configs_str = [
-            json.loads(r["package"]["ydata_profiling_config"]) for r in reports  # type: ignore
+            json.loads(r.package["ydata_profiling_config"]) for r in reports  # type: ignore
         ]
         all_configs = []
         for c_str in configs_str:
             c_setting = Settings()
             c_setting = c_setting.update(c_str)
             all_configs.append(c_setting)
 
@@ -299,19 +300,19 @@
         for report in reports[1:]:
             cols_2_compare = [col for col in base_features if col in report.df.columns]  # type: ignore
             report.df = report.df.loc[:, cols_2_compare]  # type: ignore
         reports = [r for r in reports if not r.df.empty]  # type: ignore
         if len(reports) == 1:
             return reports[0]  # type: ignore
     else:
-        base_features = list(reports[0]["variables"].keys())
+        base_features = list(reports[0].variables.keys())
         non_empty_reports = 0
         for report in reports[1:]:
             cols_2_compare = [
-                col for col in base_features if col in list(report["variables"].keys())  # type: ignore
+                col for col in base_features if col in list(report.variables.keys())  # type: ignore
             ]
             if len(cols_2_compare) > 0:
                 non_empty_reports += 1
         if non_empty_reports == 0:
             profile = ProfileReport(None, config=all_configs[0])
             profile._description_set = reports[0]
             return profile
@@ -332,29 +333,29 @@
                     report._description_set = None  # type: ignore
 
     if all(isinstance(report, ProfileReport) for report in reports):
         # Type ignore is needed as mypy does not pick up on the type narrowing
         # Consider using TypeGuard (3.10): https://docs.python.org/3/library/typing.html#typing.TypeGuard
         _update_titles(reports)  # type: ignore
         labels, descriptions = _compare_profile_report_preprocess(reports, _config)  # type: ignore
-    elif all(isinstance(report, dict) for report in reports):
+    elif all(isinstance(report, BaseDescription) for report in reports):
         labels, descriptions = _compare_dataset_description_preprocess(reports)  # type: ignore
     else:
         raise TypeError(
             "The input must have the same data type for all reports. Comparing ProfileReport objects to summaries obtained from the get_description() method is not supported."
         )
 
     _config.html.style._labels = labels
 
-    _placeholders(*descriptions)
+    _placeholders(descriptions)
 
-    descriptions = [_apply_config(d, _config) for d in descriptions]
+    descriptions_dict = [asdict(_apply_config(d, _config)) for d in descriptions]
 
-    res: dict = _update_merge(None, descriptions[0])
-    for r in descriptions[1:]:
+    res: dict = _update_merge(None, descriptions_dict[0])
+    for r in descriptions_dict[1:]:
         res = _update_merge(res, r)
 
     res["analysis"]["title"] = _compare_title(res["analysis"]["title"])
     res["alerts"] = _create_placehoder_alerts(res["alerts"])
     profile = ProfileReport(None, config=_config)
-    profile._description_set = res
+    profile._description_set = from_dict(data_class=BaseDescription, data=res)
     return profile
```

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/config.py` & `ydata-profiling-4.2.0/src/ydata_profiling/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,25 @@
     quantiles: List[float] = [0.05, 0.25, 0.5, 0.75, 0.95]
     skewness_threshold: int = 20
     low_categorical_threshold: int = 5
     # Set to zero to disable
     chi_squared_threshold: float = 0.999
 
 
+class TextVars(BaseModel):
+    length: bool = True
+    words: bool = True
+    characters: bool = True
+    redact: bool = False
+    # if text has more than threshold categories, its not category
+    categorical_threshold: int = 50
+    # if text has more than threshold % distinct values, its not category
+    percentage_cat_threshold: float = 0.5
+
+
 class CatVars(BaseModel):
     length: bool = True
     characters: bool = True
     words: bool = True
     cardinality_threshold: int = 50
     imbalance_threshold: float = 0.5
     n_obs: int = 5
@@ -102,14 +113,15 @@
     lags: List[int] = [1, 7, 12, 24, 30]
     significance: float = 0.05
     pacf_acf_lag: int = 100
 
 
 class Univariate(BaseModel):
     num: NumVars = NumVars()
+    text: TextVars = TextVars()
     cat: CatVars = CatVars()
     image: ImageVars = ImageVars()
     bool: BoolVars = BoolVars()
     path: PathVars = PathVars()
     file: FileVars = FileVars()
     url: UrlVars = UrlVars()
     timeseries: TimeseriesVars = TimeseriesVars()
@@ -391,15 +403,15 @@
 
 
 class Config:
     arg_groups: Dict[str, Any] = {
         "sensitive": {
             "samples": None,
             "duplicates": None,
-            "vars": {"cat": {"redact": True}},
+            "vars": {"cat": {"redact": True}, "text": {"redact": True}},
         },
         "dark_mode": {
             "html": {
                 "style": {
                     "theme": Theme.flatly,
                     "primary_color": "#2c3e50",
                 }
```

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/config_default.yaml` & `ydata-profiling-4.2.0/src/ydata_profiling/config_default.yaml`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/config_minimal.yaml` & `ydata-profiling-4.2.0/src/ydata_profiling/config_minimal.yaml`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/controller/console.py` & `ydata-profiling-4.2.0/src/ydata_profiling/controller/console.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/expectations_report.py` & `ydata-profiling-4.2.0/src/ydata_profiling/expectations_report.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from typing import Any, Optional
 
 import pandas as pd
 from visions import VisionsTypeset
 
 from ydata_profiling.config import Settings
-from ydata_profiling.model import expectation_algorithms
+from ydata_profiling.model import BaseDescription, expectation_algorithms
 from ydata_profiling.model.handler import Handler
 from ydata_profiling.utils.dataframe import slugify
 
 
 class ExpectationHandler(Handler):
     """Default handler"""
 
     def __init__(self, typeset: VisionsTypeset, *args, **kwargs):
         mapping = {
             "Unsupported": [expectation_algorithms.generic_expectations],
+            "Text": [expectation_algorithms.categorical_expectations],
             "Categorical": [expectation_algorithms.categorical_expectations],
             "Boolean": [expectation_algorithms.categorical_expectations],
             "Numeric": [expectation_algorithms.numeric_expectations],
             "URL": [expectation_algorithms.url_expectations],
             "File": [expectation_algorithms.file_expectations],
             "Path": [expectation_algorithms.path_expectations],
             "DateTime": [expectation_algorithms.datetime_expectations],
@@ -82,18 +83,18 @@
             suite_name, overwrite_existing=True
         )
 
         # Instantiate an in-memory pandas dataset
         batch = ge.dataset.PandasDataset(self.df, expectation_suite=suite)
 
         # Obtain the profiling summary
-        summary = self.get_description()  # type: ignore
+        summary: BaseDescription = self.get_description()  # type: ignore
 
         # Dispatch to expectations per semantic variable type
-        for name, variable_summary in summary["variables"].items():
+        for name, variable_summary in summary.variables.items():
             handler.handle(variable_summary["type"], name, variable_summary, batch)
 
         # We don't actually update the suite object on the batch in place, so need
         # to get the populated suite from the batch
         suite = batch.get_expectation_suite()
 
         validation_result_identifier = None
```

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/correlations.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/correlations.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/describe.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/describe.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any, Dict, Optional
 
 import pandas as pd
 from tqdm.auto import tqdm
 from visions import VisionsTypeset
 
 from ydata_profiling.config import Settings
+from ydata_profiling.model import BaseAnalysis, BaseDescription
 from ydata_profiling.model.alerts import get_alerts
 from ydata_profiling.model.correlations import (
     calculate_correlation,
     get_active_correlations,
 )
 from ydata_profiling.model.dataframe import check_dataframe, preprocess
 from ydata_profiling.model.duplicates import get_duplicates
@@ -26,15 +27,15 @@
 
 def describe(
     config: Settings,
     df: pd.DataFrame,
     summarizer: BaseSummarizer,
     typeset: VisionsTypeset,
     sample: Optional[dict] = None,
-) -> dict:
+) -> BaseDescription:
     """Calculate the statistics for each series in this DataFrame.
 
     Args:
         config: report Settings object
         df: DataFrame.
         summarizer: summarizer object
         typeset: visions typeset
@@ -164,36 +165,22 @@
         }
         pbar.update()
 
         pbar.set_postfix_str("Completed")
 
         date_end = datetime.utcnow()
 
-    analysis = {
-        "title": config.title,
-        "date_start": date_start,
-        "date_end": date_end,
-        "duration": date_end - date_start,
-    }
-
-    return {
-        # Analysis metadata
-        "analysis": analysis,
-        # Overall dataset description
-        "table": table_stats,
-        # Per variable descriptions
-        "variables": series_description,
-        # Bivariate relations
-        "scatter": scatter_matrix,
-        # Correlation matrices
-        "correlations": correlations,
-        # Missing values
-        "missing": missing,
-        # Alerts
-        "alerts": alerts,
-        # Package
-        "package": package,
-        # Sample
-        "sample": samples,
-        # Duplicates
-        "duplicates": duplicates,
-    }
+    analysis = BaseAnalysis(config.title, date_start, date_end)
+
+    description = BaseDescription(
+        analysis=analysis,
+        table=table_stats,
+        variables=series_description,
+        scatter=scatter_matrix,
+        correlations=correlations,
+        missing=missing,
+        alerts=alerts,
+        package=package,
+        sample=samples,
+        duplicates=duplicates,
+    )
+    return description
```

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/expectation_algorithms.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/expectation_algorithms.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/handler.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 def get_render_map() -> Dict[str, Callable]:
     import ydata_profiling.report.structure.variables as render_algorithms
 
     render_map = {
         "Boolean": render_algorithms.render_boolean,
         "Numeric": render_algorithms.render_real,
         "Complex": render_algorithms.render_complex,
+        "Text": render_algorithms.render_text,
         "DateTime": render_algorithms.render_date,
         "Categorical": render_algorithms.render_categorical,
         "URL": render_algorithms.render_url,
         "Path": render_algorithms.render_path,
         "File": render_algorithms.render_file,
         "Image": render_algorithms.render_image,
         "Unsupported": render_algorithms.render_generic,
```

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/missing.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/missing.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 @multimethod
 def missing_heatmap(config: Settings, df: Any) -> str:
     raise NotImplementedError()
 
 
-def get_missing_active(config: Settings, table_stats: dict) -> Dict[Any, Any]:
+def get_missing_active(config: Settings, table_stats: dict) -> Dict[str, Any]:
     """
 
     Args:
         config: report Settings object
         table_stats: The overall statistics for the DataFrame.
 
     Returns:
```

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pairwise.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pairwise.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/__init__.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     describe_date_pandas,
     describe_file_pandas,
     describe_generic_pandas,
     describe_image_pandas,
     describe_numeric_pandas,
     describe_path_pandas,
     describe_supported_pandas,
+    describe_text_pandas,
     describe_timeseries_pandas,
     describe_url_pandas,
     duplicates_pandas,
     missing_pandas,
     sample_pandas,
     summary_pandas,
     table_pandas,
@@ -29,14 +30,15 @@
     "describe_date_pandas",
     "describe_file_pandas",
     "describe_generic_pandas",
     "describe_image_pandas",
     "describe_numeric_pandas",
     "describe_path_pandas",
     "describe_supported_pandas",
+    "describe_text_pandas",
     "describe_timeseries_pandas",
     "describe_url_pandas",
     "duplicates_pandas",
     "missing_pandas",
     "sample_pandas",
     "sample_pandas",
     "summary_pandas",
```

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/correlations_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/correlations_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/dataframe_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/dataframe_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_boolean_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_boolean_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_categorical_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_categorical_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_counts_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_counts_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_date_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_date_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_file_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_file_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_generic_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_generic_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_image_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_image_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_numeric_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_numeric_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_path_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_path_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_supported_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_supported_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_timeseries_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_timeseries_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/describe_url_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/describe_url_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/discretize_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/discretize_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/duplicates_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/duplicates_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/imbalance_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/imbalance_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/missing_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/missing_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/sample_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/sample_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/summary_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/summary_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/table_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/table_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/pandas/utils_pandas.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/pandas/utils_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/sample.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/sample.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/spark/__init__.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/spark/correlations_spark.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/correlations_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/spark/dataframe_spark.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/dataframe_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/spark/describe_boolean_spark.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_boolean_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/spark/describe_categorical_spark.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_categorical_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/spark/describe_counts_spark.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_counts_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/spark/describe_date_spark.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_date_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/spark/describe_generic_spark.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_generic_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/spark/describe_numeric_spark.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_numeric_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/spark/describe_supported_spark.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/describe_supported_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/spark/duplicates_spark.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/duplicates_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/spark/missing_spark.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/missing_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/spark/sample_spark.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/sample_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/spark/summary_spark.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/summary_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/spark/table_spark.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/spark/table_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/summary.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/summary.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/summary_algorithms.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/summary_algorithms.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,28 +32,31 @@
     n_unique: int,
     name: str = "histogram",
     weights: Optional[np.ndarray] = None,
 ) -> dict:
     stats = {}
     bins = config.plot.histogram.bins
     bins_arg = "auto" if bins == 0 else min(bins, n_unique)
-    stats[name] = np.histogram(finite_values, bins=bins_arg, weights=weights)
+    bins = np.histogram_bin_edges(finite_values, bins=bins_arg)
+    stats[name] = np.histogram(finite_values, bins=bins, weights=weights)
 
     max_bins = config.plot.histogram.max_bins
     if bins_arg == "auto" and len(stats[name][1]) > max_bins:
-        stats[name] = np.histogram(finite_values, bins=max_bins, weights=None)
+        bins = np.histogram_bin_edges(finite_values, bins=max_bins)
+        stats[name] = np.histogram(finite_values, bins=bins, weights=None)
 
     return stats
 
 
 def chi_square(
     values: Optional[np.ndarray] = None, histogram: Optional[np.ndarray] = None
 ) -> dict:
     if histogram is None:
-        histogram, _ = np.histogram(values, bins="auto")
+        bins = np.histogram_bin_edges(values, bins="auto")
+        histogram, _ = np.histogram(values, bins=bins)
     return dict(chisquare(histogram)._asdict())
 
 
 def series_hashable(
     fn: Callable[[Settings, pd.Series, dict], Tuple[Settings, pd.Series, dict]]
 ) -> Callable[[Settings, pd.Series, dict], Tuple[Settings, pd.Series, dict]]:
     @functools.wraps(fn)
@@ -120,14 +123,21 @@
 def describe_numeric_1d(
     config: Settings, series: Any, summary: dict
 ) -> Tuple[Settings, Any, dict]:
     raise NotImplementedError()
 
 
 @multimethod
+def describe_text_1d(
+    config: Settings, series: Any, summary: dict
+) -> Tuple[Settings, Any, dict, Any]:
+    raise NotImplementedError()
+
+
+@multimethod
 def describe_date_1d(
     config: Settings, series: Any, summary: dict
 ) -> Tuple[Settings, Any, dict]:
     raise NotImplementedError()
 
 
 @multimethod
```

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/typeset.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/typeset.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,20 +10,23 @@
 from multimethod import multimethod
 from pandas.api import types as pdt
 from visions.backends.pandas.series_utils import series_not_empty
 from visions.relations import IdentityRelation, InferenceRelation, TypeRelation
 
 from ydata_profiling.config import Settings
 from ydata_profiling.model.typeset_relations import (
-    category_is_numeric,
-    category_to_numeric,
     numeric_is_category,
     series_is_string,
     string_is_bool,
+    string_is_category,
+    string_is_datetime,
+    string_is_numeric,
     string_to_bool,
+    string_to_datetime,
+    string_to_numeric,
     to_bool,
     to_category,
 )
 
 pandas_has_string_dtype_flag = hasattr(pdt, "is_string_dtype")
 
 
@@ -45,90 +48,172 @@
     return inner
 
 
 def typeset_types(config: Settings) -> Set[visions.VisionsBaseType]:
     """Define types based on the config"""
 
     class Unsupported(visions.Generic):
+        """Base type. All other types have relationship with this type."""
+
         pass
 
     class Numeric(visions.VisionsBaseType):
+        """Type for all numeric (float, int) columns.
+
+        Can be transformed from
+        - Unsupported
+        - String
+
+        Examples
+        --------
+        >>> s = pd.Series([1, 2, 5, 3, 8, 9])
+        >>> s in Numeric
+        True
+
+        >>> s = pd.Series([.34, 2.9, 55, 3.14, 89, 91])
+        >>> s in Numeric
+        True
+        """
+
         @staticmethod
         def get_relations() -> Sequence[TypeRelation]:
             return [
                 IdentityRelation(Unsupported),
                 InferenceRelation(
-                    Categorical,
-                    relationship=lambda x, y: partial(category_is_numeric, k=config)(
+                    Text,
+                    relationship=lambda x, y: partial(string_is_numeric, k=config)(
                         x, y
                     ),
-                    transformer=category_to_numeric,
+                    transformer=string_to_numeric,
                 ),
             ]
 
         @staticmethod
         @multimethod
         @series_not_empty
         @series_handle_nulls
         def contains_op(series: pd.Series, state: dict) -> bool:
             return pdt.is_numeric_dtype(series) and not pdt.is_bool_dtype(series)
 
+    class Text(visions.VisionsBaseType):
+        """Type for plaintext columns.
+        Like name, note, string identifier, residence etc.
+
+        Examples
+        --------
+        >>> s = pd.Series(["AX01", "BC32", "AC00"])
+        >>> s in Categorical
+        True
+
+        >>> s = pd.Series([1, 2, 3, 4])
+        >>> s in Categorical
+        False
+        """
+
+        @staticmethod
+        def get_relations() -> Sequence[TypeRelation]:
+            return [
+                IdentityRelation(Unsupported),
+            ]
+
+        @staticmethod
+        @multimethod
+        @series_not_empty
+        @series_handle_nulls
+        def contains_op(series: pd.Series, state: dict) -> bool:
+            return pdt.is_string_dtype(series) and series_is_string(series, state)
+
     class DateTime(visions.VisionsBaseType):
         @staticmethod
         def get_relations() -> Sequence[TypeRelation]:
             return [
                 IdentityRelation(Unsupported),
+                InferenceRelation(
+                    Text,
+                    relationship=lambda x, y: partial(string_is_datetime)(x, y),
+                    transformer=string_to_datetime,
+                ),
             ]
 
         @staticmethod
         @multimethod
         @series_not_empty
         @series_handle_nulls
         def contains_op(series: pd.Series, state: dict) -> bool:
             return pdt.is_datetime64_any_dtype(series)
 
     class Categorical(visions.VisionsBaseType):
+        """Type for categorical columns.
+        Categorical columns in pandas categorical format
+        and columns in string format with small count of unique values.
+
+        Can be transformed from:
+            - Unsupported
+            - Numeric
+            - String
+
+        Examples
+        --------
+        >>> s = pd.Series(["male", "female", "female", "male"], dtype="category")
+        >>> s in Categorical
+        True
+
+        >>> s = pd.Series(["male", "female"])
+        >>> s in Categorical
+        False
+
+        >>> s = pd.Series(["male", "female", "female", "male"])
+        >>> s in Categorical
+        True
+        """
+
         @staticmethod
         def get_relations() -> Sequence[TypeRelation]:
             return [
                 IdentityRelation(Unsupported),
                 InferenceRelation(
                     Numeric,
                     relationship=lambda x, y: partial(numeric_is_category, k=config)(
                         x, y
                     ),
                     transformer=to_category,
                 ),
+                InferenceRelation(
+                    Text,
+                    relationship=lambda x, y: partial(string_is_category, k=config)(
+                        x, y
+                    ),
+                    transformer=to_category,
+                ),
             ]
 
         @staticmethod
         @multimethod
         @series_not_empty
         @series_handle_nulls
         def contains_op(series: pd.Series, state: dict) -> bool:
             is_valid_dtype = pdt.is_categorical_dtype(series) and not pdt.is_bool_dtype(
                 series
             )
             if is_valid_dtype:
                 return True
-            elif not pdt.is_object_dtype(series):
-                return pandas_has_string_dtype_flag and pdt.is_string_dtype(series)
-
-            return series_is_string(series, state)
+            return False
 
     class Boolean(visions.VisionsBaseType):
+        """Type for boolean columns."""
+
         @staticmethod
         def get_relations() -> Sequence[TypeRelation]:
             # Numeric [0, 1] goes via Categorical with distinct_count_without_nan <= 2
             mapping = config.vars.bool.mappings
 
             return [
                 IdentityRelation(Unsupported),
                 InferenceRelation(
-                    Categorical,
+                    Text,
                     relationship=lambda x, y: partial(string_is_bool, k=mapping)(x, y),
                     transformer=lambda s, st: to_bool(
                         partial(string_to_bool, k=mapping)(s, st)
                     ),
                 ),
             ]
 
@@ -144,15 +229,15 @@
                     return False
 
             return pdt.is_bool_dtype(series)
 
     class URL(visions.VisionsBaseType):
         @staticmethod
         def get_relations() -> Sequence[TypeRelation]:
-            return [IdentityRelation(Categorical)]
+            return [IdentityRelation(Text)]
 
         @staticmethod
         @multimethod
         @series_handle_nulls
         def contains_op(series: pd.Series, state: dict) -> bool:
             # TODO: use coercion utils
             try:
@@ -160,15 +245,15 @@
                 return all(x.netloc and x.scheme for x in url_gen)  # noqa: TC300
             except AttributeError:
                 return False
 
     class Path(visions.VisionsBaseType):
         @staticmethod
         def get_relations() -> Sequence[TypeRelation]:
-            return [IdentityRelation(Categorical)]
+            return [IdentityRelation(Text)]
 
         @staticmethod
         @multimethod
         @series_handle_nulls
         def contains_op(series: pd.Series, state: dict) -> bool:
             # TODO: use coercion utils
             try:
@@ -219,15 +304,15 @@
                             return True
 
                 return False
 
             is_numeric = pdt.is_numeric_dtype(series) and not pdt.is_bool_dtype(series)
             return is_numeric and is_timedependent(series)
 
-    types = {Unsupported, Boolean, Numeric, Categorical, DateTime}
+    types = {Unsupported, Boolean, Numeric, Text, Categorical, DateTime}
     if config.vars.path.active:
         types.add(Path)
         if config.vars.file.active:
             types.add(File)
             if config.vars.image.active:
                 types.add(Image)
```

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/model/typeset_relations.py` & `ydata-profiling-4.2.0/src/ydata_profiling/model/typeset_relations.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import functools
-from typing import Callable
+from typing import Callable, Dict
 
 import numpy as np
 import pandas as pd
 from pandas.api import types as pdt
 from visions.backends.pandas.series_utils import series_handle_nulls
 
 from ydata_profiling.config import Settings
@@ -20,27 +20,27 @@
             return fn(series, *args, **kwargs)
         except:  # noqa: E722
             return False
 
     return inner
 
 
-def string_is_bool(series: pd.Series, state: dict, k: Settings) -> bool:
+def string_is_bool(series: pd.Series, state: dict, k: Dict[str, bool]) -> bool:
     @series_handle_nulls
     @try_func
     def tester(s: pd.Series, state: dict) -> bool:
         return s.str.lower().isin(k.keys()).all()
 
     if pdt.is_categorical_dtype(series):
         return False
 
     return tester(series, state)
 
 
-def string_to_bool(series: pd.Series, state: dict, k: Settings) -> pd.Series:
+def string_to_bool(series: pd.Series, state: dict, k: Dict[str, bool]) -> pd.Series:
     return series.str.lower().map(k)
 
 
 def numeric_is_category(series: pd.Series, state: dict, k: Settings) -> bool:
     n_unique = series.nunique()
     threshold = k.vars.num.low_categorical_threshold
     return 1 <= n_unique <= threshold
@@ -62,30 +62,59 @@
     try:
         return (series.astype(str).values == series.values).all()
     except (TypeError, ValueError):
         return False
 
 
 @series_handle_nulls
-def category_is_numeric(series: pd.Series, state: dict, k: Settings) -> bool:
+def string_is_category(series: pd.Series, state: dict, k: Settings) -> bool:
+    """String is category, if following conditions are met
+    - has at least one and less or equal distinct values as threshold
+    - (distinct values / count of all values) is less than threshold
+    - is not bool"""
+    n_unique = series.nunique()
+    unique_threshold = k.vars.text.percentage_cat_threshold
+    threshold = k.vars.text.categorical_threshold
+    return (
+        1 <= n_unique <= threshold
+        and n_unique / series.size < unique_threshold
+        and not string_is_bool(series, state, k.vars.bool.mappings)
+    )
+
+
+@series_handle_nulls
+def string_is_datetime(series: pd.Series, state: dict) -> bool:
+    """If we can transform data to datetime and at least one is valid date."""
+    try:
+        return not series.astype("datetime64").isna().all()
+    except:  # noqa: E722
+        return False
+
+
+@series_handle_nulls
+def string_is_numeric(series: pd.Series, state: dict, k: Settings) -> bool:
     if pdt.is_bool_dtype(series) or object_is_bool(series, state):
         return False
 
     try:
         _ = series.astype(float)
         r = pd.to_numeric(series, errors="coerce")
         if r.hasnans and r.count() == 0:
             return False
     except:  # noqa: E722
         return False
 
     return not numeric_is_category(series, state, k)
 
 
-def category_to_numeric(series: pd.Series, state: dict) -> pd.Series:
+def string_to_datetime(series: pd.Series, state: dict) -> pd.Series:
+    return series.astype("datetime64")
+
+
+def string_to_numeric(series: pd.Series, state: dict) -> pd.Series:
     return pd.to_numeric(series, errors="coerce")
 
 
 hasnan_bool_name = "boolean"
 
 
 def to_bool(series: pd.Series) -> pd.Series:
```

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/profile_report.py` & `ydata-profiling-4.2.0/src/ydata_profiling/profile_report.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import copy
 import json
 import warnings
 from pathlib import Path
-from typing import Any, Dict, Optional, Union
+from typing import Any, Optional, Union
 
 try:
     from pyspark.sql import DataFrame as sDataFrame
 except:  # noqa: E722
     from typing import TypeVar
 
     sDataFrame = TypeVar("sDataFrame")  # type: ignore
 
+from dataclasses import asdict, is_dataclass
+
 import numpy as np
 import pandas as pd
 from tqdm.auto import tqdm
 from typeguard import typechecked
 from visions import VisionsTypeset
 
 from ydata_profiling.config import Config, Settings, SparkSettings
 from ydata_profiling.expectations_report import ExpectationsReport
+from ydata_profiling.model import BaseDescription
 from ydata_profiling.model.alerts import AlertType
 from ydata_profiling.model.describe import describe as describe_df
 from ydata_profiling.model.sample import Sample
 from ydata_profiling.model.summarizer import (
     BaseSummarizer,
     PandasProfilingSummarizer,
     format_summary,
+    redact_summary,
 )
 from ydata_profiling.model.typeset import ProfilingTypeSet
 from ydata_profiling.report import get_report_structure
 from ydata_profiling.report.presentation.core import Root
 from ydata_profiling.report.presentation.flavours.html.templates import (
     create_html_assets,
 )
@@ -153,15 +157,14 @@
     def __validate_inputs(
         df: Optional[Union[pd.DataFrame, sDataFrame]],
         minimal: bool,
         tsmode: bool,
         config_file: Optional[Union[Path, str]],
         lazy: bool,
     ) -> None:
-
         # Lazy profile cannot be set if no DataFrame is provided
         if df is None and not lazy:
             raise ValueError("Can init a not-lazy ProfileReport with no DataFrame")
 
         if config_file is not None and minimal:
             raise ValueError(
                 "Arguments `config_file` and `minimal` are mutually exclusive."
@@ -239,15 +242,15 @@
     @property
     def summarizer(self) -> BaseSummarizer:
         if self._summarizer is None:
             self._summarizer = PandasProfilingSummarizer(self.typeset)
         return self._summarizer
 
     @property
-    def description_set(self) -> Dict[str, Any]:
+    def description_set(self) -> BaseDescription:
         if self._description_set is None:
             self._description_set = describe_df(
                 self.config,
                 self.df,
                 self.summarizer,
                 self.typeset,
                 self._sample,
@@ -277,16 +280,16 @@
         if self._json is None:
             self._json = self._render_json()
         return self._json
 
     @property
     def widgets(self) -> Any:
         if (
-            isinstance(self.description_set["table"]["n"], list)
-            and len(self.description_set["table"]["n"]) > 1
+            isinstance(self.description_set.table["n"], list)
+            and len(self.description_set.table["n"]) > 1
         ):
             raise RuntimeError(
                 "Widgets interface not (yet) supported for comparing reports, please use the HTML rendering."
             )
 
         if self._widgets is None:
             self._widgets = self._render_widgets()
@@ -294,25 +297,25 @@
 
     def get_duplicates(self) -> Optional[pd.DataFrame]:
         """Get duplicate rows and counts based on the configuration
 
         Returns:
             A DataFrame with the duplicate rows and their counts.
         """
-        return self.description_set["duplicates"]
+        return self.description_set.duplicates
 
     def get_sample(self) -> dict:
         """Get head/tail samples based on the configuration
 
         Returns:
             A dict with the head and tail samples.
         """
-        return self.description_set["sample"]
+        return self.description_set.sample
 
-    def get_description(self) -> dict:
+    def get_description(self) -> BaseDescription:
         """Return the description (a raw statistical summary) of the dataset.
 
         Returns:
             Dict containing a description for each variable in the DataFrame.
         """
         return self.description_set
 
@@ -320,15 +323,15 @@
         """Get variables that are rejected for analysis (e.g. constant, mixed data types)
 
         Returns:
             a set of column names that are unsupported
         """
         return {
             alert.column_name
-            for alert in self.description_set["alerts"]
+            for alert in self.description_set.alerts
             if alert.alert_type == AlertType.REJECTED
         }
 
     def to_file(self, output_file: Union[str, Path], silent: bool = True) -> None:
         """Write the report to a file.
 
         Args:
@@ -386,17 +389,17 @@
                 nav=self.config.html.navbar_show,
                 offline=self.config.html.use_local_assets,
                 inline=self.config.html.inline,
                 assets_prefix=self.config.html.assets_prefix,
                 primary_color=self.config.html.style.primary_colors[0],
                 logo=self.config.html.style.logo,
                 theme=self.config.html.style.theme,
-                title=self.description_set["analysis"]["title"],
-                date=self.description_set["analysis"]["date_start"],
-                version=self.description_set["package"]["ydata_profiling_version"],
+                title=self.description_set.analysis.title,
+                date=self.description_set.analysis.date_start,
+                version=self.description_set.package["ydata_profiling_version"],
             )
 
             if self.config.html.minify_html:
                 from htmlmin.main import minify
 
                 html = minify(html, remove_all_empty_space=True, remove_comments=True)
             pbar.update()
@@ -415,14 +418,16 @@
         ) as pbar:
             widgets = WidgetReport(copy.deepcopy(report)).render()
             pbar.update()
         return widgets
 
     def _render_json(self) -> str:
         def encode_it(o: Any) -> Any:
+            if is_dataclass(o):
+                o = asdict(o)
             if isinstance(o, dict):
                 return {encode_it(k): encode_it(v) for k, v in o.items()}
             else:
                 if isinstance(o, (bool, int, float, str)):
                     return o
                 elif isinstance(o, list):
                     return [encode_it(v) for v in o]
@@ -440,17 +445,19 @@
                     return str(o)
 
         description = self.description_set
 
         with tqdm(
             total=1, desc="Render JSON", disable=not self.config.progress_bar
         ) as pbar:
-            description = format_summary(description)
-            description = encode_it(description)
-            data = json.dumps(description, indent=4)
+            description_dict = format_summary(description)
+            description_dict = encode_it(description_dict)
+            description_dict = redact_summary(description_dict, self.config)
+
+            data = json.dumps(description_dict, indent=4)
             pbar.update()
         return data
 
     def to_html(self) -> str:
         """Generate and return complete template as lengthy string
             for using with frameworks.
```

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/formatters.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/formatters.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/__init__.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/alerts.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/alerts.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/collapse.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/collapse.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/container.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/container.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/correlation_table.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/correlation_table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/dropdown.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/dropdown.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/image.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/image.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/renderable.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/renderable.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/root.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/root.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/sample.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/sample.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/table.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/variable.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/variable.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/core/variable_info.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/core/variable_info.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/flavours.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/flavours.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/__init__.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/alerts.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/alerts.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/container.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/container.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/correlation_table.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/correlation_table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/duplicate.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/duplicate.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/frequency_table.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/frequency_table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/frequency_table_small.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/frequency_table_small.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/alerts.html` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table.html` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table_small.html` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table_small.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/report.html` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/report.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/batch_grid.html` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/batch_grid.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/grid.html` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/grid.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/sections.html` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/sections.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/select.html` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/select.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/tabs.html` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/tabs.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/table.html` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/table.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/toggle_button.html` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/toggle_button.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/variable_info.html` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/variable_info.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap-theme.min.css` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.css` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.js` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/cosmo.bootstrap.min.css` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/cosmo.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/flatly.bootstrap.min.css` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/flatly.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/jquery-1.12.4.min.js` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/jquery-1.12.4.min.js`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/script.js` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/script.js`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/simplex.bootstrap.min.css` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/simplex.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/style.css` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/style.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/united.bootstrap.min.css` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/united.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/javascript.html` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/javascript.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/navigation.html` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/navigation.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/style.html` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/style.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/html/templates.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/html/templates.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/__init__.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/alerts.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/alerts.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/collapse.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/collapse.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/container.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/container.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/dropdown.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/dropdown.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/frequency_table.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/frequency_table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/frequency_table_small.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/frequency_table_small.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/image.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/image.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/notebook.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/notebook.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/table.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/flavours/widget/toggle_button.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/flavours/widget/toggle_button.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/presentation/frequency_table_utils.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/presentation/frequency_table_utils.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/structure/correlations.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/correlations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from typing import List, Optional
 
 from ydata_profiling.config import Settings
+from ydata_profiling.model import BaseDescription
 from ydata_profiling.report.presentation.core import Container, CorrelationTable, Image
 from ydata_profiling.report.presentation.core.renderable import Renderable
 from ydata_profiling.visualisation import plot
 
 
-def get_correlation_items(config: Settings, summary: dict) -> Optional[Renderable]:
+def get_correlation_items(
+    config: Settings, summary: BaseDescription
+) -> Optional[Renderable]:
     """Create the list of correlation items
 
     Args:
         config: report Settings object
         summary: dict of correlations
 
     Returns:
@@ -25,15 +28,15 @@
         "phi_k": (0, "Phik (φk)"),
         "cramers": (0, "Cramér's V (φc)"),
         "auto": (-1, "Auto"),
     }
 
     image_format = config.plot.image_format
 
-    for key, item in summary["correlations"].items():
+    for key, item in summary.correlations.items():
         vmin, name = key_to_data[key]
 
         if isinstance(item, list):
             diagrams: List[Renderable] = []
             for idx, i in enumerate(item):
                 diagram: Renderable = Image(
                     plot.correlation_matrix(config, i, vmin=vmin),
```

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/structure/overview.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/overview.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from typing import List
 from urllib.parse import quote
 
 from ydata_profiling.config import Settings
+from ydata_profiling.model import BaseDescription
 from ydata_profiling.model.alerts import AlertType
 from ydata_profiling.report.formatters import (
     fmt,
     fmt_bytesize,
     fmt_number,
     fmt_numeric,
     fmt_percent,
     fmt_timespan,
     list_args,
 )
 from ydata_profiling.report.presentation.core import Alerts, Container, Table
 from ydata_profiling.report.presentation.core.renderable import Renderable
 
 
-def get_dataset_overview(config: Settings, summary: dict) -> Renderable:
+def get_dataset_overview(config: Settings, summary: BaseDescription) -> Renderable:
     table_metrics = [
         {
             "name": "Number of variables",
-            "value": fmt_number(summary["table"]["n_var"]),
+            "value": fmt_number(summary.table["n_var"]),
         },
         {
             "name": "Number of observations",
-            "value": fmt_number(summary["table"]["n"]),
+            "value": fmt_number(summary.table["n"]),
         },
         {
             "name": "Missing cells",
-            "value": fmt_number(summary["table"]["n_cells_missing"]),
+            "value": fmt_number(summary.table["n_cells_missing"]),
         },
         {
             "name": "Missing cells (%)",
-            "value": fmt_percent(summary["table"]["p_cells_missing"]),
+            "value": fmt_percent(summary.table["p_cells_missing"]),
         },
     ]
-    if "n_duplicates" in summary["table"]:
+    if "n_duplicates" in summary.table:
         table_metrics.extend(
             [
                 {
                     "name": "Duplicate rows",
-                    "value": fmt_number(summary["table"]["n_duplicates"]),
+                    "value": fmt_number(summary.table["n_duplicates"]),
                 },
                 {
                     "name": "Duplicate rows (%)",
-                    "value": fmt_percent(summary["table"]["p_duplicates"]),
+                    "value": fmt_percent(summary.table["p_duplicates"]),
                 },
             ]
         )
-    if "memory_size" in summary["table"]:
+    if "memory_size" in summary.table:
         table_metrics.extend(
             [
                 {
                     "name": "Total size in memory",
-                    "value": fmt_bytesize(summary["table"]["memory_size"]),
+                    "value": fmt_bytesize(summary.table["memory_size"]),
                 },
                 {
                     "name": "Average record size in memory",
-                    "value": fmt_bytesize(summary["table"]["record_size"]),
+                    "value": fmt_bytesize(summary.table["record_size"]),
                 },
             ]
         )
 
     dataset_info = Table(
         table_metrics, name="Dataset statistics", style=config.html.style
     )
 
     dataset_types = Table(
         [
             {
                 "name": str(type_name),
                 "value": fmt_numeric(count, precision=config.report.precision),
             }
-            for type_name, count in summary["table"]["types"].items()
+            for type_name, count in summary.table["types"].items()
         ],
         name="Variable types",
         style=config.html.style,
     )
 
     return Container(
         [dataset_info, dataset_types],
@@ -131,30 +132,30 @@
         ],
         name="Dataset",
         anchor_id="dataset",
         sequence_type="grid",
     )
 
 
-def get_dataset_reproduction(config: Settings, summary: dict) -> Renderable:
+def get_dataset_reproduction(config: Settings, summary: BaseDescription) -> Renderable:
     """Dataset reproduction part of the report
 
     Args:
         config: settings object
         summary: the dataset summary.
 
     Returns:
         A renderable object
     """
 
-    version = summary["package"]["ydata_profiling_version"]
-    config_file = summary["package"]["ydata_profiling_config"]
-    date_start = summary["analysis"]["date_start"]
-    date_end = summary["analysis"]["date_end"]
-    duration = summary["analysis"]["duration"]
+    version = summary.package["ydata_profiling_version"]
+    config_file = summary.package["ydata_profiling_config"]
+    date_start = summary.analysis.date_start
+    date_end = summary.analysis.date_end
+    duration = summary.analysis.duration
 
     @list_args
     def fmt_version(version: str) -> str:
         return f'<a href="https://github.com/ydataai/ydata-profiling">ydata-profiling v{version}</a>'
 
     @list_args
     def fmt_config(config: str) -> str:
@@ -261,15 +262,15 @@
         alerts=alerts,
         name=f"Alerts ({count})",
         anchor_id="alerts",
         style=config.html.style,
     )
 
 
-def get_dataset_items(config: Settings, summary: dict, alerts: list) -> list:
+def get_dataset_items(config: Settings, summary: BaseDescription, alerts: list) -> list:
     """Returns the dataset overview (at the top of the report)
 
     Args:
         config: settings object
         summary: the calculated summary
         alerts: the alerts
```

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/structure/report.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Generate the report."""
 from typing import List, Sequence
 
 import pandas as pd
 from tqdm.auto import tqdm
 
 from ydata_profiling.config import Settings
+from ydata_profiling.model import BaseDescription
 from ydata_profiling.model.alerts import AlertType
 from ydata_profiling.model.handler import get_render_map
 from ydata_profiling.report.presentation.core import (
     HTML,
     Collapse,
     Container,
     Dropdown,
@@ -19,15 +20,15 @@
 from ydata_profiling.report.presentation.core.renderable import Renderable
 from ydata_profiling.report.presentation.core.root import Root
 from ydata_profiling.report.structure.correlations import get_correlation_items
 from ydata_profiling.report.structure.overview import get_dataset_items
 from ydata_profiling.utils.dataframe import slugify
 
 
-def get_missing_items(config: Settings, summary: dict) -> list:
+def get_missing_items(config: Settings, summary: BaseDescription) -> list:
     """Return the missing diagrams
 
     Args:
         config: report Settings object
         summary: the dataframe summary
 
     Returns:
@@ -56,21 +57,23 @@
                 for i in range(len(item["name"]))
             ],
             sequence_type="batch_grid",
             batch_size=len(config.html.style._labels),
             anchor_id=key,
             name=item["name"][0],
         )
-        for key, item in summary["missing"].items()
+        for key, item in summary.missing.items()
     ]
 
     return items
 
 
-def render_variables_section(config: Settings, dataframe_summary: dict) -> list:
+def render_variables_section(
+    config: Settings, dataframe_summary: BaseDescription
+) -> list:
     """Render the HTML for each of the variables in the DataFrame.
 
     Args:
         config: report Settings object
         dataframe_summary: The statistics for each variable.
 
     Returns:
@@ -81,53 +84,52 @@
 
     descriptions = config.variables.descriptions
     show_description = config.show_variable_description
     reject_variables = config.reject_variables
 
     render_map = get_render_map()
 
-    for idx, summary in dataframe_summary["variables"].items():
-
+    for idx, summary in dataframe_summary.variables.items():
         # Common template variables
-        if not isinstance(dataframe_summary["alerts"], tuple):
+        if not isinstance(dataframe_summary.alerts, tuple):
             alerts = [
                 alert.fmt()
-                for alert in dataframe_summary["alerts"]
+                for alert in dataframe_summary.alerts
                 if alert.column_name == idx
             ]
 
             alert_fields = {
                 field
-                for alert in dataframe_summary["alerts"]
+                for alert in dataframe_summary.alerts
                 if alert.column_name == idx
                 for field in alert.fields
             }
 
             alert_types = {
                 alert.alert_type
-                for alert in dataframe_summary["alerts"]
+                for alert in dataframe_summary.alerts
                 if alert.column_name == idx
             }
         else:
             alerts = tuple(
                 [alert.fmt() for alert in summary_alerts if alert.column_name == idx]
-                for summary_alerts in dataframe_summary["alerts"]
+                for summary_alerts in dataframe_summary.alerts
             )  # type: ignore
 
             alert_fields = {
                 field
-                for summary_alerts in dataframe_summary["alerts"]
+                for summary_alerts in dataframe_summary.alerts
                 for alert in summary_alerts
                 if alert.column_name == idx
                 for field in alert.fields
             }
 
             alert_types = {
                 alert.alert_type
-                for summary_alerts in dataframe_summary["alerts"]
+                for summary_alerts in dataframe_summary.alerts
                 for alert in summary_alerts
                 if alert.column_name == idx
             }
 
         template_variables = {
             "varname": idx,
             "varid": hash(idx),
@@ -193,15 +195,16 @@
 
     Returns:
         List of duplicates items to show in the interface.
     """
     items: List[Renderable] = []
     if duplicates is not None and len(duplicates) > 0:
         if isinstance(duplicates, list):
-            if any([d is None for d in duplicates]):
+            generator = (d is None for d in duplicates)
+            if any(generator):
                 return items
 
             for idx, df in enumerate(duplicates):
                 items.append(
                     Duplicate(
                         duplicate=df,
                         name=config.html.style._labels[idx],
@@ -341,58 +344,58 @@
                 nested=len(interactions) > 10,
                 anchor_id=f"interactions_{slugify(x_col)}",
             )
         )
     return titems
 
 
-def get_report_structure(config: Settings, summary: dict) -> Root:
+def get_report_structure(config: Settings, summary: BaseDescription) -> Root:
     """Generate a HTML report from summary statistics and a given sample.
 
     Args:
       config: report Settings object
       summary: Statistics to use for the overview, variables, correlations and missing values.
 
     Returns:
       The profile report in HTML format
     """
     disable_progress_bar = not config.progress_bar
     with tqdm(
         total=1, desc="Generate report structure", disable=disable_progress_bar
     ) as pbar:
-        alerts = summary["alerts"]
+        alerts = summary.alerts
 
         section_items: List[Renderable] = [
             Container(
                 get_dataset_items(config, summary, alerts),
                 sequence_type="tabs",
                 name="Overview",
                 anchor_id="overview",
             ),
         ]
 
-        if len(summary["variables"]) > 0:
+        if len(summary.variables) > 0:
             section_items.append(
                 Dropdown(
                     name="Variables",
                     anchor_id="variables-dropdown",
                     id="variables-dropdown",
                     is_row=True,
                     classes=["dropdown-toggle"],
-                    items=list(summary["variables"]),
+                    items=list(summary.variables),
                     item=Container(
                         render_variables_section(config, summary),
                         sequence_type="accordion",
                         name="Variables",
                         anchor_id="variables",
                     ),
                 )
             )
 
-        scatter_items = get_interactions(config, summary["scatter"])
+        scatter_items = get_interactions(config, summary.scatter)
         if len(scatter_items) > 0:
             section_items.append(
                 Container(
                     scatter_items,
                     sequence_type="tabs" if len(scatter_items) <= 10 else "select",
                     name="Interactions",
                     anchor_id="interactions",
@@ -410,26 +413,26 @@
                     missing_items,
                     sequence_type="tabs",
                     name="Missing values",
                     anchor_id="missing",
                 )
             )
 
-        sample_items = get_sample_items(config, summary["sample"])
+        sample_items = get_sample_items(config, summary.sample)
         if len(sample_items) > 0:
             section_items.append(
                 Container(
                     items=sample_items,
                     sequence_type="tabs",
                     name="Sample",
                     anchor_id="sample",
                 )
             )
 
-        duplicate_items = get_duplicates_items(config, summary["duplicates"])
+        duplicate_items = get_duplicates_items(config, summary.duplicates)
         if len(duplicate_items) > 0:
             section_items.append(
                 Container(
                     items=duplicate_items,
                     sequence_type="batch_grid",
                     batch_size=len(duplicate_items),
                     name="Duplicate rows",
```

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/__init__.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ydata_profiling.report.structure.variables.render_count import render_count
 from ydata_profiling.report.structure.variables.render_date import render_date
 from ydata_profiling.report.structure.variables.render_file import render_file
 from ydata_profiling.report.structure.variables.render_generic import render_generic
 from ydata_profiling.report.structure.variables.render_image import render_image
 from ydata_profiling.report.structure.variables.render_path import render_path
 from ydata_profiling.report.structure.variables.render_real import render_real
+from ydata_profiling.report.structure.variables.render_text import render_text
 from ydata_profiling.report.structure.variables.render_timeseries import (
     render_timeseries,
 )
 from ydata_profiling.report.structure.variables.render_url import render_url
 
 __all__ = [
     "render_boolean",
@@ -24,10 +25,11 @@
     "render_count",
     "render_date",
     "render_file",
     "render_generic",
     "render_image",
     "render_path",
     "render_real",
+    "render_text",
     "render_timeseries",
     "render_url",
 ]
```

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_boolean.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_boolean.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_categorical.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_categorical.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_common.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_common.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_complex.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_complex.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_count.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_count.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_date.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_date.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_file.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_file.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_generic.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_generic.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_image.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_image.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_path.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_path.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_real.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_real.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_timeseries.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_timeseries.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/report/structure/variables/render_url.py` & `ydata-profiling-4.2.0/src/ydata_profiling/report/structure/variables/render_url.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/serialize_report.py` & `ydata-profiling-4.2.0/src/ydata_profiling/serialize_report.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Optional, Union
 
 if TYPE_CHECKING:
     from ydata_profiling.profile_report import ProfileReport
 
 from ydata_profiling.config import Settings
+from ydata_profiling.model import BaseDescription
 from ydata_profiling.report.presentation.core import Root
 from ydata_profiling.version import __version__
 
 
 class SerializeReport:
     """Extend the report to be able to dump and load reports."""
 
@@ -68,15 +69,15 @@
             raise ValueError("Failed to load data") from e
 
         if not all(
             (
                 df_hash is None or isinstance(df_hash, str),
                 isinstance(loaded_config, Settings),
                 loaded_description_set is None
-                or isinstance(loaded_description_set, dict),
+                or isinstance(loaded_description_set, BaseDescription),
                 loaded_report is None or isinstance(loaded_report, Root),
             )
         ):
             raise ValueError(
                 "Failed to load data: file may be damaged or from an incompatible version"
             )
         if (df_hash == self.df_hash) or (self.df is None):
@@ -97,20 +98,20 @@
 
             # overwrite config
             self.config = loaded_config
 
             # warn if version not equal
             if (
                 loaded_description_set is not None
-                and loaded_description_set["package"]["ydata_profiling_version"]
+                and loaded_description_set.package["ydata_profiling_version"]
                 != __version__
             ):
                 warnings.warn(
                     f"The package version specified in the loaded data is not equal to the version installed. "
-                    f"Currently running on ydata-profiling {__version__} , while loaded data is generated by ydata_profiling, {loaded_description_set['package']['ydata_profiling_version']}."
+                    f"Currently running on ydata-profiling {__version__} , while loaded data is generated by ydata_profiling, {loaded_description_set.package['ydata_profiling_version']}."
                 )
 
             # set df_hash
             self._df_hash = df_hash
 
         else:
             raise ValueError("DataFrame does not match with the current ProfileReport.")
```

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/utils/cache.py` & `ydata-profiling-4.2.0/src/ydata_profiling/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/utils/common.py` & `ydata-profiling-4.2.0/src/ydata_profiling/utils/common.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/utils/dataframe.py` & `ydata-profiling-4.2.0/src/ydata_profiling/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/utils/imghdr_patch.py` & `ydata-profiling-4.2.0/src/ydata_profiling/utils/imghdr_patch.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/utils/paths.py` & `ydata-profiling-4.2.0/src/ydata_profiling/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/visualisation/context.py` & `ydata-profiling-4.2.0/src/ydata_profiling/visualisation/context.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/visualisation/missing.py` & `ydata-profiling-4.2.0/src/ydata_profiling/visualisation/missing.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/visualisation/plot.py` & `ydata-profiling-4.2.0/src/ydata_profiling/visualisation/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,25 +9,40 @@
 from matplotlib import pyplot as plt
 from matplotlib.collections import PolyCollection
 from matplotlib.colors import Colormap, LinearSegmentedColormap, ListedColormap, rgb2hex
 from matplotlib.patches import Patch
 from matplotlib.ticker import FuncFormatter
 from statsmodels.graphics.tsaplots import plot_acf, plot_pacf
 from typeguard import typechecked
+from wordcloud import WordCloud
 
 from ydata_profiling.config import Settings
 from ydata_profiling.utils.common import convert_timestamp_to_datetime
 from ydata_profiling.visualisation.context import manage_matplotlib_context
 from ydata_profiling.visualisation.utils import plot_360_n0sc0pe
 
 
 def format_fn(tick_val: int, tick_pos: Any) -> str:
     return convert_timestamp_to_datetime(tick_val).strftime("%Y-%m-%d %H:%M:%S")
 
 
+def _plot_word_cloud(
+    series: pd.Series,
+    figsize: tuple = (6, 4),
+) -> plt.Figure:
+    word_dict = series.to_dict()
+    wordcloud = WordCloud(
+        background_color="white", random_state=123, width=300, height=200, scale=2
+    ).generate_from_frequencies(word_dict)
+    plt.figure(figsize=figsize)
+    plot = plt.imshow(wordcloud, interpolation="bilinear")
+    plt.axis("off")
+    return plot
+
+
 def _plot_histogram(
     config: Settings,
     series: np.ndarray,
     bins: Union[int, np.ndarray],
     figsize: tuple = (6, 4),
     date: bool = False,
     hide_yaxis: bool = False,
@@ -96,14 +111,20 @@
         if not config.plot.histogram.x_axis_labels:
             plot.set_xticklabels([])
 
     return plot
 
 
 @manage_matplotlib_context()
+def plot_word_cloud(config: Settings, word_counts: pd.Series) -> str:
+    _plot_word_cloud(series=word_counts)
+    return plot_360_n0sc0pe(config)
+
+
+@manage_matplotlib_context()
 def histogram(
     config: Settings,
     series: np.ndarray,
     bins: Union[int, np.ndarray],
     date: bool = False,
 ) -> str:
     """Plot an histogram of the data.
```

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling/visualisation/utils.py` & `ydata-profiling-4.2.0/src/ydata_profiling/visualisation/utils.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling.egg-info/PKG-INFO` & `ydata-profiling-4.2.0/src/ydata_profiling.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydata-profiling
-Version: 4.1.2
+Version: 4.2.0
 Summary: Generate profile report for pandas DataFrame
 Home-page: https://github.com/ydataai/ydata-profiling
 Author: YData Labs Inc
 Author-email: opensource@ydata.ai
 License: MIT
 Description: # ydata-profiling
         
@@ -31,24 +31,44 @@
         
         <p align="center">
           Do you like this project? Show us your love and <a href="https://engage.ydata.ai">give feedback!</a>
         </p>
         
         `ydata-profiling` primary goal is to provide a one-line Exploratory Data Analysis (EDA) experience in a consistent and fast solution. Like pandas `df.describe()` function, that is so handy, ydata-profiling delivers an extended analysis of a DataFrame while allowing the data analysis to be exported in different formats such as **html** and **json**.
         
-        The package outputs a simple and digested analysis of a dataset, including **time-series** and **text**. 
+        The package outputs a simple and digested analysis of a dataset, including **time-series** and **text**.
         
-        ### 🎊 New year, new face, more functionalities! 
         
-        Thank you for using and following ``pandas-profiling`` developments. Yet, we have a new exciting feature - we are now thrilled to announce
-        that <u>Spark</u> is now part of the Data Profiling family from version 4.0.0 onwards
-         
-        With its introduction, there was also the need for a new naming, one that will allow to decouple the concept of profiling from the Pandas Dataframes - `ydata-profiling`! 
-         
-        But fear not, `pip install pandas-profiling` will still be a valid for a while, and we will keep investing in growing the best open-source for data profiling, so you can use it for even more use cases.
+        ## ▶️ Quickstart
+        
+        ### Install
+        ```cmd
+        pip install ydata-profiling
+        ```
+        or
+        ```cmd
+        conda install -c conda-forge ydata-profiling
+        ```
+        ### Start profiling
+        
+        Start by loading your pandas `DataFrame` as you normally would, e.g. by using:
+        
+        ```python
+        import numpy as np
+        import pandas as pd
+        from ydata_profiling import ProfileReport
+        
+        df = pd.DataFrame(np.random.rand(100, 5), columns=["a", "b", "c", "d", "e"])
+        ```
+        
+        To generate the standard profiling report, merely run:
+        
+        ```python
+        profile = ProfileReport(df, title="Profiling Report")
+        ```
         
         ## Key features
         
         - **Type inference**: automatic detection of columns' data types (*Categorical*, *Numerical*, *Date*, etc.)
         - **Warnings**: A summary of the problems/challenges in the data that you might need to work on (*missing data*, *inaccuracies*, *skewness*, etc.)
         - **Univariate analysis**: including descriptive statistics (mean, median, mode, etc) and informative visualizations such as distribution histograms
         - **Multivariate analysis**: including correlations, a detailed analysis of missing data, duplicate rows, and visual support for variables pairwise interaction
@@ -83,32 +103,14 @@
         | [Comparing datasets](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/comparing_datasets.html )                        | Comparing multiple version of the same dataset                                              |
         | [Profiling a Time-Series dataset](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/time_series_datasets.html)               | Generating a report for a time-series dataset with a single line of code                    |
         |[Profiling large datasets](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/big_data.html )                            | Tips on how to prepare data and configure `ydata-profiling` for working with large datasets |
         | [Handling sensitive data](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/sensitive_data.html )                       | Generating reports which are mindful about sensitive data in the input dataset              |
         | [Dataset metadata and data dictionaries](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/metadata.html)               | Complementing the report with dataset details and column-specific data dictionaries         |
         | [Customizing the report's appearance](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/custom_report_appearance.html ) | Changing the appearance of the report's page and of the contained visualizations            |
         
-        ## ▶️ Quickstart
-        
-        Start by loading your pandas `DataFrame` as you normally would, e.g. by using:
-        
-        ```python
-        import numpy as np
-        import pandas as pd
-        from ydata_profiling import ProfileReport
-        
-        df = pd.DataFrame(np.random.rand(100, 5), columns=["a", "b", "c", "d", "e"])
-        ```
-        
-        To generate the standard profiling report, merely run:
-        
-        ```python
-        profile = ProfileReport(df, title="Profiling Report")
-        ```
-        
         ### Using inside Jupyter Notebooks
         
         There are two interfaces to consume the report inside a Jupyter notebook: through widgets and through an embedded HTML report.
         
         <img alt="Notebook Widgets" src="https://ydata-profiling.ydata.ai/docs/master/assets/widgets.gif" width="800" />
         
         The above is achieved by simply displaying the report as a set of widgets. In a Jupyter Notebook, run:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ydata-profiling Version: 4.1.2 Summary: Generate
+Metadata-Version: 2.1 Name: ydata-profiling Version: 4.2.0 Summary: Generate
 profile report for pandas DataFrame Home-page: https://github.com/ydataai/
 ydata-profiling Author: YData Labs Inc Author-email: opensource@ydata.ai
 License: MIT Description: # ydata-profiling [![Build Status](https://
 github.com/ydataai/pandas-profiling/actions/workflows/tests.yml/
 badge.svg?branch=master)](https://github.com/ydataai/pandas-profiling/actions/
 workflows/tests.yml) [![PyPI download month](https://img.shields.io/pypi/dm/
 ydata-profiling.svg)](https://pypi.python.org/pypi/ydata-profiling/) [![]
@@ -20,86 +20,79 @@
         Do you like this project? Show us your love and give_feedback!
 `ydata-profiling` primary goal is to provide a one-line Exploratory Data
 Analysis (EDA) experience in a consistent and fast solution. Like pandas
 `df.describe()` function, that is so handy, ydata-profiling delivers an
 extended analysis of a DataFrame while allowing the data analysis to be
 exported in different formats such as **html** and **json**. The package
 outputs a simple and digested analysis of a dataset, including **time-series**
-and **text**. ### ð New year, new face, more functionalities! Thank you for
-using and following ``pandas-profiling`` developments. Yet, we have a new
-exciting feature - we are now thrilled to announce that Spark is now part of
-the Data Profiling family from version 4.0.0 onwards With its introduction,
-there was also the need for a new naming, one that will allow to decouple the
-concept of profiling from the Pandas Dataframes - `ydata-profiling`! But fear
-not, `pip install pandas-profiling` will still be a valid for a while, and we
-will keep investing in growing the best open-source for data profiling, so you
-can use it for even more use cases. ## Key features - **Type inference**:
-automatic detection of columns' data types (*Categorical*, *Numerical*, *Date*,
-etc.) - **Warnings**: A summary of the problems/challenges in the data that you
-might need to work on (*missing data*, *inaccuracies*, *skewness*, etc.) -
-**Univariate analysis**: including descriptive statistics (mean, median, mode,
-etc) and informative visualizations such as distribution histograms -
-**Multivariate analysis**: including correlations, a detailed analysis of
-missing data, duplicate rows, and visual support for variables pairwise
-interaction - **Time-Series**: including different statistical information
-relative to time dependent data such as auto-correlation and seasonality, along
-ACF and PACF plots. - **Text analysis**: most common categories (uppercase,
-lowercase, separator), scripts (Latin, Cyrillic) and blocks (ASCII, Cyrilic) -
-**File and Image analysis**: file sizes, creation dates, dimensions, indication
-of truncated images and existence of EXIF metadata - **Compare datasets**: one-
-line solution to enable a fast and complete report on the comparison of
-datasets - **Flexible output formats**: all analysis can be exported to an HTML
-report that can be easily shared with different parties, as JSON for an easy
-integration in automated systems and as a widget in a Jupyter Notebook. The
-report contains three additional sections: - **Overview**: mostly global
-details about the dataset (number of records, number of variables, overall
-missigness and duplicates, memory footprint) - **Alerts**: a comprehensive and
-automatic list of potential data quality issues (high correlation, skewness,
-uniformity, zeros, missing values, constant values, between others) -
-**Reproduction**: technical details about the analysis (time, version and
-configuration) ### ð Latest features - Want to scale? Check the latest
-release with â­â¡[Spark support](https://ydata-profiling.ydata.ai/docs/
-master/pages/integrations/pypspark.html)! - Looking for how you can do an EDA
-for Time-Series ð ? Check [this blogpost](https://towardsdatascience.com/
-how-to-do-an-eda-for-time-series-cbb92b3b1913). - You want to compare 2
-datasets and get a report? Check [this blogpost](https://medium.com/towards-
-artificial-intelligence/how-to-compare-2-dataset-with-pandas-profiling-
-2ae3a9d7695e) ### â¡ Spark Spark support has been released, but we are always
-looking for an extra pair of hands ð. [Check current work in progress!]
-(https://github.com/ydataai/ydata-profiling/projects/3). ## ð Use cases
-YData-profiling can be used to deliver a variety of different use-case. The
-documentation includes guides, tips and tricks for tackling them: | Use case |
-Description | |----------|-----------------------------------------------------
-----------------------------------------| | [Comparing datasets](https://ydata-
-profiling.ydata.ai/docs/master/pages/use_cases/comparing_datasets.html ) |
-Comparing multiple version of the same dataset | | [Profiling a Time-Series
-dataset](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/
-time_series_datasets.html) | Generating a report for a time-series dataset with
-a single line of code | |[Profiling large datasets](https://ydata-
-profiling.ydata.ai/docs/master/pages/use_cases/big_data.html ) | Tips on how to
-prepare data and configure `ydata-profiling` for working with large datasets |
-| [Handling sensitive data](https://ydata-profiling.ydata.ai/docs/master/pages/
-use_cases/sensitive_data.html ) | Generating reports which are mindful about
-sensitive data in the input dataset | | [Dataset metadata and data
-dictionaries](https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/
-metadata.html) | Complementing the report with dataset details and column-
-specific data dictionaries | | [Customizing the report's appearance](https://
-ydata-profiling.ydata.ai/docs/master/pages/use_cases/
+and **text**. ## â¶ï¸ Quickstart ### Install ```cmd pip install ydata-
+profiling ``` or ```cmd conda install -c conda-forge ydata-profiling ``` ###
+Start profiling Start by loading your pandas `DataFrame` as you normally would,
+e.g. by using: ```python import numpy as np import pandas as pd from
+ydata_profiling import ProfileReport df = pd.DataFrame(np.random.rand(100, 5),
+columns=["a", "b", "c", "d", "e"]) ``` To generate the standard profiling
+report, merely run: ```python profile = ProfileReport(df, title="Profiling
+Report") ``` ## Key features - **Type inference**: automatic detection of
+columns' data types (*Categorical*, *Numerical*, *Date*, etc.) - **Warnings**:
+A summary of the problems/challenges in the data that you might need to work on
+(*missing data*, *inaccuracies*, *skewness*, etc.) - **Univariate analysis**:
+including descriptive statistics (mean, median, mode, etc) and informative
+visualizations such as distribution histograms - **Multivariate analysis**:
+including correlations, a detailed analysis of missing data, duplicate rows,
+and visual support for variables pairwise interaction - **Time-Series**:
+including different statistical information relative to time dependent data
+such as auto-correlation and seasonality, along ACF and PACF plots. - **Text
+analysis**: most common categories (uppercase, lowercase, separator), scripts
+(Latin, Cyrillic) and blocks (ASCII, Cyrilic) - **File and Image analysis**:
+file sizes, creation dates, dimensions, indication of truncated images and
+existence of EXIF metadata - **Compare datasets**: one-line solution to enable
+a fast and complete report on the comparison of datasets - **Flexible output
+formats**: all analysis can be exported to an HTML report that can be easily
+shared with different parties, as JSON for an easy integration in automated
+systems and as a widget in a Jupyter Notebook. The report contains three
+additional sections: - **Overview**: mostly global details about the dataset
+(number of records, number of variables, overall missigness and duplicates,
+memory footprint) - **Alerts**: a comprehensive and automatic list of potential
+data quality issues (high correlation, skewness, uniformity, zeros, missing
+values, constant values, between others) - **Reproduction**: technical details
+about the analysis (time, version and configuration) ### ð Latest features -
+Want to scale? Check the latest release with â­â¡[Spark support](https://
+ydata-profiling.ydata.ai/docs/master/pages/integrations/pypspark.html)! -
+Looking for how you can do an EDA for Time-Series ð ? Check [this blogpost]
+(https://towardsdatascience.com/how-to-do-an-eda-for-time-series-cbb92b3b1913).
+- You want to compare 2 datasets and get a report? Check [this blogpost](https:
+//medium.com/towards-artificial-intelligence/how-to-compare-2-dataset-with-
+pandas-profiling-2ae3a9d7695e) ### â¡ Spark Spark support has been released,
+but we are always looking for an extra pair of hands ð. [Check current work
+in progress!](https://github.com/ydataai/ydata-profiling/projects/3). ## ð
+Use cases YData-profiling can be used to deliver a variety of different use-
+case. The documentation includes guides, tips and tricks for tackling them: |
+Use case | Description | |----------|------------------------------------------
+---------------------------------------------------| | [Comparing datasets]
+(https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/
+comparing_datasets.html ) | Comparing multiple version of the same dataset | |
+[Profiling a Time-Series dataset](https://ydata-profiling.ydata.ai/docs/master/
+pages/use_cases/time_series_datasets.html) | Generating a report for a time-
+series dataset with a single line of code | |[Profiling large datasets](https:/
+/ydata-profiling.ydata.ai/docs/master/pages/use_cases/big_data.html ) | Tips on
+how to prepare data and configure `ydata-profiling` for working with large
+datasets | | [Handling sensitive data](https://ydata-profiling.ydata.ai/docs/
+master/pages/use_cases/sensitive_data.html ) | Generating reports which are
+mindful about sensitive data in the input dataset | | [Dataset metadata and
+data dictionaries](https://ydata-profiling.ydata.ai/docs/master/pages/
+use_cases/metadata.html) | Complementing the report with dataset details and
+column-specific data dictionaries | | [Customizing the report's appearance]
+(https://ydata-profiling.ydata.ai/docs/master/pages/use_cases/
 custom_report_appearance.html ) | Changing the appearance of the report's page
-and of the contained visualizations | ## â¶ï¸ Quickstart Start by loading
-your pandas `DataFrame` as you normally would, e.g. by using: ```python import
-numpy as np import pandas as pd from ydata_profiling import ProfileReport df =
-pd.DataFrame(np.random.rand(100, 5), columns=["a", "b", "c", "d", "e"]) ``` To
-generate the standard profiling report, merely run: ```python profile =
-ProfileReport(df, title="Profiling Report") ``` ### Using inside Jupyter
-Notebooks There are two interfaces to consume the report inside a Jupyter
-notebook: through widgets and through an embedded HTML report. [Notebook
-Widgets] The above is achieved by simply displaying the report as a set of
-widgets. In a Jupyter Notebook, run: ```python profile.to_widgets() ``` The
-HTML report can be directly embedded in a cell in a similar fashion: ```python
+and of the contained visualizations | ### Using inside Jupyter Notebooks There
+are two interfaces to consume the report inside a Jupyter notebook: through
+widgets and through an embedded HTML report. [Notebook Widgets] The above is
+achieved by simply displaying the report as a set of widgets. In a Jupyter
+Notebook, run: ```python profile.to_widgets() ``` The HTML report can be
+directly embedded in a cell in a similar fashion: ```python
 profile.to_notebook_iframe() ``` [HTML] ### Exporting the report to a file To
 generate a HTML report file, save the `ProfileReport` to an object and use the
 `to_file()` function: ```python profile.to_file("your_report.html") ```
 Alternatively, the report's data can be obtained as a JSON file: ```python # As
 a JSON string json_data = profile.to_json() # As a file profile.to_file
 ("your_report.json") ``` ### Using in the command line For standard formatted
 CSV files (which can be read directly by pandas without additional settings),
```

### Comparing `ydata-profiling-4.1.2/src/ydata_profiling.egg-info/SOURCES.txt` & `ydata-profiling-4.2.0/src/ydata_profiling.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 src/ydata_profiling/controller/console.py
 src/ydata_profiling/controller/pandas_decorator.py
 src/ydata_profiling/model/__init__.py
 src/ydata_profiling/model/alerts.py
 src/ydata_profiling/model/correlations.py
 src/ydata_profiling/model/dataframe.py
 src/ydata_profiling/model/describe.py
+src/ydata_profiling/model/description.py
 src/ydata_profiling/model/duplicates.py
 src/ydata_profiling/model/expectation_algorithms.py
 src/ydata_profiling/model/handler.py
 src/ydata_profiling/model/missing.py
 src/ydata_profiling/model/pairwise.py
 src/ydata_profiling/model/sample.py
 src/ydata_profiling/model/summarizer.py
@@ -54,14 +55,15 @@
 src/ydata_profiling/model/pandas/describe_date_pandas.py
 src/ydata_profiling/model/pandas/describe_file_pandas.py
 src/ydata_profiling/model/pandas/describe_generic_pandas.py
 src/ydata_profiling/model/pandas/describe_image_pandas.py
 src/ydata_profiling/model/pandas/describe_numeric_pandas.py
 src/ydata_profiling/model/pandas/describe_path_pandas.py
 src/ydata_profiling/model/pandas/describe_supported_pandas.py
+src/ydata_profiling/model/pandas/describe_text_pandas.py
 src/ydata_profiling/model/pandas/describe_timeseries_pandas.py
 src/ydata_profiling/model/pandas/describe_url_pandas.py
 src/ydata_profiling/model/pandas/discretize_pandas.py
 src/ydata_profiling/model/pandas/duplicates_pandas.py
 src/ydata_profiling/model/pandas/imbalance_pandas.py
 src/ydata_profiling/model/pandas/missing_pandas.py
 src/ydata_profiling/model/pandas/sample_pandas.py
@@ -74,14 +76,15 @@
 src/ydata_profiling/model/spark/describe_boolean_spark.py
 src/ydata_profiling/model/spark/describe_categorical_spark.py
 src/ydata_profiling/model/spark/describe_counts_spark.py
 src/ydata_profiling/model/spark/describe_date_spark.py
 src/ydata_profiling/model/spark/describe_generic_spark.py
 src/ydata_profiling/model/spark/describe_numeric_spark.py
 src/ydata_profiling/model/spark/describe_supported_spark.py
+src/ydata_profiling/model/spark/describe_text_spark.py
 src/ydata_profiling/model/spark/duplicates_spark.py
 src/ydata_profiling/model/spark/missing_spark.py
 src/ydata_profiling/model/spark/sample_spark.py
 src/ydata_profiling/model/spark/summary_spark.py
 src/ydata_profiling/model/spark/table_spark.py
 src/ydata_profiling/report/__init__.py
 src/ydata_profiling/report/formatters.py
@@ -209,14 +212,15 @@
 src/ydata_profiling/report/structure/variables/render_count.py
 src/ydata_profiling/report/structure/variables/render_date.py
 src/ydata_profiling/report/structure/variables/render_file.py
 src/ydata_profiling/report/structure/variables/render_generic.py
 src/ydata_profiling/report/structure/variables/render_image.py
 src/ydata_profiling/report/structure/variables/render_path.py
 src/ydata_profiling/report/structure/variables/render_real.py
+src/ydata_profiling/report/structure/variables/render_text.py
 src/ydata_profiling/report/structure/variables/render_timeseries.py
 src/ydata_profiling/report/structure/variables/render_url.py
 src/ydata_profiling/utils/__init__.py
 src/ydata_profiling/utils/cache.py
 src/ydata_profiling/utils/common.py
 src/ydata_profiling/utils/compat.py
 src/ydata_profiling/utils/dataframe.py
```

