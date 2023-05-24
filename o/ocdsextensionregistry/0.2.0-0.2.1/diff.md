# Comparing `tmp/ocdsextensionregistry-0.2.0.tar.gz` & `tmp/ocdsextensionregistry-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocdsextensionregistry-0.2.0.tar", last modified: Sat Oct 29 06:55:32 2022, max compression
+gzip compressed data, was "ocdsextensionregistry-0.2.1.tar", last modified: Wed May 24 20:51:21 2023, max compression
```

## Comparing `ocdsextensionregistry-0.2.0.tar` & `ocdsextensionregistry-0.2.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 06:55:32.548686 ocdsextensionregistry-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2662 2022-10-29 06:55:32.548686 ocdsextensionregistry-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 06:55:32.540686 ocdsextensionregistry-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 06:55:32.540686 ocdsextensionregistry-0.2.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/docs/api/codelist.rst
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/docs/api/codelist_code.rst
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/docs/api/extension.rst
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/docs/api/extension_registry.rst
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/docs/api/extension_version.rst
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/docs/api/profile_builder.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/docs/api/util.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13708 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7430 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2466 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/docs/library.rst
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2520 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/docs/translation.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 06:55:32.540686 ocdsextensionregistry-0.2.0/ocdsextensionregistry/
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5800 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     3737 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry/codelist.py
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry/codelist_code.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 06:55:32.544686 ocdsextensionregistry-0.2.0/ocdsextensionregistry/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2804 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (121)     7784 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry/commands/generate_data_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     9181 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry/commands/generate_pot_files.py
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      517 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry/extension.py
--rw-r--r--   0 runner    (1001) docker     (121)     5472 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry/extension_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)    12452 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry/extension_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    15700 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry/profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3063 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 06:55:32.544686 ocdsextensionregistry-0.2.0/ocdsextensionregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2662 2022-10-29 06:55:32.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1798 2022-10-29 06:55:32.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 06:55:32.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-10-29 06:55:32.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-10-29 06:55:32.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-29 06:55:32.000000 ocdsextensionregistry-0.2.0/ocdsextensionregistry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-29 06:55:32.548686 ocdsextensionregistry-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1786 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 06:55:32.544686 ocdsextensionregistry-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 06:55:32.544686 ocdsextensionregistry-0.2.0/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4579 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/tests/commands/test_download.py
--rw-r--r--   0 runner    (1001) docker     (121)     7243 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/tests/commands/test_generate_data_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     2883 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/tests/commands/test_generate_pot_files.py
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/tests/commands/test_none.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 06:55:32.544686 ocdsextensionregistry-0.2.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)    17612 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/tests/fixtures/location-v1.1.4.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 06:55:32.544686 ocdsextensionregistry-0.2.0/tests/fixtures/ocds_coveredBy_extension/
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/tests/fixtures/ocds_coveredBy_extension/release-schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     2824 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     5874 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/tests/test_codelist.py
--rw-r--r--   0 runner    (1001) docker     (121)     2162 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/tests/test_codelist_code.py
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (121)    10484 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/tests/test_extension_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)    11052 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/tests/test_extension_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    15543 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/tests/test_profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2040 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-10-29 06:55:29.000000 ocdsextensionregistry-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:21.342183 ocdsextensionregistry-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-24 20:51:21.342183 ocdsextensionregistry-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:21.334182 ocdsextensionregistry-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:21.334182 ocdsextensionregistry-0.2.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/api/codelist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/api/codelist_code.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/api/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/api/extension_registry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/api/extension_version.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/api/profile_builder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13831 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/library.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/docs/translation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:21.338183 ocdsextensionregistry-0.2.1/ocdsextensionregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/codelist_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:21.338183 ocdsextensionregistry-0.2.1/ocdsextensionregistry/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/commands/generate_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/commands/generate_pot_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/extension_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/extension_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:21.338183 ocdsextensionregistry-0.2.1/ocdsextensionregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-24 20:51:21.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-24 20:51:21.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:51:21.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-24 20:51:21.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-24 20:51:21.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 20:51:21.000000 ocdsextensionregistry-0.2.1/ocdsextensionregistry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-24 20:51:21.342183 ocdsextensionregistry-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:21.338183 ocdsextensionregistry-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:21.342183 ocdsextensionregistry-0.2.1/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/commands/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/commands/test_generate_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/commands/test_generate_pot_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/commands/test_none.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:21.342183 ocdsextensionregistry-0.2.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/fixtures/location-v1.1.4.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:51:21.342183 ocdsextensionregistry-0.2.1/tests/fixtures/ocds_coveredBy_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/fixtures/ocds_coveredBy_extension/release-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/test_codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/test_codelist_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/test_extension_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/test_extension_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/test_profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-24 20:51:10.000000 ocdsextensionregistry-0.2.1/tox.ini
```

### Comparing `ocdsextensionregistry-0.2.0/LICENSE` & `ocdsextensionregistry-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/PKG-INFO` & `ocdsextensionregistry-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ocdsextensionregistry
-Version: 0.2.0
+Version: 0.2.1
 Summary: Eases access to information from the extension registry of the Open Contracting Data Standard
 Home-page: https://github.com/open-contracting/extension_registry.py
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: cli
 License-File: LICENSE
```

### Comparing `ocdsextensionregistry-0.2.0/README.rst` & `ocdsextensionregistry-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/docs/Makefile` & `ocdsextensionregistry-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/docs/changelog.rst` & `ocdsextensionregistry-0.2.1/docs/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+0.2.1 (2023-05-24)
+------------------
+
+-  feat: Add a ``--no-frozen`` option to all commands.
+-  Drop Python 3.7 support.
+
 0.2.0 (2022-10-29)
 ------------------
 
 -  fix: :meth:`~ocdsextensionregistry.profile_builder.ProfileBuilder.release_package_schema` and :meth:`~ocdsextensionregistry.profile_builder.ProfileBuilder.record_package_schema` return a JSON-serializable object when ``embed=True``.
 
 0.1.14 (2022-09-07)
 -------------------
```

### Comparing `ocdsextensionregistry-0.2.0/docs/cli.rst` & `ocdsextensionregistry-0.2.1/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/docs/conf.py` & `ocdsextensionregistry-0.2.1/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "OCDS Extension Registry Python Package"
 copyright = "2018, Open Contracting Partnership"
 author = "Open Contracting Partnership"
 
 # The short X.Y version
-version = "0.2.0"
+version = "0.2.1"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `ocdsextensionregistry-0.2.0/docs/index.rst` & `ocdsextensionregistry-0.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/docs/translation.rst` & `ocdsextensionregistry-0.2.1/docs/translation.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Translation
 ===========
 
 Setup
 -----
 
-:doc:`Install this package with command-line tools<cli>`, and then install ``sphinx-intl`` and ``transifex-client``:
+:doc:`Install this package with command-line tools<cli>`, `install the Transifex Client <https://developers.transifex.com/docs/cli>`__, and install ``sphinx-intl``:
 
 .. code-block:: bash
 
-    pip install 'sphinx-intl<1' transifex-client
-
-Create a `~/.transifexrc <https://docs.transifex.com/client/client-configuration#%7E/-transifexrc>`__ file (replace ``USERNAME`` and ``PASSWORD``):
-
-.. code-block:: bash
-
-    sphinx-intl create-transifexrc --transifex-username USERNAME --transifex-password PASSWORD
+    pip install sphinx-intl
 
 Create new translations
 -----------------------
 
 Create a project on Transifex (in this example, our project's identifier is ``ocds-extensions``).
 
 Generate POT files for all versions of all extensions:
 
 .. code-block:: bash
 
     ocdsextensionregistry generate-pot-files build/locale
 
+Or, generate POT files for only live versions of extensions:
+
+.. code-block:: bash
+
+    ocdsextensionregistry generate-pot-files --no-frozen build/locale
+
 Or, generate POT files for the versions of extensions you want to translate, for example:
 
 .. code-block:: bash
 
     ocdsextensionregistry generate-pot-files build/locale lots bids==v1.1.4
 
 Remove any existing ``.tx/config`` file:
@@ -41,31 +41,31 @@
 
 Create a new ``.tx/config`` file:
 
 .. code-block:: bash
 
     sphinx-intl create-txconfig
 
-Update the ``.tx/config`` file based on the POT files (replace ``ocds-extensions`` with your project):
+Update the ``.tx/config`` file based on the POT files (replace ``open-contracting-partnership-1`` with your organization and ``ocds-extensions`` with your project):
 
 .. code-block:: bash
 
-    sphinx-intl update-txconfig-resources --transifex-project-name ocds-extensions --pot-dir build/locale --locale-dir locale
+    sphinx-intl update-txconfig-resources --transifex-organization-name open-contracting-partnership-1 --transifex-project-name ocds-extensions --pot-dir build/locale --locale-dir locale
 
 Push source files to Transifex for translation:
 
 .. code-block:: bash
 
     tx push -s
 
 Once you've translated strings on Transifex, email data@open-contracting.org so that we can pull translation files from Transifex, build MO files, and commit the changes:
 
 .. code-block:: bash
 
-    tx pull -a -f
+    tx pull -f -a
     sphinx-intl build -d locale
 
 Update existing translations
 ----------------------------
 
 Existing translations are stored in `ocds-extensions-translations <https://github.com/open-contracting/ocds-extensions-translations>`__.
 
@@ -77,14 +77,14 @@
 
 Change into its directory:
 
 .. code-block:: bash
 
     cd ocds-extensions-translations
 
-And push its translations. See `Transifex's documentation <https://docs.transifex.com/client/push>`__ for more information on how to specify which languages or resources to push:
+And push its translations. See `Transifex's documentation <https://developers.transifex.com/docs/using-the-client#pushing-files-to-transifex>`__ for more information on how to specify which languages or resources to push:
 
 .. code-block:: bash
 
     tx push -t
 
 Once you've translated strings on Transifex, follow the same final step under creating new translations.
```

### Comparing `ocdsextensionregistry-0.2.0/ocdsextensionregistry/__init__.py` & `ocdsextensionregistry-0.2.1/ocdsextensionregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/ocdsextensionregistry/__main__.py` & `ocdsextensionregistry-0.2.1/ocdsextensionregistry/__main__.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/ocdsextensionregistry/api.py` & `ocdsextensionregistry-0.2.1/ocdsextensionregistry/api.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/ocdsextensionregistry/codelist.py` & `ocdsextensionregistry-0.2.1/ocdsextensionregistry/codelist.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/ocdsextensionregistry/codelist_code.py` & `ocdsextensionregistry-0.2.1/ocdsextensionregistry/codelist_code.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/ocdsextensionregistry/commands/base.py` & `ocdsextensionregistry-0.2.1/ocdsextensionregistry/commands/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 class BaseCommand:
     def __init__(self, subparsers):
         """
         Initializes the subparser and adds arguments.
         """
         self.subparser = subparsers.add_parser(self.name, description=self.help)
+        self.add_argument('--no-frozen', action='store_true', help='exclude frozen versions')
         self.add_arguments()
 
     def add_arguments(self):
         pass
 
     def add_argument(self, *args, **kwargs):
         """
@@ -35,10 +36,13 @@
             elif '=' in value:
                 # Help users with a common error.
                 raise CommandError(f"Couldn't parse '{value}'. Use '==' not '='.")
             else:
                 versions[value]
 
         for version in registry:
-            if ((not self.args.versions or version.id in versions) and
-                    (not versions[version.id] or version.version in versions[version.id])):
+            if (
+                (not self.args.versions or version.id in versions)
+                and (not versions[version.id] or version.version in versions[version.id])
+                and (not self.args.no_frozen or not version.date)
+            ):
                 yield version
```

### Comparing `ocdsextensionregistry-0.2.0/ocdsextensionregistry/commands/download.py` & `ocdsextensionregistry-0.2.1/ocdsextensionregistry/commands/download.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/ocdsextensionregistry/commands/generate_data_file.py` & `ocdsextensionregistry-0.2.1/ocdsextensionregistry/commands/generate_data_file.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/ocdsextensionregistry/commands/generate_pot_files.py` & `ocdsextensionregistry-0.2.1/ocdsextensionregistry/commands/generate_pot_files.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/ocdsextensionregistry/exceptions.py` & `ocdsextensionregistry-0.2.1/ocdsextensionregistry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/ocdsextensionregistry/extension.py` & `ocdsextensionregistry-0.2.1/ocdsextensionregistry/extension.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/ocdsextensionregistry/extension_registry.py` & `ocdsextensionregistry-0.2.1/ocdsextensionregistry/extension_registry.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/ocdsextensionregistry/extension_version.py` & `ocdsextensionregistry-0.2.1/ocdsextensionregistry/extension_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     def get_url(self, basename):
         """
         Returns the URL of the file within the extension.
         """
         if basename in self._file_urls:
             return self._file_urls[basename]
-        return ''.join([self.base_url, basename])
+        return self.base_url + basename
 
     def remote(self, basename, default=None):
         """
         Returns the contents of the file within the extension. If the ``default`` is set and the file does not exist,
         returns the provided ``default`` value.
 
         If the extension has a download URL, caches all the files' contents. Otherwise, downloads and caches the
```

### Comparing `ocdsextensionregistry-0.2.0/ocdsextensionregistry/profile_builder.py` & `ocdsextensionregistry-0.2.1/ocdsextensionregistry/profile_builder.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/ocdsextensionregistry/util.py` & `ocdsextensionregistry-0.2.1/ocdsextensionregistry/util.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/ocdsextensionregistry.egg-info/PKG-INFO` & `ocdsextensionregistry-0.2.1/ocdsextensionregistry.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ocdsextensionregistry
-Version: 0.2.0
+Version: 0.2.1
 Summary: Eases access to information from the extension registry of the Open Contracting Data Standard
 Home-page: https://github.com/open-contracting/extension_registry.py
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: cli
 License-File: LICENSE
```

### Comparing `ocdsextensionregistry-0.2.0/ocdsextensionregistry.egg-info/SOURCES.txt` & `ocdsextensionregistry-0.2.1/ocdsextensionregistry.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.rst
-setup.py
+pyproject.toml
+setup.cfg
 tox.ini
 docs/Makefile
 docs/changelog.rst
 docs/cli.rst
 docs/conf.py
 docs/index.rst
 docs/library.rst
```

### Comparing `ocdsextensionregistry-0.2.0/tests/commands/test_download.py` & `ocdsextensionregistry-0.2.1/tests/commands/test_download.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,25 @@
 
     assert len(caplog.records) == 1
     assert caplog.records[0].levelname == 'CRITICAL'
     assert caplog.records[0].message == "Couldn't parse 'location=v1.1.4'. Use '==' not '='."
     assert excinfo.value.code == 1
 
 
+def test_command_versions_no_frozen(capsys, monkeypatch, tmpdir):
+    monkeypatch.setattr(sys, 'argv', args + ['--no-frozen', str(tmpdir), 'location'])
+    main()
+
+    assert capsys.readouterr().out == ''
+
+    tree = list(os.walk(tmpdir))
+
+    assert len(tree[1][1]) == 1
+
+
 # Require the user to decide what to overwrite.
 def test_command_repeated(capsys, monkeypatch, tmpdir, caplog):
     caplog.set_level(logging.INFO, logger='ocdsextensionregistry')
     argv = args + [str(tmpdir), 'location==v1.1.4']
 
     monkeypatch.setattr(sys, 'argv', argv)
     main()
```

### Comparing `ocdsextensionregistry-0.2.0/tests/commands/test_generate_data_file.py` & `ocdsextensionregistry-0.2.1/tests/commands/test_generate_data_file.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/tests/commands/test_generate_pot_files.py` & `ocdsextensionregistry-0.2.1/tests/commands/test_generate_pot_files.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/tests/fixtures/location-v1.1.4.json` & `ocdsextensionregistry-0.2.1/tests/fixtures/location-v1.1.4.json`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/tests/fixtures/ocds_coveredBy_extension/release-schema.json` & `ocdsextensionregistry-0.2.1/tests/fixtures/ocds_coveredBy_extension/release-schema.json`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/tests/test_api.py` & `ocdsextensionregistry-0.2.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/tests/test_codelist.py` & `ocdsextensionregistry-0.2.1/tests/test_codelist.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/tests/test_codelist_code.py` & `ocdsextensionregistry-0.2.1/tests/test_codelist_code.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/tests/test_extension.py` & `ocdsextensionregistry-0.2.1/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/tests/test_extension_registry.py` & `ocdsextensionregistry-0.2.1/tests/test_extension_registry.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/tests/test_extension_version.py` & `ocdsextensionregistry-0.2.1/tests/test_extension_version.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/tests/test_profile_builder.py` & `ocdsextensionregistry-0.2.1/tests/test_profile_builder.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.2.0/tests/test_util.py` & `ocdsextensionregistry-0.2.1/tests/test_util.py`

 * *Files identical despite different names*

