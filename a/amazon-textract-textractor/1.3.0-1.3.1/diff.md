# Comparing `tmp/amazon-textract-textractor-1.3.0.tar.gz` & `tmp/amazon-textract-textractor-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-textract-textractor-1.3.0.tar", last modified: Tue Apr 18 22:36:15 2023, max compression
+gzip compressed data, was "amazon-textract-textractor-1.3.1.tar", last modified: Wed May 24 03:35:03 2023, max compression
```

## Comparing `amazon-textract-textractor-1.3.0.tar` & `amazon-textract-textractor-1.3.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:15.532288 amazon-textract-textractor-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-04-18 22:36:15.532288 amazon-textract-textractor-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:15.528288 amazon-textract-textractor-1.3.0/amazon_textract_textractor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-04-18 22:36:15.000000 amazon-textract-textractor-1.3.0/amazon_textract_textractor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-18 22:36:15.000000 amazon-textract-textractor-1.3.0/amazon_textract_textractor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:36:15.000000 amazon-textract-textractor-1.3.0/amazon_textract_textractor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-18 22:36:15.000000 amazon-textract-textractor-1.3.0/amazon_textract_textractor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-18 22:36:15.000000 amazon-textract-textractor-1.3.0/amazon_textract_textractor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 22:36:15.000000 amazon-textract-textractor-1.3.0/amazon_textract_textractor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:15.528288 amazon-textract-textractor-1.3.0/extras/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/extras/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/extras/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/extras/pandas.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/extras/pdf.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/extras/torch.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-18 22:36:15.532288 amazon-textract-textractor-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:15.528288 amazon-textract-textractor-1.3.0/textractor/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:15.528288 amazon-textract-textractor-1.3.0/textractor/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15145 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:15.528288 amazon-textract-textractor-1.3.0/textractor/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/data/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:15.532288 amazon-textract-textractor-1.3.0/textractor/entities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    30720 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/document_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/expense_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/expense_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/identity_document.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/identity_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/key_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/lazy_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/line.py
--rw-r--r--   0 runner    (1001) docker     (123)    34524 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/selection_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    23273 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/table_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/table_footer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/table_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/word.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:15.532288 amazon-textract-textractor-1.3.0/textractor/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35059 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/parsers/response_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    37612 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/textractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:15.532288 amazon-textract-textractor-1.3.0/textractor/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/utils/geometry_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/utils/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/utils/search_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:15.532288 amazon-textract-textractor-1.3.0/textractor/visualizers/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/visualizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   367112 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/visualizers/arial.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    42343 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/visualizers/entitylist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:35:03.900584 amazon-textract-textractor-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-24 03:34:55.000000 amazon-textract-textractor-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-24 03:34:55.000000 amazon-textract-textractor-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 03:34:55.000000 amazon-textract-textractor-1.3.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-05-24 03:35:03.900584 amazon-textract-textractor-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-05-24 03:34:55.000000 amazon-textract-textractor-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:35:03.892584 amazon-textract-textractor-1.3.1/amazon_textract_textractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-05-24 03:35:03.000000 amazon-textract-textractor-1.3.1/amazon_textract_textractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-24 03:35:03.000000 amazon-textract-textractor-1.3.1/amazon_textract_textractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 03:35:03.000000 amazon-textract-textractor-1.3.1/amazon_textract_textractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-24 03:35:03.000000 amazon-textract-textractor-1.3.1/amazon_textract_textractor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-24 03:35:03.000000 amazon-textract-textractor-1.3.1/amazon_textract_textractor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-24 03:35:03.000000 amazon-textract-textractor-1.3.1/amazon_textract_textractor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:35:03.892584 amazon-textract-textractor-1.3.1/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/extras/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/extras/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/extras/pandas.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/extras/pdf.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/extras/torch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-24 03:35:03.900584 amazon-textract-textractor-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:35:03.896584 amazon-textract-textractor-1.3.1/textractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:35:03.896584 amazon-textract-textractor-1.3.1/textractor/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15145 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:35:03.896584 amazon-textract-textractor-1.3.1/textractor/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/data/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:35:03.900584 amazon-textract-textractor-1.3.1/textractor/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30720 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/document_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/expense_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/expense_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/identity_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/identity_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/key_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/lazy_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34524 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/selection_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23273 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/table_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/table_footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/table_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/word.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:35:03.900584 amazon-textract-textractor-1.3.1/textractor/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35542 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/parsers/response_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37612 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/textractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:35:03.900584 amazon-textract-textractor-1.3.1/textractor/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/utils/geometry_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/utils/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/utils/search_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:35:03.900584 amazon-textract-textractor-1.3.1/textractor/visualizers/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/visualizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   367112 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/visualizers/arial.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    42343 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/visualizers/entitylist.py
```

### Comparing `amazon-textract-textractor-1.3.0/LICENSE` & `amazon-textract-textractor-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/PKG-INFO` & `amazon-textract-textractor-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-textract-textractor
-Version: 1.3.0
+Version: 1.3.1
 Summary: A package to use AWS Textract services.
 Home-page: https://github.com/aws-samples/amazon-textract-textractor
 License: Apache 2.0
 Keywords: amazon textract aws ocr document
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `amazon-textract-textractor-1.3.0/README.md` & `amazon-textract-textractor-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/amazon_textract_textractor.egg-info/PKG-INFO` & `amazon-textract-textractor-1.3.1/amazon_textract_textractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-textract-textractor
-Version: 1.3.0
+Version: 1.3.1
 Summary: A package to use AWS Textract services.
 Home-page: https://github.com/aws-samples/amazon-textract-textractor
 License: Apache 2.0
 Keywords: amazon textract aws ocr document
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `amazon-textract-textractor-1.3.0/amazon_textract_textractor.egg-info/SOURCES.txt` & `amazon-textract-textractor-1.3.1/amazon_textract_textractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/amazon_textract_textractor.egg-info/requires.txt` & `amazon-textract-textractor-1.3.1/amazon_textract_textractor.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/setup.py` & `amazon-textract-textractor-1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         requirements = [line for line in f.readlines()]
     return requirements
 
 
 setup(
     # include data files
     name="amazon-textract-textractor",
-    version="1.3.0",
+    version="1.3.1",
     license="Apache 2.0",
     description="A package to use AWS Textract services.",
     url="https://github.com/aws-samples/amazon-textract-textractor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `amazon-textract-textractor-1.3.0/textractor/cli/cli.py` & `amazon-textract-textractor-1.3.1/textractor/cli/cli.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/data/constants.py` & `amazon-textract-textractor-1.3.1/textractor/data/constants.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/entities/bbox.py` & `amazon-textract-textractor-1.3.1/textractor/entities/bbox.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/entities/document.py` & `amazon-textract-textractor-1.3.1/textractor/entities/document.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/entities/document_entity.py` & `amazon-textract-textractor-1.3.1/textractor/entities/document_entity.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/entities/expense_document.py` & `amazon-textract-textractor-1.3.1/textractor/entities/expense_document.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/entities/expense_field.py` & `amazon-textract-textractor-1.3.1/textractor/entities/expense_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,26 +57,31 @@
 
 class ExpenseField(DocumentEntity):
     """
     The ExpenseField holds the information a given summary field, key, value and type.
     The bounding box of that ExpenseField is the enclosing one of all its components
     """
     def __init__(self, type: ExpenseType, value: Expense, group_properties: List[ExpenseGroupProperty], page:int, label: Expense = None, currency=None):
-        super(ExpenseField, self).__init__('', BoundingBox.enclosing_bbox([label, value], spatial_object=value.bbox.spatial_object))
+        if label:
+            enclosing_bbox = BoundingBox.enclosing_bbox([label.bbox, value.bbox], spatial_object=label.bbox.spatial_object)
+        else:
+            enclosing_bbox = BoundingBox.enclosing_bbox([label, value], spatial_object=value.bbox.spatial_object)
+        super(ExpenseField, self).__init__('', enclosing_bbox)
+        self._enclosing_bbox = enclosing_bbox
         self._type = type
         self._key = label
         self._value = value
         self._group_properties = group_properties
         self._currency = currency
         self.raw_object = None
         self._page = page
 
     @property
     def bbox(self) -> BoundingBox:
-        return BoundingBox.enclosing_bbox([self.key, self.value], spatial_object=self.value.bbox.spatial_object)
+        return self._enclosing_bbox
 
     @property
     def type(self) -> ExpenseType:
         return self._type
 
     @property
     def key(self) -> Expense:
```

### Comparing `amazon-textract-textractor-1.3.0/textractor/entities/identity_document.py` & `amazon-textract-textractor-1.3.1/textractor/entities/identity_document.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/entities/key_value.py` & `amazon-textract-textractor-1.3.1/textractor/entities/key_value.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/entities/lazy_document.py` & `amazon-textract-textractor-1.3.1/textractor/entities/lazy_document.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/entities/line.py` & `amazon-textract-textractor-1.3.1/textractor/entities/line.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/entities/page.py` & `amazon-textract-textractor-1.3.1/textractor/entities/page.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/entities/query.py` & `amazon-textract-textractor-1.3.1/textractor/entities/query.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/entities/query_result.py` & `amazon-textract-textractor-1.3.1/textractor/entities/query_result.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/entities/selection_element.py` & `amazon-textract-textractor-1.3.1/textractor/entities/selection_element.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/entities/signature.py` & `amazon-textract-textractor-1.3.1/textractor/entities/signature.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/entities/table.py` & `amazon-textract-textractor-1.3.1/textractor/entities/table.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/entities/table_cell.py` & `amazon-textract-textractor-1.3.1/textractor/entities/table_cell.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/entities/table_footer.py` & `amazon-textract-textractor-1.3.1/textractor/entities/table_footer.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/entities/table_title.py` & `amazon-textract-textractor-1.3.1/textractor/entities/table_title.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/entities/value.py` & `amazon-textract-textractor-1.3.1/textractor/entities/value.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/entities/word.py` & `amazon-textract-textractor-1.3.1/textractor/entities/word.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/exceptions.py` & `amazon-textract-textractor-1.3.1/textractor/exceptions.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/parsers/response_parser.py` & `amazon-textract-textractor-1.3.1/textractor/parsers/response_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,15 +413,26 @@
 
     query_results = {}
     for block in page_query_results:
         query_results[block["Id"]] = QueryResult(
             entity_id=block["Id"],
             confidence=block["Confidence"],
             result_bbox=BoundingBox.from_normalized_dict(
-                block["Geometry"]["BoundingBox"], spatial_object=page
+                block.get(
+                    "Geometry",
+                    {
+                        'BoundingBox': {
+                            'Width': 1.0,
+                            'Height': 1.0,
+                            'Left': 0.0,
+                            'Top': 0.0
+                        }
+                    }
+                )["BoundingBox"],
+                spatial_object=page
             ),
             answer=block["Text"],
         )
         query_results[block["Id"]].raw_object = block
 
     for query_result_id, query_result in query_results.items():
         query_result.page = page.page_num
@@ -860,16 +871,21 @@
         type_expense = ExpenseType(
             field["Type"]["Text"], field["Type"]["Confidence"], field["Type"]
         )
     else:
         type_expense = None
     if "ValueDetection" in field:
         value_expense = Expense(
-            bbox=BoundingBox.from_normalized_dict(
-                field["ValueDetection"]["Geometry"]["BoundingBox"], spatial_object=page
+            bbox=(
+                None
+                if not "Geometry" in field["ValueDetection"] else 
+                BoundingBox.from_normalized_dict(
+                    field["ValueDetection"]["Geometry"]["BoundingBox"],
+                    spatial_object=page
+                )
             ),
             text=field["ValueDetection"]["Text"],
             confidence=field["ValueDetection"]["Confidence"],
             page = page.page_num
         )
         value_expense.raw_object = field["ValueDetection"]
     else:
```

### Comparing `amazon-textract-textractor-1.3.0/textractor/textractor.py` & `amazon-textract-textractor-1.3.1/textractor/textractor.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/utils/geometry_util.py` & `amazon-textract-textractor-1.3.1/textractor/utils/geometry_util.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/utils/s3_utils.py` & `amazon-textract-textractor-1.3.1/textractor/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/utils/search_utils.py` & `amazon-textract-textractor-1.3.1/textractor/utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/visualizers/arial.ttf` & `amazon-textract-textractor-1.3.1/textractor/visualizers/arial.ttf`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.0/textractor/visualizers/entitylist.py` & `amazon-textract-textractor-1.3.1/textractor/visualizers/entitylist.py`

 * *Files identical despite different names*

