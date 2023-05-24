# Comparing `tmp/rattr-0.1.4.tar.gz` & `tmp/rattr-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rattr-0.1.4.tar", last modified: Wed Mar  1 14:05:39 2023, max compression
+gzip compressed data, was "rattr-0.1.5.tar", last modified: Wed May 24 13:49:36 2023, max compression
```

## Comparing `rattr-0.1.4.tar` & `rattr-0.1.5.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:39.718534 rattr-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:39.706534 rattr-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:39.710534 rattr-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-01 14:05:23.000000 rattr-0.1.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-03-01 14:05:23.000000 rattr-0.1.4/.github/workflows/staticanalysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-01 14:05:23.000000 rattr-0.1.4/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-01 14:05:23.000000 rattr-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-01 14:05:23.000000 rattr-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-01 14:05:23.000000 rattr-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-03-01 14:05:39.718534 rattr-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-03-01 14:05:23.000000 rattr-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:39.710534 rattr-0.1.4/rattr/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-01 14:05:39.000000 rattr-0.1.4/rattr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:39.714534 rattr-0.1.4/rattr/analyser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/analyser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/analyser/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/analyser/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/analyser/cls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:39.714534 rattr-0.1.4/rattr/analyser/context/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/analyser/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20909 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/analyser/context/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/analyser/context/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/analyser/context/symbol_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/analyser/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17963 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/analyser/function.py
--rw-r--r--   0 runner    (1001) docker     (123)    10901 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/analyser/ir_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/analyser/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/analyser/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    33180 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/analyser/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:39.714534 rattr-0.1.4/rattr/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/cli/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    22526 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/cli/toml_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/cli/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:39.714534 rattr-0.1.4/rattr/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:39.714534 rattr-0.1.4/rattr/error/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/error/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:39.714534 rattr-0.1.4/rattr/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:39.714534 rattr-0.1.4/rattr/plugins/analysers/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/plugins/analysers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/plugins/analysers/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/plugins/analysers/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:39.714534 rattr-0.1.4/rattr/plugins/assertors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/plugins/assertors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-03-01 14:05:23.000000 rattr-0.1.4/rattr/plugins/assertors/import_clobbering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:39.710534 rattr-0.1.4/rattr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-03-01 14:05:39.000000 rattr-0.1.4/rattr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-03-01 14:05:39.000000 rattr-0.1.4/rattr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 14:05:39.000000 rattr-0.1.4/rattr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-01 14:05:39.000000 rattr-0.1.4/rattr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-01 14:05:39.000000 rattr-0.1.4/rattr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-01 14:05:39.000000 rattr-0.1.4/rattr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-01 14:05:23.000000 rattr-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-01 14:05:39.718534 rattr-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-03-01 14:05:23.000000 rattr-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:39.718534 rattr-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20806 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:39.718534 rattr-0.1.4/tests/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28992 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/context/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/context/test_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/context/test_symbol_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:39.718534 rattr-0.1.4/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:39.718534 rattr-0.1.4/tests/plugins/analysers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/plugins/analysers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/plugins/analysers/test_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/plugins/analysers/test_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:39.718534 rattr-0.1.4/tests/plugins/assertors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/plugins/assertors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15049 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/plugins/assertors/test_import_clobbering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:39.718534 rattr-0.1.4/tests/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/snippets/not_a_py.file
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/snippets/rattr_full_one.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/snippets/rattr_results_one.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/snippets/rattr_results_two.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/test_analysers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/test_bin.py
--rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/test_cls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    17199 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/test_ir_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/test_rattr.py
--rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/test_regressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    43225 2023-03-01 14:05:23.000000 rattr-0.1.4/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.581004 rattr-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.565003 rattr-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.569003 rattr-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-24 13:49:14.000000 rattr-0.1.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-24 13:49:14.000000 rattr-0.1.5/.github/workflows/staticanalysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-24 13:49:14.000000 rattr-0.1.5/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-24 13:49:14.000000 rattr-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-24 13:49:14.000000 rattr-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 13:49:14.000000 rattr-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-05-24 13:49:36.581004 rattr-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-05-24 13:49:14.000000 rattr-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.569003 rattr-0.1.5/rattr/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-24 13:49:36.000000 rattr-0.1.5/rattr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.573003 rattr-0.1.5/rattr/analyser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/cls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.573003 rattr-0.1.5/rattr/analyser/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20909 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/context/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/context/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/context/symbol_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17963 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10901 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/ir_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33184 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.573003 rattr-0.1.5/rattr/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/cli/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22526 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/cli/toml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/cli/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.573003 rattr-0.1.5/rattr/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.573003 rattr-0.1.5/rattr/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/error/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.573003 rattr-0.1.5/rattr/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.577004 rattr-0.1.5/rattr/plugins/analysers/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/plugins/analysers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/plugins/analysers/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/plugins/analysers/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.577004 rattr-0.1.5/rattr/plugins/assertors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/plugins/assertors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/plugins/assertors/import_clobbering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.573003 rattr-0.1.5/rattr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-05-24 13:49:36.000000 rattr-0.1.5/rattr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-24 13:49:36.000000 rattr-0.1.5/rattr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:49:36.000000 rattr-0.1.5/rattr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 13:49:36.000000 rattr-0.1.5/rattr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-24 13:49:36.000000 rattr-0.1.5/rattr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 13:49:36.000000 rattr-0.1.5/rattr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 13:49:14.000000 rattr-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-24 13:49:36.581004 rattr-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-24 13:49:14.000000 rattr-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.577004 rattr-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20806 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.577004 rattr-0.1.5/tests/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28992 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/context/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/context/test_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/context/test_symbol_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.577004 rattr-0.1.5/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.581004 rattr-0.1.5/tests/plugins/analysers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/plugins/analysers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/plugins/analysers/test_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/plugins/analysers/test_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.581004 rattr-0.1.5/tests/plugins/assertors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/plugins/assertors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15049 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/plugins/assertors/test_import_clobbering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.581004 rattr-0.1.5/tests/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/snippets/not_a_py.file
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/snippets/rattr_full_one.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/snippets/rattr_results_one.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/snippets/rattr_results_two.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_analysers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17199 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_ir_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_rattr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43225 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_util.py
```

### Comparing `rattr-0.1.4/.github/workflows/publish.yml` & `rattr-0.1.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/.github/workflows/staticanalysis.yml` & `rattr-0.1.5/.github/workflows/staticanalysis.yml`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/.github/workflows/tests.yml` & `rattr-0.1.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/.gitignore` & `rattr-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/LICENSE` & `rattr-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/PKG-INFO` & `rattr-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattr
-Version: 0.1.4
+Version: 0.1.5
 Summary: Rattr rats on your attrs.
 Home-page: https://github.com/SuadeLabs/ratter
 Author: Suade Labs
 License: MIT
 Keywords: automation linting type-checking attributes rats
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `rattr-0.1.4/README.md` & `rattr-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/__main__.py` & `rattr-0.1.5/rattr/__main__.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/analyser/annotations.py` & `rattr-0.1.5/rattr/analyser/annotations.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/analyser/base.py` & `rattr-0.1.5/rattr/analyser/base.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/analyser/cls.py` & `rattr-0.1.5/rattr/analyser/cls.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/analyser/context/context.py` & `rattr-0.1.5/rattr/analyser/context/context.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/analyser/context/symbol.py` & `rattr-0.1.5/rattr/analyser/context/symbol.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/analyser/context/symbol_table.py` & `rattr-0.1.5/rattr/analyser/context/symbol_table.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/analyser/file.py` & `rattr-0.1.5/rattr/analyser/file.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/analyser/function.py` & `rattr-0.1.5/rattr/analyser/function.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/analyser/ir_dag.py` & `rattr-0.1.5/rattr/analyser/ir_dag.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/analyser/results.py` & `rattr-0.1.5/rattr/analyser/results.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/analyser/types.py` & `rattr-0.1.5/rattr/analyser/types.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/analyser/util.py` & `rattr-0.1.5/rattr/analyser/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     Optional,
     Set,
     Tuple,
     Type,
     Union,
 )
 
-from isort import place_module
+from isort.api import place_module
 
 from rattr import config, error
 from rattr.analyser.context.symbol import get_possible_module_names  # noqa
 from rattr.analyser.context.symbol import (
     Class,
     Import,
     Name,
```

### Comparing `rattr-0.1.4/rattr/cli/argparse.py` & `rattr-0.1.5/rattr/cli/argparse.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/cli/parser.py` & `rattr-0.1.5/rattr/cli/parser.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/cli/toml_parser.py` & `rattr-0.1.5/rattr/cli/toml_parser.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/cli/util.py` & `rattr-0.1.5/rattr/cli/util.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/config/__init__.py` & `rattr-0.1.5/rattr/config/__init__.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/error/error.py` & `rattr-0.1.5/rattr/error/error.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/plugins/__init__.py` & `rattr-0.1.5/rattr/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/plugins/analysers/builtins.py` & `rattr-0.1.5/rattr/plugins/analysers/builtins.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/plugins/analysers/collections.py` & `rattr-0.1.5/rattr/plugins/analysers/collections.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr/plugins/assertors/import_clobbering.py` & `rattr-0.1.5/rattr/plugins/assertors/import_clobbering.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/rattr.egg-info/PKG-INFO` & `rattr-0.1.5/rattr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattr
-Version: 0.1.4
+Version: 0.1.5
 Summary: Rattr rats on your attrs.
 Home-page: https://github.com/SuadeLabs/ratter
 Author: Suade Labs
 License: MIT
 Keywords: automation linting type-checking attributes rats
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `rattr-0.1.4/rattr.egg-info/SOURCES.txt` & `rattr-0.1.5/rattr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/setup.py` & `rattr-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/tests/conftest.py` & `rattr-0.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/tests/context/test_context.py` & `rattr-0.1.5/tests/context/test_context.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/tests/context/test_symbol.py` & `rattr-0.1.5/tests/context/test_symbol.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/tests/context/test_symbol_table.py` & `rattr-0.1.5/tests/context/test_symbol_table.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/tests/plugins/analysers/test_builtins.py` & `rattr-0.1.5/tests/plugins/analysers/test_builtins.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/tests/plugins/analysers/test_collections.py` & `rattr-0.1.5/tests/plugins/analysers/test_collections.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/tests/plugins/assertors/test_import_clobbering.py` & `rattr-0.1.5/tests/plugins/assertors/test_import_clobbering.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/tests/snippets/rattr_full_one.py` & `rattr-0.1.5/tests/snippets/rattr_full_one.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/tests/test_analysers.py` & `rattr-0.1.5/tests/test_analysers.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/tests/test_base.py` & `rattr-0.1.5/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/tests/test_cls.py` & `rattr-0.1.5/tests/test_cls.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/tests/test_error.py` & `rattr-0.1.5/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/tests/test_file.py` & `rattr-0.1.5/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/tests/test_function.py` & `rattr-0.1.5/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/tests/test_ir_dag.py` & `rattr-0.1.5/tests/test_ir_dag.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/tests/test_parser.py` & `rattr-0.1.5/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/tests/test_rattr.py` & `rattr-0.1.5/tests/test_rattr.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/tests/test_regressions.py` & `rattr-0.1.5/tests/test_regressions.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/tests/test_results.py` & `rattr-0.1.5/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.4/tests/test_util.py` & `rattr-0.1.5/tests/test_util.py`

 * *Files identical despite different names*

