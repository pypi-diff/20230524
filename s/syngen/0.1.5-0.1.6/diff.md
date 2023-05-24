# Comparing `tmp/syngen-0.1.5.tar.gz` & `tmp/syngen-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.1.5.tar", last modified: Mon May 22 08:44:40 2023, max compression
+gzip compressed data, was "syngen-0.1.6.tar", last modified: Wed May 24 07:19:11 2023, max compression
```

## Comparing `syngen-0.1.5.tar` & `syngen-0.1.6.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.261839 syngen-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-22 08:43:19.000000 syngen-0.1.5/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-22 08:43:19.000000 syngen-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-22 08:43:19.000000 syngen-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    16393 2023-05-22 08:44:40.261839 syngen-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    15654 2023-05-22 08:43:19.000000 syngen-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-22 08:43:19.000000 syngen-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-05-22 08:44:40.261839 syngen-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.245839 syngen-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.253839 syngen-0.1.5/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2677 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.253839 syngen-0.1.5/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.253839 syngen-0.1.5/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/config/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.253839 syngen-0.1.5/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.253839 syngen-0.1.5/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7887 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.253839 syngen-0.1.5/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.257839 syngen-0.1.5/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.249839 syngen-0.1.5/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.257839 syngen-0.1.5/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.257839 syngen-0.1.5/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.257839 syngen-0.1.5/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.257839 syngen-0.1.5/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.257839 syngen-0.1.5/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6972 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.257839 syngen-0.1.5/src/syngen/ml/train_chain/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/train_chain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15251 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/train_chain/train_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.257839 syngen-0.1.5/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      373 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6064 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.257839 syngen-0.1.5/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.261839 syngen-0.1.5/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    33024 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (122)    10467 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.261839 syngen-0.1.5/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.261839 syngen-0.1.5/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2115 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.261839 syngen-0.1.5/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13244 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3987 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.253839 syngen-0.1.5/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    16393 2023-05-22 08:44:40.000000 syngen-0.1.5/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-05-22 08:44:40.000000 syngen-0.1.5/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 08:44:40.000000 syngen-0.1.5/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-22 08:44:40.000000 syngen-0.1.5/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-05-22 08:44:40.000000 syngen-0.1.5/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-22 08:44:40.000000 syngen-0.1.5/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.215860 syngen-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-24 07:17:30.000000 syngen-0.1.6/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-24 07:17:30.000000 syngen-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-24 07:17:30.000000 syngen-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    17434 2023-05-24 07:19:11.215860 syngen-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    16695 2023-05-24 07:17:30.000000 syngen-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-24 07:17:30.000000 syngen-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-05-24 07:19:11.215860 syngen-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.199858 syngen-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.207859 syngen-0.1.6/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3368 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.207859 syngen-0.1.6/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.207859 syngen-0.1.6/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/config/configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.211859 syngen-0.1.6/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.211859 syngen-0.1.6/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7887 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.211859 syngen-0.1.6/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.211859 syngen-0.1.6/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.203858 syngen-0.1.6/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.211859 syngen-0.1.6/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.211859 syngen-0.1.6/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.215860 syngen-0.1.6/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.215860 syngen-0.1.6/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.215860 syngen-0.1.6/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6972 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.215860 syngen-0.1.6/src/syngen/ml/train_chain/
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/train_chain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15251 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/train_chain/train_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.215860 syngen-0.1.6/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      391 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6255 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.215860 syngen-0.1.6/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.215860 syngen-0.1.6/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33156 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10467 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.215860 syngen-0.1.6/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.215860 syngen-0.1.6/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2115 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.215860 syngen-0.1.6/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13244 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/ml/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4673 2023-05-24 07:17:30.000000 syngen-0.1.6/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:19:11.207859 syngen-0.1.6/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    17434 2023-05-24 07:19:11.000000 syngen-0.1.6/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-05-24 07:19:11.000000 syngen-0.1.6/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 07:19:11.000000 syngen-0.1.6/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-24 07:19:11.000000 syngen-0.1.6/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-05-24 07:19:11.000000 syngen-0.1.6/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-24 07:19:11.000000 syngen-0.1.6/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.1.5/LICENSE` & `syngen-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/PKG-INFO` & `syngen-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.1.5
+Version: 0.1.6
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
@@ -144,14 +144,25 @@
 * <i>random_seed</i> - data type - integer, must be equal to or more than 0
 * <i>print_report</i> - data type - boolean, default value is False
 * <i>metadata_path</i> - data type - string
 
 The metadata can contain any of the arguments above for each table. If so, the duplicated arguments from the CLI 
 will be ignored.
 
+<i>Note:</i> If you want to set the logging level, you can use the parameter <i>log_level</i> in the CLI call:
+
+```bash
+train --source STR --table_name STR --log_level STR
+train --metadata_path STR --log_level STR
+infer --size INT --table_name STR --log_level STR
+infer --metadata_path STR --log_level STR
+```
+
+where <i>log_level</i> might be one of the following values: <i>DEBUG, INFO, WARNING, ERROR, CRITICAL</i>.
+
 
 ### Linked tables generation
 
 To generate one or more tables, you might provide metadata in yaml format. By providing information about the relationships 
 between tables via metadata, it becomes possible to manage complex relationships across any number of tables. 
 You can also specify additional parameters needed for training and inference in the metadata file and in this case, 
 they will be ignored in the CLI call.
@@ -305,14 +316,30 @@
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-infer \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 ```
 
 You can add any arguments listed in the corresponding sections for infer and training processes in the CLI call, however, they will be 
 overwritten by corresponding arguments in the metadata file.
 
+#### Logging level
+
+Set the `LOGURU_LEVEL` environment variable to desired level of logging.
+For example, to suppress the debug messages, add `-e LOGURU_LEVEL=INFO` to the `docker run` command:
+```bash
+docker pull tdspora/syngen-train:latest
+docker run --rm -e LOGURU_LEVEL=INFO \
+  -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-train \
+  --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
+
+docker pull tdspora/syngen-infer:latest
+docker run --rm -e LOGURU_LEVEL=INFO \
+  -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-infer \
+  --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
+```
+
 ## Contribution
 
 We welcome contributions from the community to help us improve and maintain our public GitHub repository. We appreciate any feedback, bug reports, or feature requests, and we encourage developers to submit fixes or new features using issues.
 
 If you have found a bug or have a feature request, please submit an issue to our GitHub repository. Please provide as much detail as possible, including steps to reproduce the issue or a clear description of the feature request. Our team will review the issue and work with you to address any problems or discuss any potential new features.
 
 If you would like to contribute a fix or a new feature, please submit a pull request to our GitHub repository. Please make sure your code follows our coding standards and best practices. Our team will review your pull request and work with you to ensure that it meets our standards and is ready for inclusion in our codebase.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.1.5 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.1.6 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
@@ -76,15 +76,20 @@
 Requirements for parameters of generation process: * size - data type -
 integer, must be equal to or more than 1, default value is 100 * table_name -
 data type - string * run_parallel - data type - boolean, default value is False
 * batch_size - data type - integer, must be equal to or more than 1 *
 random_seed - data type - integer, must be equal to or more than 0 *
 print_report - data type - boolean, default value is False * metadata_path -
 data type - string The metadata can contain any of the arguments above for each
-table. If so, the duplicated arguments from the CLI will be ignored. ### Linked
+table. If so, the duplicated arguments from the CLI will be ignored. Note: If
+you want to set the logging level, you can use the parameter log_level in the
+CLI call: ```bash train --source STR --table_name STR --log_level STR train --
+metadata_path STR --log_level STR infer --size INT --table_name STR --log_level
+STR infer --metadata_path STR --log_level STR ``` where log_level might be one
+of the following values: DEBUG, INFO, WARNING, ERROR, CRITICAL. ### Linked
 tables generation To generate one or more tables, you might provide metadata in
 yaml format. By providing information about the relationships between tables
 via metadata, it becomes possible to manage complex relationships across any
 number of tables. You can also specify additional parameters needed for
 training and inference in the metadata file and in this case, they will be
 ignored in the CLI call. Note: By using metadata file, you can also generate
 tables with absent relationships. In this case, the tables will be generated
@@ -163,21 +168,30 @@
 train:latest docker run --rm \ -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts
 tdspora/syngen-train \ --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 docker pull tdspora/syngen-infer:latest docker run --rm \ -
 v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-infer \ --
 metadata_path=./model_artifacts/PATH_TO_METADATA_YAML ``` You can add any
 arguments listed in the corresponding sections for infer and training processes
 in the CLI call, however, they will be overwritten by corresponding arguments
-in the metadata file. ## Contribution We welcome contributions from the
-community to help us improve and maintain our public GitHub repository. We
-appreciate any feedback, bug reports, or feature requests, and we encourage
-developers to submit fixes or new features using issues. If you have found a
-bug or have a feature request, please submit an issue to our GitHub repository.
-Please provide as much detail as possible, including steps to reproduce the
-issue or a clear description of the feature request. Our team will review the
-issue and work with you to address any problems or discuss any potential new
-features. If you would like to contribute a fix or a new feature, please submit
-a pull request to our GitHub repository. Please make sure your code follows our
-coding standards and best practices. Our team will review your pull request and
-work with you to ensure that it meets our standards and is ready for inclusion
-in our codebase. We appreciate your contributions and thank you for your
-interest in helping us maintain and improve our public GitHub repository.
+in the metadata file. #### Logging level Set the `LOGURU_LEVEL` environment
+variable to desired level of logging. For example, to suppress the debug
+messages, add `-e LOGURU_LEVEL=INFO` to the `docker run` command: ```bash
+docker pull tdspora/syngen-train:latest docker run --rm -e LOGURU_LEVEL=INFO \
+-v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-train \ --
+metadata_path=./model_artifacts/PATH_TO_METADATA_YAML docker pull tdspora/
+syngen-infer:latest docker run --rm -e LOGURU_LEVEL=INFO \ -
+v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-infer \ --
+metadata_path=./model_artifacts/PATH_TO_METADATA_YAML ``` ## Contribution We
+welcome contributions from the community to help us improve and maintain our
+public GitHub repository. We appreciate any feedback, bug reports, or feature
+requests, and we encourage developers to submit fixes or new features using
+issues. If you have found a bug or have a feature request, please submit an
+issue to our GitHub repository. Please provide as much detail as possible,
+including steps to reproduce the issue or a clear description of the feature
+request. Our team will review the issue and work with you to address any
+problems or discuss any potential new features. If you would like to contribute
+a fix or a new feature, please submit a pull request to our GitHub repository.
+Please make sure your code follows our coding standards and best practices. Our
+team will review your pull request and work with you to ensure that it meets
+our standards and is ready for inclusion in our codebase. We appreciate your
+contributions and thank you for your interest in helping us maintain and
+improve our public GitHub repository.
```

### Comparing `syngen-0.1.5/README.md` & `syngen-0.1.6/src/syngen.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: syngen
+Version: 0.1.6
+Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
+Home-page: https://github.com/tdspora/syngen
+Author: EPAM Systems, Inc.
+Maintainer: Pavel Bobyrev
+License: GPLv3 License
+Keywords: data,generation,synthetic,vae,tabular
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # EPAM Syngen
 
 EPAM Syngen is an unsupervised tabular data generation tool. It is useful for generation of test data with a given table as a template. Most datatypes including floats, integers, datetime, text, categorical, binary are supported. The linked tables i.e., tables sharing a key can also be generated using the simple statistical approach. 
 The source of data might be in CSV, Avro format and should be located locally and be in UTF-8 encoding.
 
 The tool is based on the variational autoencoder model (VAE). The Bayesian Gaussian Mixture model is used to further detangle the latent space.
 
@@ -125,14 +144,25 @@
 * <i>random_seed</i> - data type - integer, must be equal to or more than 0
 * <i>print_report</i> - data type - boolean, default value is False
 * <i>metadata_path</i> - data type - string
 
 The metadata can contain any of the arguments above for each table. If so, the duplicated arguments from the CLI 
 will be ignored.
 
+<i>Note:</i> If you want to set the logging level, you can use the parameter <i>log_level</i> in the CLI call:
+
+```bash
+train --source STR --table_name STR --log_level STR
+train --metadata_path STR --log_level STR
+infer --size INT --table_name STR --log_level STR
+infer --metadata_path STR --log_level STR
+```
+
+where <i>log_level</i> might be one of the following values: <i>DEBUG, INFO, WARNING, ERROR, CRITICAL</i>.
+
 
 ### Linked tables generation
 
 To generate one or more tables, you might provide metadata in yaml format. By providing information about the relationships 
 between tables via metadata, it becomes possible to manage complex relationships across any number of tables. 
 You can also specify additional parameters needed for training and inference in the metadata file and in this case, 
 they will be ignored in the CLI call.
@@ -286,14 +316,30 @@
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-infer \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 ```
 
 You can add any arguments listed in the corresponding sections for infer and training processes in the CLI call, however, they will be 
 overwritten by corresponding arguments in the metadata file.
 
+#### Logging level
+
+Set the `LOGURU_LEVEL` environment variable to desired level of logging.
+For example, to suppress the debug messages, add `-e LOGURU_LEVEL=INFO` to the `docker run` command:
+```bash
+docker pull tdspora/syngen-train:latest
+docker run --rm -e LOGURU_LEVEL=INFO \
+  -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-train \
+  --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
+
+docker pull tdspora/syngen-infer:latest
+docker run --rm -e LOGURU_LEVEL=INFO \
+  -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-infer \
+  --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
+```
+
 ## Contribution
 
 We welcome contributions from the community to help us improve and maintain our public GitHub repository. We appreciate any feedback, bug reports, or feature requests, and we encourage developers to submit fixes or new features using issues.
 
 If you have found a bug or have a feature request, please submit an issue to our GitHub repository. Please provide as much detail as possible, including steps to reproduce the issue or a clear description of the feature request. Our team will review the issue and work with you to address any problems or discuss any potential new features.
 
 If you would like to contribute a fix or a new feature, please submit a pull request to our GitHub repository. Please make sure your code follows our coding standards and best practices. Our team will review your pull request and work with you to ensure that it meets our standards and is ready for inclusion in our codebase.
```

#### html2text {}

```diff
@@ -1,9 +1,19 @@
-# EPAM Syngen EPAM Syngen is an unsupervised tabular data generation tool. It
-is useful for generation of test data with a given table as a template. Most
+Metadata-Version: 2.1 Name: syngen Version: 0.1.6 Summary: The tool uncovers
+patterns, trends, and correlations hidden within your production datasets.
+Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
+Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
+data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
+Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
+Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
+GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Requires-
+Python: >3.7 Description-Content-Type: text/markdown License-File: LICENSE #
+EPAM Syngen EPAM Syngen is an unsupervised tabular data generation tool. It is
+useful for generation of test data with a given table as a template. Most
 datatypes including floats, integers, datetime, text, categorical, binary are
 supported. The linked tables i.e., tables sharing a key can also be generated
 using the simple statistical approach. The source of data might be in CSV, Avro
 format and should be located locally and be in UTF-8 encoding. The tool is
 based on the variational autoencoder model (VAE). The Bayesian Gaussian Mixture
 model is used to further detangle the latent space. ## Getting started Use pip
 to install the library: `pip install syngen` The training and inference
@@ -66,15 +76,20 @@
 Requirements for parameters of generation process: * size - data type -
 integer, must be equal to or more than 1, default value is 100 * table_name -
 data type - string * run_parallel - data type - boolean, default value is False
 * batch_size - data type - integer, must be equal to or more than 1 *
 random_seed - data type - integer, must be equal to or more than 0 *
 print_report - data type - boolean, default value is False * metadata_path -
 data type - string The metadata can contain any of the arguments above for each
-table. If so, the duplicated arguments from the CLI will be ignored. ### Linked
+table. If so, the duplicated arguments from the CLI will be ignored. Note: If
+you want to set the logging level, you can use the parameter log_level in the
+CLI call: ```bash train --source STR --table_name STR --log_level STR train --
+metadata_path STR --log_level STR infer --size INT --table_name STR --log_level
+STR infer --metadata_path STR --log_level STR ``` where log_level might be one
+of the following values: DEBUG, INFO, WARNING, ERROR, CRITICAL. ### Linked
 tables generation To generate one or more tables, you might provide metadata in
 yaml format. By providing information about the relationships between tables
 via metadata, it becomes possible to manage complex relationships across any
 number of tables. You can also specify additional parameters needed for
 training and inference in the metadata file and in this case, they will be
 ignored in the CLI call. Note: By using metadata file, you can also generate
 tables with absent relationships. In this case, the tables will be generated
@@ -153,21 +168,30 @@
 train:latest docker run --rm \ -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts
 tdspora/syngen-train \ --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 docker pull tdspora/syngen-infer:latest docker run --rm \ -
 v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-infer \ --
 metadata_path=./model_artifacts/PATH_TO_METADATA_YAML ``` You can add any
 arguments listed in the corresponding sections for infer and training processes
 in the CLI call, however, they will be overwritten by corresponding arguments
-in the metadata file. ## Contribution We welcome contributions from the
-community to help us improve and maintain our public GitHub repository. We
-appreciate any feedback, bug reports, or feature requests, and we encourage
-developers to submit fixes or new features using issues. If you have found a
-bug or have a feature request, please submit an issue to our GitHub repository.
-Please provide as much detail as possible, including steps to reproduce the
-issue or a clear description of the feature request. Our team will review the
-issue and work with you to address any problems or discuss any potential new
-features. If you would like to contribute a fix or a new feature, please submit
-a pull request to our GitHub repository. Please make sure your code follows our
-coding standards and best practices. Our team will review your pull request and
-work with you to ensure that it meets our standards and is ready for inclusion
-in our codebase. We appreciate your contributions and thank you for your
-interest in helping us maintain and improve our public GitHub repository.
+in the metadata file. #### Logging level Set the `LOGURU_LEVEL` environment
+variable to desired level of logging. For example, to suppress the debug
+messages, add `-e LOGURU_LEVEL=INFO` to the `docker run` command: ```bash
+docker pull tdspora/syngen-train:latest docker run --rm -e LOGURU_LEVEL=INFO \
+-v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-train \ --
+metadata_path=./model_artifacts/PATH_TO_METADATA_YAML docker pull tdspora/
+syngen-infer:latest docker run --rm -e LOGURU_LEVEL=INFO \ -
+v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-infer \ --
+metadata_path=./model_artifacts/PATH_TO_METADATA_YAML ``` ## Contribution We
+welcome contributions from the community to help us improve and maintain our
+public GitHub repository. We appreciate any feedback, bug reports, or feature
+requests, and we encourage developers to submit fixes or new features using
+issues. If you have found a bug or have a feature request, please submit an
+issue to our GitHub repository. Please provide as much detail as possible,
+including steps to reproduce the issue or a clear description of the feature
+request. Our team will review the issue and work with you to address any
+problems or discuss any potential new features. If you would like to contribute
+a fix or a new feature, please submit a pull request to our GitHub repository.
+Please make sure your code follows our coding standards and best practices. Our
+team will review your pull request and work with you to ensure that it meets
+our standards and is ready for inclusion in our codebase. We appreciate your
+contributions and thank you for your interest in helping us maintain and
+improve our public GitHub repository.
```

### Comparing `syngen-0.1.5/setup.cfg` & `syngen-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/infer.py` & `syngen-0.1.6/src/syngen/infer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional
 
 import click
 from loguru import logger
 
 from syngen.ml.worker import Worker
+from syngen.ml.utils import setup_logger
 
 
 @click.command()
 @click.option("--metadata_path", type=str, default=None, help="Path to the metadata file")
 @click.option("--size", default=100, type=click.IntRange(1),
               help="Desired number of rows to generate. If absent, it's defaulted to 100")
 @click.option("--table_name", default=None, type=str, help="Name of the table, same as in training")
@@ -18,44 +19,54 @@
               help="If specified, the generation is split into batches. This can save the RAM")
 @click.option("--random_seed", default=None, type=click.IntRange(0),
               help="Set any int in case you want reproducible results. To reproduce generated data again, "
                    "use the same int in this command.")
 @click.option("--print_report", default=False, type=click.BOOL,
               help="Whether to print quality report. Might require significant time "
                    "for big generated tables (>1000 rows). If absent, it's defaulted to False")
+@click.option("--log_level", default="INFO", type=click.Choice(["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]),
+              help="Set the logging level which will be used in the process. If absent, it's defaulted to 'INFO'")
 def launch_infer(
         metadata_path: Optional[str],
         size: Optional[int],
         table_name: Optional[str],
         run_parallel: bool,
         batch_size: Optional[int],
         print_report: bool,
-        random_seed: Optional[int]
+        random_seed: Optional[int],
+        log_level: str
 ):
     """
     Launch the work of infer process
     Parameters
     ----------
     metadata_path
     size
     table_name
     run_parallel
     batch_size
     print_report
     random_seed
+    log_level
     -------
 
     """
+    setup_logger(log_level)
     if not metadata_path and not table_name:
         raise AttributeError("It seems that the information of 'metadata_path' or 'table_name' is absent. "
                              "Please provide either the information of 'metadata_path' or the information of 'table_name'")
     if metadata_path and table_name:
         logger.warning("The information of 'metadata_path' was provided. "
                        "In this case the information of 'table_name' will be ignored")
         table_name = None
+    logger.warning(
+        "The inference process will be executed according to the information mentioned in 'infer_settings' "
+        "in the metadata file. If appropriate information is absent from the metadata file, then the values "
+        "of parameters sent through CLI will be used. Otherwise, the values of parameters will be defaulted"
+    )
     settings = {
         "size": size,
         "run_parallel": run_parallel,
         "batch_size": batch_size,
         "print_report": print_report,
         "random_seed": random_seed
     }
```

### Comparing `syngen-0.1.5/src/syngen/ml/config/configurations.py` & `syngen-0.1.6/src/syngen/ml/config/configurations.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/ml/convertor/convertor.py` & `syngen-0.1.6/src/syngen/ml/convertor/convertor.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.1.6/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/ml/metrics/__init__.py` & `syngen-0.1.6/src/syngen/ml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.1.6/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.1.6/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.1.6/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.1.6/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.1.6/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.1.6/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/ml/metrics/utils.py` & `syngen-0.1.6/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/ml/reporters/reporters.py` & `syngen-0.1.6/src/syngen/ml/reporters/reporters.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/ml/strategies/strategies.py` & `syngen-0.1.6/src/syngen/ml/strategies/strategies.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/ml/train_chain/train_chain.py` & `syngen-0.1.6/src/syngen/ml/train_chain/train_chain.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/ml/utils/utils.py` & `syngen-0.1.6/src/syngen/ml/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import List, Dict
 from dateutil.parser import parse
 import pickle
 from datetime import datetime, timedelta
+import sys
 
 import pandas as pd
 import numpy as np
 from slugify import slugify
 from loguru import logger
 import pickle as pkl
 import uuid
 from ulid import ULID
-from uuid import UUID
 import random
 
 def generate_uuids(version: int, size: int):
     ulid = ULID()
     generated_uuid_column = []
     for i in range(size):
         if version != "ulid":
@@ -202,7 +202,15 @@
 
 def fetch_training_config(train_config_pickle_path):
     """
     Fetch the parameters of the training configuration
     """
     with open(train_config_pickle_path, "rb") as f:
         return pkl.load(f)
+
+def setup_logger(log_level: str):
+    """
+    Setup logger depending on the log level
+    :param log_level: the level of logging
+    """
+    logger.remove()
+    logger.add(sys.stdout, level=log_level)
```

### Comparing `syngen-0.1.5/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.1.6/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/ml/vae/models/dataset.py` & `syngen-0.1.6/src/syngen/ml/vae/models/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import base32_crockford
 
 from loguru import logger
 import numpy as np
 import dill
 import pandas as pd
 from scipy.stats import gaussian_kde
+import tqdm
 
 from syngen.ml.vae.models.features import (
     CategoricalFeature,
     CharBasedTextFeature,
     ContinuousFeature,
     DateFeature,
     BinaryFeature,
@@ -500,15 +501,18 @@
     def inverse_transform(self, data, excluded_features=set()):
         inverse_transformed_data = list()
         column_names = list()
         if not isinstance(data, list):
             data = [data]
         assert self._check_count_features(data)
 
-        for transformed_data, (name, feature) in zip(data, self.features.items()):
+        for transformed_data, (name, feature) in tqdm.tqdm(
+                iterable=zip(data, self.features.items()),
+                desc="Generation of the data...",
+                total=len(data)):
             if name not in excluded_features and name not in self.fk_columns:
                 column_names.extend(self.columns[name])
                 inverse_transformed_data.append(
                     feature.inverse_transform(transformed_data)
                 )
 
         stacked_data = np.column_stack(inverse_transformed_data)
```

### Comparing `syngen-0.1.5/src/syngen/ml/vae/models/features.py` & `syngen-0.1.6/src/syngen/ml/vae/models/features.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/ml/vae/models/model.py` & `syngen-0.1.6/src/syngen/ml/vae/models/model.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.1.6/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/ml/validation_schema/validation_schema.py` & `syngen-0.1.6/src/syngen/ml/validation_schema/validation_schema.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/ml/worker/worker.py` & `syngen-0.1.6/src/syngen/ml/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.5/src/syngen/train.py` & `syngen-0.1.6/src/syngen/train.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'
 
 import click
 from loguru import logger
 
 from syngen.ml.worker import Worker
+from syngen.ml.utils import setup_logger
 
 
 @click.command()
 @click.option("--metadata_path", type=str, default=None, help="Path to the metadata file")
 @click.option("--source", type=str, default=None, help="Path to the table that you want to use as a reference")
 @click.option("--table_name", type=str, default=None, help="Arbitrary string to name the directories")
 @click.option("--epochs", default=10, type=click.IntRange(1),
@@ -19,42 +20,47 @@
                    "If absent, it's defaulted to False")
 @click.option("--row_limit", default=None, type=click.IntRange(1),
               help="Number of rows to train over. A number less than the original table length will randomly subset "
                    "the specified rows number")
 @click.option("--print_report", default=False, type=click.BOOL,
               help="Whether to print quality report. Might require significant time "
                    "for big generated tables (>1000 rows). If absent, it's defaulted to False")
+@click.option("--log_level", default="INFO", type=click.Choice(["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]),
+              help="Set the logging level which will be used in the process. If absent, it's defaulted to 'INFO'")
 @click.option("--batch_size", default=32, type=click.IntRange(1),
               help="Number of rows that goes in one batch. This parameter can help to control memory consumption.")
 def launch_train(
     metadata_path: Optional[str],
     source: Optional[str],
     table_name: Optional[str],
     epochs: int,
     drop_null: bool,
     row_limit: Optional[int],
     print_report: bool,
+    log_level: str,
     batch_size: int = 32,
 ):
     """
     Launch the work of training process
 
     Parameters
     ----------
     metadata_path
     source
     table_name
     epochs
     drop_null
     row_limit
     print_report
+    log_level
     batch_size
     -------
 
     """
+    setup_logger(log_level)
     if not metadata_path and not source and not table_name:
         raise AttributeError("It seems that the information of 'metadata_path' or 'table_name' and 'source' is absent. "
                              "Please provide either the information of 'metadata_path' or "
                              "the information of 'source' and 'table_name'")
     elif metadata_path and table_name and source:
         logger.warning("The information of 'metadata_path' was provided. "
                        "In this case the information of 'table_name' and 'source' will be ignored")
@@ -70,14 +76,19 @@
         raise AttributeError("It seems that the information of 'metadata_path' or 'table_name' is absent. "
                              "Please provide either the information of 'metadata_path' or "
                              "the information of 'source' and 'table_name'")
     elif table_name and not source:
         raise AttributeError("It seems that the information of 'metadata_path' or 'source' is absent. "
                              "Please provide either the information of 'metadata_path' or "
                              "the information of 'source' and 'table_name'")
+    logger.warning(
+        "The training process will be executed according to the information mentioned in 'train_settings' "
+        "in the metadata file. If appropriate information is absent from the metadata file, then the values "
+        "of parameters sent through CLI will be used. Otherwise, the values of parameters will be defaulted"
+    )
     settings = {
         "source": source,
         "epochs": epochs,
         "drop_null": drop_null,
         "row_limit": row_limit,
         "batch_size": batch_size,
         "print_report": print_report
```

### Comparing `syngen-0.1.5/src/syngen.egg-info/PKG-INFO` & `syngen-0.1.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: syngen
-Version: 0.1.5
-Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
-Home-page: https://github.com/tdspora/syngen
-Author: EPAM Systems, Inc.
-Maintainer: Pavel Bobyrev
-License: GPLv3 License
-Keywords: data,generation,synthetic,vae,tabular
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # EPAM Syngen
 
 EPAM Syngen is an unsupervised tabular data generation tool. It is useful for generation of test data with a given table as a template. Most datatypes including floats, integers, datetime, text, categorical, binary are supported. The linked tables i.e., tables sharing a key can also be generated using the simple statistical approach. 
 The source of data might be in CSV, Avro format and should be located locally and be in UTF-8 encoding.
 
 The tool is based on the variational autoencoder model (VAE). The Bayesian Gaussian Mixture model is used to further detangle the latent space.
 
@@ -144,14 +125,25 @@
 * <i>random_seed</i> - data type - integer, must be equal to or more than 0
 * <i>print_report</i> - data type - boolean, default value is False
 * <i>metadata_path</i> - data type - string
 
 The metadata can contain any of the arguments above for each table. If so, the duplicated arguments from the CLI 
 will be ignored.
 
+<i>Note:</i> If you want to set the logging level, you can use the parameter <i>log_level</i> in the CLI call:
+
+```bash
+train --source STR --table_name STR --log_level STR
+train --metadata_path STR --log_level STR
+infer --size INT --table_name STR --log_level STR
+infer --metadata_path STR --log_level STR
+```
+
+where <i>log_level</i> might be one of the following values: <i>DEBUG, INFO, WARNING, ERROR, CRITICAL</i>.
+
 
 ### Linked tables generation
 
 To generate one or more tables, you might provide metadata in yaml format. By providing information about the relationships 
 between tables via metadata, it becomes possible to manage complex relationships across any number of tables. 
 You can also specify additional parameters needed for training and inference in the metadata file and in this case, 
 they will be ignored in the CLI call.
@@ -305,14 +297,30 @@
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-infer \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 ```
 
 You can add any arguments listed in the corresponding sections for infer and training processes in the CLI call, however, they will be 
 overwritten by corresponding arguments in the metadata file.
 
+#### Logging level
+
+Set the `LOGURU_LEVEL` environment variable to desired level of logging.
+For example, to suppress the debug messages, add `-e LOGURU_LEVEL=INFO` to the `docker run` command:
+```bash
+docker pull tdspora/syngen-train:latest
+docker run --rm -e LOGURU_LEVEL=INFO \
+  -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-train \
+  --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
+
+docker pull tdspora/syngen-infer:latest
+docker run --rm -e LOGURU_LEVEL=INFO \
+  -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-infer \
+  --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
+```
+
 ## Contribution
 
 We welcome contributions from the community to help us improve and maintain our public GitHub repository. We appreciate any feedback, bug reports, or feature requests, and we encourage developers to submit fixes or new features using issues.
 
 If you have found a bug or have a feature request, please submit an issue to our GitHub repository. Please provide as much detail as possible, including steps to reproduce the issue or a clear description of the feature request. Our team will review the issue and work with you to address any problems or discuss any potential new features.
 
 If you would like to contribute a fix or a new feature, please submit a pull request to our GitHub repository. Please make sure your code follows our coding standards and best practices. Our team will review your pull request and work with you to ensure that it meets our standards and is ready for inclusion in our codebase.
```

#### html2text {}

```diff
@@ -1,19 +1,9 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.1.5 Summary: The tool uncovers
-patterns, trends, and correlations hidden within your production datasets.
-Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
-Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
-data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
-Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
-Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
-GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Requires-
-Python: >3.7 Description-Content-Type: text/markdown License-File: LICENSE #
-EPAM Syngen EPAM Syngen is an unsupervised tabular data generation tool. It is
-useful for generation of test data with a given table as a template. Most
+# EPAM Syngen EPAM Syngen is an unsupervised tabular data generation tool. It
+is useful for generation of test data with a given table as a template. Most
 datatypes including floats, integers, datetime, text, categorical, binary are
 supported. The linked tables i.e., tables sharing a key can also be generated
 using the simple statistical approach. The source of data might be in CSV, Avro
 format and should be located locally and be in UTF-8 encoding. The tool is
 based on the variational autoencoder model (VAE). The Bayesian Gaussian Mixture
 model is used to further detangle the latent space. ## Getting started Use pip
 to install the library: `pip install syngen` The training and inference
@@ -76,15 +66,20 @@
 Requirements for parameters of generation process: * size - data type -
 integer, must be equal to or more than 1, default value is 100 * table_name -
 data type - string * run_parallel - data type - boolean, default value is False
 * batch_size - data type - integer, must be equal to or more than 1 *
 random_seed - data type - integer, must be equal to or more than 0 *
 print_report - data type - boolean, default value is False * metadata_path -
 data type - string The metadata can contain any of the arguments above for each
-table. If so, the duplicated arguments from the CLI will be ignored. ### Linked
+table. If so, the duplicated arguments from the CLI will be ignored. Note: If
+you want to set the logging level, you can use the parameter log_level in the
+CLI call: ```bash train --source STR --table_name STR --log_level STR train --
+metadata_path STR --log_level STR infer --size INT --table_name STR --log_level
+STR infer --metadata_path STR --log_level STR ``` where log_level might be one
+of the following values: DEBUG, INFO, WARNING, ERROR, CRITICAL. ### Linked
 tables generation To generate one or more tables, you might provide metadata in
 yaml format. By providing information about the relationships between tables
 via metadata, it becomes possible to manage complex relationships across any
 number of tables. You can also specify additional parameters needed for
 training and inference in the metadata file and in this case, they will be
 ignored in the CLI call. Note: By using metadata file, you can also generate
 tables with absent relationships. In this case, the tables will be generated
@@ -163,21 +158,30 @@
 train:latest docker run --rm \ -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts
 tdspora/syngen-train \ --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 docker pull tdspora/syngen-infer:latest docker run --rm \ -
 v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-infer \ --
 metadata_path=./model_artifacts/PATH_TO_METADATA_YAML ``` You can add any
 arguments listed in the corresponding sections for infer and training processes
 in the CLI call, however, they will be overwritten by corresponding arguments
-in the metadata file. ## Contribution We welcome contributions from the
-community to help us improve and maintain our public GitHub repository. We
-appreciate any feedback, bug reports, or feature requests, and we encourage
-developers to submit fixes or new features using issues. If you have found a
-bug or have a feature request, please submit an issue to our GitHub repository.
-Please provide as much detail as possible, including steps to reproduce the
-issue or a clear description of the feature request. Our team will review the
-issue and work with you to address any problems or discuss any potential new
-features. If you would like to contribute a fix or a new feature, please submit
-a pull request to our GitHub repository. Please make sure your code follows our
-coding standards and best practices. Our team will review your pull request and
-work with you to ensure that it meets our standards and is ready for inclusion
-in our codebase. We appreciate your contributions and thank you for your
-interest in helping us maintain and improve our public GitHub repository.
+in the metadata file. #### Logging level Set the `LOGURU_LEVEL` environment
+variable to desired level of logging. For example, to suppress the debug
+messages, add `-e LOGURU_LEVEL=INFO` to the `docker run` command: ```bash
+docker pull tdspora/syngen-train:latest docker run --rm -e LOGURU_LEVEL=INFO \
+-v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-train \ --
+metadata_path=./model_artifacts/PATH_TO_METADATA_YAML docker pull tdspora/
+syngen-infer:latest docker run --rm -e LOGURU_LEVEL=INFO \ -
+v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-infer \ --
+metadata_path=./model_artifacts/PATH_TO_METADATA_YAML ``` ## Contribution We
+welcome contributions from the community to help us improve and maintain our
+public GitHub repository. We appreciate any feedback, bug reports, or feature
+requests, and we encourage developers to submit fixes or new features using
+issues. If you have found a bug or have a feature request, please submit an
+issue to our GitHub repository. Please provide as much detail as possible,
+including steps to reproduce the issue or a clear description of the feature
+request. Our team will review the issue and work with you to address any
+problems or discuss any potential new features. If you would like to contribute
+a fix or a new feature, please submit a pull request to our GitHub repository.
+Please make sure your code follows our coding standards and best practices. Our
+team will review your pull request and work with you to ensure that it meets
+our standards and is ready for inclusion in our codebase. We appreciate your
+contributions and thank you for your interest in helping us maintain and
+improve our public GitHub repository.
```

### Comparing `syngen-0.1.5/src/syngen.egg-info/SOURCES.txt` & `syngen-0.1.6/src/syngen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

