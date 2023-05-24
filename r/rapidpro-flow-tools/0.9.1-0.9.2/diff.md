# Comparing `tmp/rapidpro_flow_tools-0.9.1.tar.gz` & `tmp/rapidpro_flow_tools-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpro_flow_tools-0.9.1.tar", last modified: Wed May 24 04:27:48 2023, max compression
+gzip compressed data, was "rapidpro_flow_tools-0.9.2.tar", last modified: Wed May 24 04:32:03 2023, max compression
```

## Comparing `rapidpro_flow_tools-0.9.1.tar` & `rapidpro_flow_tools-0.9.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 04:27:48.861796 rapidpro_flow_tools-0.9.1/
--rw-rw-rw-   0        0        0      242 2023-05-24 04:27:48.862800 rapidpro_flow_tools-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     2906 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/README.md
--rw-rw-rw-   0        0        0      115 2023-05-24 04:27:48.864810 rapidpro_flow_tools-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0      379 2023-05-24 04:27:15.000000 rapidpro_flow_tools-0.9.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:27:48.719494 rapidpro_flow_tools-0.9.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 04:27:48.736079 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/__init__.py
--rw-rw-rw-   0        0        0     1322 2023-05-24 03:55:45.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/flow_converter.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:27:48.757624 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:27:48.766406 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/__init__.py
--rw-rw-rw-   0        0        0     4152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/cellparser.py
--rw-rw-rw-   0        0        0     3205 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py
--rw-rw-rw-   0        0        0    15945 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/rowparser.py
--rw-rw-rw-   0        0        0     1849 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/sheetparser.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:27:48.784978 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/tests/__init__.py
--rw-rw-rw-   0        0        0      163 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/tests/mock_cell_parser.py
--rw-rw-rw-   0        0        0      292 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/tests/mock_row_parser.py
--rw-rw-rw-   0        0        0      826 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py
--rw-rw-rw-   0        0        0      600 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/tests/models.py
--rw-rw-rw-   0        0        0     6080 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py
--rw-rw-rw-   0        0        0     3508 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py
--rw-rw-rw-   0        0        0     5026 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py
--rw-rw-rw-   0        0        0     3050 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py
--rw-rw-rw-   0        0        0     2022 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py
--rw-rw-rw-   0        0        0     4684 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:27:48.800164 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/__init__.py
--rw-rw-rw-   0        0        0      152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/constants.py
--rw-rw-rw-   0        0        0     7120 2023-05-24 03:59:07.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py
--rw-rw-rw-   0        0        0      952 2023-05-24 03:59:15.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py
--rw-rw-rw-   0        0        0      122 2023-05-24 03:59:21.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/datarowmodel.py
--rw-rw-rw-   0        0        0    26825 2023-05-24 03:59:45.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/flowparser.py
--rw-rw-rw-   0        0        0     5262 2023-05-24 03:59:53.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py
--rw-rw-rw-   0        0        0     1076 2023-05-24 04:00:05.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:27:48.812206 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/tests/__init__.py
--rw-rw-rw-   0        0        0      478 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/tests/mock_sheetreader.py
--rw-rw-rw-   0        0        0     1030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py
--rw-rw-rw-   0        0        0    17043 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0    39668 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py
--rw-rw-rw-   0        0        0    14789 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py
--rw-rw-rw-   0        0        0      259 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/tests/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:27:48.819733 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/sheets/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/sheets/__init__.py
--rw-rw-rw-   0        0        0      626 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py
--rw-rw-rw-   0        0        0     3199 2023-05-17 13:33:29.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py
--rw-rw-rw-   0        0        0      711 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:27:48.822729 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:27:48.832443 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/models/
--rw-rw-rw-   0        0        0        0 2023-05-24 04:27:06.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/models/__init__.py
--rw-rw-rw-   0        0        0    11728 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/models/actions.py
--rw-rw-rw-   0        0        0     1004 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/models/common.py
--rw-rw-rw-   0        0        0    10931 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/models/containers.py
--rw-rw-rw-   0        0        0    20809 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/models/nodes.py
--rw-rw-rw-   0        0        0    18753 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/models/routers.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:27:48.843420 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/tests/__init__.py
--rw-rw-rw-   0        0        0      542 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py
--rw-rw-rw-   0        0        0     3453 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py
--rw-rw-rw-   0        0        0     4525 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py
--rw-rw-rw-   0        0        0     1304 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py
--rw-rw-rw-   0        0        0     6368 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py
--rw-rw-rw-   0        0        0       73 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:27:48.854133 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/tests/__init__.py
--rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/tests/test_flowparser.py
--rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/tests/test_flowparser_reverse.py
--rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/tests/test_template_sheet_parser.py
--rw-rw-rw-   0        0        0    11693 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/tests/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:27:48.756625 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools.egg-info/
--rw-rw-rw-   0        0        0      242 2023-05-24 04:27:48.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3604 2023-05-24 04:27:48.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 04:27:48.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-24 04:27:48.000000 rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 04:27:48.860131 rapidpro_flow_tools-0.9.1/tests/
--rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/tests/test_flowparser.py
--rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/tests/test_flowparser_reverse.py
--rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.1/tests/test_template_sheet_parser.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.492570 rapidpro_flow_tools-0.9.2/
+-rw-rw-rw-   0        0        0      242 2023-05-24 04:32:03.492570 rapidpro_flow_tools-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2906 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-24 04:32:03.493085 rapidpro_flow_tools-0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0      379 2023-05-24 04:31:54.000000 rapidpro_flow_tools-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.355843 rapidpro_flow_tools-0.9.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.374428 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/__init__.py
+-rw-rw-rw-   0        0        0     1322 2023-05-24 03:55:45.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/flow_converter.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.393027 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.400582 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/__init__.py
+-rw-rw-rw-   0        0        0     4152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/cellparser.py
+-rw-rw-rw-   0        0        0     3205 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py
+-rw-rw-rw-   0        0        0    15945 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/rowparser.py
+-rw-rw-rw-   0        0        0     1849 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/sheetparser.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.422117 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/mock_cell_parser.py
+-rw-rw-rw-   0        0        0      292 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/mock_row_parser.py
+-rw-rw-rw-   0        0        0      826 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py
+-rw-rw-rw-   0        0        0      600 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/models.py
+-rw-rw-rw-   0        0        0     6080 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py
+-rw-rw-rw-   0        0        0     3508 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py
+-rw-rw-rw-   0        0        0     5026 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py
+-rw-rw-rw-   0        0        0     3050 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py
+-rw-rw-rw-   0        0        0     2022 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py
+-rw-rw-rw-   0        0        0     4684 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.434665 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/constants.py
+-rw-rw-rw-   0        0        0     7120 2023-05-24 03:59:07.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py
+-rw-rw-rw-   0        0        0      952 2023-05-24 03:59:15.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py
+-rw-rw-rw-   0        0        0      122 2023-05-24 03:59:21.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/datarowmodel.py
+-rw-rw-rw-   0        0        0    26825 2023-05-24 03:59:45.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/flowparser.py
+-rw-rw-rw-   0        0        0     5262 2023-05-24 03:59:53.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py
+-rw-rw-rw-   0        0        0     1076 2023-05-24 04:00:05.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.444666 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/__init__.py
+-rw-rw-rw-   0        0        0      478 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/mock_sheetreader.py
+-rw-rw-rw-   0        0        0     1030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py
+-rw-rw-rw-   0        0        0    17043 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0    39668 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0    14789 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py
+-rw-rw-rw-   0        0        0      259 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.451828 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/sheets/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/sheets/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py
+-rw-rw-rw-   0        0        0     3199 2023-05-17 13:33:29.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py
+-rw-rw-rw-   0        0        0      711 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.454825 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.464367 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/
+-rw-rw-rw-   0        0        0        0 2023-05-24 04:27:06.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/__init__.py
+-rw-rw-rw-   0        0        0    11748 2023-05-24 04:30:12.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/actions.py
+-rw-rw-rw-   0        0        0     1024 2023-05-24 04:30:28.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/common.py
+-rw-rw-rw-   0        0        0    11011 2023-05-24 04:30:44.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/containers.py
+-rw-rw-rw-   0        0        0    20909 2023-05-24 04:31:04.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/nodes.py
+-rw-rw-rw-   0        0        0    18813 2023-05-24 04:31:44.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/routers.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.474367 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/__init__.py
+-rw-rw-rw-   0        0        0      542 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py
+-rw-rw-rw-   0        0        0     3453 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py
+-rw-rw-rw-   0        0        0     4525 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py
+-rw-rw-rw-   0        0        0     1304 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py
+-rw-rw-rw-   0        0        0     6368 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py
+-rw-rw-rw-   0        0        0       73 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.484916 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/__init__.py
+-rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/test_flowparser_reverse.py
+-rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/test_template_sheet_parser.py
+-rw-rw-rw-   0        0        0    11693 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.391029 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools.egg-info/
+-rw-rw-rw-   0        0        0      242 2023-05-24 04:32:03.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3604 2023-05-24 04:32:03.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 04:32:03.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-24 04:32:03.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.490908 rapidpro_flow_tools-0.9.2/tests/
+-rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/tests/test_flowparser_reverse.py
+-rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/tests/test_template_sheet_parser.py
```

### Comparing `rapidpro_flow_tools-0.9.1/README.md` & `rapidpro_flow_tools-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/flow_converter.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/flow_converter.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/cellparser.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/cellparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/rowparser.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/rowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/sheetparser.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/tests/models.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/models.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/flowparser.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/models/actions.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from rapidpro.utils import generate_new_uuid
+from rapidpro_flow_tools.rapidpro.utils import generate_new_uuid
 
 import copy
 import re
 
 # TODO: Check enter flow
 # Node classification:
 # - Action-only node (for various actions)
```

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/models/common.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from rapidpro.utils import generate_new_uuid
+from rapidpro_flow_tools.rapidpro.utils import generate_new_uuid
 
 
 class Exit:
     def __init__(self, destination_uuid=None, uuid=None):
         self.uuid = uuid if uuid else generate_new_uuid()
         self.destination_uuid = destination_uuid
```

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/models/containers.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/containers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from rapidpro.utils import generate_new_uuid
-from rapidpro.models.nodes import BaseNode
-from rapidpro.models.actions import Group
-from parsers.creation.flowrowmodel import FlowRowModel, Edge
+from rapidpro_flow_tools.rapidpro.utils import generate_new_uuid
+from rapidpro_flow_tools.rapidpro.models.nodes import BaseNode
+from rapidpro_flow_tools.rapidpro.models.actions import Group
+from rapidpro_flow_tools.parsers.creation.flowrowmodel import FlowRowModel, Edge
 import copy
 
 
 class RapidProContainer:
     def __init__(self, campaigns=None, fields=None, flows=None, groups=None, site=None, triggers=None, version='13'):
         self.campaigns = campaigns or []
         self.fields = fields or []
```

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/models/nodes.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from abc import ABC, abstractmethod
 
-from parsers.creation.flowrowmodel import FlowRowModel, Edge
-from rapidpro.models.actions import Action, EnterFlowAction
-from rapidpro.models.common import Exit
-from rapidpro.models.routers import SwitchRouter, RandomRouter
-from rapidpro.utils import generate_new_uuid
+from rapidpro_flow_tools.parsers.creation.flowrowmodel import FlowRowModel, Edge
+from rapidpro_flow_tools.rapidpro.models.actions import Action, EnterFlowAction
+from rapidpro_flow_tools.rapidpro.models.common import Exit
+from rapidpro_flow_tools.rapidpro.models.routers import SwitchRouter, RandomRouter
+from rapidpro_flow_tools.rapidpro.utils import generate_new_uuid
 
 # TODO: EnterFlowNode and WebhookNode are currently children of BaseNode.
 # Ideal class tree of nodes:
 # BaseNode
 #   BasicNode (allows for actions, only has one exit [no router])
 #   SwitchRouterNode (has router and multiple exits; should support actions for its subclasses.)
 #     EnterFlowNode
```

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/models/routers.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/routers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import string
 
-from rapidpro.models.common import Exit
-from rapidpro.utils import generate_new_uuid
-from parsers.creation.flowrowmodel import Condition, Edge
+from rapidpro_flow_tools.rapidpro.models.common import Exit
+from rapidpro_flow_tools.rapidpro.utils import generate_new_uuid
+from rapidpro_flow_tools.parsers.creation.flowrowmodel import Condition, Edge
 
 logger = logging.getLogger(__name__)
 
 
 class BaseRouter:
     def __init__(self, result_name=None, categories=None):
         self.type = None
```

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/tests/test_contentindexparser.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/tests/test_flowparser.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/tests/test_flowparser_reverse.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/test_flowparser_reverse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/tests/test_template_sheet_parser.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/test_template_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools/tests/utils.py` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/utils.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/src/rapidpro_flow_tools.egg-info/SOURCES.txt` & `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/tests/test_contentindexparser.py` & `rapidpro_flow_tools-0.9.2/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/tests/test_flowparser.py` & `rapidpro_flow_tools-0.9.2/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/tests/test_flowparser_reverse.py` & `rapidpro_flow_tools-0.9.2/tests/test_flowparser_reverse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.1/tests/test_template_sheet_parser.py` & `rapidpro_flow_tools-0.9.2/tests/test_template_sheet_parser.py`

 * *Files identical despite different names*

