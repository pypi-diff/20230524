# Comparing `tmp/aind_metadata_service-0.4.2.tar.gz` & `tmp/aind_metadata_service-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_metadata_service-0.4.2.tar", last modified: Thu May  4 23:30:28 2023, max compression
+gzip compressed data, was "aind_metadata_service-0.4.3.tar", last modified: Wed May 24 21:12:00 2023, max compression
```

## Comparing `aind_metadata_service-0.4.2.tar` & `aind_metadata_service-0.4.3.tar`

### file list

```diff
@@ -1,117 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.173261 aind_metadata_service-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.137261 aind_metadata_service-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.145261 aind_metadata_service-0.4.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.149261 aind_metadata_service-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-04 23:30:28.173261 aind_metadata_service-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.149261 aind_metadata_service-0.4.2/doc_template/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.149261 aind_metadata_service-0.4.2/doc_template/source/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/doc_template/source/aind_metadata_service.labtracks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/doc_template/source/aind_metadata_service.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/doc_template/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 23:30:28.173261 aind_metadata_service-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.141261 aind_metadata_service-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.149261 aind_metadata_service-0.4.2/src/aind_metadata_service/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 23:30:12.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.153261 aind_metadata_service-0.4.2/src/aind_metadata_service/labtracks/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/labtracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/labtracks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/labtracks/query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/response_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.153261 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.157261 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2019/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66133 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2019/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    41586 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2019/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2019/procedures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.157261 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2023/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2023/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19552 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2023/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    35167 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2023/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.153261 aind_metadata_service-0.4.2/src/aind_metadata_service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-04 23:30:28.000000 aind_metadata_service-0.4.2/src/aind_metadata_service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-04 23:30:28.000000 aind_metadata_service-0.4.2/src/aind_metadata_service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 23:30:28.000000 aind_metadata_service-0.4.2/src/aind_metadata_service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-04 23:30:28.000000 aind_metadata_service-0.4.2/src/aind_metadata_service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 23:30:28.000000 aind_metadata_service-0.4.2/src/aind_metadata_service.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.157261 aind_metadata_service-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.157261 aind_metadata_service-0.4.2/tests/labtracks/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/labtracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/labtracks/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/labtracks/test_query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/labtracks/test_response_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.141261 aind_metadata_service-0.4.2/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.141261 aind_metadata_service-0.4.2/tests/resources/sharepoint/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.141261 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.161261 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item12.json
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.165261 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item1.json
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item12.json
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item4.json
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item5.json
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item6.json
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item7.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.145261 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.165261 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item13.json
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json
--rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json
--rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.169261 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item10.json
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item11.json
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item13.json
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item14.json
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item15.json
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item16.json
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item17.json
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item8.json
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item9.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.169261 aind_metadata_service-0.4.2/tests/sharepoint/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/sharepoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.169261 aind_metadata_service-0.4.2/tests/sharepoint/nsb2019/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/sharepoint/nsb2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/sharepoint/nsb2019/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/sharepoint/nsb2019/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:30:28.173261 aind_metadata_service-0.4.2/tests/sharepoint/nsb2023/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/sharepoint/nsb2023/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/sharepoint/nsb2023/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/sharepoint/nsb2023/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/sharepoint/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-04 23:30:11.000000 aind_metadata_service-0.4.2/tests/test_response_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.579331 aind_metadata_service-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.567331 aind_metadata_service-0.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.571331 aind_metadata_service-0.4.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.571331 aind_metadata_service-0.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-24 21:12:00.579331 aind_metadata_service-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.571331 aind_metadata_service-0.4.3/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.571331 aind_metadata_service-0.4.3/doc_template/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/doc_template/source/aind_metadata_service.labtracks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/doc_template/source/aind_metadata_service.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/doc_template/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 21:12:00.579331 aind_metadata_service-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.567331 aind_metadata_service-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.571331 aind_metadata_service-0.4.3/src/aind_metadata_service/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 21:11:44.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.571331 aind_metadata_service-0.4.3/src/aind_metadata_service/labtracks/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/labtracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/labtracks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/labtracks/query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.571331 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.571331 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2019/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66133 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2019/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41586 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2019/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2019/procedures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.571331 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2023/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2023/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19552 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2023/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35167 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2023/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.571331 aind_metadata_service-0.4.3/src/aind_metadata_service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-24 21:12:00.000000 aind_metadata_service-0.4.3/src/aind_metadata_service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-24 21:12:00.000000 aind_metadata_service-0.4.3/src/aind_metadata_service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 21:12:00.000000 aind_metadata_service-0.4.3/src/aind_metadata_service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-24 21:12:00.000000 aind_metadata_service-0.4.3/src/aind_metadata_service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 21:12:00.000000 aind_metadata_service-0.4.3/src/aind_metadata_service.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.575331 aind_metadata_service-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.575331 aind_metadata_service-0.4.3/tests/labtracks/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/labtracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/labtracks/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/labtracks/test_query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/labtracks/test_response_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.567331 aind_metadata_service-0.4.3/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.575331 aind_metadata_service-0.4.3/tests/resources/json_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/json_responses/combined.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/json_responses/mapped_las_procedure.json
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/json_responses/mapped_sp_procedure.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.567331 aind_metadata_service-0.4.3/tests/resources/sharepoint/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.567331 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.575331 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item12.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.575331 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item12.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item4.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item5.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item7.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.567331 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.579331 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item13.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.579331 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item11.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item13.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item14.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item15.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item17.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item9.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.579331 aind_metadata_service-0.4.3/tests/sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/sharepoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.579331 aind_metadata_service-0.4.3/tests/sharepoint/nsb2019/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/sharepoint/nsb2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/sharepoint/nsb2019/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/sharepoint/nsb2019/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.579331 aind_metadata_service-0.4.3/tests/sharepoint/nsb2023/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/sharepoint/nsb2023/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/sharepoint/nsb2023/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/sharepoint/nsb2023/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/sharepoint/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/test_response_handle.py
```

### Comparing `aind_metadata_service-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_metadata_service-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_metadata_service-0.4.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/.github/ISSUE_TEMPLATE/user-story.md` & `aind_metadata_service-0.4.3/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/.github/workflows/ci.yml` & `aind_metadata_service-0.4.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/.github/workflows/publish.yml` & `aind_metadata_service-0.4.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/.gitignore` & `aind_metadata_service-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/Dockerfile` & `aind_metadata_service-0.4.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/LICENSE` & `aind_metadata_service-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/PKG-INFO` & `aind_metadata_service-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_metadata_service
-Version: 0.4.2
+Version: 0.4.3
 Summary: REST service to retrive metadata from databases.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_metadata_service-0.4.2/README.md` & `aind_metadata_service-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/doc_template/Makefile` & `aind_metadata_service-0.4.3/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/doc_template/make.bat` & `aind_metadata_service-0.4.3/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/doc_template/source/aind_metadata_service.labtracks.rst` & `aind_metadata_service-0.4.3/doc_template/source/aind_metadata_service.labtracks.rst`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/doc_template/source/conf.py` & `aind_metadata_service-0.4.3/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/pyproject.toml` & `aind_metadata_service-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/src/aind_metadata_service/client.py` & `aind_metadata_service-0.4.3/src/aind_metadata_service/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
     CONNECTION_ERROR = 503
     INTERNAL_SERVER_ERROR = 500
     MULTIPLE_RESPONSES = 300
     VALID_DATA = 200
     INVALID_DATA = 406
     NO_DATA_FOUND = 404
+    MULTI_STATUS = 207
 
 
 class AindMetadataServiceClient:
     """Class to handle client api calls to the service."""
 
     def __init__(self, domain: str):
         """
```

### Comparing `aind_metadata_service-0.4.2/src/aind_metadata_service/labtracks/client.py` & `aind_metadata_service-0.4.3/src/aind_metadata_service/labtracks/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """Module to create clients to connect to databases."""
 from enum import Enum
 from typing import List, Optional
 from xml.etree import ElementTree as ET
 
 import pyodbc
-from aind_data_schema import Subject
+from aind_data_schema import Procedures, Subject
+from aind_data_schema.procedures import (
+    Perfusion,
+    RetroOrbitalInjection,
+    SubjectProcedure,
+)
 from aind_data_schema.subject import BackgroundStrain, Sex, Species
 from fastapi.responses import JSONResponse
 
 from aind_metadata_service.labtracks.query_builder import (
     LabTracksQueries,
     SubjectQueryColumns,
+    TaskSetQueryColumns,
 )
 from aind_metadata_service.response_handler import Responses
 
 
 class LabTracksClient:
     """This class contains the api to connect to LabTracks db."""
 
@@ -103,14 +109,46 @@
                 else:
                     subject = subjects[0]
                     response = Responses.model_response(subject)
                     return response
         except pyodbc.Error:
             return Responses.internal_server_error_response()
 
+    def get_procedures_info(self, subject_id: str) -> JSONResponse:
+        """
+        Method to retrieve LAS procedures from subject_id (int)
+        Parameters
+        ----------
+        subject_id: str
+        """
+        try:
+            query = LabTracksQueries.procedures_from_subject_id(subject_id)
+            session = self.create_session()
+            cursor = session.cursor()
+            cursor.execute(query)
+            column_names = cursor.description
+            columns = [column[0].lower() for column in column_names]
+            fetched_rows = cursor.fetchall()
+            cursor.close()
+            self.close_session(session)
+            results = []
+            for row in fetched_rows:
+                results.append(dict(zip(columns, row)))
+            if not results:
+                response = Responses.no_data_found_response()
+            else:
+                lth = LabTracksResponseHandler()
+                subject_procedures = lth.map_response_to_procedures(results)
+                procedures = Procedures.construct(subject_id=subject_id)
+                procedures.subject_procedures = subject_procedures
+                response = Responses.model_response(procedures)
+            return response
+        except pyodbc.Error:
+            return Responses.internal_server_error_response()
+
 
 class MouseCustomClassFields(Enum):
     """
     LabTracks stores an XML string in the class_values field. We can extract
     the full genotype of the mouse from that field.
     """
 
@@ -138,14 +176,21 @@
     """How LabTracks labels its strains"""
 
     # TODO: Double check this
     C57BL_6J = "C57BL/6J"
     BALB_C = "BALB/c"
 
 
+class LabTracksProcedures(Enum):
+    """Keywords for LabTracks procedures"""
+
+    PERFUSION = "Perfusion"
+    RO_INJECTION = "RO Injection"
+
+
 class LabTracksResponseHandler:
     """This class will contain methods to handle the response from LabTracks"""
 
     @staticmethod
     def _map_class_values_to_genotype(
         class_values: Optional[str],
     ) -> Optional[str]:
@@ -300,7 +345,64 @@
                 date_of_birth=date_of_birth,
                 genotype=full_genotype,
                 breeding_group=breeding_group,
                 background_strain=background_strain,
             )
             subjects.append(subject)
         return subjects
+
+    @staticmethod
+    def map_response_to_procedures(
+        results: List[dict],
+    ) -> List[SubjectProcedure]:
+        """
+        Maps a response from LabTracks to an aind_data_schema.Procedure
+        Parameters
+        ----------
+        results : List[dict]
+            Results pulled from LabTracks. In the form of [row]
+
+        Returns
+        -------
+            A List of mapped Subjects (not validated)
+        """
+
+        procedures_list = []
+
+        for result in results:
+            start_date = result.get(TaskSetQueryColumns.DATE_START.value)
+            if start_date:
+                start_date = start_date.date()
+            end_date = result.get(TaskSetQueryColumns.DATE_END.value)
+            if end_date:
+                end_date = end_date.date()
+            experimenter_full_name = result.get(
+                TaskSetQueryColumns.INVESTIGATOR_ID.value
+            )
+            iacuc_protocol = result.get(
+                TaskSetQueryColumns.PROTOCOL_NUMBER.value
+            )
+            type_name = result.get(TaskSetQueryColumns.TYPE_NAME.value)
+            if type_name:
+                if LabTracksProcedures.PERFUSION.value in type_name:
+                    output_specimen_ids = [
+                        result.get(TaskSetQueryColumns.TASK_OBJECT.value)
+                    ]
+                    perfusion = Perfusion.construct(
+                        start_date=start_date,
+                        end_date=end_date,
+                        experimenter_full_name=experimenter_full_name,
+                        iacuc_protocol=iacuc_protocol,
+                        output_specimen_ids=output_specimen_ids,
+                    )
+                    procedures_list.append(perfusion)
+
+                elif LabTracksProcedures.RO_INJECTION.value in type_name:
+                    # TODO: parse inj info from comments
+                    ro_injection = RetroOrbitalInjection.construct(
+                        start_date=start_date,
+                        end_date=end_date,
+                        experimenter_full_name=experimenter_full_name,
+                        iacuc_protocol=iacuc_protocol,
+                    )
+                    procedures_list.append(ro_injection)
+        return procedures_list
```

### Comparing `aind_metadata_service-0.4.2/src/aind_metadata_service/labtracks/query_builder.py` & `aind_metadata_service-0.4.3/src/aind_metadata_service/labtracks/query_builder.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,18 +14,72 @@
     MATERNAL_ID = "maternal_id"
     MATERNAL_CLASS_VALUES = "maternal_class_values"
     SPECIES_NAME = "species_name"
     GROUP_NAME = "group_name"
     GROUP_DESCRIPTION = "group_description"
 
 
+class TaskSetQueryColumns(Enum):
+    """Expected columns in the task set query response."""
+
+    TASK_ID = "id"
+    TASK_TYPE_ID = "task_type_id"
+    DATE_START = "date_start"
+    DATE_END = "date_end"
+    INVESTIGATOR_ID = "investigator_id"
+    TASK_OBJECT = "task_object"
+    TYPE_NAME = "type_name"
+    PROTOCOL_NUMBER = "protocol_number"
+
+
 class LabTracksQueries:
     """Class to hold sql query strings for LabTracks"""
 
     @staticmethod
+    def procedures_from_subject_id(subject_id: str) -> str:
+        """
+        Retrieves the information to populate metadata about subjects.
+
+        Parameters
+        ----------
+        subject_id : str
+            This is the id in the LabTracks Task_Set table
+
+        Returns
+        -------
+        str
+            SQL query that can be used to retrieve the data from LabTracks
+            sqlserver db.
+        """
+        # TODO: parsers for comments/descriptions?
+        return (
+            "SELECT"
+            f"    TS.ID AS {TaskSetQueryColumns.TASK_ID.value},"
+            f"    TS.TASK_TYPE_ID AS {TaskSetQueryColumns.TASK_TYPE_ID.value},"
+            f"    TT.TYPE_NAME AS {TaskSetQueryColumns.TYPE_NAME.value},"
+            f"    TS.DATE_START AS {TaskSetQueryColumns.DATE_START.value},"
+            f"    TS.DATE_END AS {TaskSetQueryColumns.DATE_END.value},"
+            f"    TS.INVESTIGATOR_ID AS "
+            f"    {TaskSetQueryColumns.INVESTIGATOR_ID.value},"
+            f"    TSO.TASK_OBJECT AS {TaskSetQueryColumns.TASK_OBJECT.value},"
+            f"    AP.PROTOCOL_NUMBER AS "
+            f"    {TaskSetQueryColumns.PROTOCOL_NUMBER.value}"
+            "  FROM TASK_SET TS"
+            "    INNER JOIN TASK_SET_OBJECT TSO "
+            "    ON TS.ID = TSO.TASK_ID"
+            "    INNER JOIN ANIMALS_COMMON AC "
+            "    ON TSO.TASK_OBJECT = AC.ID"
+            "    INNER JOIN TASK_TYPE TT "
+            "    ON TS.TASK_TYPE_ID = TT.ID"
+            "    INNER JOIN ACUC_PROTOCOL AP "
+            "    ON TS.ACUC_LINK_ID = AP.LINK_INDEX"
+            f" WHERE AC.ID={subject_id};"
+        )
+
+    @staticmethod
     def subject_from_subject_id(subject_id: str) -> str:
         """
         Retrieves the information to populate metadata about subjects.
 
         Parameters
         ----------
         subject_id : str
```

### Comparing `aind_metadata_service-0.4.2/src/aind_metadata_service/server.py` & `aind_metadata_service-0.4.3/src/aind_metadata_service/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import RedirectResponse
 
 from aind_metadata_service.labtracks.client import LabTracksClient
+from aind_metadata_service.response_handler import Responses
 from aind_metadata_service.sharepoint.client import SharePointClient
 
 app = FastAPI()
 
 app.add_middleware(
     CORSMiddleware,
     allow_origins=["*"],
@@ -62,17 +63,25 @@
     sharepoint_client = SharePointClient(
         nsb_site_url=nsb_sharepoint_url,
         nsb_list_title_2019=nsb_sharepoint_list_2019,
         nsb_list_title_2023=nsb_sharepoint_list_2023,
         client_id=nsb_sharepoint_user,
         client_secret=nsb_sharepoint_password,
     )
-
-    response = sharepoint_client.get_procedure_info(subject_id=subject_id)
-
+    lb_client = LabTracksClient(
+        driver=labtracks_driver,
+        server=labtracks_server,
+        port=labtracks_port,
+        db=labtracks_db,
+        user=labtracks_user,
+        password=labtracks_password,
+    )
+    lb_response = lb_client.get_procedures_info(subject_id=subject_id)
+    sp_response = sharepoint_client.get_procedure_info(subject_id=subject_id)
+    response = Responses.combine_procedure_responses(lb_response, sp_response)
     return response
 
 
 @app.get(
     "/favicon.ico",
     include_in_schema=False,
     response_class=RedirectResponse,
```

### Comparing `aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/client.py` & `aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2019/mapping.py` & `aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2019/mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2019/models.py` & `aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2019/models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2019/procedures.py` & `aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2019/procedures.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2023/mapping.py` & `aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2023/mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/src/aind_metadata_service/sharepoint/nsb2023/models.py` & `aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2023/models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/src/aind_metadata_service.egg-info/PKG-INFO` & `aind_metadata_service-0.4.3/src/aind_metadata_service.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-service
-Version: 0.4.2
+Version: 0.4.3
 Summary: REST service to retrive metadata from databases.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_metadata_service-0.4.2/src/aind_metadata_service.egg-info/SOURCES.txt` & `aind_metadata_service-0.4.3/src/aind_metadata_service.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 tests/__init__.py
 tests/test_client.py
 tests/test_response_handle.py
 tests/labtracks/__init__.py
 tests/labtracks/test_client.py
 tests/labtracks/test_query_builder.py
 tests/labtracks/test_response_handler.py
+tests/resources/json_responses/combined.json
+tests/resources/json_responses/mapped_las_procedure.json
+tests/resources/json_responses/mapped_sp_procedure.json
 tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json
 tests/resources/sharepoint/nsb2019/mapped/mapped_list_item12.json
 tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json
 tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json
 tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json
 tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json
 tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json
```

### Comparing `aind_metadata_service-0.4.2/tests/labtracks/test_client.py` & `aind_metadata_service-0.4.3/tests/labtracks/test_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -67,18 +67,21 @@
         def mock_cursor(_):
             """Mock the pyodbc.cursor() function."""
             raise pyodbc.ProgrammingError
 
         type(mock_connect.return_value).cursor = mock_cursor
 
         response1 = self.lb_client.get_subject_info("123")
+        response2 = self.lb_client.get_procedures_info("123")
         expected_response = Responses.internal_server_error_response()
         mock_connect.assert_called()
         self.assertEqual(response1.status_code, expected_response.status_code)
         self.assertEqual(response1.body, expected_response.body)
+        self.assertEqual(response2.status_code, expected_response.status_code)
+        self.assertEqual(response2.body, expected_response.body)
 
     @patch("pyodbc.connect")
     def test_id_does_not_exist(self, _) -> None:
         """
         Tests that JSONResponse error is returned to client properly
         when queried subject_id does not exist.
         Parameters
@@ -89,26 +92,31 @@
 
         Returns
         -------
             pass
         """
         subject_id = "00000"
 
-        actual_response = self.lb_client.get_subject_info(subject_id)
+        subject_response = self.lb_client.get_subject_info(subject_id)
+        procedure_response = self.lb_client.get_procedures_info(subject_id)
         expected_response = Responses.no_data_found_response()
         self.assertEqual(
-            expected_response.status_code, actual_response.status_code
+            expected_response.status_code, subject_response.status_code
         )
-        self.assertEqual(expected_response.body, actual_response.body)
+        self.assertEqual(expected_response.body, subject_response.body)
+        self.assertEqual(
+            expected_response.status_code, procedure_response.status_code
+        )
+        self.assertEqual(expected_response.body, procedure_response.body)
 
     @patch("pyodbc.connect")
-    def test_id_does_exist(self, mock_connect: Mock) -> None:
+    def test_get_subject_info_success(self, mock_connect: Mock) -> None:
         """
-        Tests that JSONResponse error is returned to client properly
-        when queried subject_id does not exist.
+        Tests that JSONResponse is returned to client properly
+        when queried subject_id does exist.
         Parameters
         ----------
         mock_connect : Mock
             A mocked Connection class that can be used to override methods
             without connecting to sqlserver
 
         Returns
@@ -177,15 +185,15 @@
         )
         self.assertEqual(expected_response.body, actual_response.body)
 
     @patch("pyodbc.connect")
     def test_multiple_ids_exist(self, mock_connect: Mock) -> None:
         """
         Tests that JSONResponse error is returned to client properly
-        when queried subject_id does not exist.
+        when queried subject_id returns multiple items.
         Parameters
         ----------
         mock_connect : Mock
             A mocked Connection class that can be used to override methods
             without connecting to sqlserver
 
         Returns
@@ -266,10 +274,89 @@
             [TestResponseExamples.expected_subject, expected_subject2]
         )
         self.assertEqual(
             expected_response.status_code, actual_response.status_code
         )
         self.assertEqual(expected_response.body, actual_response.body)
 
+    @patch("pyodbc.connect")
+    def test_get_procedure_info_success(self, mock_connect: Mock) -> None:
+        """
+        Tests that JSONResponse is returned to client properly
+        when queried subject_id does exist.
+        Parameters
+        ----------
+        mock_connect : Mock
+            A mocked Connection class that can be used to override methods
+            without connecting to sqlserver
+
+        Returns
+        -------
+            pass
+        """
+
+        class MockCursor:
+            """Mocked cursor object"""
+
+            description = [
+                ["id"],
+                ["task_type_id"],
+                ["date_start"],
+                ["date_end"],
+                ["investigator_id"],
+                ["task_object"],
+                ["type_name"],
+                ["protocol_number"],
+            ]
+
+            @staticmethod
+            def execute(_):
+                """Mock execute"""
+                return None
+
+            @staticmethod
+            def fetchall():
+                """Mock fetchall"""
+                return [
+                    [
+                        decimal.Decimal("00000"),
+                        decimal.Decimal("12345"),
+                        datetime.datetime(2022, 10, 11, 0, 0),
+                        datetime.datetime(2022, 10, 11, 4, 30),
+                        decimal.Decimal("28803"),
+                        decimal.Decimal("115977"),
+                        "Perfusion",
+                        decimal.Decimal("2002"),
+                    ],
+                    [
+                        decimal.Decimal("10000"),
+                        decimal.Decimal("23"),
+                        datetime.datetime(2022, 5, 11, 0, 0),
+                        datetime.datetime(2022, 5, 12, 0, 0),
+                        decimal.Decimal("28803"),
+                        decimal.Decimal("115977"),
+                        "RO Injection",
+                        decimal.Decimal("2002"),
+                    ],
+                ]
+
+            @staticmethod
+            def close():
+                """Mock close"""
+                return None
+
+        subject_id = "115977"
+
+        type(mock_connect.return_value).cursor = MockCursor
+
+        actual_response = self.lb_client.get_procedures_info(subject_id)
+        expected_response = Responses.model_response(
+            TestResponseExamples.expected_procedures
+        )
+        self.assertEqual(
+            expected_response.status_code, actual_response.status_code
+        )
+        self.assertEqual(expected_response.body, actual_response.body)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item1.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item1.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item12.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item12.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item2.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item2.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item3.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item3.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item4.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item4.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item5.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item5.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item6.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item6.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2019/raw/list_item7.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item7.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item10.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item10.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item11.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item11.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item13.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item13.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item14.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item14.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item15.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item15.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item16.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item16.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item17.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item17.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item8.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item8.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/resources/sharepoint/nsb2023/raw/list_item9.json` & `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item9.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/sharepoint/nsb2019/test_mapping.py` & `aind_metadata_service-0.4.3/tests/sharepoint/nsb2019/test_mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/sharepoint/nsb2019/test_models.py` & `aind_metadata_service-0.4.3/tests/sharepoint/nsb2019/test_models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/sharepoint/nsb2023/test_mapping.py` & `aind_metadata_service-0.4.3/tests/sharepoint/nsb2023/test_mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/sharepoint/nsb2023/test_models.py` & `aind_metadata_service-0.4.3/tests/sharepoint/nsb2023/test_models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/sharepoint/test_client.py` & `aind_metadata_service-0.4.3/tests/sharepoint/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.2/tests/test_client.py` & `aind_metadata_service-0.4.3/tests/test_client.py`

 * *Files identical despite different names*

