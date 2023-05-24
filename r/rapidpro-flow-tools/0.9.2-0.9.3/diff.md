# Comparing `tmp/rapidpro_flow_tools-0.9.2.tar.gz` & `tmp/rapidpro_flow_tools-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpro_flow_tools-0.9.2.tar", last modified: Wed May 24 04:32:03 2023, max compression
+gzip compressed data, was "rapidpro_flow_tools-0.9.3.tar", last modified: Wed May 24 15:02:58 2023, max compression
```

## Comparing `rapidpro_flow_tools-0.9.2.tar` & `rapidpro_flow_tools-0.9.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.492570 rapidpro_flow_tools-0.9.2/
--rw-rw-rw-   0        0        0      242 2023-05-24 04:32:03.492570 rapidpro_flow_tools-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     2906 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/README.md
--rw-rw-rw-   0        0        0      115 2023-05-24 04:32:03.493085 rapidpro_flow_tools-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0      379 2023-05-24 04:31:54.000000 rapidpro_flow_tools-0.9.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.355843 rapidpro_flow_tools-0.9.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.374428 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/__init__.py
--rw-rw-rw-   0        0        0     1322 2023-05-24 03:55:45.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/flow_converter.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.393027 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.400582 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/__init__.py
--rw-rw-rw-   0        0        0     4152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/cellparser.py
--rw-rw-rw-   0        0        0     3205 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py
--rw-rw-rw-   0        0        0    15945 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/rowparser.py
--rw-rw-rw-   0        0        0     1849 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/sheetparser.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.422117 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/__init__.py
--rw-rw-rw-   0        0        0      163 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/mock_cell_parser.py
--rw-rw-rw-   0        0        0      292 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/mock_row_parser.py
--rw-rw-rw-   0        0        0      826 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py
--rw-rw-rw-   0        0        0      600 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/models.py
--rw-rw-rw-   0        0        0     6080 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py
--rw-rw-rw-   0        0        0     3508 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py
--rw-rw-rw-   0        0        0     5026 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py
--rw-rw-rw-   0        0        0     3050 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py
--rw-rw-rw-   0        0        0     2022 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py
--rw-rw-rw-   0        0        0     4684 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.434665 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/__init__.py
--rw-rw-rw-   0        0        0      152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/constants.py
--rw-rw-rw-   0        0        0     7120 2023-05-24 03:59:07.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py
--rw-rw-rw-   0        0        0      952 2023-05-24 03:59:15.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py
--rw-rw-rw-   0        0        0      122 2023-05-24 03:59:21.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/datarowmodel.py
--rw-rw-rw-   0        0        0    26825 2023-05-24 03:59:45.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/flowparser.py
--rw-rw-rw-   0        0        0     5262 2023-05-24 03:59:53.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py
--rw-rw-rw-   0        0        0     1076 2023-05-24 04:00:05.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.444666 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/__init__.py
--rw-rw-rw-   0        0        0      478 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/mock_sheetreader.py
--rw-rw-rw-   0        0        0     1030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py
--rw-rw-rw-   0        0        0    17043 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0    39668 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py
--rw-rw-rw-   0        0        0    14789 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py
--rw-rw-rw-   0        0        0      259 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.451828 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/sheets/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/sheets/__init__.py
--rw-rw-rw-   0        0        0      626 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py
--rw-rw-rw-   0        0        0     3199 2023-05-17 13:33:29.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py
--rw-rw-rw-   0        0        0      711 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.454825 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.464367 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/
--rw-rw-rw-   0        0        0        0 2023-05-24 04:27:06.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/__init__.py
--rw-rw-rw-   0        0        0    11748 2023-05-24 04:30:12.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/actions.py
--rw-rw-rw-   0        0        0     1024 2023-05-24 04:30:28.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/common.py
--rw-rw-rw-   0        0        0    11011 2023-05-24 04:30:44.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/containers.py
--rw-rw-rw-   0        0        0    20909 2023-05-24 04:31:04.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/nodes.py
--rw-rw-rw-   0        0        0    18813 2023-05-24 04:31:44.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/routers.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.474367 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/__init__.py
--rw-rw-rw-   0        0        0      542 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py
--rw-rw-rw-   0        0        0     3453 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py
--rw-rw-rw-   0        0        0     4525 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py
--rw-rw-rw-   0        0        0     1304 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py
--rw-rw-rw-   0        0        0     6368 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py
--rw-rw-rw-   0        0        0       73 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.484916 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/__init__.py
--rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/test_flowparser.py
--rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/test_flowparser_reverse.py
--rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/test_template_sheet_parser.py
--rw-rw-rw-   0        0        0    11693 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.391029 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools.egg-info/
--rw-rw-rw-   0        0        0      242 2023-05-24 04:32:03.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3604 2023-05-24 04:32:03.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 04:32:03.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-24 04:32:03.000000 rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 04:32:03.490908 rapidpro_flow_tools-0.9.2/tests/
--rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/tests/test_flowparser.py
--rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/tests/test_flowparser_reverse.py
--rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.2/tests/test_template_sheet_parser.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:02:58.923131 rapidpro_flow_tools-0.9.3/
+-rw-rw-rw-   0        0        0      242 2023-05-24 15:02:58.923131 rapidpro_flow_tools-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2906 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-24 15:02:58.925130 rapidpro_flow_tools-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0      379 2023-05-24 15:02:34.000000 rapidpro_flow_tools-0.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:02:58.395687 rapidpro_flow_tools-0.9.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 15:02:58.469051 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/__init__.py
+-rw-rw-rw-   0        0        0     1344 2023-05-24 15:01:45.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/flow_converter.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:02:58.489123 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:02:58.523447 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/__init__.py
+-rw-rw-rw-   0        0        0     4152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/cellparser.py
+-rw-rw-rw-   0        0        0     3205 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py
+-rw-rw-rw-   0        0        0    15945 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/rowparser.py
+-rw-rw-rw-   0        0        0     1883 2023-05-24 04:48:55.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/sheetparser.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:02:58.611487 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/tests/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/tests/mock_cell_parser.py
+-rw-rw-rw-   0        0        0      292 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/tests/mock_row_parser.py
+-rw-rw-rw-   0        0        0      826 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py
+-rw-rw-rw-   0        0        0      600 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/tests/models.py
+-rw-rw-rw-   0        0        0     6080 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py
+-rw-rw-rw-   0        0        0     3508 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py
+-rw-rw-rw-   0        0        0     5026 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py
+-rw-rw-rw-   0        0        0     3050 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py
+-rw-rw-rw-   0        0        0     2022 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py
+-rw-rw-rw-   0        0        0     4684 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:02:58.668229 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/constants.py
+-rw-rw-rw-   0        0        0     7156 2023-05-24 04:49:46.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py
+-rw-rw-rw-   0        0        0      952 2023-05-24 03:59:15.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py
+-rw-rw-rw-   0        0        0      122 2023-05-24 03:59:21.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/datarowmodel.py
+-rw-rw-rw-   0        0        0    26861 2023-05-24 04:52:23.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/flowparser.py
+-rw-rw-rw-   0        0        0     5262 2023-05-24 03:59:53.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py
+-rw-rw-rw-   0        0        0     1076 2023-05-24 04:00:05.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:02:58.733197 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/tests/__init__.py
+-rw-rw-rw-   0        0        0      478 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/tests/mock_sheetreader.py
+-rw-rw-rw-   0        0        0     1030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py
+-rw-rw-rw-   0        0        0    17043 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0    39668 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0    14789 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py
+-rw-rw-rw-   0        0        0      259 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:02:58.759753 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/sheets/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/sheets/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py
+-rw-rw-rw-   0        0        0     3149 2023-05-24 14:56:12.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py
+-rw-rw-rw-   0        0        0      711 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:02:58.767409 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:02:58.821058 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/models/
+-rw-rw-rw-   0        0        0        0 2023-05-24 04:27:06.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/models/__init__.py
+-rw-rw-rw-   0        0        0    11748 2023-05-24 04:30:12.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/models/actions.py
+-rw-rw-rw-   0        0        0     1024 2023-05-24 04:30:28.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/models/common.py
+-rw-rw-rw-   0        0        0    11011 2023-05-24 04:30:44.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/models/containers.py
+-rw-rw-rw-   0        0        0    20909 2023-05-24 04:31:04.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/models/nodes.py
+-rw-rw-rw-   0        0        0    18813 2023-05-24 04:53:20.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/models/routers.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:02:58.862790 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/tests/__init__.py
+-rw-rw-rw-   0        0        0      542 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py
+-rw-rw-rw-   0        0        0     3453 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py
+-rw-rw-rw-   0        0        0     4525 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py
+-rw-rw-rw-   0        0        0     1304 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py
+-rw-rw-rw-   0        0        0     6368 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py
+-rw-rw-rw-   0        0        0       73 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:02:58.910098 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/tests/__init__.py
+-rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/tests/test_flowparser_reverse.py
+-rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/tests/test_template_sheet_parser.py
+-rw-rw-rw-   0        0        0    11693 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:02:58.487120 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools.egg-info/
+-rw-rw-rw-   0        0        0      242 2023-05-24 15:02:58.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3604 2023-05-24 15:02:58.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 15:02:58.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-24 15:02:58.000000 rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 15:02:58.922129 rapidpro_flow_tools-0.9.3/tests/
+-rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/tests/test_flowparser_reverse.py
+-rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-0.9.3/tests/test_template_sheet_parser.py
```

### Comparing `rapidpro_flow_tools-0.9.2/README.md` & `rapidpro_flow_tools-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/flow_converter.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/flow_converter.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,17 +11,17 @@
         return
 
     if sheet_format == 'csv':
         sheet_reader = CSVSheetReader(input_file)
     elif sheet_format == 'xlsx':
         sheet_reader = XLSXSheetReader(input_file)
     elif sheet_format == 'google_sheets':
-        credentials_path = credentials or 'credentials.json'
-        token_path = token or 'token.json'
-        sheet_reader = GoogleSheetReader(input_file, credentials_path, token_path)
+        credentials_file = credentials or json.load('credentials.json')
+        token_file = token or json.load('token.json')
+        sheet_reader = GoogleSheetReader(input_file, credentials_file, token_file)
     else:
         print(f"Format {sheet_format} currently unsupported.")
         return
 
     ci_parser = ContentIndexParser(sheet_reader, data_models)
     output = ci_parser.parse_all_flows()
     json.dump(output.render(), open(output_file, 'w'), indent=4)
```

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/cellparser.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/cellparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/rowparser.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/rowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/sheetparser.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/sheetparser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import copy
-from .rowdatasheet import RowDataSheet
+from rapidpro_flow_tools.parsers.common.rowdatasheet import RowDataSheet
 
 class SheetParser:
 
     def __init__(self, row_parser, table, context={}):
         '''
         Args:
             row_parser: parser to convert flat dicts to RowModel instances.
```

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/models.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/tests/models.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import importlib
 from collections import OrderedDict
-from .contentindexrowmodel import ContentIndexRowModel
+from rapidpro_flow_tools.parsers.creation.contentindexrowmodel import ContentIndexRowModel
 from rapidpro_flow_tools.parsers.common.cellparser import CellParser
 from rapidpro_flow_tools.parsers.common.sheetparser import SheetParser
 from rapidpro_flow_tools.parsers.common.rowparser import RowParser
 from rapidpro_flow_tools.rapidpro.models.containers import RapidProContainer
 from rapidpro_flow_tools.parsers.creation.flowparser import FlowParser
```

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/flowparser.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/flowparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from rapidpro_flow_tools.rapidpro.models.containers import FlowContainer
 from rapidpro_flow_tools.rapidpro.models.nodes import BaseNode, BasicNode, SwitchRouterNode, RandomRouterNode, EnterFlowNode
 from rapidpro_flow_tools.rapidpro.models.routers import SwitchRouter, RandomRouter
 from rapidpro_flow_tools.parsers.common.cellparser import CellParser
 from rapidpro_flow_tools.parsers.common.sheetparser import SheetParser
 from rapidpro_flow_tools.parsers.common.rowparser import RowParser
 from rapidpro_flow_tools.parsers.creation.flowrowmodel import FlowRowModel
-from .flowrowmodel import Condition
+from rapidpro_flow_tools.parsers.creation.flowrowmodel import Condition
 
 
 class NodeGroup:
     # NodeGroups may have multiple exit nodes.
     # add_exit connects ALL of them, except for those
     # which are marked as hard exits
     # (which are not tracked as loose_exits)
```

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,40 +3,39 @@
 from google_auth_oauthlib.flow import InstalledAppFlow
 from google.auth.transport.requests import Request
 from google.oauth2.credentials import Credentials
 import os
 
 
 class GoogleSheetReader:
-
-    # If modifying these scopes, delete the file token.json.
     SCOPES = ['https://www.googleapis.com/auth/spreadsheets.readonly']
 
-    def __init__(self, spreadsheet_id, credentials_path='credentials.json', token_path='token.json'):
+    def __init__(self, spreadsheet_id, credentials_file=None, token_file=None):
         '''
         Args:
             spreadsheet_id: You can extract it from the spreadsheet URL, like this:
                             https://docs.google.com/spreadsheets/d/[spreadsheet_id]/edit
-            credentials_path: Path to the 'credentials.json' file (default: 'credentials.json')
-            token_path: Path to the 'token.json' file (default: 'token.json')
+            credentials_file: File object of the 'credentials.json' file (default: None)
+            token_file: File object of the 'token.json' file (default: None)
         '''
         creds = None
 
-        if os.path.exists(token_path):
-            creds = Credentials.from_authorized_user_file(token_path, GoogleSheetReader.SCOPES)
+        if token_file is not None:
+            creds = Credentials.from_authorized_user_file(token_file, GoogleSheetReader.SCOPES)
 
         if not creds or not creds.valid:
             if creds and creds.expired and creds.refresh_token:
                 creds.refresh(Request())
             else:
-                flow = InstalledAppFlow.from_client_secrets_file(credentials_path, GoogleSheetReader.SCOPES)
+                flow = InstalledAppFlow.from_client_secrets_file(credentials_file, GoogleSheetReader.SCOPES)
                 creds = flow.run_local_server(port=0)
 
-            with open(token_path, 'w') as token:
-                token.write(creds.to_json())
+            if token_file is not None:
+                with open(token_file, 'w') as token:
+                    token.write(creds.to_json())
 
         service = build('sheets', 'v4', credentials=creds)
 
         # Call the Sheets API
         sheet_metadata = service.spreadsheets().get(spreadsheetId=spreadsheet_id).execute()
         sheets = sheet_metadata.get('sheets', '')
         titles = []
```

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/actions.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/models/actions.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/common.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/models/common.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/containers.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/models/containers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/nodes.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/models/nodes.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/models/routers.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/models/routers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/test_contentindexparser.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/test_flowparser.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/test_flowparser_reverse.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/tests/test_flowparser_reverse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/test_template_sheet_parser.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/tests/test_template_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools/tests/utils.py` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools/tests/utils.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/src/rapidpro_flow_tools.egg-info/SOURCES.txt` & `rapidpro_flow_tools-0.9.3/src/rapidpro_flow_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/tests/test_contentindexparser.py` & `rapidpro_flow_tools-0.9.3/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/tests/test_flowparser.py` & `rapidpro_flow_tools-0.9.3/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/tests/test_flowparser_reverse.py` & `rapidpro_flow_tools-0.9.3/tests/test_flowparser_reverse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.9.2/tests/test_template_sheet_parser.py` & `rapidpro_flow_tools-0.9.3/tests/test_template_sheet_parser.py`

 * *Files identical despite different names*

