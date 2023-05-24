# Comparing `tmp/kiara_plugin.onboarding-0.4.3.tar.gz` & `tmp/kiara_plugin.onboarding-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.onboarding-0.4.3.tar", last modified: Mon Feb 13 18:40:21 2023, max compression
+gzip compressed data, was "kiara_plugin.onboarding-0.4.4.tar", last modified: Wed May 24 13:48:03 2023, max compression
```

## Comparing `kiara_plugin.onboarding-0.4.3.tar` & `kiara_plugin.onboarding-0.4.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.980377 kiara_plugin.onboarding-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.972376 kiara_plugin.onboarding-0.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.976377 kiara_plugin.onboarding-0.4.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.976377 kiara_plugin.onboarding-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-02-13 18:40:21.980377 kiara_plugin.onboarding-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.972376 kiara_plugin.onboarding-0.4.3/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.976377 kiara_plugin.onboarding-0.4.3/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/ci/conda/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.976377 kiara_plugin.onboarding-0.4.3/ci/conda/kiara_plugin.onboarding/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/ci/conda/kiara_plugin.onboarding/meta.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.976377 kiara_plugin.onboarding-0.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.976377 kiara_plugin.onboarding-0.4.3/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.972376 kiara_plugin.onboarding-0.4.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.976377 kiara_plugin.onboarding-0.4.3/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.980377 kiara_plugin.onboarding-0.4.3/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/examples/data/journals/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.972376 kiara_plugin.onboarding-0.4.3/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.980377 kiara_plugin.onboarding-0.4.3/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-02-13 18:40:21.984377 kiara_plugin.onboarding-0.4.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1396 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.972376 kiara_plugin.onboarding-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.972376 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.980377 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.980377 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.980377 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/modules/files/
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/modules/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/modules/files/import_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/modules/files/import_file_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/modules/zenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.980377 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.980377 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.980377 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/utils/download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.980377 kiara_plugin.onboarding-0.4.3/src/kiara_plugin.onboarding.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-02-13 18:40:21.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin.onboarding.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-02-13 18:40:21.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin.onboarding.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 18:40:21.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin.onboarding.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-02-13 18:40:21.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin.onboarding.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 18:39:43.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin.onboarding.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-02-13 18:40:21.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin.onboarding.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-13 18:40:21.000000 kiara_plugin.onboarding-0.4.3/src/kiara_plugin.onboarding.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:40:21.980377 kiara_plugin.onboarding-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      236 2023-02-13 18:39:34.000000 kiara_plugin.onboarding-0.4.3/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.049426 kiara_plugin.onboarding-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.025426 kiara_plugin.onboarding-0.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.037426 kiara_plugin.onboarding-0.4.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.037426 kiara_plugin.onboarding-0.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-24 13:48:03.049426 kiara_plugin.onboarding-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.025426 kiara_plugin.onboarding-0.4.4/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.037426 kiara_plugin.onboarding-0.4.4/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/ci/conda/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.037426 kiara_plugin.onboarding-0.4.4/ci/conda/kiara_plugin.onboarding/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/ci/conda/kiara_plugin.onboarding/meta.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.037426 kiara_plugin.onboarding-0.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.037426 kiara_plugin.onboarding-0.4.4/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.025426 kiara_plugin.onboarding-0.4.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.041426 kiara_plugin.onboarding-0.4.4/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.041426 kiara_plugin.onboarding-0.4.4/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/examples/data/journals/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.025426 kiara_plugin.onboarding-0.4.4/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.041426 kiara_plugin.onboarding-0.4.4/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-24 13:48:03.053426 kiara_plugin.onboarding-0.4.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1396 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.029426 kiara_plugin.onboarding-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.029426 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.045426 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.045426 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.045426 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/files/import_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/files/import_file_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/zenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.049426 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.049426 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.049426 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/utils/download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.045426 kiara_plugin.onboarding-0.4.4/src/kiara_plugin.onboarding.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-24 13:48:02.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin.onboarding.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-24 13:48:03.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin.onboarding.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:48:02.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin.onboarding.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-24 13:48:02.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin.onboarding.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:47:16.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin.onboarding.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-24 13:48:02.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin.onboarding.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 13:48:02.000000 kiara_plugin.onboarding-0.4.4/src/kiara_plugin.onboarding.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:48:03.049426 kiara_plugin.onboarding-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      236 2023-05-24 13:47:05.000000 kiara_plugin.onboarding-0.4.4/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.onboarding-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.onboarding-0.4.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.3/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.onboarding-0.4.4/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.3/.github/workflows/build-darwin.yaml` & `kiara_plugin.onboarding-0.4.4/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.3/.github/workflows/build-linux.yaml` & `kiara_plugin.onboarding-0.4.4/.github/workflows/build-linux.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -66,41 +66,49 @@
           python-version: "${{ matrix.python_version }}"
       - uses: actions/checkout@v3
       - name: install kiara_plugin.onboarding
         run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ .[all,dev_testing]
       - name: Test with mypy
         run: make mypy
 
-  flake8-linux:
-    name: flake8 on linux
+  linting-linux:
     runs-on: ubuntu-latest
     steps:
-      - name: Set up Python 3.9
+      - uses: actions/checkout@v3
+      - name: Install Python
         uses: actions/setup-python@v4
         with:
-          python-version: "3.9"
-      - uses: actions/checkout@v3
-      - name: install kiara_plugin.onboarding
-        run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ .[all,dev_testing]
-      - name: Test with flake8
-        run: make flake
+          python-version: "3.11"
+      - name: pip cache
+        id: pip-cache
+        uses: actions/cache@v3
+        with:
+          path: ~/.cache/pip
+          key: ${{ runner.os }}-pip-${{ hashFiles('**/setup.*') }}
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install ruff
+      # Include `--format=github` to enable automatic inline annotations.
+      - name: Run Ruff
+        run: ruff --format=github src/
 
   build-docs:
     name: build documentation
     if: ${{ github.ref == 'refs/heads/develop' }} || ${{ github.ref == 'refs/heads/main' }} || startsWith(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
     needs:
       - test-linux
       - mypy-linux
-      - flake8-linux
+      - linting-linux
     steps:
-      - name: Set up Python 3.9
+      - name: Set up Python 3.11
         uses: actions/setup-python@v4
         with:
-          python-version: "3.9"
+          python-version: "3.11"
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: install kiara_plugin.onboarding package
         run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ .[all,dev_documentation]
       - run: git config --global user.email "Markus Binsteiner"
       - run: git config --global user.name "markus@frkl.io"
@@ -116,15 +124,15 @@
   release_package:
     name: publish python package
     if: ${{ github.ref == 'refs/heads/develop' }} || ${{ github.ref == 'refs/heads/main' }} || startsWith(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
     needs:
       - test-linux
       - mypy-linux
-      - flake8-linux
+      - linting-linux
     env:
         GEMFURY_PUSH_TOKEN: ${{ secrets.GEMFURY_PUSH_TOKEN }}
     steps:
       - name: Set up Python 3.9
         uses: actions/setup-python@v4
         with:
           python-version: "3.9"
@@ -152,31 +160,33 @@
 
   conda_package_build:
     name: conda package build (and upload if release)
     runs-on: ubuntu-latest
     needs:
       - test-linux
       - mypy-linux
-      - flake8-linux
+      - linting-linux
     steps:
-      - name: "Set up Python 3.9"
+      - name: "Set up Python 3.11"
         uses: actions/setup-python@v4
         with:
-          python-version: "3.9"
+          python-version: "3.11"
       - name: pip cache
         id: pip-cache
         uses: actions/cache@v3
         with:
           path: ~/.cache/pip
           key: ${{ runner.os }}-pip-${{ hashFiles('**/setup.*') }}
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
+      - name: install kiara
+        run: pip install kiara
       - name: install required plugin packages
-        run: pip install -U --pre --extra-index-url https://pypi.fury.io/dharpa/ kiara_plugin.develop
+        run: pip install git+https://github.com/DHARPA-Project/kiara_plugin.develop.git@develop
       - name: build conda package
         if: ${{ ( github.ref == 'refs/heads/develop') }}
         run: kiara conda build-package --patch-data ci/conda/conda-pkg-patch.yaml .
       - name: extract tag name
         run: echo "RELEASE_VERSION=${GITHUB_REF#refs/*/}" >> $GITHUB_ENV
       - name: build & publish conda package
         if: ${{ startsWith(github.ref, 'refs/tags/') }}
@@ -185,15 +195,15 @@
   merge_tag_to_main:
     name: merge current tag to main branch
     runs-on: ubuntu-latest
     if: ${{ startsWith(github.ref, 'refs/tags') }}
     needs:
       - test-linux
       - mypy-linux
-      - flake8-linux
+      - linting-linux
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - run: git config --global user.email "markus@frkl.io"
     - run: git config --global user.name "Markus Binsteiner"
     - name: extract tag name
```

### Comparing `kiara_plugin.onboarding-0.4.3/.github/workflows/build-windows.yaml` & `kiara_plugin.onboarding-0.4.4/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.3/.gitignore` & `kiara_plugin.onboarding-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.3/.pre-commit-config.yaml` & `kiara_plugin.onboarding-0.4.4/.pre-commit-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -6,47 +6,36 @@
 - repo: https://github.com/alessandrojcm/commitlint-pre-commit-hook
   rev: 'v9.3.0'
   hooks:
     - id: commitlint
       stages: [commit-msg]
       additional_dependencies: ['@commitlint/config-conventional']
 
-- repo: https://github.com/pycqa/isort
-  rev: 5.10.1
-  hooks:
-    - id: isort
-
 - repo: https://github.com/psf/black
-  rev: 22.10.0
+  rev: 22.12.0
   hooks:
     - id: black
 
-- repo: https://github.com/myint/autoflake
-  rev: 'v2.0.0'
-  hooks:
-    - id: autoflake
-      args: ['--in-place', '--remove-all-unused-imports']
-      # args: ['--in-place', '--remove-all-unused-imports', '--remove-unused-variable']
-
-- repo: https://github.com/PyCQA/flake8
-  rev: 5.0.4
-  hooks:
-    - id: flake8
-
 - repo: https://github.com/pre-commit/mirrors-mypy
   rev: 'v0.991'  # Use the sha / tag you want to point at
   hooks:
   - id: mypy
     files: "^src/"
     pass_filenames: true
     args: ["--config-file", "setup.cfg", "--ignore-missing-imports", "--explicit-package-bases"]
-    additional_dependencies: [pydantic>=1.8.0, rich>=10.0.0, ruamel.yaml, sqlalchemy-stubs, types-python-slugify, types-setuptools, types-python-dateutil, types-pytz, types-orjson]
+    additional_dependencies: [pydantic>=1.8.0, rich>=10.0.0, ruamel.yaml, anyio>=3.0.0, pyzmq>=22.0.3, bidict, sqlalchemy-stubs, types-python-slugify, types-setuptools, types-python-dateutil, dag_cbor, multiformats, textual, regex, types-pytz, types-orjson]
+
+- repo: https://github.com/charliermarsh/ruff-pre-commit
+  # Ruff version.
+  rev: 'v0.0.243'
+  hooks:
+    - id: ruff
 
 - repo: https://github.com/Kludex/no-optional
-  rev: 0.3.1
+  rev: 0.4.0
   hooks:
     - id: no_optional
 
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: 'v4.3.0'
   hooks:
   - id: trailing-whitespace
```

### Comparing `kiara_plugin.onboarding-0.4.3/LICENSE` & `kiara_plugin.onboarding-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.3/Makefile` & `kiara_plugin.onboarding-0.4.4/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.3/PKG-INFO` & `kiara_plugin.onboarding-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.onboarding
-Version: 0.4.3
+Version: 0.4.4
 Summary: kiara modules for data onboarding.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.onboarding
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.onboarding
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.onboarding
 Keywords: kiara
```

### Comparing `kiara_plugin.onboarding-0.4.3/README.md` & `kiara_plugin.onboarding-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.3/ci/conda/kiara_plugin.onboarding/meta.yaml.template` & `kiara_plugin.onboarding-0.4.4/ci/conda/kiara_plugin.onboarding/meta.yaml.template`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.3/docs/development.md` & `kiara_plugin.onboarding-0.4.4/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.3/docs/index.md` & `kiara_plugin.onboarding-0.4.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.3/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.onboarding-0.4.4/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.3/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.onboarding-0.4.4/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.3/mkdocs.yml` & `kiara_plugin.onboarding-0.4.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.3/pyproject.toml` & `kiara_plugin.onboarding-0.4.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -39,21 +39,17 @@
 
 [project.optional-dependencies]
 dev_documentation = [
     "kiara[dev_documentation]"
 ]
 dev_testing = [
     "kiara[dev_testing]",
-    "types-setuptools",
-    "sqlalchemy-stubs",
-    "types-orjson",
-    "types-pytz"
 ]
 dev_utils = [
-    "kiara[dev_utils]"
+    "kiara[dev_utils]",
 ]
 dev_all = [
     "kiara[dev_all]"
 ]
 
 [project.entry-points."kiara.plugin"]
 onboarding = "kiara_plugin.onboarding"
@@ -91,7 +87,98 @@
   | dist
   | external
 )/
 '''
 
 [tool.setuptools_scm]
 write_to = "src/kiara_plugin/onboarding/version.txt"
+
+[tool.pytest.ini_options]
+pythonpath = [
+    "src"
+]
+
+[tool.ruff]
+line-length = 88
+
+src = ["src", "tests"]
+
+select = [
+    "E",
+    "F",
+    "RUF",
+    "I001",
+    "YTT",
+    "S",
+    "C4",
+    "T10",
+    "ISC",
+    "ICN",
+    "T20",
+    "Q",
+    "TID",
+    "PD",
+    "PLC",
+    "PLE",
+    "PLR",
+    "PLW",
+    "PIE",
+]
+ignore = ["E501", "S101", "SIM118", "SIM108", "PLR2004", "PLR0913", "S110", "PLR0912", "PLR0915", "PIE810"]
+
+fix = true
+fixable = ["E", "F", "RUF100", "I001", "Q"]
+
+
+#fixable = ["E", "F", "RUF100", "I001"]
+# Enable Pyflakes `E` and `F` codes by default.
+
+# Exclude a variety of commonly ignored directories.
+exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".hg",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "venv",
+]
+per-file-ignores = { }
+
+# Allow unused variables when underscore-prefixed.
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+
+# Assume Python 3.10.
+target-version = "py310"
+
+[tool.ruff.mccabe]
+# Unlike Flake8, default to a complexity level of 10.
+max-complexity = 10
+
+[tool.ruff.isort]
+known-first-party = ["kiara", "kiara_plugin"]
+
+[tool.ruff.pydocstyle]
+convention = "google"
+
+[tool.pyright]
+include = ["src"]
+exclude = ["**/__pycache__"]
+ignore = []
+
+reportMissingImports = true
+reportMissingTypeStubs = false
+
+executionEnvironments = [
+]
```

### Comparing `kiara_plugin.onboarding-0.4.3/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.onboarding-0.4.4/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.3/scripts/documentation/gen_info_pages.py` & `kiara_plugin.onboarding-0.4.4/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.3/scripts/documentation/gen_module_doc.py` & `kiara_plugin.onboarding-0.4.4/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.3/setup.cfg` & `kiara_plugin.onboarding-0.4.4/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -39,22 +39,14 @@
 deps = 
 	-e{toxinidir}[dev_testing,all]
 install_command = pip install --pre --extra-index-url https://pypi.fury.io/dharpa/ {opts} {packages}
 commands = 
 	pip install -U pip
 	py.test --basetemp={envtmpdir}
 
-[testenv:flake8]
-basepython = python
-deps = 
-	-e{toxinidir}[dev_testing,all]
-	flake8
-install_command = pip install --pre --extra-index-url https://pypi.fury.io/dharpa/ {opts} {packages}
-commands = flake8 src
-
 [coverage:run]
 branch = True
 source = kiara_plugin.onboarding
 
 [coverage:paths]
 source = 
 	src/
@@ -69,29 +61,14 @@
 	
 	raise AssertionError
 	raise NotImplementedError
 	
 	if 0:
 	if __name__ == .__main__.:
 
-[flake8]
-exclude = 
-	.tox
-	build
-	dist
-	.eggs
-	docs/conf.py
-	.git
-	__pycache__
-ignore = F405, W503, E501
-max-line-length = 88
-
-[isort]
-profile = black
-
 [mypy]
 mypy_path = 
 	src/
 namespace_packages = true
 plugins = pydantic.mypy
 
 [mypy-appdirs]
```

### Comparing `kiara_plugin.onboarding-0.4.3/setup.py` & `kiara_plugin.onboarding-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/__init__.py` & `kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/models.py` & `kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/modules/files/__init__.py` & `kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/files/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 import atexit
 import os
 import shutil
 import tempfile
 from typing import Any, Dict, Union
 
-from kiara.api import KiaraModule, KiaraModuleConfig, ValueMap, ValueMapSchema
-from kiara.models.filesystem import FileBundle
 from pydantic import Field
 
+from kiara.api import KiaraModule, KiaraModuleConfig, ValueMap, ValueMapSchema
+from kiara.exceptions import KiaraProcessingException
+from kiara.models.filesystem import FileBundle
 from kiara_plugin.onboarding.utils.download import download_file
 
 
 class DownloadFileConfig(KiaraModuleConfig):
     download_metadata: bool = Field(
         description="Whether to return the download metadata as well.",
         default=True,
@@ -107,43 +108,64 @@
                 "doc": "Metadata about the download.",
             }
         return result
 
     def process(self, inputs: ValueMap, outputs: ValueMap):
 
         from datetime import datetime
+        from urllib.parse import urlparse
 
         import httpx
         import pytz
 
         url = inputs.get_value_data("url")
+        suffix = None
+        try:
+            parsed_url = urlparse(url)
+            _, suffix = os.path.splitext(parsed_url.path)
+        except Exception:
+            pass
+        if not suffix:
+            suffix = ""
+
         sub_path: Union[None, str] = inputs.get_value_data("sub_path")
-        tmp_file = tempfile.NamedTemporaryFile(delete=False)
+        tmp_file = tempfile.NamedTemporaryFile(delete=False, suffix=suffix)
         atexit.register(tmp_file.close)
 
         history = []
         datetime.utcnow().replace(tzinfo=pytz.utc)
         with open(tmp_file.name, "wb") as f:
             with httpx.stream("GET", url, follow_redirects=True) as r:
                 history.append(dict(r.headers))
                 for h in r.history:
                     history.append(dict(h.headers))
                 for data in r.iter_bytes():
                     f.write(data)
 
-        import patoolib
-
         out_dir = tempfile.mkdtemp()
 
         def del_out_dir():
             shutil.rmtree(out_dir, ignore_errors=True)
 
-        # atexit.register(del_out_dir)
+        atexit.register(del_out_dir)
+
+        error = None
+        try:
+            shutil.unpack_archive(tmp_file.name, out_dir)
+        except Exception:
+            # try patool, maybe we're lucky
+            try:
+                import patoolib
+
+                patoolib.extract_archive(tmp_file.name, outdir=out_dir)
+            except Exception as e:
+                error = e
 
-        patoolib.extract_archive(tmp_file.name, outdir=out_dir)
+        if error is not None:
+            raise KiaraProcessingException(f"Could not extract archive: {error}.")
 
         path = out_dir
         if sub_path:
             path = os.path.join(out_dir, sub_path)
         bundle = FileBundle.import_folder(path)
 
         metadata = {
```

### Comparing `kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/modules/files/import_file.py` & `kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/files/import_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 import os
 from typing import Any, Dict, Tuple
 
+from pydantic import BaseModel, Field
+
 from kiara.api import KiaraModule, KiaraModuleConfig, ValueMap, ValueMapSchema
 from kiara.exceptions import KiaraProcessingException
 from kiara.models.filesystem import FileModel
-from pydantic import BaseModel, Field
 
 
 class ImportFileConfig(KiaraModuleConfig):
 
     import_metadata: bool = Field(
         description="Whether to return the import metadata as well.",
         default=True,
```

### Comparing `kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/modules/files/import_file_bundle.py` & `kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/files/import_file_bundle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 from typing import Any, Dict
 
-from kiara.api import KiaraModule, KiaraModuleConfig, ValueMap, ValueMapSchema
 from pydantic import Field
 
+from kiara.api import KiaraModule, KiaraModuleConfig, ValueMap, ValueMapSchema
+
 
 class ImportFileBundleConfig(KiaraModuleConfig):
 
     import_metadata: bool = Field(
         description="Whether to return the import metadata as well.",
         default=True,
     )
```

### Comparing `kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/modules/zenodo.py` & `kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/modules/zenodo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 import hashlib
 import shutil
 from pathlib import Path
 from typing import Any, Mapping
 
 import orjson
+from pydantic import Field
+
 from kiara.api import KiaraModule, KiaraModuleConfig, ValueMap, ValueMapSchema
 from kiara.exceptions import KiaraProcessingException
 from kiara.models.filesystem import FileBundle
-from pydantic import Field
 
 
 class ZenodoDownloadConfig(KiaraModuleConfig):
 
     metadata_filename: str = Field(
         description="The filename for the zenodo metadata.", default="metadata.json"
     )
@@ -59,15 +60,15 @@
         target_file = target_path / file_name
 
         if target_file.exists():
             raise KiaraProcessingException(
                 f"Can't download file, target path already exists: {target_path.as_posix()}."
             )
 
-        hash_md5 = hashlib.md5()
+        hash_md5 = hashlib.md5()  # noqa
 
         with open(target_file, "ab") as file2:
             with httpx.Client() as client:
                 with client.stream("GET", url) as resp:
                     for chunk in resp.iter_bytes():
                         hash_md5.update(chunk)
                         file2.write(chunk)
```

### Comparing `kiara_plugin.onboarding-0.4.3/src/kiara_plugin/onboarding/utils/download.py` & `kiara_plugin.onboarding-0.4.4/src/kiara_plugin/onboarding/utils/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 import tempfile
 from datetime import datetime
 from typing import Any, Dict, Tuple, Union
 
 import httpx
 import pytz
+
 from kiara.models.filesystem import FileModel
 
 
 def download_file(
     url: str, file_name: Union[str, None] = None
 ) -> Tuple[FileModel, Dict[str, Any]]:
```

### Comparing `kiara_plugin.onboarding-0.4.3/src/kiara_plugin.onboarding.egg-info/PKG-INFO` & `kiara_plugin.onboarding-0.4.4/src/kiara_plugin.onboarding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.onboarding
-Version: 0.4.3
+Version: 0.4.4
 Summary: kiara modules for data onboarding.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.onboarding
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.onboarding
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.onboarding
 Keywords: kiara
```

### Comparing `kiara_plugin.onboarding-0.4.3/src/kiara_plugin.onboarding.egg-info/SOURCES.txt` & `kiara_plugin.onboarding-0.4.4/src/kiara_plugin.onboarding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

