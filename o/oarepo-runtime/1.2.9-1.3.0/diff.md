# Comparing `tmp/oarepo-runtime-1.2.9.tar.gz` & `tmp/oarepo-runtime-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-runtime-1.2.9.tar", last modified: Thu Mar 16 11:57:58 2023, max compression
+gzip compressed data, was "oarepo-runtime-1.3.0.tar", last modified: Wed May 24 11:31:27 2023, max compression
```

## Comparing `oarepo-runtime-1.2.9.tar` & `oarepo-runtime-1.3.0.tar`

### file list

```diff
@@ -1,76 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:57:58.646314 oarepo-runtime-1.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-03-16 11:57:58.646314 oarepo-runtime-1.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:57:58.618313 oarepo-runtime-1.2.9/oarepo_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:57:58.622313 oarepo-runtime-1.2.9/oarepo_runtime/cf/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/cf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/cf/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/cf/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:57:58.626313 oarepo-runtime-1.2.9/oarepo_runtime/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/config/permissions_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/config/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:57:58.630313 oarepo-runtime-1.2.9/oarepo_runtime/datastreams/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/datastreams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/datastreams/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/datastreams/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/datastreams/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/datastreams/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/datastreams/datastreams.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/datastreams/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/datastreams/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:57:58.634314 oarepo-runtime-1.2.9/oarepo_runtime/datastreams/readers/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/datastreams/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/datastreams/readers/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/datastreams/readers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/datastreams/readers/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/datastreams/readers/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/datastreams/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:57:58.634314 oarepo-runtime-1.2.9/oarepo_runtime/datastreams/writers/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/datastreams/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/datastreams/writers/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/datastreams/writers/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:57:58.634314 oarepo-runtime-1.2.9/oarepo_runtime/expansions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/expansions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/expansions/expandable_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/expansions/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/ext_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:57:58.638314 oarepo-runtime-1.2.9/oarepo_runtime/facets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/facets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/facets/max_facet.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/facets/nested_facet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:57:58.638314 oarepo-runtime-1.2.9/oarepo_runtime/i18n/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/i18n/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/i18n/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/i18n/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:57:58.642314 oarepo-runtime-1.2.9/oarepo_runtime/relations/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/relations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/relations/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/relations/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/relations/lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/relations/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/relations/pid_relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:57:58.642314 oarepo-runtime-1.2.9/oarepo_runtime/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/tasks/datastreams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:57:58.642314 oarepo-runtime-1.2.9/oarepo_runtime/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/ui/marshmallow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:57:58.646314 oarepo-runtime-1.2.9/oarepo_runtime/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/oarepo_runtime/validation/dates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:57:58.622313 oarepo-runtime-1.2.9/oarepo_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-03-16 11:57:58.000000 oarepo-runtime-1.2.9/oarepo_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-03-16 11:57:58.000000 oarepo-runtime-1.2.9/oarepo_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 11:57:58.000000 oarepo-runtime-1.2.9/oarepo_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-16 11:57:58.000000 oarepo-runtime-1.2.9/oarepo_runtime.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-16 11:57:58.000000 oarepo-runtime-1.2.9/oarepo_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-16 11:57:58.000000 oarepo-runtime-1.2.9/oarepo_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-03-16 11:57:58.646314 oarepo-runtime-1.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-16 11:54:23.000000 oarepo-runtime-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.042367 oarepo-runtime-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-24 11:31:27.042367 oarepo-runtime-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.022367 oarepo-runtime-1.3.0/oarepo_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.026367 oarepo-runtime-1.3.0/oarepo_runtime/cf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/cf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/cf/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/cf/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.026367 oarepo-runtime-1.3.0/oarepo_runtime/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/cli/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/cli/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/cli/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.026367 oarepo-runtime-1.3.0/oarepo_runtime/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/config/permissions_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/config/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.030367 oarepo-runtime-1.3.0/oarepo_runtime/datastreams/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/datastreams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/datastreams/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/datastreams/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/datastreams/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/datastreams/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/datastreams/datastreams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/datastreams/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/datastreams/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.030367 oarepo-runtime-1.3.0/oarepo_runtime/datastreams/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/datastreams/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/datastreams/readers/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/datastreams/readers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/datastreams/readers/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/datastreams/readers/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/datastreams/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.034367 oarepo-runtime-1.3.0/oarepo_runtime/datastreams/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/datastreams/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/datastreams/writers/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/datastreams/writers/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.034367 oarepo-runtime-1.3.0/oarepo_runtime/expansions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/expansions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/expansions/expandable_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/expansions/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/ext_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.034367 oarepo-runtime-1.3.0/oarepo_runtime/facets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/facets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/facets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/facets/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/facets/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/facets/max_facet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/facets/nested_facet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.038367 oarepo-runtime-1.3.0/oarepo_runtime/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/i18n/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/i18n/default_translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/i18n/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/i18n/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/i18n/ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/i18n/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/polymorphic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.038367 oarepo-runtime-1.3.0/oarepo_runtime/relations/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/relations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/relations/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/relations/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/relations/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/relations/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/relations/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/relations/pid_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/relations/uow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.038367 oarepo-runtime-1.3.0/oarepo_runtime/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/resolvers/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.038367 oarepo-runtime-1.3.0/oarepo_runtime/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/tasks/datastreams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.038367 oarepo-runtime-1.3.0/oarepo_runtime/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.018367 oarepo-runtime-1.3.0/oarepo_runtime/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.038367 oarepo-runtime-1.3.0/oarepo_runtime/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.018367 oarepo-runtime-1.3.0/oarepo_runtime/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.038367 oarepo-runtime-1.3.0/oarepo_runtime/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.038367 oarepo-runtime-1.3.0/oarepo_runtime/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/ui/marshmallow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.042367 oarepo-runtime-1.3.0/oarepo_runtime/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/oarepo_runtime/validation/dates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:31:27.022367 oarepo-runtime-1.3.0/oarepo_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-24 11:31:26.000000 oarepo-runtime-1.3.0/oarepo_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-24 11:31:26.000000 oarepo-runtime-1.3.0/oarepo_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:31:26.000000 oarepo-runtime-1.3.0/oarepo_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-24 11:31:26.000000 oarepo-runtime-1.3.0/oarepo_runtime.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-24 11:31:26.000000 oarepo-runtime-1.3.0/oarepo_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 11:31:26.000000 oarepo-runtime-1.3.0/oarepo_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-24 11:31:27.042367 oarepo-runtime-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-24 11:27:47.000000 oarepo-runtime-1.3.0/setup.py
```

### Comparing `oarepo-runtime-1.2.9/LICENSE` & `oarepo-runtime-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/PKG-INFO` & `oarepo-runtime-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-runtime
-Version: 1.2.9
+Version: 1.3.0
 Summary: A set of runtime extensions of Invenio repository
 Description-Content-Type: text/markdown
 Provides-Extra: devs
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo runtime
```

### Comparing `oarepo-runtime-1.2.9/README.md` & `oarepo-runtime-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/cf/__init__.py` & `oarepo-runtime-1.3.0/oarepo_runtime/cf/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/cf/cli.py` & `oarepo-runtime-1.3.0/oarepo_runtime/cf/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/cf/mappings.py` & `oarepo-runtime-1.3.0/oarepo_runtime/cf/mappings.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/config/permissions_presets.py` & `oarepo-runtime-1.3.0/oarepo_runtime/config/permissions_presets.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,44 @@
 from invenio_records_permissions import RecordPermissionPolicy
 from invenio_records_permissions.generators import AnyUser, SystemProcess
 
 
+class OaiHarvesterPermissionPolicy(RecordPermissionPolicy):
+    """record policy for oai harvester (by default same as read only)"""
+
+    can_search = [SystemProcess(), AnyUser()]
+    can_read = [SystemProcess(), AnyUser()]
+    can_create = [SystemProcess()]
+    can_update = [SystemProcess()]
+    can_delete = [SystemProcess()]
+    can_manage = [SystemProcess()]
+
+    can_create_files = [SystemProcess()]
+    can_set_content_files = [SystemProcess()]
+    can_get_content_files = [AnyUser(), SystemProcess()]
+    can_commit_files = [SystemProcess()]
+    can_read_files = [AnyUser(), SystemProcess()]
+    can_update_files = [SystemProcess()]
+    can_delete_files = [SystemProcess()]
+
+    can_edit = [SystemProcess()]
+    can_new_version = [SystemProcess()]
+    can_search_drafts = [SystemProcess()]
+    can_read_draft = [SystemProcess()]
+    can_update_draft = [SystemProcess()]
+    can_delete_draft = [SystemProcess()]
+    can_publish = [SystemProcess()]
+    can_draft_create_files = [SystemProcess()]
+    can_draft_set_content_files = [SystemProcess()]
+    can_draft_get_content_files = [SystemProcess()]
+    can_draft_commit_files = [SystemProcess()]
+    can_draft_read_files = [SystemProcess()]
+    can_draft_update_files = [SystemProcess()]
+
+
 class ReadOnlyPermissionPolicy(RecordPermissionPolicy):
     """record policy for read only repository"""
 
     can_search = [SystemProcess(), AnyUser()]
     can_read = [SystemProcess(), AnyUser()]
     can_create = [SystemProcess()]
     can_update = [SystemProcess()]
```

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/datastreams/__init__.py` & `oarepo-runtime-1.3.0/oarepo_runtime/datastreams/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #
 #
 # These files were taken and adapted from invenio-vocabularies and adapted so that they can be used
 # to
 #
 #
+from .batch import StreamBatch
 from .catalogue import DataStreamCatalogue
 from .datastreams import DataStream, DataStreamResult, StreamEntry
 from .errors import DataStreamCatalogueError, ReaderError, TransformerError, WriterError
 from .readers import BaseReader
 from .transformers import BaseTransformer
 from .writers import BaseWriter
 
@@ -19,8 +20,9 @@
     "BaseReader",
     "BaseWriter",
     "BaseTransformer",
     "DataStreamCatalogueError",
     "ReaderError",
     "WriterError",
     "TransformerError",
+    "StreamBatch",
 ]
```

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/datastreams/catalogue.py` & `oarepo-runtime-1.3.0/oarepo_runtime/datastreams/catalogue.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from pathlib import Path
 
 import yaml
 from flask import current_app
+from invenio_access.permissions import system_identity
 
 from .config import get_instance
 from .datastreams import DataStream
 from .errors import DataStreamCatalogueError
 
 
 class DataStreamCatalogue:
-    def __init__(self, catalogue, content=None) -> None:
+    def __init__(self, catalogue, content=None, identity=system_identity) -> None:
         """
         Catalogue of data streams. The catalogue contains a dict of:
         stream_name: stream_definition, where stream definition is an array of:
 
         - reader: reader_class
           <rest of parameters go to reader constructor>
         - transformer: transformer_class
@@ -30,14 +31,15 @@
         """
         self._catalogue_path = Path(catalogue)
         if content:
             self._catalogue = content
         else:
             with open(catalogue) as f:
                 self._catalogue = yaml.safe_load(f)
+        self.identity = identity
 
     @property
     def path(self):
         return self._catalogue_path
 
     @property
     def directory(self):
@@ -61,32 +63,35 @@
                 if "reader" in entry:
                     readers.append(
                         get_instance(
                             "DATASTREAMS_READERS",
                             "reader",
                             entry,
                             base_path=self.directory,
+                            identity=self.identity,
                         )
                     )
                 elif "transformer" in entry:
                     transformers.append(
                         get_instance(
                             "DATASTREAMS_TRANSFORMERS",
                             "transformer",
                             entry,
                             base_path=self.directory,
+                            identity=self.identity,
                         )
                     )
                 elif "writer" in entry:
                     writers.append(
                         get_instance(
                             "DATASTREAMS_WRITERS",
                             "writer",
                             entry,
                             base_path=self.directory,
+                            identity=self.identity,
                         )
                     )
                 elif "source" in entry:
                     readers.append(self.get_reader(entry))
                 elif "service" in entry:
                     writers.append(self.get_service_writer(entry))
                 else:
@@ -114,14 +119,20 @@
                 )
                 entry["reader"] = reader_class
             except KeyError:
                 raise DataStreamCatalogueError(
                     f"Do not have loader for file {source} - extension {ext} not defined in DATASTREAMS_READERS_BY_EXTENSION config"
                 )
         return get_instance(
-            "DATASTREAMS_READERS", "reader", entry, base_path=self.directory
+            "DATASTREAMS_READERS",
+            "reader",
+            entry,
+            base_path=self.directory,
+            identity=self.identity,
         )
 
     def get_service_writer(self, entry):
         from .writers.service import ServiceWriter
 
-        return get_instance(None, ServiceWriter, entry, base_path=self.directory)
+        return get_instance(
+            None, ServiceWriter, entry, base_path=self.directory, identity=self.identity
+        )
```

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/datastreams/cli.py` & `oarepo-runtime-1.3.0/oarepo_runtime/datastreams/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/datastreams/config.py` & `oarepo-runtime-1.3.0/oarepo_runtime/datastreams/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,8 +19,14 @@
             )
         except KeyError:
             raise DataStreamCatalogueError(
                 f"Do not have implementation - '{clz}' not defined in {config_section} config"
             )
         if isinstance(clz, str):
             clz = import_string(clz)
-    return clz(**entry, **kwargs)
+    try:
+        return clz(**entry, **kwargs)
+    except Exception as e:
+        args = {**entry, **kwargs}
+        raise DataStreamCatalogueError(
+            f"Exception instantiating {clz} with arguments {args}"
+        ) from e
```

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/datastreams/errors.py` & `oarepo-runtime-1.3.0/oarepo_runtime/datastreams/errors.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/datastreams/fixtures.py` & `oarepo-runtime-1.3.0/oarepo_runtime/datastreams/fixtures.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/datastreams/readers/__init__.py` & `oarepo-runtime-1.3.0/oarepo_runtime/datastreams/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/datastreams/readers/excel.py` & `oarepo-runtime-1.3.0/oarepo_runtime/datastreams/readers/excel.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/datastreams/readers/json.py` & `oarepo-runtime-1.3.0/oarepo_runtime/datastreams/readers/json.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/datastreams/readers/service.py` & `oarepo-runtime-1.3.0/oarepo_runtime/datastreams/readers/service.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/datastreams/transformers.py` & `oarepo-runtime-1.3.0/oarepo_runtime/datastreams/transformers.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/datastreams/writers/__init__.py` & `oarepo-runtime-1.3.0/oarepo_runtime/datastreams/writers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,37 +8,37 @@
 class BaseWriter(ABC):
     """Base writer."""
 
     def __init__(self, **kwargs) -> None:
         """kwargs for extensions"""
 
     @abstractmethod
-    def write(self, entry: StreamEntry, *args, **kwargs):
+    def write(self, entry: StreamEntry, uow=None, *args, **kwargs):
         """Writes the input entry to the target output.
         :returns: nothing
                   Raises WriterException in case of errors.
         """
 
     @abstractmethod
-    def delete(self, entry: StreamEntry, *args, **kwargs):
+    def delete(self, entry: StreamEntry, uow=None, *args, **kwargs):
         """Removes the stream entry
         :returns: nothing
                   Raises WriterException in case of errors.
         """
 
     def finish(self):
         """Finalizes writing"""
 
 
 class BatchWriter(ABC):
     def __init__(self, **kwargs) -> None:
         """kwargs for extensions"""
 
     @abstractmethod
-    def write_batch(self, batch: StreamBatch, *args, **kwargs) -> StreamBatch:
+    def write_batch(self, batch: StreamBatch, uow=None, *args, **kwargs) -> StreamBatch:
         """Writes the batch to teh stream
         :returns: the batch written. If there are any errors writing entries
         of the batch, should mark them on entries[x].errors.
 
         Note: the batch contains all items, even the filtered ones or the ones
         with errors. Get StreamEntry.ok property to write only the correct batch
         entries.
```

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/datastreams/writers/service.py` & `oarepo-runtime-1.3.0/oarepo_runtime/datastreams/writers/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,30 +30,40 @@
     def _entry_id(self, entry):
         """Get the id from an entry."""
         return entry["id"]
 
     def _resolve(self, id_):
         return self._service.read(self._identity, id_)
 
-    def write(self, stream_entry: StreamEntry, *args, **kwargs):
+    def write(self, stream_entry: StreamEntry, *args, uow=None, **kwargs):
         """Writes the input entry using a given service."""
         entry = stream_entry.entry
+        service_kwargs = {}
+        if uow:
+            service_kwargs["uow"] = uow
         try:
             try:
-                return self._service.create(self._identity, entry)
+                entry = self._service.create(self._identity, entry, **service_kwargs)
             except PIDAlreadyExists:
                 if not self._update:
                     raise WriterError([f"Entry already exists: {entry}"])
                 entry_id = self._entry_id(entry)
                 current = self._resolve(entry_id)
                 updated = dict(current.to_dict(), **entry)
-                return self._service.update(self._identity, entry_id, updated)
+                entry = self._service.update(
+                    self._identity, entry_id, updated, **service_kwargs
+                )
+            stream_entry.entry = entry.data
+            return stream_entry
 
         except ValidationError as err:
             raise WriterError([{"ValidationError": err.messages}])
         except InvalidRelationValue as err:
             # TODO: Check if we can get the error message easier
             raise WriterError([{"InvalidRelationValue": err.args[0]}])
 
-    def delete(self, stream_entry: StreamEntry):
+    def delete(self, stream_entry: StreamEntry, uow=None):
+        service_kwargs = {}
+        if uow:
+            service_kwargs["uow"] = uow
         entry = stream_entry.entry
-        self._service.delete(self._identity, entry["id"])
+        self._service.delete(self._identity, entry["id"], **service_kwargs)
```

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/datastreams/writers/yaml.py` & `oarepo-runtime-1.3.0/oarepo_runtime/datastreams/writers/yaml.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/expansions/expandable_fields.py` & `oarepo-runtime-1.3.0/oarepo_runtime/expansions/expandable_fields.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/ext.py` & `oarepo-runtime-1.3.0/oarepo_runtime/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/ext_config.py` & `oarepo-runtime-1.3.0/oarepo_runtime/ext_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from oarepo_runtime.config.permissions_presets import (
     EveryonePermissionPolicy,
+    OaiHarvesterPermissionPolicy,
     ReadOnlyPermissionPolicy,
 )
 from oarepo_runtime.datastreams.fixtures import default_config_generator
 from oarepo_runtime.datastreams.readers.excel import ExcelReader
 from oarepo_runtime.datastreams.readers.json import JSONLinesReader, JSONReader
 from oarepo_runtime.datastreams.readers.service import ServiceReader
 from oarepo_runtime.datastreams.readers.yaml import YamlReader
 from oarepo_runtime.datastreams.writers.service import ServiceWriter
 from oarepo_runtime.datastreams.writers.yaml import YamlWriter
 
 OAREPO_PERMISSIONS_PRESETS = {
     "read_only": ReadOnlyPermissionPolicy,
     "everyone": EveryonePermissionPolicy,
+    "oai_harvester": OaiHarvesterPermissionPolicy,
 }
 
 
 DEFAULT_DATASTREAMS_READERS = {
     "excel": ExcelReader,
     "yaml": YamlReader,
     "json": JSONReader,
```

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/facets/nested_facet.py` & `oarepo-runtime-1.3.0/oarepo_runtime/facets/nested_facet.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/relations/base.py` & `oarepo-runtime-1.3.0/oarepo_runtime/relations/base.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/relations/internal.py` & `oarepo-runtime-1.3.0/oarepo_runtime/relations/internal.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/relations/lookup.py` & `oarepo-runtime-1.3.0/oarepo_runtime/relations/lookup.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/relations/pid_relation.py` & `oarepo-runtime-1.3.0/oarepo_runtime/relations/pid_relation.py`

 * *Files identical despite different names*

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime/ui/marshmallow.py` & `oarepo-runtime-1.3.0/oarepo_runtime/ui/marshmallow.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import datetime
 import re
 from functools import partial
 
+import marshmallow as ma
+from babel.dates import format_date
+from babel_edtf import format_edtf
 from flask import current_app
 from flask_babelex import get_locale, gettext
 from marshmallow_utils.fields import (
     BabelGettextDictField,
     FormatDate,
     FormatDatetime,
     FormatEDTF,
     FormatTime,
 )
+from marshmallow_utils.fields.babel import BabelFormatField
 
 
 def current_default_locale():
     """Get the Flask app's default locale."""
     if current_app:
         return current_app.config.get("BABEL_DEFAULT_LOCALE", "en")
     # Use english by default if not specified
@@ -37,23 +41,33 @@
                     minute=int(match.group(2)),
                     second=int(match.group(4)) if match.group(4) else 0,
                 )
 
         return super().parse(value, as_time, as_date, as_datetime)
 
 
+class MultilayerFormatEDTF(BabelFormatField):
+    def format_value(self, value):
+        try:
+            return format_date(
+                self.parse(value, as_date=True), format=self._format, locale=self.locale
+            )
+        except:
+            return format_edtf(value, format=self._format, locale=self.locale)
+
+
+# localized edtf
+LocalizedEDTF = partial(MultilayerFormatEDTF, locale=get_locale)
+
 # localized time field
 LocalizedTime = partial(FormatTimeString, locale=get_locale)
 
 # localized datetime field
 LocalizedDateTime = partial(FormatDatetime, locale=get_locale)
 
-# localized edtf
-LocalizedEDTF = partial(FormatEDTF, locale=get_locale)
-
 # localized edtf interval uses the same class as plain EDTF
 LocalizedEDTFInterval = partial(FormatEDTF, locale=get_locale)
 
 
 class PrefixedGettextField(BabelGettextDictField):
     def __init__(self, *, value_prefix, locale, default_locale, **kwargs):
         super().__init__(locale, default_locale, **kwargs)
@@ -71,7 +85,15 @@
     locale=get_locale,
     default_locale=current_default_locale,
 )
 
 if False:  # NOSONAR
     # just for the makemessages to pick up the translations
     translations = [_("True"), _("True")]
+
+
+class InvenioUISchema(ma.Schema):
+    id = ma.fields.Str()
+    created = LocalizedDateTime(dump_only=True)
+    updated = LocalizedDateTime(dump_only=True)
+    links = ma.fields.Raw(dump_only=True)
+    revision_id = ma.fields.Integer(dump_only=True)
```

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime.egg-info/PKG-INFO` & `oarepo-runtime-1.3.0/oarepo_runtime.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-runtime
-Version: 1.2.9
+Version: 1.3.0
 Summary: A set of runtime extensions of Invenio repository
 Description-Content-Type: text/markdown
 Provides-Extra: devs
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo runtime
```

### Comparing `oarepo-runtime-1.2.9/oarepo_runtime.egg-info/SOURCES.txt` & `oarepo-runtime-1.3.0/oarepo_runtime.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 oarepo_runtime/__init__.py
-oarepo_runtime/cli.py
 oarepo_runtime/ext.py
 oarepo_runtime/ext_config.py
+oarepo_runtime/polymorphic.py
 oarepo_runtime.egg-info/PKG-INFO
 oarepo_runtime.egg-info/SOURCES.txt
 oarepo_runtime.egg-info/dependency_links.txt
 oarepo_runtime.egg-info/entry_points.txt
 oarepo_runtime.egg-info/requires.txt
 oarepo_runtime.egg-info/top_level.txt
 oarepo_runtime/cf/__init__.py
 oarepo_runtime/cf/cli.py
 oarepo_runtime/cf/mappings.py
+oarepo_runtime/cli/__init__.py
+oarepo_runtime/cli/assets.py
+oarepo_runtime/cli/base.py
+oarepo_runtime/cli/index.py
+oarepo_runtime/cli/validate.py
 oarepo_runtime/config/__init__.py
 oarepo_runtime/config/permissions_presets.py
 oarepo_runtime/config/service.py
 oarepo_runtime/datastreams/__init__.py
 oarepo_runtime/datastreams/batch.py
 oarepo_runtime/datastreams/catalogue.py
 oarepo_runtime/datastreams/cli.py
@@ -37,24 +42,38 @@
 oarepo_runtime/datastreams/writers/__init__.py
 oarepo_runtime/datastreams/writers/service.py
 oarepo_runtime/datastreams/writers/yaml.py
 oarepo_runtime/expansions/__init__.py
 oarepo_runtime/expansions/expandable_fields.py
 oarepo_runtime/expansions/service.py
 oarepo_runtime/facets/__init__.py
+oarepo_runtime/facets/base.py
+oarepo_runtime/facets/date.py
+oarepo_runtime/facets/enum.py
 oarepo_runtime/facets/max_facet.py
 oarepo_runtime/facets/nested_facet.py
 oarepo_runtime/i18n/__init__.py
+oarepo_runtime/i18n/default_translations.py
+oarepo_runtime/i18n/dumper.py
 oarepo_runtime/i18n/schema.py
+oarepo_runtime/i18n/ui_schema.py
 oarepo_runtime/i18n/validation.py
 oarepo_runtime/relations/__init__.py
 oarepo_runtime/relations/base.py
+oarepo_runtime/relations/components.py
 oarepo_runtime/relations/internal.py
 oarepo_runtime/relations/lookup.py
 oarepo_runtime/relations/mapping.py
 oarepo_runtime/relations/pid_relation.py
+oarepo_runtime/relations/uow.py
+oarepo_runtime/resolvers/__init__.py
+oarepo_runtime/resolvers/proxies.py
 oarepo_runtime/tasks/__init__.py
 oarepo_runtime/tasks/datastreams.py
+oarepo_runtime/translations/messages.pot
+oarepo_runtime/translations/cs/LC_MESSAGES/messages.mo
+oarepo_runtime/translations/cs/LC_MESSAGES/messages.po
+oarepo_runtime/translations/en/LC_MESSAGES/messages.po
 oarepo_runtime/ui/__init__.py
 oarepo_runtime/ui/marshmallow.py
 oarepo_runtime/validation/__init__.py
 oarepo_runtime/validation/dates.py
```

### Comparing `oarepo-runtime-1.2.9/setup.cfg` & `oarepo-runtime-1.3.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = oarepo-runtime
-version = 1.2.9
+version = 1.3.0
 description = A set of runtime extensions of Invenio repository
-authors = Alzbeta
+authors = Alzbeta Pokorna
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
 python = >=3.9
 install_requires = 
@@ -14,14 +14,15 @@
 	invenio-search>=2.1.0
 	invenio_records_resources>=0.21.4
 	marshmallow
 	langcodes
 	pyyaml
 	openpyxl
 	flask-babelex
+	deepmerge
 
 [options.extras_require]
 devs = 
 	pytest>=7.1.2
 	black
 	isort
 	autoflake
@@ -31,14 +32,15 @@
 	invenio-app
 	invenio-search[opensearch2]
 	oarepo>=11.0,<12
 	uritemplate>=4.1.1
 
 [options.package_data]
 * = *.json, *.rst, *.md, *.json5, *.jinja2
+oarepo_runtime = translations/*, translations/cs/LC_MESSAGES/*, translations/en/LC_MESSAGES/*
 
 [tool:pytest]
 testpaths = 
 	tests
 
 [options.entry_points]
 invenio_base.apps =
```

