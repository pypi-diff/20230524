# Comparing `tmp/rapidpro_flow_tools-0.8.0.tar.gz` & `tmp/rapidpro_flow_tools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpro_flow_tools-0.8.0.tar", last modified: Wed May 24 03:56:15 2023, max compression
+gzip compressed data, was "rapidpro_flow_tools-0.9.0.tar", last modified: Wed May 24 04:24:59 2023, max compression
```

## Comparing `rapidpro_flow_tools-0.8.0.tar` & `rapidpro_flow_tools-0.9.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 03:56:15.512761 rapidpro_flow_tools-0.8.0/
--rw-rw-rw-   0        0        0      242 2023-05-24 03:56:15.512761 rapidpro_flow_tools-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     2906 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/README.md
--rw-rw-rw-   0        0        0      115 2023-05-24 03:56:15.515783 rapidpro_flow_tools-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0      379 2023-05-24 03:55:57.000000 rapidpro_flow_tools-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:56:15.389012 rapidpro_flow_tools-0.8.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 03:56:15.410573 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/__init__.py
--rw-rw-rw-   0        0        0     1322 2023-05-24 03:55:45.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/flow_converter.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:56:15.426682 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:56:15.435779 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/__init__.py
--rw-rw-rw-   0        0        0     4152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/cellparser.py
--rw-rw-rw-   0        0        0     3205 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py
--rw-rw-rw-   0        0        0    15945 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/rowparser.py
--rw-rw-rw-   0        0        0     1849 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/sheetparser.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:56:15.452880 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/tests/__init__.py
--rw-rw-rw-   0        0        0      163 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/tests/mock_cell_parser.py
--rw-rw-rw-   0        0        0      292 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/tests/mock_row_parser.py
--rw-rw-rw-   0        0        0      826 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py
--rw-rw-rw-   0        0        0      600 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/tests/models.py
--rw-rw-rw-   0        0        0     6080 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py
--rw-rw-rw-   0        0        0     3508 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py
--rw-rw-rw-   0        0        0     5026 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py
--rw-rw-rw-   0        0        0     3050 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py
--rw-rw-rw-   0        0        0     2022 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py
--rw-rw-rw-   0        0        0     4684 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:56:15.465442 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/__init__.py
--rw-rw-rw-   0        0        0      152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/constants.py
--rw-rw-rw-   0        0        0     7020 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py
--rw-rw-rw-   0        0        0      932 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py
--rw-rw-rw-   0        0        0      102 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/datarowmodel.py
--rw-rw-rw-   0        0        0    26665 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/flowparser.py
--rw-rw-rw-   0        0        0     5242 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py
--rw-rw-rw-   0        0        0     1016 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:56:15.476440 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/tests/__init__.py
--rw-rw-rw-   0        0        0      478 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/tests/mock_sheetreader.py
--rw-rw-rw-   0        0        0     1030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py
--rw-rw-rw-   0        0        0    17043 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0    39668 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py
--rw-rw-rw-   0        0        0    14789 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py
--rw-rw-rw-   0        0        0      259 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/tests/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:56:15.483008 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/sheets/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/sheets/__init__.py
--rw-rw-rw-   0        0        0      626 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py
--rw-rw-rw-   0        0        0     3199 2023-05-17 13:33:29.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py
--rw-rw-rw-   0        0        0      711 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:56:15.486016 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/rapidpro/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/rapidpro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:56:15.495565 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/rapidpro/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/rapidpro/tests/__init__.py
--rw-rw-rw-   0        0        0      542 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py
--rw-rw-rw-   0        0        0     3453 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py
--rw-rw-rw-   0        0        0     4525 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py
--rw-rw-rw-   0        0        0     1304 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py
--rw-rw-rw-   0        0        0     6368 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py
--rw-rw-rw-   0        0        0       73 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/rapidpro/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:56:15.505592 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/tests/__init__.py
--rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/tests/test_flowparser.py
--rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/tests/test_flowparser_reverse.py
--rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/tests/test_template_sheet_parser.py
--rw-rw-rw-   0        0        0    11693 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/tests/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:56:15.425701 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools.egg-info/
--rw-rw-rw-   0        0        0      242 2023-05-24 03:56:15.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3297 2023-05-24 03:56:15.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 03:56:15.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-24 03:56:15.000000 rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 03:56:15.511590 rapidpro_flow_tools-0.8.0/tests/
--rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/tests/test_flowparser.py
--rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/tests/test_flowparser_reverse.py
--rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.8.0/tests/test_template_sheet_parser.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:24:59.141448 rapidpro_flow_tools-0.9.0/
+-rw-rw-rw-   0        0        0      242 2023-05-24 04:24:59.142449 rapidpro_flow_tools-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2906 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-24 04:24:59.145263 rapidpro_flow_tools-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      379 2023-05-24 04:24:51.000000 rapidpro_flow_tools-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:24:58.992065 rapidpro_flow_tools-0.9.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 04:24:59.010604 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/__init__.py
+-rw-rw-rw-   0        0        0     1322 2023-05-24 03:55:45.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/flow_converter.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:24:59.031434 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:24:59.039470 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/__init__.py
+-rw-rw-rw-   0        0        0     4152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/cellparser.py
+-rw-rw-rw-   0        0        0     3205 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py
+-rw-rw-rw-   0        0        0    15945 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/rowparser.py
+-rw-rw-rw-   0        0        0     1849 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/sheetparser.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:24:59.057719 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/tests/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/tests/mock_cell_parser.py
+-rw-rw-rw-   0        0        0      292 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/tests/mock_row_parser.py
+-rw-rw-rw-   0        0        0      826 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py
+-rw-rw-rw-   0        0        0      600 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/tests/models.py
+-rw-rw-rw-   0        0        0     6080 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py
+-rw-rw-rw-   0        0        0     3508 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py
+-rw-rw-rw-   0        0        0     5026 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py
+-rw-rw-rw-   0        0        0     3050 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py
+-rw-rw-rw-   0        0        0     2022 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py
+-rw-rw-rw-   0        0        0     4684 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:24:59.073307 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/constants.py
+-rw-rw-rw-   0        0        0     7120 2023-05-24 03:59:07.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py
+-rw-rw-rw-   0        0        0      952 2023-05-24 03:59:15.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py
+-rw-rw-rw-   0        0        0      122 2023-05-24 03:59:21.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/datarowmodel.py
+-rw-rw-rw-   0        0        0    26825 2023-05-24 03:59:45.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/flowparser.py
+-rw-rw-rw-   0        0        0     5262 2023-05-24 03:59:53.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py
+-rw-rw-rw-   0        0        0     1076 2023-05-24 04:00:05.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:24:59.088790 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/tests/__init__.py
+-rw-rw-rw-   0        0        0      478 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/tests/mock_sheetreader.py
+-rw-rw-rw-   0        0        0     1030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py
+-rw-rw-rw-   0        0        0    17043 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0    39668 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0    14789 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py
+-rw-rw-rw-   0        0        0      259 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:24:59.102331 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/sheets/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/sheets/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py
+-rw-rw-rw-   0        0        0     3199 2023-05-17 13:33:29.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py
+-rw-rw-rw-   0        0        0      711 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:24:59.106333 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/rapidpro/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/rapidpro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:24:59.119910 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/rapidpro/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/rapidpro/tests/__init__.py
+-rw-rw-rw-   0        0        0      542 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py
+-rw-rw-rw-   0        0        0     3453 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py
+-rw-rw-rw-   0        0        0     4525 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py
+-rw-rw-rw-   0        0        0     1304 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py
+-rw-rw-rw-   0        0        0     6368 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py
+-rw-rw-rw-   0        0        0       73 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/rapidpro/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:24:59.132450 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/tests/__init__.py
+-rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/tests/test_flowparser_reverse.py
+-rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/tests/test_template_sheet_parser.py
+-rw-rw-rw-   0        0        0    11693 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:24:59.029418 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools.egg-info/
+-rw-rw-rw-   0        0        0      242 2023-05-24 04:24:58.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3297 2023-05-24 04:24:58.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 04:24:58.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-24 04:24:58.000000 rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 04:24:59.140446 rapidpro_flow_tools-0.9.0/tests/
+-rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/tests/test_flowparser_reverse.py
+-rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.0/tests/test_template_sheet_parser.py
```

### Comparing `rapidpro_flow_tools-0.8.0/README.md` & `rapidpro_flow_tools-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/flow_converter.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/flow_converter.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/cellparser.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/cellparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/rowparser.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/rowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/sheetparser.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/tests/models.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/tests/models.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import importlib
 from collections import OrderedDict
 from .contentindexrowmodel import ContentIndexRowModel
-from parsers.common.cellparser import CellParser
-from parsers.common.sheetparser import SheetParser
-from parsers.common.rowparser import RowParser
-from rapidpro.models.containers import RapidProContainer
-from parsers.creation.flowparser import FlowParser
+from rapidpro_flow_tools.parsers.common.cellparser import CellParser
+from rapidpro_flow_tools.parsers.common.sheetparser import SheetParser
+from rapidpro_flow_tools.parsers.common.rowparser import RowParser
+from rapidpro_flow_tools.rapidpro.models.containers import RapidProContainer
+from rapidpro_flow_tools.parsers.creation.flowparser import FlowParser
 
 
 class TemplateSheet:
 	def __init__(self, table, argument_definitions):
 		self.table = table
 		self.argument_definitions = argument_definitions
```

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from parsers.common.rowparser import ParserModel
+from rapidpro_flow_tools.parsers.common.rowparser import ParserModel
 from typing import List
 
 class TemplateArgument(ParserModel):
     name: str
     type: str = ''
     default_value: str = ''
```

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/flowparser.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/flowparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import re
 import json
 from collections import defaultdict
 
-from rapidpro.models.actions import SendMessageAction, SetContactFieldAction, AddContactGroupAction, \
+from rapidpro_flow_tools.rapidpro.models.actions import SendMessageAction, SetContactFieldAction, AddContactGroupAction, \
     RemoveContactGroupAction, SetRunResultAction, SetContactPropertyAction, Group
-from rapidpro.models.containers import FlowContainer
-from rapidpro.models.nodes import BaseNode, BasicNode, SwitchRouterNode, RandomRouterNode, EnterFlowNode
-from rapidpro.models.routers import SwitchRouter, RandomRouter
-from parsers.common.cellparser import CellParser
-from parsers.common.sheetparser import SheetParser
-from parsers.common.rowparser import RowParser
-from parsers.creation.flowrowmodel import FlowRowModel
+from rapidpro_flow_tools.rapidpro.models.containers import FlowContainer
+from rapidpro_flow_tools.rapidpro.models.nodes import BaseNode, BasicNode, SwitchRouterNode, RandomRouterNode, EnterFlowNode
+from rapidpro_flow_tools.rapidpro.models.routers import SwitchRouter, RandomRouter
+from rapidpro_flow_tools.parsers.common.cellparser import CellParser
+from rapidpro_flow_tools.parsers.common.sheetparser import SheetParser
+from rapidpro_flow_tools.parsers.common.rowparser import RowParser
+from rapidpro_flow_tools.parsers.creation.flowrowmodel import FlowRowModel
 from .flowrowmodel import Condition
 
 
 class NodeGroup:
     # NodeGroups may have multiple exit nodes.
     # add_exit connects ALL of them, except for those
     # which are marked as hard exits
```

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List
-from parsers.common.rowparser import ParserModel
+from rapidpro_flow_tools.parsers.common.rowparser import ParserModel
 from pydantic import Field
 
 
 class Condition(ParserModel):
     value: str = ''  # Technically, this should be a list as a case may have multiple args
     variable: str = ''
     type: str = ''
```

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/tests/test_contentindexparser.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/tests/test_flowparser.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/tests/test_flowparser_reverse.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/tests/test_flowparser_reverse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/tests/test_template_sheet_parser.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/tests/test_template_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools/tests/utils.py` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools/tests/utils.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/src/rapidpro_flow_tools.egg-info/SOURCES.txt` & `rapidpro_flow_tools-0.9.0/src/rapidpro_flow_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/tests/test_contentindexparser.py` & `rapidpro_flow_tools-0.9.0/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/tests/test_flowparser.py` & `rapidpro_flow_tools-0.9.0/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/tests/test_flowparser_reverse.py` & `rapidpro_flow_tools-0.9.0/tests/test_flowparser_reverse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.8.0/tests/test_template_sheet_parser.py` & `rapidpro_flow_tools-0.9.0/tests/test_template_sheet_parser.py`

 * *Files identical despite different names*

