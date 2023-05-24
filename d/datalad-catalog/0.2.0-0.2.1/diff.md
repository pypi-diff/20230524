# Comparing `tmp/datalad_catalog-0.2.0.tar.gz` & `tmp/datalad_catalog-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalad_catalog-0.2.0.tar", last modified: Thu Nov 24 08:01:55 2022, max compression
+gzip compressed data, was "datalad_catalog-0.2.1.tar", last modified: Tue Mar  7 12:46:35 2023, max compression
```

## Comparing `datalad_catalog-0.2.0.tar` & `datalad_catalog-0.2.1.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:55.973935 datalad_catalog-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)      120 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/CONTRIBUTORS
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      124 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    19844 2022-11-24 08:01:55.973935 datalad_catalog-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    19370 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:55.941935 datalad_catalog-0.2.0/_datalad_buildsupport/
--rw-r--r--   0 runner    (1001) docker     (122)      529 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/_datalad_buildsupport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10698 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/_datalad_buildsupport/formatters.py
--rw-r--r--   0 runner    (1001) docker     (122)     9752 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/_datalad_buildsupport/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:55.973935 datalad_catalog-0.2.0/datalad_catalog/
--rw-r--r--   0 runner    (1001) docker     (122)      961 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      498 2022-11-24 08:01:55.973935 datalad_catalog-0.2.0/datalad_catalog/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:55.945935 datalad_catalog-0.2.0/datalad_catalog/catalog/
--rw-r--r--   0 runner    (1001) docker     (122)     2390 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:55.945935 datalad_catalog-0.2.0/datalad_catalog/catalog/artwork/
--rw-r--r--   0 runner    (1001) docker     (122)    15465 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/artwork/404.svg
--rw-r--r--   0 runner    (1001) docker     (122)     6792 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/artwork/catalog_logo.svg
--rw-r--r--   0 runner    (1001) docker     (122)     5821 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/artwork/datalad_catalog_logo_1_dark.svg
--rw-r--r--   0 runner    (1001) docker     (122)     5836 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/artwork/datalad_catalog_logo_1_light.svg
--rw-r--r--   0 runner    (1001) docker     (122)     3076 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/artwork/datalad_logo_wide.svg
--rw-r--r--   0 runner    (1001) docker     (122)    11021 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/artwork/ginfavicon.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:55.949935 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/
--rw-r--r--   0 runner    (1001) docker     (122)     2496 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/app.js
--rw-r--r--   0 runner    (1001) docker     (122)      324 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/app_component_about.js
--rw-r--r--   0 runner    (1001) docker     (122)    22971 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/app_component_dataset.js
--rw-r--r--   0 runner    (1001) docker     (122)     4805 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/app_component_item.js
--rw-r--r--   0 runner    (1001) docker     (122)      177 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/app_component_notfound.js
--rw-r--r--   0 runner    (1001) docker     (122)     2641 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/app_globals.js
--rw-r--r--   0 runner    (1001) docker     (122)     1486 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/app_router.js
--rw-r--r--   0 runner    (1001) docker     (122)    76102 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/bootstrap-vue.2.21.2.min.css
--rw-r--r--   0 runner    (1001) docker     (122)   360511 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/bootstrap-vue.2.21.2.min.js
--rw-r--r--   0 runner    (1001) docker     (122)   163873 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/bootstrap.5.1.3.min.css
--rw-r--r--   0 runner    (1001) docker     (122)    17473 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/brands.min.css
--rw-r--r--   0 runner    (1001) docker     (122)    19663 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/display_schema.js
--rw-r--r--   0 runner    (1001) docker     (122)   105536 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (122)    23940 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (122)   154228 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/fa-solid-900.woff2
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:55.949935 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/favicon/
--rw-r--r--   0 runner    (1001) docker     (122)      272 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/favicon/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (122)      375 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/favicon/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)    15086 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/favicon/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)    80388 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/fontawesome.min.css
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/jsonschema_authors.json
--rw-r--r--   0 runner    (1001) docker     (122)      579 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/jsonschema_catalog.json
--rw-r--r--   0 runner    (1001) docker     (122)     7070 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/jsonschema_dataset.json
--rw-r--r--   0 runner    (1001) docker     (122)     1487 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/jsonschema_extractors.json
--rw-r--r--   0 runner    (1001) docker     (122)     1954 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/jsonschema_file.json
--rw-r--r--   0 runner    (1001) docker     (122)    47938 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/marked.4.0.17.min.js
--rw-r--r--   0 runner    (1001) docker     (122)     8572 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/md5-2.3.0.js
--rw-r--r--   0 runner    (1001) docker     (122)     2643 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/meta_entry.js
--rw-r--r--   0 runner    (1001) docker     (122)     3733 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/style.css
--rw-r--r--   0 runner    (1001) docker     (122)    29206 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/vue-router.3.5.3.min.js
--rw-r--r--   0 runner    (1001) docker     (122)    94151 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/assets/vue.2.6.14.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      467 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/config.json
--rw-r--r--   0 runner    (1001) docker     (122)    16275 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/display_schema.html
--rw-r--r--   0 runner    (1001) docker     (122)     3610 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/index.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:55.949935 datalad_catalog-0.2.0/datalad_catalog/catalog/metadata/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/metadata/super.json
--rw-r--r--   0 runner    (1001) docker     (122)     6096 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/metadata-entry.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:55.949935 datalad_catalog-0.2.0/datalad_catalog/catalog/templates/
--rw-r--r--   0 runner    (1001) docker     (122)    35922 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/templates/dataset-template.html
--rw-r--r--   0 runner    (1001) docker     (122)     1379 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/templates/item-template.html
--rw-r--r--   0 runner    (1001) docker     (122)      209 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog/templates/main-template.html
--rw-r--r--   0 runner    (1001) docker     (122)    28071 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:55.949935 datalad_catalog-0.2.0/datalad_catalog/config/
--rw-r--r--   0 runner    (1001) docker     (122)      866 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/config/config.json
--rw-r--r--   0 runner    (1001) docker     (122)      966 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/config/config.yml
--rw-r--r--   0 runner    (1001) docker     (122)       43 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1401 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:55.949935 datalad_catalog-0.2.0/datalad_catalog/extractors/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4024 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/extractors/datacite_gin.py
--rw-r--r--   0 runner    (1001) docker     (122)     9805 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/meta_item.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:55.953935 datalad_catalog-0.2.0/datalad_catalog/schema/
--rw-r--r--   0 runner    (1001) docker     (122)     2587 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/schema/_bidsdataset2catalog.json
--rw-r--r--   0 runner    (1001) docker     (122)     2444 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/schema/_datacitegin2catalog.json
--rw-r--r--   0 runner    (1001) docker     (122)     2160 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/schema/_metaladcore2catalog_dataset.json
--rw-r--r--   0 runner    (1001) docker     (122)     1091 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/schema/_metaladcore2catalog_file.json
--rw-r--r--   0 runner    (1001) docker     (122)     3181 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/schema/_studyminimeta2catalog.json
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/schema/jsonschema_authors.json
--rw-r--r--   0 runner    (1001) docker     (122)      579 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/schema/jsonschema_catalog.json
--rw-r--r--   0 runner    (1001) docker     (122)     7070 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/schema/jsonschema_dataset.json
--rw-r--r--   0 runner    (1001) docker     (122)     1487 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/schema/jsonschema_extractors.json
--rw-r--r--   0 runner    (1001) docker     (122)     1954 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/schema/jsonschema_file.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:55.953935 datalad_catalog-0.2.0/datalad_catalog/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:55.957935 datalad_catalog-0.2.0/datalad_catalog/tests/data/
--rw-r--r--   0 runner    (1001) docker     (122)     5360 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/data/catalog_metadata_dataset.json
--rw-r--r--   0 runner    (1001) docker     (122)       68 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/data/catalog_metadata_invalid.json
--rw-r--r--   0 runner    (1001) docker     (122)     9652 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/data/catalog_metadata_valid.json
--rw-r--r--   0 runner    (1001) docker     (122)     8876 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_bids_dataset.json
--rw-r--r--   0 runner    (1001) docker     (122)     2833 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_bids_dataset.jsonl
--rw-r--r--   0 runner    (1001) docker     (122)     9438 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_bids_dataset2.json
--rw-r--r--   0 runner    (1001) docker     (122)     7933 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_bids_dataset2.jsonl
--rw-r--r--   0 runner    (1001) docker     (122)     8711 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_core.json
--rw-r--r--   0 runner    (1001) docker     (122)     4764 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_core.jsonl
--rw-r--r--   0 runner    (1001) docker     (122)      802 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_core_dataset.json
--rw-r--r--   0 runner    (1001) docker     (122)     5331 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_datacite_gin.json
--rw-r--r--   0 runner    (1001) docker     (122)     4337 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_datacite_gin.jsonl
--rw-r--r--   0 runner    (1001) docker     (122)    13503 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_studyminimeta.json
--rw-r--r--   0 runner    (1001) docker     (122)     6753 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_studyminimeta.jsonl
--rw-r--r--   0 runner    (1001) docker     (122)      434 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/data/test_config_file.json
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/data/test_config_file.yml
--rw-r--r--   0 runner    (1001) docker     (122)      493 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/data/workflow_generated_meta_dir.json
--rw-r--r--   0 runner    (1001) docker     (122)     6315 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/data/workflow_generated_meta_sub.json
--rw-r--r--   0 runner    (1001) docker     (122)     6641 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/data/workflow_generated_meta_super.json
--rw-r--r--   0 runner    (1001) docker     (122)      284 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/register.py
--rw-r--r--   0 runner    (1001) docker     (122)      175 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/test_action_add.py
--rw-r--r--   0 runner    (1001) docker     (122)     2995 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/test_action_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     2539 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/test_action_setsuper.py
--rw-r--r--   0 runner    (1001) docker     (122)     4724 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     1716 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/test_catalog_arguments.py
--rw-r--r--   0 runner    (1001) docker     (122)     2373 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     8928 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/test_multisource.py
--rw-r--r--   0 runner    (1001) docker     (122)     5873 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/test_node.py
--rw-r--r--   0 runner    (1001) docker     (122)     1612 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     1584 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      915 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/test_webcatalog.py
--rw-r--r--   0 runner    (1001) docker     (122)    17908 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/tests/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (122)      900 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    19582 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/webcatalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     9690 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/datalad_catalog/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:55.945935 datalad_catalog-0.2.0/datalad_catalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    19844 2022-11-24 08:01:55.000000 datalad_catalog-0.2.0/datalad_catalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6276 2022-11-24 08:01:55.000000 datalad_catalog-0.2.0/datalad_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 08:01:55.000000 datalad_catalog-0.2.0/datalad_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      218 2022-11-24 08:01:55.000000 datalad_catalog-0.2.0/datalad_catalog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       88 2022-11-24 08:01:55.000000 datalad_catalog-0.2.0/datalad_catalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2022-11-24 08:01:55.000000 datalad_catalog-0.2.0/datalad_catalog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:55.957935 datalad_catalog-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7508 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:55.957935 datalad_catalog-0.2.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:55.973935 datalad_catalog-0.2.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (122)   548128 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/_static/catalog_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (122)   457781 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/_static/datacat0_hero.svg
--rw-r--r--   0 runner    (1001) docker     (122)   457833 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/_static/datacat0_hero_lightbg.svg
--rw-r--r--   0 runner    (1001) docker     (122)  1197513 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/_static/datacat1_the_challenge.svg
--rw-r--r--   0 runner    (1001) docker     (122)   793508 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/_static/datacat2_the_opportunity.svg
--rw-r--r--   0 runner    (1001) docker     (122)  1692043 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/_static/datacat3_the_toolset.svg
--rw-r--r--   0 runner    (1001) docker     (122)  1692147 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/_static/datacat3_the_toolset_lightbg.svg
--rw-r--r--   0 runner    (1001) docker     (122)  1736126 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/_static/datacat4_the_catalog.svg
--rw-r--r--   0 runner    (1001) docker     (122)  1736178 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/_static/datacat4_the_catalog_lightbg.svg
--rw-r--r--   0 runner    (1001) docker     (122)   370286 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/_static/datacat_logo.svg
--rw-r--r--   0 runner    (1001) docker     (122)   638140 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/_static/datalad_catalog_demo.svg
--rw-r--r--   0 runner    (1001) docker     (122)    61542 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/_static/datalad_catalog_functionality.svg
--rw-r--r--   0 runner    (1001) docker     (122)  2103419 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/_static/datalad_catalog_logo_1_dark.svg
--rw-r--r--   0 runner    (1001) docker     (122)      958 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/_static/datalad_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:55.941935 datalad_catalog-0.2.0/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 08:01:55.973935 datalad_catalog-0.2.0/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (122)      436 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1220 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/catalog_schema.rst
--rw-r--r--   0 runner    (1001) docker     (122)       66 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (122)      111 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/command_line_reference.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4821 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      362 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1214 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2609 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3277 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/metadata_formats.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5107 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/overview.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8408 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/pipeline_description.rst
--rw-r--r--   0 runner    (1001) docker     (122)      134 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/python_module_reference.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4375 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (122)      343 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1376 2022-11-24 08:01:55.973935 datalad_catalog-0.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1146 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    68611 2022-11-24 08:01:45.000000 datalad_catalog-0.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:35.654828 datalad_catalog-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/CONTRIBUTORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19844 2023-03-07 12:46:35.654828 datalad_catalog-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19370 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:35.618825 datalad_catalog-0.2.1/_datalad_buildsupport/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/_datalad_buildsupport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/_datalad_buildsupport/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/_datalad_buildsupport/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:35.654828 datalad_catalog-0.2.1/datalad_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-03-07 12:46:35.654828 datalad_catalog-0.2.1/datalad_catalog/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:35.622826 datalad_catalog-0.2.1/datalad_catalog/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:35.622826 datalad_catalog-0.2.1/datalad_catalog/catalog/artwork/
+-rw-r--r--   0 runner    (1001) docker     (123)    15465 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/artwork/404.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/artwork/catalog_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/artwork/datalad_catalog_logo_1_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/artwork/datalad_catalog_logo_1_light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/artwork/datalad_logo_wide.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/artwork/ginfavicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:35.626826 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/app_component_about.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22971 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/app_component_dataset.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/app_component_item.js
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/app_component_notfound.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/app_globals.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/app_router.js
+-rw-r--r--   0 runner    (1001) docker     (123)    76102 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/bootstrap-vue.2.21.2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   360511 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/bootstrap-vue.2.21.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   163873 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/bootstrap.5.1.3.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17473 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/brands.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    19663 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/display_schema.js
+-rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   154228 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/fa-solid-900.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:35.626826 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/favicon/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/favicon/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/favicon/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/favicon/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    80388 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/fontawesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/jsonschema_authors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/jsonschema_catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/jsonschema_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/jsonschema_extractors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/jsonschema_file.json
+-rw-r--r--   0 runner    (1001) docker     (123)    47938 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/marked.4.0.17.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/md5-2.3.0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/meta_entry.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)    29206 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/vue-router.3.5.3.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    94151 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/assets/vue.2.6.14.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16275 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/display_schema.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:35.626826 datalad_catalog-0.2.1/datalad_catalog/catalog/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/metadata/super.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/metadata-entry.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:35.630826 datalad_catalog-0.2.1/datalad_catalog/catalog/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    35922 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/templates/dataset-template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/templates/item-template.html
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog/templates/main-template.html
+-rw-r--r--   0 runner    (1001) docker     (123)    28071 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:35.630826 datalad_catalog-0.2.1/datalad_catalog/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/config/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/config/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:35.630826 datalad_catalog-0.2.1/datalad_catalog/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/extractors/datacite_gin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/meta_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:35.630826 datalad_catalog-0.2.1/datalad_catalog/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/schema/_bidsdataset2catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/schema/_datacitegin2catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/schema/_metaladcore2catalog_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/schema/_metaladcore2catalog_file.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/schema/_studyminimeta2catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/schema/jsonschema_authors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/schema/jsonschema_catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/schema/jsonschema_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/schema/jsonschema_extractors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/schema/jsonschema_file.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:35.630826 datalad_catalog-0.2.1/datalad_catalog/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:35.634827 datalad_catalog-0.2.1/datalad_catalog/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/data/catalog_metadata_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/data/catalog_metadata_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/data/catalog_metadata_valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_bids_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_bids_dataset.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_bids_dataset2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_bids_dataset2.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_core.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_core.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_core_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_datacite_gin.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_datacite_gin.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_studyminimeta.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_studyminimeta.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/data/test_config_file.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/data/test_config_file.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/data/workflow_generated_meta_dir.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/data/workflow_generated_meta_sub.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/data/workflow_generated_meta_super.json
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/test_action_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/test_action_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/test_action_setsuper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/test_catalog_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/test_multisource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/test_webcatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17952 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/tests/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19582 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/webcatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/datalad_catalog/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:35.622826 datalad_catalog-0.2.1/datalad_catalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19844 2023-03-07 12:46:35.000000 datalad_catalog-0.2.1/datalad_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-03-07 12:46:35.000000 datalad_catalog-0.2.1/datalad_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 12:46:35.000000 datalad_catalog-0.2.1/datalad_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-07 12:46:35.000000 datalad_catalog-0.2.1/datalad_catalog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-07 12:46:35.000000 datalad_catalog-0.2.1/datalad_catalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-07 12:46:35.000000 datalad_catalog-0.2.1/datalad_catalog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:35.634827 datalad_catalog-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:35.638827 datalad_catalog-0.2.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:35.654828 datalad_catalog-0.2.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   548128 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/_static/catalog_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)   457781 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/_static/datacat0_hero.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   457833 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/_static/datacat0_hero_lightbg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1197513 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/_static/datacat1_the_challenge.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   793508 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/_static/datacat2_the_opportunity.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1692043 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/_static/datacat3_the_toolset.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1692147 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/_static/datacat3_the_toolset_lightbg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1736126 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/_static/datacat4_the_catalog.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1736178 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/_static/datacat4_the_catalog_lightbg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   370286 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/_static/datacat_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   638140 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/_static/datalad_catalog_demo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    61542 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/_static/datalad_catalog_functionality.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  2103419 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/_static/datalad_catalog_logo_1_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/_static/datalad_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:35.618825 datalad_catalog-0.2.1/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:46:35.654828 datalad_catalog-0.2.1/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/catalog_schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/command_line_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/metadata_formats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/pipeline_description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/python_module_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-03-07 12:46:35.654828 datalad_catalog-0.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1146 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-03-07 12:46:23.000000 datalad_catalog-0.2.1/versioneer.py
```

### Comparing `datalad_catalog-0.2.0/LICENSE` & `datalad_catalog-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/PKG-INFO` & `datalad_catalog-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad_catalog
-Version: 0.2.0
+Version: 0.2.1
 Summary: DataLad Catalog
 Home-page: https://github.com/datalad/datalad-catalog
 Author: DataLad Developers
 Author-email: team@datalad.org
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `datalad_catalog-0.2.0/README.md` & `datalad_catalog-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/_datalad_buildsupport/__init__.py` & `datalad_catalog-0.2.1/_datalad_buildsupport/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/_datalad_buildsupport/formatters.py` & `datalad_catalog-0.2.1/_datalad_buildsupport/formatters.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/_datalad_buildsupport/setup.py` & `datalad_catalog-0.2.1/_datalad_buildsupport/setup.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/__init__.py` & `datalad_catalog-0.2.1/datalad_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/README.md` & `datalad_catalog-0.2.1/datalad_catalog/catalog/README.md`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/artwork/404.svg` & `datalad_catalog-0.2.1/datalad_catalog/catalog/artwork/404.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/artwork/catalog_logo.svg` & `datalad_catalog-0.2.1/datalad_catalog/catalog/artwork/catalog_logo.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/artwork/datalad_catalog_logo_1_dark.svg` & `datalad_catalog-0.2.1/datalad_catalog/catalog/artwork/datalad_catalog_logo_1_dark.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/artwork/datalad_catalog_logo_1_light.svg` & `datalad_catalog-0.2.1/datalad_catalog/catalog/artwork/datalad_catalog_logo_1_light.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/artwork/datalad_logo_wide.svg` & `datalad_catalog-0.2.1/datalad_catalog/catalog/artwork/datalad_logo_wide.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/artwork/ginfavicon.png` & `datalad_catalog-0.2.1/datalad_catalog/catalog/artwork/ginfavicon.png`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/app.js` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/app.js`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/app_component_dataset.js` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/app_component_dataset.js`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/app_component_item.js` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/app_component_item.js`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/app_globals.js` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/app_globals.js`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/app_router.js` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/app_router.js`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/bootstrap-vue.2.21.2.min.css` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/bootstrap-vue.2.21.2.min.css`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/bootstrap-vue.2.21.2.min.js` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/bootstrap-vue.2.21.2.min.js`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/bootstrap.5.1.3.min.css` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/bootstrap.5.1.3.min.css`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/brands.min.css` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/brands.min.css`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/display_schema.js` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/display_schema.js`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/fa-brands-400.woff2` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/fa-regular-400.woff2` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/fa-solid-900.woff2` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/favicon/favicon.ico` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/fontawesome.min.css` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/jsonschema_authors.json` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/jsonschema_authors.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/jsonschema_catalog.json` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/jsonschema_catalog.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/jsonschema_dataset.json` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/jsonschema_dataset.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/jsonschema_extractors.json` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/jsonschema_extractors.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/jsonschema_file.json` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/jsonschema_file.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/marked.4.0.17.min.js` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/marked.4.0.17.min.js`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/md5-2.3.0.js` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/md5-2.3.0.js`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/meta_entry.js` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/meta_entry.js`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/style.css` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/style.css`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/vue-router.3.5.3.min.js` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/vue-router.3.5.3.min.js`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/assets/vue.2.6.14.min.js` & `datalad_catalog-0.2.1/datalad_catalog/catalog/assets/vue.2.6.14.min.js`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/display_schema.html` & `datalad_catalog-0.2.1/datalad_catalog/catalog/display_schema.html`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/index.html` & `datalad_catalog-0.2.1/datalad_catalog/catalog/index.html`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/metadata-entry.html` & `datalad_catalog-0.2.1/datalad_catalog/catalog/metadata-entry.html`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/templates/dataset-template.html` & `datalad_catalog-0.2.1/datalad_catalog/catalog/templates/dataset-template.html`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog/templates/item-template.html` & `datalad_catalog-0.2.1/datalad_catalog/catalog/templates/item-template.html`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/catalog.py` & `datalad_catalog-0.2.1/datalad_catalog/catalog.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     Node,
     WebCatalog,
 )
 
 # Create named logger
 lgr = logging.getLogger("datalad.catalog.catalog")
 
+
 # Decoration auto-generates standard help
 @build_doc
 # All extension commands must be derived from Interface
 class Catalog(Interface):
     # first docstring line is used a short description in the cmdline help
     # the rest is put in the verbose help and manpage
     """Generate a user-friendly web-based data catalog from structured
@@ -268,15 +269,14 @@
         dataset_id=None,
         dataset_version=None,
         force: bool = False,
         config_file=None,
         dataset_path=None,
         subdataset_path=None,
     ):
-
         """
         [summary]
 
         Args:
             catalog_action (str): [description]
             catalog_dir ([type], optional): [description]. Defaults to None.
             metadata ([type], optional): [description]. Defaults to None.
```

### Comparing `datalad_catalog-0.2.0/datalad_catalog/config/config.json` & `datalad_catalog-0.2.1/datalad_catalog/config/config.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/config/config.yml` & `datalad_catalog-0.2.1/datalad_catalog/config/config.yml`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/constants.py` & `datalad_catalog-0.2.1/datalad_catalog/constants.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/extractors/datacite_gin.py` & `datalad_catalog-0.2.1/datalad_catalog/extractors/datacite_gin.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,20 +14,23 @@
 
 from datalad_metalad.extractors.base import (
     DatasetMetadataExtractor,
     DataOutputCategory,
     ExtractorResult,
 )
 from datalad.log import log_progress
-from datalad.metadata.definitions import vocabulary_id
 from datalad.utils import assure_unicode
 
 
 lgr = logging.getLogger("datalad.metadata.extractors.datacite_gin")
 
+# From metalad legacy; TODO: remove/replace when it becomes useful
+# identifiers that defines an ontology as a whole
+vocabulary_id = "http://purl.org/dc/dcam/VocabularyEncodingScheme"
+
 datacite_context = {
     "@id": "https://gin.g-node.org/G-Node/Info/src/master/datacite.yml",
     "description": "ad-hoc vocabulary for the DataCite GIN yml format",
     "type": vocabulary_id,
 }
```

### Comparing `datalad_catalog-0.2.0/datalad_catalog/meta_item.py` & `datalad_catalog-0.2.1/datalad_catalog/meta_item.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/schema/_bidsdataset2catalog.json` & `datalad_catalog-0.2.1/datalad_catalog/schema/_bidsdataset2catalog.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/schema/_datacitegin2catalog.json` & `datalad_catalog-0.2.1/datalad_catalog/schema/_datacitegin2catalog.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/schema/_metaladcore2catalog_dataset.json` & `datalad_catalog-0.2.1/datalad_catalog/schema/_metaladcore2catalog_dataset.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/schema/_metaladcore2catalog_file.json` & `datalad_catalog-0.2.1/datalad_catalog/schema/_metaladcore2catalog_file.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/schema/_studyminimeta2catalog.json` & `datalad_catalog-0.2.1/datalad_catalog/schema/_studyminimeta2catalog.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/schema/jsonschema_authors.json` & `datalad_catalog-0.2.1/datalad_catalog/schema/jsonschema_authors.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/schema/jsonschema_catalog.json` & `datalad_catalog-0.2.1/datalad_catalog/schema/jsonschema_catalog.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/schema/jsonschema_dataset.json` & `datalad_catalog-0.2.1/datalad_catalog/schema/jsonschema_dataset.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/schema/jsonschema_extractors.json` & `datalad_catalog-0.2.1/datalad_catalog/schema/jsonschema_extractors.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/schema/jsonschema_file.json` & `datalad_catalog-0.2.1/datalad_catalog/schema/jsonschema_file.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/data/catalog_metadata_dataset.json` & `datalad_catalog-0.2.1/datalad_catalog/tests/data/catalog_metadata_dataset.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/data/catalog_metadata_valid.json` & `datalad_catalog-0.2.1/datalad_catalog/tests/data/catalog_metadata_valid.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_bids_dataset.json` & `datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_bids_dataset.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_bids_dataset.jsonl` & `datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_bids_dataset.jsonl`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_bids_dataset2.json` & `datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_bids_dataset2.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_bids_dataset2.jsonl` & `datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_bids_dataset2.jsonl`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_core.json` & `datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_core.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_core.jsonl` & `datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_core.jsonl`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_core_dataset.json` & `datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_core_dataset.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_datacite_gin.json` & `datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_datacite_gin.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_datacite_gin.jsonl` & `datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_datacite_gin.jsonl`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_studyminimeta.json` & `datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_studyminimeta.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/data/metadata_studyminimeta.jsonl` & `datalad_catalog-0.2.1/datalad_catalog/tests/data/metadata_studyminimeta.jsonl`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/data/test_config_file.yml` & `datalad_catalog-0.2.1/datalad_catalog/tests/data/test_config_file.yml`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/data/workflow_generated_meta_sub.json` & `datalad_catalog-0.2.1/datalad_catalog/tests/data/workflow_generated_meta_sub.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/data/workflow_generated_meta_super.json` & `datalad_catalog-0.2.1/datalad_catalog/tests/data/workflow_generated_meta_super.json`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/test_action_create.py` & `datalad_catalog-0.2.1/datalad_catalog/tests/test_action_create.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/test_action_setsuper.py` & `datalad_catalog-0.2.1/datalad_catalog/tests/test_action_setsuper.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/test_catalog.py` & `datalad_catalog-0.2.1/datalad_catalog/tests/test_catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,14 @@
             metadata_file,
         ],
     )
 
 
 @with_tempfile(content="[]")
 def test_metadata_type_mismatch_detection(metadata_file: str = ""):
-
     with patch("datalad_catalog.catalog.lgr") as lgr_mock:
         assert_raises(
             ValidationError,
             _unwind,
             _validate_metadata,
             [
                 metadata_file,
@@ -121,30 +120,28 @@
     ) as f2, patch("datalad_catalog.catalog._serve_catalog") as f3, patch(
         "datalad_catalog.catalog._add_to_catalog"
     ) as f4, patch(
         "datalad_catalog.catalog._remove_from_catalog"
     ) as f5, patch(
         "datalad_catalog.catalog._set_super_of_catalog"
     ) as f6:
-
         for mock, name in zip(
             (f1, f2, f3, f4, f5, f6), (f"f{i}" for i in range(1, 7))
         ):
             mock.return_value = iter([{**result_template, "action": name}])
 
         results = []
         for action, create_dir in (
             ("create", False),
             ("validate", False),
             ("add", True),
             ("remove", True),
             ("set-super", True),
             ("serve", True),
         ):
-
             test_catalog_path = Path(temp_dir) / "test_catalog"
 
             if create_dir:
                 try:
                     test_catalog_path.mkdir()
                     (test_catalog_path / "assets").mkdir()
                     (test_catalog_path / "artwork").mkdir()
```

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/test_catalog_arguments.py` & `datalad_catalog-0.2.1/datalad_catalog/tests/test_catalog_arguments.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/test_config.py` & `datalad_catalog-0.2.1/datalad_catalog/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/test_multisource.py` & `datalad_catalog-0.2.1/datalad_catalog/tests/test_multisource.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/test_node.py` & `datalad_catalog-0.2.1/datalad_catalog/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/test_schema.py` & `datalad_catalog-0.2.1/datalad_catalog/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/test_translate.py` & `datalad_catalog-0.2.1/datalad_catalog/tests/test_translate.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/test_utils.py` & `datalad_catalog-0.2.1/datalad_catalog/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/test_webcatalog.py` & `datalad_catalog-0.2.1/datalad_catalog/tests/test_webcatalog.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/tests/test_workflow.py` & `datalad_catalog-0.2.1/datalad_catalog/tests/test_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 )
 from datalad.tests.utils_pytest import (
     with_tree,
     with_tempfile,
     assert_equal,
     assert_repo_status,
     skip_if_adjusted_branch,
+    skip_if_on_windows,
 )
 from datalad.api import create, Dataset
 
 import json
 import pytest
 
 package_path = Path(__file__).resolve().parent.parent
@@ -294,14 +295,15 @@
             "datacite.yml": datacitegin_content,
             "random_file.txt": "some content",
         },
     },
 }
 
 
+@skip_if_on_windows
 @skip_if_adjusted_branch
 @with_tree(tree=super_ds_tree)
 @with_tempfile(mkdir=True)
 def test_workflow_new(super_path=None, cat_path=None):
     ckwa = dict(result_renderer="disabled")
     # Create super and subdataset, save all
     sub_ds = create(super_path + "/some_dir/subdataset", force=True, **ckwa)
```

### Comparing `datalad_catalog-0.2.0/datalad_catalog/utils.py` & `datalad_catalog-0.2.1/datalad_catalog/utils.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/webcatalog.py` & `datalad_catalog-0.2.1/datalad_catalog/webcatalog.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/datalad_catalog/workflows.py` & `datalad_catalog-0.2.1/datalad_catalog/workflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         recursion_limit=1,
         on_failure="continue",
     )
     # Create catalog
     cat = catalog
     if not cat.is_created():
         cat.create()
+
     # Call per-dataset workflow
     def _dataset_workflow_inner(ds, refds, **kwargs):
         """Internal function to allow passing"""
         return dataset_workflow(ds, catalog=cat, **kwargs)
 
     try:
         # for the superdataset and all top-level subdatasets
```

### Comparing `datalad_catalog-0.2.0/datalad_catalog.egg-info/PKG-INFO` & `datalad_catalog-0.2.1/datalad_catalog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad-catalog
-Version: 0.2.0
+Version: 0.2.1
 Summary: DataLad Catalog
 Home-page: https://github.com/datalad/datalad-catalog
 Author: DataLad Developers
 Author-email: team@datalad.org
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `datalad_catalog-0.2.0/datalad_catalog.egg-info/SOURCES.txt` & `datalad_catalog-0.2.1/datalad_catalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/Makefile` & `datalad_catalog-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/_static/catalog_screenshot.png` & `datalad_catalog-0.2.1/docs/source/_static/catalog_screenshot.png`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/_static/datacat0_hero.svg` & `datalad_catalog-0.2.1/docs/source/_static/datacat0_hero.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/_static/datacat0_hero_lightbg.svg` & `datalad_catalog-0.2.1/docs/source/_static/datacat0_hero_lightbg.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/_static/datacat1_the_challenge.svg` & `datalad_catalog-0.2.1/docs/source/_static/datacat1_the_challenge.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/_static/datacat2_the_opportunity.svg` & `datalad_catalog-0.2.1/docs/source/_static/datacat2_the_opportunity.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/_static/datacat3_the_toolset.svg` & `datalad_catalog-0.2.1/docs/source/_static/datacat3_the_toolset.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/_static/datacat3_the_toolset_lightbg.svg` & `datalad_catalog-0.2.1/docs/source/_static/datacat3_the_toolset_lightbg.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/_static/datacat4_the_catalog.svg` & `datalad_catalog-0.2.1/docs/source/_static/datacat4_the_catalog.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/_static/datacat4_the_catalog_lightbg.svg` & `datalad_catalog-0.2.1/docs/source/_static/datacat4_the_catalog_lightbg.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/_static/datacat_logo.svg` & `datalad_catalog-0.2.1/docs/source/_static/datacat_logo.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/_static/datalad_catalog_demo.svg` & `datalad_catalog-0.2.1/docs/source/_static/datalad_catalog_demo.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/_static/datalad_catalog_functionality.svg` & `datalad_catalog-0.2.1/docs/source/_static/datalad_catalog_functionality.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/_static/datalad_catalog_logo_1_dark.svg` & `datalad_catalog-0.2.1/docs/source/_static/datalad_catalog_logo_1_dark.svg`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/_static/datalad_logo.png` & `datalad_catalog-0.2.1/docs/source/_static/datalad_logo.png`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/catalog_schema.rst` & `datalad_catalog-0.2.1/docs/source/catalog_schema.rst`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/conf.py` & `datalad_catalog-0.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/index.rst` & `datalad_catalog-0.2.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/installation.rst` & `datalad_catalog-0.2.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/metadata_formats.rst` & `datalad_catalog-0.2.1/docs/source/metadata_formats.rst`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/overview.rst` & `datalad_catalog-0.2.1/docs/source/overview.rst`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/pipeline_description.rst` & `datalad_catalog-0.2.1/docs/source/pipeline_description.rst`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/docs/source/usage.rst` & `datalad_catalog-0.2.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/setup.cfg` & `datalad_catalog-0.2.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 [options]
 python_requires = >= 3.7
 install_requires = 
 	datalad >= 0.17
 	datalad-metalad >= 0.4.1
 	jsonschema
 	pyyaml
-	jq
+	jq;platform_system!='Windows'
 packages = find:
 include_package_data = True
 
 [options.package_data]
 * = catalog/*, catalog/artwork/*, catalog/assets/*, catalog/assets/favicon/*, catalog/metadata/*, catalog/templates/*, config/*, schema/*, tests/data/*
 
 [options.extras_require]
```

### Comparing `datalad_catalog-0.2.0/setup.py` & `datalad_catalog-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `datalad_catalog-0.2.0/versioneer.py` & `datalad_catalog-0.2.1/versioneer.py`

 * *Files identical despite different names*

