# Comparing `tmp/ubkg_api-0.0.1.tar.gz` & `tmp/ubkg_api-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "ubkg_api-1.3.0.tar", last modified: Wed May 24 15:11:05 2023, max compression
```

## Comparing `ubkg_api-0.0.1.tar` & `ubkg_api-1.3.0.tar`

### file list

```diff
@@ -1,72 +1,73 @@
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/.dockerignore
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/VERSION
--rwxr-xr-x   0        0        0      739 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/generate-build-version.sh
--rw-r--r--   0        0        0    29283 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/ubkg-api-spec.yaml
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/docker/docker-compose.deployment.data-distillery.api.yml
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/docker/docker-compose.deployment.data-distillery.neo4j.yml
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/docker/docker-compose.deployment.hubmap.api.yml
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/docker/docker-compose.deployment.hubmap.neo4j.yml
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/docker/docker-compose.localhost.yml
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/docker/ubkg-api/Dockerfile
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/docker/ubkg-api/entrypoint.sh
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/docker/ubkg-api/start.sh
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/docker/ubkg-api/nginx/nginx.conf
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/docker/ubkg-api/nginx/conf.d/ubkg-api.conf
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/log/README.md
--rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/postman/HuBMAP Ontology API.postman_collection.json
--rw-r--r--   0        0        0    12357 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/postman/HuBMAP Ontology Dev Cypers.postman_collection.json
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/instance/app.cfg
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/__init__.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/app.py
--rw-r--r--   0        0        0    54272 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/neo4j_manager.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/requirements.txt
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/uwsgi.ini
--rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/wsgi.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/instance/app.cfg.example
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/__init__.py
--rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/assay_type_property_info.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/base_model_.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/codes_codes_obj.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/concept_detail.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/concept_prefterm.py
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/concept_sab_rel.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/concept_sab_rel_depth.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/concept_term.py
--rw-r--r--   0        0        0     8368 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/dataset_property_info.py
--rw-r--r--   0        0        0     5645 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/qconcept_tconcept_sab_rel.py
--rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/qqst.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/sab_code_term.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/sab_code_term_rui_code.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/sab_definition.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/sab_relationship_concept_prefterm.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/sab_relationship_concept_term.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/semantic_stn.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/sty_tui_stn.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/termtype_code.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/typing_utils.py
--rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/models/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/routes/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/routes/assaytype/__init__.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/routes/assaytype/assaytype_controller.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/routes/codes/__init__.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/routes/codes/codes_controller.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/routes/concepts/__init__.py
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/routes/concepts/concepts_controller.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/routes/datasets/__init__.py
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/routes/datasets/datasets_controller.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/routes/organs/__init__.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/routes/organs/organs_controller.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/routes/semantics/__init__.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/routes/semantics/semantics_controller.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/routes/terms/__init__.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/routes/terms/terms_controller.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/routes/tui/__init__.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/routes/tui/tui_controller.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/routes/valueset/__init__.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/src/ubkg_api/routes/valueset/valueset_controller.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/LICENSE
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/README.md
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 ubkg_api-0.0.1/PKG-INFO
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.650232 ubkg_api-1.3.0/
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1087 2023-04-26 01:44:08.000000 ubkg_api-1.3.0/LICENSE
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1423 2023-05-24 15:11:05.649984 ubkg_api-1.3.0/PKG-INFO
+-rw-r--r--   0 ZHY19      (503) staff       (20)      850 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/README.md
+-rw-r--r--   0 ZHY19      (503) staff       (20)      761 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/pyproject.toml
+-rw-r--r--   0 ZHY19      (503) staff       (20)       38 2023-05-24 15:11:05.650282 ubkg_api-1.3.0/setup.cfg
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.547011 ubkg_api-1.3.0/src/
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.569704 ubkg_api-1.3.0/src/ubkg_api/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        1 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3649 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/app.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.624138 ubkg_api-1.3.0/src/ubkg_api/models/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     6262 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/assay_type_property_info.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1900 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/base_model_.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2518 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/codes_codes_obj.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2037 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/concept_detail.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2069 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/concept_prefterm.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2615 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/concept_sab_rel.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3336 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/concept_sab_rel_depth.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1909 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/concept_term.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     8368 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/dataset_property_info.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     5645 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3704 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/qconcept_tconcept_sab_rel.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3677 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/qqst.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2404 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/sab_code_term.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      472 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/sab_code_term_rui_code.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1988 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/sab_definition.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3895 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/sab_relationship_concept_prefterm.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3537 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/sab_relationship_concept_term.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1909 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/semantic_stn.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2314 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/sty_tui_stn.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1949 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/termtype_code.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      809 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/typing_utils.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3507 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/util.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)    55155 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/neo4j_manager.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.626485 ubkg_api-1.3.0/src/ubkg_api/routes/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/__init__.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.629116 ubkg_api-1.3.0/src/ubkg_api/routes/assaytype/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/assaytype/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1338 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/assaytype/assaytype_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.631552 ubkg_api-1.3.0/src/ubkg_api/routes/codes/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/codes/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1179 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/codes/codes_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.634148 ubkg_api-1.3.0/src/ubkg_api/routes/concepts/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/concepts/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     4450 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/concepts/concepts_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.636693 ubkg_api-1.3.0/src/ubkg_api/routes/datasets/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/datasets/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2684 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/datasets/datasets_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.639140 ubkg_api-1.3.0/src/ubkg_api/routes/organs/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/organs/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      750 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/organs/organs_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.641076 ubkg_api-1.3.0/src/ubkg_api/routes/semantics/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/semantics/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      633 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/semantics/semantics_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.643147 ubkg_api-1.3.0/src/ubkg_api/routes/terms/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/terms/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1471 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/terms/terms_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.645100 ubkg_api-1.3.0/src/ubkg_api/routes/tui/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/tui/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      559 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/tui/tui_controller.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      364 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/validate.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.647409 ubkg_api-1.3.0/src/ubkg_api/routes/valueset/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/valueset/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1396 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/valueset/valueset_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.572192 ubkg_api-1.3.0/src/ubkg_api.egg-info/
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1423 2023-05-24 15:11:05.000000 ubkg_api-1.3.0/src/ubkg_api.egg-info/PKG-INFO
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2124 2023-05-24 15:11:05.000000 ubkg_api-1.3.0/src/ubkg_api.egg-info/SOURCES.txt
+-rw-r--r--   0 ZHY19      (503) staff       (20)        1 2023-05-24 15:11:05.000000 ubkg_api-1.3.0/src/ubkg_api.egg-info/dependency_links.txt
+-rw-r--r--   0 ZHY19      (503) staff       (20)       68 2023-05-24 15:11:05.000000 ubkg_api-1.3.0/src/ubkg_api.egg-info/requires.txt
+-rw-r--r--   0 ZHY19      (503) staff       (20)        9 2023-05-24 15:11:05.000000 ubkg_api-1.3.0/src/ubkg_api.egg-info/top_level.txt
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.649579 ubkg_api-1.3.0/tests/
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3136 2023-05-24 14:49:10.000000 ubkg_api-1.3.0/tests/test_controllers.py
```

### Comparing `ubkg_api-0.0.1/src/ubkg_api/neo4j_manager.py` & `ubkg_api-1.3.0/src/ubkg_api/neo4j_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import logging
 import re
 from typing import List
 
 import neo4j
 
-from ubkg_api.models.assay_type_property_info import AssayTypePropertyInfo
-from ubkg_api.models.codes_codes_obj import CodesCodesObj
-from ubkg_api.models.concept_detail import ConceptDetail
-from ubkg_api.models.concept_prefterm import ConceptPrefterm
-from ubkg_api.models.concept_sab_rel_depth import ConceptSabRelDepth
-from ubkg_api.models.concept_term import ConceptTerm
-from ubkg_api.models.dataset_property_info import DatasetPropertyInfo
-from ubkg_api.models.path_item_concept_relationship_sab_prefterm import \
+from models.assay_type_property_info import AssayTypePropertyInfo
+from models.codes_codes_obj import CodesCodesObj
+from models.concept_detail import ConceptDetail
+from models.concept_prefterm import ConceptPrefterm
+from models.concept_sab_rel_depth import ConceptSabRelDepth
+from models.concept_term import ConceptTerm
+from models.dataset_property_info import DatasetPropertyInfo
+from models.path_item_concept_relationship_sab_prefterm import \
     PathItemConceptRelationshipSabPrefterm
-from ubkg_api.models.qqst import QQST
-from ubkg_api.models.sab_code_term import SabCodeTerm
-from ubkg_api.models.sab_code_term_rui_code import SabCodeTermRuiCode
-from ubkg_api.models.sab_definition import SabDefinition
-from ubkg_api.models.sab_relationship_concept_prefterm import SabRelationshipConceptPrefterm
-from ubkg_api.models.sab_relationship_concept_term import SabRelationshipConceptTerm
-from ubkg_api.models.semantic_stn import SemanticStn
-from ubkg_api.models.sty_tui_stn import StyTuiStn
-from ubkg_api.models.termtype_code import TermtypeCode
+from models.qqst import QQST
+from models.sab_code_term import SabCodeTerm
+from models.sab_code_term_rui_code import SabCodeTermRuiCode
+from models.sab_definition import SabDefinition
+from models.sab_relationship_concept_prefterm import SabRelationshipConceptPrefterm
+from models.sab_relationship_concept_term import SabRelationshipConceptTerm
+from models.semantic_stn import SemanticStn
+from models.sty_tui_stn import StyTuiStn
+from models.termtype_code import TermtypeCode
 
 logging.basicConfig(format='[%(asctime)s] %(levelname)s in %(module)s:%(lineno)d: %(message)s',
                     datefmt='%Y-%m-%d %H:%M:%S',
                     level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 cypher_tail: str = \
@@ -87,14 +87,24 @@
         if not re.match(r"\*|[a-zA-Z_]+", r[0]):
             raise Exception(f"Invalid Type in rel optional parameter list", 400)
         if not re.match(r"\*|[a-zA-Z_]+", r[1]):
             raise Exception(f"Invalid SAB in rel optional parameter list", 400)
     return rel_list
 
 
+def make_assaytype_property_info(record):
+    return AssayTypePropertyInfo(
+        record['data_type'],
+        record['primary'],
+        record['description'],
+        record['vitessce_hints'],
+        record['contains_pii'],
+        record['vis_only'])
+
+
 instance = None
 
 
 class Neo4jManager(object):
     @staticmethod
     def create(server, username, password):
         if instance is not None:
@@ -575,25 +585,26 @@
         query = query + 'WHERE conceptChild.CUI = conceptChildCUI '
         query = query + 'AND ' + sab_case + ' = minSAB '
         query = query + 'RETURN codeChild '
         query = query + 'ORDER BY codeChild.CODE '
         query = query + 'LIMIT 1'
         query = query + '} '
 
-        # Get the term associated with the child concept code with the earliest SAB.
-        query = query + 'WITH codeChild '
-        query = query + 'MATCH (termChild:Term)<-[:PT]-(codeChild:Code) '
+        # 5. Get the term associated with the child concept code with the earliest SAB.
+        query = query + 'WITH codeChild,conceptChildCUI '
+        query = query + 'MATCH (termChild:Term)<-[r:PT]-(codeChild:Code) '
+        query = query + 'WHERE r.CUI = conceptChildCUI '
         query = query + 'RETURN termChild.name AS term, codeChild.CODE as code,codeChild.SAB as sab'
 
         # Execute Cypher query and return result.
         with self.driver.session() as session:
             recds: neo4j.Result = session.run(query)
             for record in recds:
                 try:
-                    sabcodeterm: [SabCodeTerm] = SabCodeTerm(record.get('sab'), record.get('code'), record.get('term'))
+                    sabcodeterm: [SabCodeTerm] = SabCodeTerm(record.get('sab'), record.get('code'), record.get('term')).serialize()
                     sabcodeterms.append(sabcodeterm)
                 except KeyError:
                     pass
 
         return sabcodeterms
 
     def __subquery_dataset_synonym_property(self, sab: str, cuialias: str, returnalias: str,
@@ -924,14 +935,32 @@
 
                         datasets.append(dataset)
                     except KeyError:
                         pass
 
         return datasets
 
+    def assaytype_get(self, primary: bool, application_context: str = 'HUBMAP') -> AssayTypePropertyInfo:
+        # Build the Cypher query that will return the table of data.
+        query = self.__query_cypher_dataset_info(application_context)
+
+        assaytypes: List[dict] = []
+        # Execute Cypher query and return result.
+        with self.driver.session() as session:
+            recds: neo4j.Result = session.run(query)
+            for record in recds:
+                if primary is None:
+                    assaytypes.append(make_assaytype_property_info(record).serialize())
+                elif primary is True and record['primary'] is True:
+                    assaytypes.append(make_assaytype_property_info(record).serialize())
+                elif primary is False and record['primary'] is False:
+                    assaytypes.append(make_assaytype_property_info(record).serialize())
+        result: dict = {"result": assaytypes}
+        return result
+
     def assaytype_name_get(self, name: str, application_context: str = 'HUBMAP') -> AssayTypePropertyInfo:
         """
         This is intended to be a drop in replacement for the same endpoint in search-src.
 
         The only difference is the optional application_contect to make it consistent with a HUBMAP or SENNET
         environment.
         """
@@ -942,22 +971,15 @@
 
         # Execute Cypher query and return result.
         with self.driver.session() as session:
             recds: neo4j.Result = session.run(query)
             for record in recds:
                 if record.get('data_type') == name:
                     # Accessing the record by .get('str') does not appear to work?! :-(
-                    return AssayTypePropertyInfo(
-                        record['data_type'],
-                        record['primary'],
-                        record['description'],
-                        record['vitessce_hints'],
-                        record['contains_pii'],
-                        record['vis_only']
-                    ).serialize()
+                    return make_assaytype_property_info(record).serialize()
         return AssayTypePropertyInfo().serialize()
 
     # Objectives: Provide crosswalk information between SenNet and RUI for organ types. Replicate the original organ_types.yaml.
     # 1.FindSAB, code, and term for all organs.
     # 2.Find UBERON codes for organs.The code for Skin maps to UBERON 0002097 and UBERON 002097 cross-references
     # UMLS with CUI C1123023; however, the UMLS CUI also maps to UBERON 0000014. It is necessary to specify the
     # UBERON code explicitly.
```

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/assay_type_property_info.py` & `ubkg_api-1.3.0/src/ubkg_api/models/assay_type_property_info.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/base_model_.py` & `ubkg_api-1.3.0/src/ubkg_api/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/codes_codes_obj.py` & `ubkg_api-1.3.0/src/ubkg_api/models/codes_codes_obj.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/concept_detail.py` & `ubkg_api-1.3.0/src/ubkg_api/models/concept_detail.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/concept_prefterm.py` & `ubkg_api-1.3.0/src/ubkg_api/models/concept_prefterm.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/concept_sab_rel.py` & `ubkg_api-1.3.0/src/ubkg_api/models/concept_sab_rel.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/concept_sab_rel_depth.py` & `ubkg_api-1.3.0/src/ubkg_api/models/concept_sab_rel_depth.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/concept_term.py` & `ubkg_api-1.3.0/src/ubkg_api/models/concept_term.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/dataset_property_info.py` & `ubkg_api-1.3.0/src/ubkg_api/models/dataset_property_info.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py` & `ubkg_api-1.3.0/src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/qconcept_tconcept_sab_rel.py` & `ubkg_api-1.3.0/src/ubkg_api/models/qconcept_tconcept_sab_rel.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/qqst.py` & `ubkg_api-1.3.0/src/ubkg_api/models/qqst.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/sab_code_term.py` & `ubkg_api-1.3.0/src/ubkg_api/models/sab_code_term.py`

 * *Files 13% similar despite different names*

```diff
@@ -102,7 +102,14 @@
 
 
         :param term: The term of this SabCodeTerm.
         :type term: str
         """
 
         self._term = term
+
+    def serialize(self):
+        return {
+            "code": self._code,
+            "sab": self._sab,
+            "term": self._term
+        }
```

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/sab_definition.py` & `ubkg_api-1.3.0/src/ubkg_api/models/sab_definition.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/sab_relationship_concept_prefterm.py` & `ubkg_api-1.3.0/src/ubkg_api/models/sab_relationship_concept_prefterm.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/sab_relationship_concept_term.py` & `ubkg_api-1.3.0/src/ubkg_api/models/sab_relationship_concept_term.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/semantic_stn.py` & `ubkg_api-1.3.0/src/ubkg_api/models/semantic_stn.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/sty_tui_stn.py` & `ubkg_api-1.3.0/src/ubkg_api/models/sty_tui_stn.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/termtype_code.py` & `ubkg_api-1.3.0/src/ubkg_api/models/termtype_code.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/typing_utils.py` & `ubkg_api-1.3.0/src/ubkg_api/models/typing_utils.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/models/util.py` & `ubkg_api-1.3.0/src/ubkg_api/models/util.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/routes/codes/codes_controller.py` & `ubkg_api-1.3.0/src/ubkg_api/routes/codes/codes_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/routes/concepts/concepts_controller.py` & `ubkg_api-1.3.0/src/ubkg_api/routes/concepts/concepts_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/routes/datasets/datasets_controller.py` & `ubkg_api-1.3.0/src/ubkg_api/routes/datasets/datasets_controller.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from flask import Blueprint, jsonify, current_app, request
 
+from routes.validate import validate_application_context
+
 datasets_blueprint = Blueprint('datasets', __name__, url_prefix='/datasets')
 
 
 @datasets_blueprint.route('', methods=['GET'])
-def dataset_get(application_context='HUBMAP', data_type=None, description=None, alt_name=None, primary=None, contains_pii=None,
-                vis_only=None, vitessce_hint=None, dataset_provider=None):
+def dataset_get():
     """Returns information on a set of HuBMAP or SenNet dataset types, with options to filter the list to those with specific property values. Filters are additive (i.e., boolean AND)
 
 
     :query application_context: Required filter to indicate application context.
     :type application_context: str
     :param data_type: Optional filter for data_type
     :type data_type: str
@@ -26,10 +27,15 @@
     :param vitessce_hint: Optional filter for a single element in the vitessce_hint list--i.e., return datasets for which vitessce_hints includes a value that matches the parameter. Although the field is named &#39;vitessce-hints&#39;, use &#39;vitessce_hint&#39; as an argument.
     :type vitessce_hint: str
     :param dataset_provider: Optional filter to identify the dataset provider - IEC (iec)  or external (lab)
     :type dataset_provider: str
 
     :rtype: Union[List[DatasetPropertyInfo], Tuple[List[DatasetPropertyInfo], int], Tuple[List[DatasetPropertyInfo], int, Dict[str, str]]
     """
+    application_context = validate_application_context()
     return jsonify(
-        current_app.neo4jManager.dataset_get(request.args.get('application_context'), data_type, description, alt_name, primary, contains_pii, vis_only,
-                                 vitessce_hint, dataset_provider))
+        current_app.neo4jManager.dataset_get(
+            application_context, request.args.get('data_type'),
+            request.args.get('description'), request.args.get('alt_name'), request.args.get('primary'),
+            request.args.get('contains_pii'), request.args.get('vis_only'),
+            request.args.get('vitessce_hint'), request.args.get('dataset_provider'))
+    )
```

### Comparing `ubkg_api-0.0.1/src/ubkg_api/routes/organs/organs_controller.py` & `ubkg_api-1.3.0/src/ubkg_api/routes/organs/organs_controller.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,24 @@
-from flask import Blueprint, jsonify, request, current_app
+from flask import Blueprint, jsonify, current_app
+
+from routes.validate import validate_application_context
 
 organs_blueprint = Blueprint('organs', __name__, url_prefix='/organs')
 
 
 @organs_blueprint.route('', methods=['GET'])
 def get_organ_types():
-    application_context = 'HUBMAP'
-    query_string = request.args.get('application_context')
-    if query_string is not None:
-        application_context = query_string.upper()
-    if application_context not in ['SENNET', 'HUBMAP']:
-        return jsonify(f'Invalid application_context specified ({application_context}) application_context query '
-                       f'string must be one of SENNET or HUBMAP'), 400
-    return jsonify(current_app.neo4jManager.get_organ_types(application_context))
+    application_context = validate_application_context()
+    return jsonify(current_app.neo4jManager.get_organ_types(application_context.upper()))
+
+
+@organs_blueprint.route('by-code', methods=['GET'])
+def get_organ_by_code():
+    application_context = validate_application_context()
+    data: list = current_app.neo4jManager.get_organ_types(application_context.upper())
+    result: dict = {}
+    for item in data:
+        result[item['rui_code']] = item['term'].strip()
+    return jsonify(result)
+
+
+
```

### Comparing `ubkg_api-0.0.1/src/ubkg_api/routes/semantics/semantics_controller.py` & `ubkg_api-1.3.0/src/ubkg_api/routes/semantics/semantics_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/routes/terms/terms_controller.py` & `ubkg_api-1.3.0/src/ubkg_api/routes/terms/terms_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/routes/tui/tui_controller.py` & `ubkg_api-1.3.0/src/ubkg_api/routes/tui/tui_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/src/ubkg_api/routes/valueset/valueset_controller.py` & `ubkg_api-1.3.0/src/ubkg_api/routes/valueset/valueset_controller.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,31 @@
-from flask import Blueprint, jsonify, current_app
+from flask import Blueprint, jsonify, current_app, request
 
 valueset_blueprint = Blueprint('valueset', __name__, url_prefix='/valueset')
 
 
-@valueset_blueprint.route('/', methods=['GET'])
-def valueset_get(parent_sab, parent_code, child_sabs):
+@valueset_blueprint.route('', methods=['GET'])
+def valueset_get():
     """Returns a valueset of concepts that are children (have as isa relationship) of another concept.
 
 
     :param parent_sab: the SAB of the parent concept
     :type parent_sab: str
     :param parent_code: the code of the parent concept in the SAB (local ontology)
     :type parent_code: str
     :param child_sabs: the list of SABs for child concepts, in order of preference (in case of parent concepts with cross-references)
     :type child_sabs: List[str]
 
     :rtype: Union[List[SabCodeTerm], Tuple[List[SabCodeTerm], int], Tuple[List[SabCodeTerm], int, Dict[str, str]]
     """
-    return jsonify(current_app.neo4jManager.valueset_get(parent_sab, parent_code, child_sabs))
+    child_sabs = request.args.getlist('child_sabs')
+    if child_sabs == []:
+        return jsonify("Invalid child_sabs (empty list) specified"), 400
+    parent_sab = request.args.get('parent_sab')
+    if parent_sab is None:
+        return jsonify(f"Invalid parent_sab ({parent_sab}) specified"), 400
+    parent_code = request.args.get('parent_code')
+    if parent_code is None:
+        return jsonify(f"Invalid parent_code ({parent_code}) specified"), 400
+    return jsonify(
+        current_app.neo4jManager.valueset_get(parent_sab, parent_code,
+                                              child_sabs))
```

### Comparing `ubkg_api-0.0.1/LICENSE` & `ubkg_api-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ubkg_api-0.0.1/pyproject.toml` & `ubkg_api-1.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "ubkg_api"
-version = "0.0.1"
+version = "1.3.0"
 authors = [
-  { name="Charles Kollar", email="charles.kollar@pitt.edu" },
+  { name="HuBMAP Consortium", email="api-developers@hubmapconsortium.org" },
 ]
-description = "A REST API infront of the Unified Biomedical Knowlegde Graph"
+description = "A REST API in front of the Unified Biomedical Knowlegde Graph"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "python_dateutil>=2.6.0",
     "setuptools>=21.0.0",
     "Flask==2.1.3",
     "neo4j==4.2.1"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/x-atlas-consortia/ubkg-api"
-"Bug Tracker" = "https://github.com/x-atlas-consortia/ubkg-api/issues"
+"Bug Tracker" = "https://github.com/x-atlas-consortia/ubkg-api/issues"
```

