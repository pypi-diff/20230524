# Comparing `tmp/appian-locust-2.0.0a4.tar.gz` & `tmp/appian-locust-2.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appian-locust-2.0.0a4.tar", last modified: Thu May 18 15:48:06 2023, max compression
+gzip compressed data, was "appian-locust-2.0.0a5.tar", last modified: Wed May 24 15:50:10 2023, max compression
```

## Comparing `appian-locust-2.0.0a4.tar` & `appian-locust-2.0.0a5.tar`

### file list

```diff
@@ -1,86 +1,88 @@
-drwxr-xr-x   0 harry.wilton   (502) staff       (20)        0 2023-05-18 15:48:06.031774 appian-locust-2.0.0a4/
--rw-r--r--   0 harry.wilton   (502) staff       (20)    11358 2022-02-17 16:44:14.000000 appian-locust-2.0.0a4/LICENSE
--rw-r--r--   0 harry.wilton   (502) staff       (20)     5403 2023-05-18 15:48:06.031988 appian-locust-2.0.0a4/PKG-INFO
--rw-r--r--   0 harry.wilton   (502) staff       (20)     4829 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/README.rst
-drwxr-xr-x   0 harry.wilton   (502) staff       (20)        0 2023-05-18 15:48:06.012314 appian-locust-2.0.0a4/appian_locust/
--rw-r--r--   0 harry.wilton   (502) staff       (20)      775 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/__init__.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     9541 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/_actions.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)      786 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/_admin.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2479 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/_base.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     5721 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/_design.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     6206 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/_feature_toggle_helper.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     7830 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/_grid_interactor.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    53252 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/_interactor.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     5171 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/_locust_error_handler.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     7765 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/_news.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1025 2023-05-15 14:44:16.000000 appian-locust-2.0.0a4/appian_locust/_portals.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    16297 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/_records.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     7380 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/_records_helper.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     7185 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/_reports.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     3016 2023-04-27 17:42:07.000000 appian-locust-2.0.0a4/appian_locust/_save_request_builder.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    10071 2023-05-18 15:35:31.000000 appian-locust-2.0.0a4/appian_locust/_sites.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     4514 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/_task_opener.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     7644 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/_tasks.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2365 2022-02-17 16:44:14.000000 appian-locust-2.0.0a4/appian_locust/_ui_reconciler.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1372 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/actions_info.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    14485 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/appianclient.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1981 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/application_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)      205 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/design_object_type.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1068 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/design_object_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     4998 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/design_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)      859 2022-02-17 16:44:14.000000 appian-locust-2.0.0a4/appian_locust/exceptions.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1792 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/feature_flag.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    16278 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/helper.py
--rwxr-xr-x   0 harry.wilton   (502) staff       (20)     1431 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/loadDriverUtils.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)      862 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/logger.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2749 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/news_info.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1941 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/record_list_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1320 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/record_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)      547 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/records_info.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1546 2023-05-17 15:35:49.000000 appian-locust-2.0.0a4/appian_locust/reports_info.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1364 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/site_helper.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)      826 2023-05-18 15:42:44.000000 appian-locust-2.0.0a4/appian_locust/site_objects.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1261 2023-05-18 15:36:39.000000 appian-locust-2.0.0a4/appian_locust/sites_info.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1406 2023-05-18 15:36:46.000000 appian-locust-2.0.0a4/appian_locust/tasks_info.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2504 2023-05-18 15:27:19.000000 appian-locust-2.0.0a4/appian_locust/tempo_navigator.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    73573 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/appian_locust/uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    13955 2023-05-15 14:44:16.000000 appian-locust-2.0.0a4/appian_locust/visitor.py
-drwxr-xr-x   0 harry.wilton   (502) staff       (20)        0 2023-05-18 15:48:06.014778 appian-locust-2.0.0a4/appian_locust.egg-info/
--rw-r--r--   0 harry.wilton   (502) staff       (20)     5403 2023-05-18 15:48:05.000000 appian-locust-2.0.0a4/appian_locust.egg-info/PKG-INFO
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2233 2023-05-18 15:48:05.000000 appian-locust-2.0.0a4/appian_locust.egg-info/SOURCES.txt
--rw-r--r--   0 harry.wilton   (502) staff       (20)        1 2023-05-18 15:48:05.000000 appian-locust-2.0.0a4/appian_locust.egg-info/dependency_links.txt
--rw-r--r--   0 harry.wilton   (502) staff       (20)       15 2023-05-18 15:48:05.000000 appian-locust-2.0.0a4/appian_locust.egg-info/requires.txt
--rw-r--r--   0 harry.wilton   (502) staff       (20)       14 2023-05-18 15:48:05.000000 appian-locust-2.0.0a4/appian_locust.egg-info/top_level.txt
--rw-r--r--   0 harry.wilton   (502) staff       (20)      100 2023-02-28 19:42:15.000000 appian-locust-2.0.0a4/pyproject.toml
--rw-r--r--   0 harry.wilton   (502) staff       (20)      595 2023-05-18 15:48:06.032962 appian-locust-2.0.0a4/setup.cfg
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1088 2023-05-15 17:00:04.000000 appian-locust-2.0.0a4/setup.py
-drwxr-xr-x   0 harry.wilton   (502) staff       (20)        0 2023-05-18 15:48:06.031077 appian-locust-2.0.0a4/tests/
--rw-r--r--   0 harry.wilton   (502) staff       (20)     6106 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/tests/test_actions.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1053 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/tests/test_admin.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     6785 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/tests/test_app_importer.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    11018 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/tests/test_appianclient.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1667 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/tests/test_application_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2981 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/tests/test_design.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1632 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/tests/test_design_object_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2596 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/tests/test_design_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    12722 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/tests/test_feature_toggle_helper.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     7834 2022-06-20 13:00:59.000000 appian-locust-2.0.0a4/tests/test_grid_interactor.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2936 2022-06-08 19:05:09.000000 appian-locust-2.0.0a4/tests/test_helper.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    19580 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/tests/test_interactor.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1458 2022-02-17 16:44:14.000000 appian-locust-2.0.0a4/tests/test_libraries_utils.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)      891 2022-02-17 16:44:14.000000 appian-locust-2.0.0a4/tests/test_locust_error_handler.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     4727 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/tests/test_news.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2391 2023-05-15 14:44:16.000000 appian-locust-2.0.0a4/tests/test_portals.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1844 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/tests/test_record_list_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     4349 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/tests/test_record_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    13429 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/tests/test_records.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2334 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/tests/test_records_helper.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     5554 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/tests/test_reports.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     3664 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/tests/test_save_request_builder.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2257 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/tests/test_site_helper.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     6343 2023-05-18 15:15:43.000000 appian-locust-2.0.0a4/tests/test_sites.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     4184 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/tests/test_tasks.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2360 2022-02-17 16:44:14.000000 appian-locust-2.0.0a4/tests/test_ui_reconciler.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    61599 2023-05-11 19:17:00.000000 appian-locust-2.0.0a4/tests/test_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)      784 2022-02-17 16:44:14.000000 appian-locust-2.0.0a4/tests/test_utils.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    22517 2023-05-15 14:44:16.000000 appian-locust-2.0.0a4/tests/test_visitor.py
+drwxr-xr-x   0 harry.wilton   (502) staff       (20)        0 2023-05-24 15:50:10.885844 appian-locust-2.0.0a5/
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    11358 2022-02-17 16:44:14.000000 appian-locust-2.0.0a5/LICENSE
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     5403 2023-05-24 15:50:10.885990 appian-locust-2.0.0a5/PKG-INFO
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     4829 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/README.rst
+drwxr-xr-x   0 harry.wilton   (502) staff       (20)        0 2023-05-24 15:50:10.858313 appian-locust-2.0.0a5/appian_locust/
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      775 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/__init__.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     9541 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_actions.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      786 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_admin.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2479 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_base.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     6282 2023-05-23 17:47:36.000000 appian-locust-2.0.0a5/appian_locust/_design.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     6206 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_feature_toggle_helper.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     7830 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_grid_interactor.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    53252 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_interactor.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     5171 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_locust_error_handler.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     7765 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_news.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1025 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_portals.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    16297 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_records.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     7380 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_records_helper.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     7185 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_reports.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     3016 2023-04-27 17:42:07.000000 appian-locust-2.0.0a5/appian_locust/_save_request_builder.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     9934 2023-05-23 18:03:22.000000 appian-locust-2.0.0a5/appian_locust/_sites.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     4514 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_task_opener.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     7644 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_tasks.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2365 2022-02-17 16:44:14.000000 appian-locust-2.0.0a5/appian_locust/_ui_reconciler.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1372 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/actions_info.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    14485 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/appianclient.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      354 2023-05-23 17:55:37.000000 appian-locust-2.0.0a5/appian_locust/application.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     3950 2023-05-24 15:47:33.000000 appian-locust-2.0.0a5/appian_locust/application_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      358 2023-05-23 17:55:55.000000 appian-locust-2.0.0a5/appian_locust/design_object.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      205 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/design_object_type.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1068 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/design_object_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     6234 2023-05-23 17:47:36.000000 appian-locust-2.0.0a5/appian_locust/design_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      859 2022-02-17 16:44:14.000000 appian-locust-2.0.0a5/appian_locust/exceptions.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1792 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/feature_flag.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    16278 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/helper.py
+-rwxr-xr-x   0 harry.wilton   (502) staff       (20)     1431 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/loadDriverUtils.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      862 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/logger.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2749 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/news_info.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1941 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/record_list_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1320 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/record_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      547 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/records_info.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1546 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/reports_info.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1364 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/site_helper.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      990 2023-05-23 17:57:12.000000 appian-locust-2.0.0a5/appian_locust/site_objects.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1261 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/sites_info.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1406 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/tasks_info.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2504 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/tempo_navigator.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    73573 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    13980 2023-05-23 18:00:11.000000 appian-locust-2.0.0a5/appian_locust/visitor.py
+drwxr-xr-x   0 harry.wilton   (502) staff       (20)        0 2023-05-24 15:50:10.863019 appian-locust-2.0.0a5/appian_locust.egg-info/
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     5403 2023-05-24 15:50:10.000000 appian-locust-2.0.0a5/appian_locust.egg-info/PKG-INFO
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2293 2023-05-24 15:50:10.000000 appian-locust-2.0.0a5/appian_locust.egg-info/SOURCES.txt
+-rw-r--r--   0 harry.wilton   (502) staff       (20)        1 2023-05-24 15:50:10.000000 appian-locust-2.0.0a5/appian_locust.egg-info/dependency_links.txt
+-rw-r--r--   0 harry.wilton   (502) staff       (20)       15 2023-05-24 15:50:10.000000 appian-locust-2.0.0a5/appian_locust.egg-info/requires.txt
+-rw-r--r--   0 harry.wilton   (502) staff       (20)       14 2023-05-24 15:50:10.000000 appian-locust-2.0.0a5/appian_locust.egg-info/top_level.txt
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      100 2023-02-28 19:42:15.000000 appian-locust-2.0.0a5/pyproject.toml
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      595 2023-05-24 15:50:10.886654 appian-locust-2.0.0a5/setup.cfg
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1088 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/setup.py
+drwxr-xr-x   0 harry.wilton   (502) staff       (20)        0 2023-05-24 15:50:10.885221 appian-locust-2.0.0a5/tests/
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     6106 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_actions.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1053 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_admin.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     6785 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_app_importer.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    11018 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_appianclient.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1667 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_application_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2981 2023-05-23 17:50:15.000000 appian-locust-2.0.0a5/tests/test_design.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1632 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_design_object_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2596 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_design_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    12722 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_feature_toggle_helper.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     7834 2022-06-20 13:00:59.000000 appian-locust-2.0.0a5/tests/test_grid_interactor.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2936 2022-06-08 19:05:09.000000 appian-locust-2.0.0a5/tests/test_helper.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    19580 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_interactor.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1458 2022-02-17 16:44:14.000000 appian-locust-2.0.0a5/tests/test_libraries_utils.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      891 2022-02-17 16:44:14.000000 appian-locust-2.0.0a5/tests/test_locust_error_handler.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     4727 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_news.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2391 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_portals.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     1844 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_record_list_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     4349 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_record_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    13429 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_records.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2334 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_records_helper.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     5554 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_reports.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     3664 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_save_request_builder.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2257 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_site_helper.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     6304 2023-05-23 18:01:25.000000 appian-locust-2.0.0a5/tests/test_sites.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     4184 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_tasks.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)     2360 2022-02-17 16:44:14.000000 appian-locust-2.0.0a5/tests/test_ui_reconciler.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    61599 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_uiform.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)      784 2022-02-17 16:44:14.000000 appian-locust-2.0.0a5/tests/test_utils.py
+-rw-r--r--   0 harry.wilton   (502) staff       (20)    22517 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_visitor.py
```

### Comparing `appian-locust-2.0.0a4/LICENSE` & `appian-locust-2.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/PKG-INFO` & `appian-locust-2.0.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appian-locust
-Version: 2.0.0a4
+Version: 2.0.0a5
 Summary: Tools and functions to make testing Appian with Locust easier
 Home-page: https://gitlab.com/appian-oss/appian-locust
 Author: Appian Performance & Reliability Engineering Squad
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `appian-locust-2.0.0a4/README.rst` & `appian-locust-2.0.0a5/README.rst`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/__init__.py` & `appian-locust-2.0.0a5/appian_locust/__init__.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/_actions.py` & `appian-locust-2.0.0a5/appian_locust/_actions.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/_admin.py` & `appian-locust-2.0.0a5/appian_locust/_admin.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/_base.py` & `appian-locust-2.0.0a5/appian_locust/_base.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/_design.py` & `appian-locust-2.0.0a5/appian_locust/_design.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,30 @@
-from enum import Enum
 from typing import Any, Dict, Optional
 
 from ._interactor import _Interactor
 from ._locust_error_handler import raises_locust_error
-from ._save_request_builder import save_builder
-from .helper import find_component_by_type_and_attribute_and_index_in_dict, find_component_by_type_and_attribute_and_index_in_dict, find_component_by_attribute_in_dict
+from .design_object import DesignObject
+from .helper import find_component_by_label_and_type_dict, find_component_by_type_and_attribute_and_index_in_dict, find_component_by_attribute_in_dict
 from .uiform import SailUiForm
 
 DESIGN_URI_PATH: str = "/suite/rest/a/applications/latest/app/design"
 
 
+def get_available_design_objects(state: Dict[str, Any]) -> Dict[str, DesignObject]:
+    name_column = find_component_by_label_and_type_dict(type="GridFieldColumn", attribute="label", value="Name",
+                                                        component_tree=state)
+    design_objects = {}
+    for element in name_column["data"]:
+        link = element["contents"]["items"][0]["item"]["value"]["values"][0]["link"]
+        name = link["testLabel"]
+        uri_split = link["uri"].split("/")
+        design_objects[name] = DesignObject(name, uri_split[len(uri_split) - 1])
+    return design_objects
+
+
 class _Design:
     def __init__(self, interactor: _Interactor):
         self.interactor = interactor
 
     @raises_locust_error
     def fetch_design_json(self) -> Dict[str, Any]:
         """
@@ -125,13 +136,13 @@
             label=locust_label)
 
     def find_design_object_opaque_id_in_grid(self, design_object_name: str, current_state: Dict[str, Any]) -> str:
         grid_component = self.find_design_grid(current_state)
         link_component = find_component_by_attribute_in_dict('testLabel', design_object_name, grid_component, throw_attribute_exception=True)
         return link_component.get("uri").split('/')[-1]
 
-    def _create_object(self, ui_form: SailUiForm, link_name: str, object_name: str) -> 'SailUiForm':
+    def create_object(self, ui_form: SailUiForm, link_name: str, object_name: str) -> 'SailUiForm':
         return ui_form.click(link_name)\
             .fill_text_field('Name', object_name)\
             .click('Create')\
             .assert_no_validations_present()\
             .click('Save')
```

### Comparing `appian-locust-2.0.0a4/appian_locust/_feature_toggle_helper.py` & `appian-locust-2.0.0a5/appian_locust/_feature_toggle_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/_grid_interactor.py` & `appian-locust-2.0.0a5/appian_locust/_grid_interactor.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/_interactor.py` & `appian-locust-2.0.0a5/appian_locust/_interactor.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/_locust_error_handler.py` & `appian-locust-2.0.0a5/appian_locust/_locust_error_handler.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/_news.py` & `appian-locust-2.0.0a5/appian_locust/_news.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/_portals.py` & `appian-locust-2.0.0a5/appian_locust/_portals.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/_records.py` & `appian-locust-2.0.0a5/appian_locust/_records.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/_records_helper.py` & `appian-locust-2.0.0a5/appian_locust/_records_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/_reports.py` & `appian-locust-2.0.0a5/appian_locust/_reports.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/_save_request_builder.py` & `appian-locust-2.0.0a5/appian_locust/_save_request_builder.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/_sites.py` & `appian-locust-2.0.0a5/appian_locust/_sites.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from . import logger
 from ._base import _Base
 from ._interactor import _Interactor
 from ._news import NEWS_NAV_PATH
 from .helper import extract_values, format_label
 from ._records_helper import get_all_records_from_json
-from .site_objects import Site, Page
+from .site_objects import Site, Page, PageType
 
 log = logger.getLogger(__name__)
 
 SITES_NAV_PATH = ["/suite/rest/a/sites/latest/", "/page/", "/nav"]
 SITES_PAGE_PATH = ["/suite/rest/a/sites/latest/", "/pages/", "/"]
 
 
@@ -219,21 +219,14 @@
 
     def _setup_headers_with_sail_json(self) -> dict:
         headers = self.interactor.setup_sail_headers()
         headers["Accept"] = "application/vnd.appian.tv.ui+json"
         return headers
 
 
-class PageType(enum.Enum):
-    ACTION: str = "action"
-    REPORT: str = "report"
-    RECORD: str = "recordType"
-    INTERFACE: str = "interface"
-
-
 class SiteNotFoundException(Exception):
     pass
 
 
 class PageNotFoundException(Exception):
     pass
```

### Comparing `appian-locust-2.0.0a4/appian_locust/_task_opener.py` & `appian-locust-2.0.0a5/appian_locust/_task_opener.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/_tasks.py` & `appian-locust-2.0.0a5/appian_locust/_tasks.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/_ui_reconciler.py` & `appian-locust-2.0.0a5/appian_locust/_ui_reconciler.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/actions_info.py` & `appian-locust-2.0.0a5/appian_locust/actions_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/appianclient.py` & `appian-locust-2.0.0a5/appian_locust/appianclient.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/design_object_uiform.py` & `appian-locust-2.0.0a5/appian_locust/design_object_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/design_uiform.py` & `appian-locust-2.0.0a5/appian_locust/design_uiform.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import Any, Dict, Optional
 
 from . import logger
-from ._design import _Design
+from ._design import _Design, get_available_design_objects
 from ._interactor import _Interactor
 from ._locust_error_handler import raises_locust_error
+from .application import Application
 from .application_uiform import ApplicationUiForm
-from .helper import find_component_by_attribute_in_dict
+from .design_object import DesignObject
+from .helper import find_component_by_attribute_in_dict, find_component_by_label_and_type_dict
 from .uiform import SailUiForm
 
 log = logger.getLogger(__name__)
 
 
 class DesignUiForm(SailUiForm):
 
@@ -38,15 +40,15 @@
     def create_application(self, application_name: str) -> 'ApplicationUiForm':
         """
         Creates an application and returns a form within representing the app contents
 
         Returns: The SAIL UI Form
 
         """
-        app_form = self.__design._create_object(self, link_name='New Application', object_name=application_name)
+        app_form = self.__design.create_object(self, link_name='New Application', object_name=application_name)
         app_form.breadcrumb = f"Design.SelectedApplicationByName.{application_name}"
         return ApplicationUiForm(self._interactor, self._state, self.breadcrumb)
 
     def import_application(self, app_file_path: str, customization_file_path: Optional[str] = None, inspect_and_import: bool = False) -> None:
         """
         Import an application into the Appian instance.
         Args:
@@ -109,7 +111,31 @@
         """
         new_state = self.__design.search_design_grid(
             search_str, self._get_update_url_for_reeval(self._state), self._state, self.context, self.uuid,
             locust_label if locust_label else f"{self.breadcrumb}.ObjectSearch"
         )
         self._reconcile_state(new_state)
         return self
+
+    def get_available_applications(self) -> Dict[str, Application]:
+        """
+            Retrieve all available applications in /design. Must be on page with application list
+
+            Returns (dict): Dictionary mapping application names to Application
+        """
+        grid_field = self.__design.find_design_grid(self._state)
+        applications = {}
+        name_column = grid_field["columns"][0]
+        num_applications = len(name_column["data"])
+        for idx in range(num_applications):
+            app_name = name_column["data"][idx]
+            href_split = name_column["links"][idx]["href"].split("/")
+            applications[app_name] = Application(app_name, href_split[len(href_split) - 1])
+        return applications
+
+    def get_available_design_objects(self) -> Dict[str, DesignObject]:
+        """
+            Retrieve all available design objects in the application. Must be on page with design object list
+
+            Returns (dict): Dictionary mapping design object names to DesignObject
+        """
+        return get_available_design_objects(self._state)
```

### Comparing `appian-locust-2.0.0a4/appian_locust/exceptions.py` & `appian-locust-2.0.0a5/appian_locust/exceptions.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/feature_flag.py` & `appian-locust-2.0.0a5/appian_locust/feature_flag.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/helper.py` & `appian-locust-2.0.0a5/appian_locust/helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/loadDriverUtils.py` & `appian-locust-2.0.0a5/appian_locust/loadDriverUtils.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/logger.py` & `appian-locust-2.0.0a5/appian_locust/logger.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/news_info.py` & `appian-locust-2.0.0a5/appian_locust/news_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/record_list_uiform.py` & `appian-locust-2.0.0a5/appian_locust/record_list_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/record_uiform.py` & `appian-locust-2.0.0a5/appian_locust/record_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/records_info.py` & `appian-locust-2.0.0a5/appian_locust/records_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/reports_info.py` & `appian-locust-2.0.0a5/appian_locust/reports_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/site_helper.py` & `appian-locust-2.0.0a5/appian_locust/site_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/site_objects.py` & `appian-locust-2.0.0a5/appian_locust/site_objects.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Dict
+from enum import Enum
 
 
 class Site:
     """
     Class representing a single site, as well as its pages
     """
 
@@ -28,7 +29,14 @@
         self.page_type = page_type
 
     def __str__(self) -> str:
         return f"Page(name={self.page_name},type={self.page_type})"
 
     def __repr__(self) -> str:
         return self.__str__()
+
+
+class PageType(Enum):
+    ACTION: str = "action"
+    REPORT: str = "report"
+    RECORD: str = "recordType"
+    INTERFACE: str = "interface"
```

### Comparing `appian-locust-2.0.0a4/appian_locust/sites_info.py` & `appian-locust-2.0.0a5/appian_locust/sites_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/tasks_info.py` & `appian-locust-2.0.0a5/appian_locust/tasks_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/tempo_navigator.py` & `appian-locust-2.0.0a5/appian_locust/tempo_navigator.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/uiform.py` & `appian-locust-2.0.0a5/appian_locust/uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/appian_locust/visitor.py` & `appian-locust-2.0.0a5/appian_locust/visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 from appian_locust.record_uiform import RecordInstanceUiForm
 from ._portals import _Portals
 from .application_uiform import ApplicationUiForm
 from .design_object_uiform import DesignObjectUiForm
 from .design_uiform import DesignUiForm
 from .design_object_type import DesignObjectType
 from .record_list_uiform import RecordListUiForm
+from .site_objects import PageType
 from .uiform import SailUiForm
 from ._actions import _Actions
 from ._design import _Design
 from ._interactor import _Interactor
 from ._records import _Records
 from ._reports import _Reports
-from ._sites import _Sites, PageType
+from ._sites import _Sites
 from ._admin import _Admin
 from ._tasks import _Tasks
 from .helper import format_label
 
 
 class Visitor:
     """
```

### Comparing `appian-locust-2.0.0a4/appian_locust.egg-info/PKG-INFO` & `appian-locust-2.0.0a5/appian_locust.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appian-locust
-Version: 2.0.0a4
+Version: 2.0.0a5
 Summary: Tools and functions to make testing Appian with Locust easier
 Home-page: https://gitlab.com/appian-oss/appian-locust
 Author: Appian Performance & Reliability Engineering Squad
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `appian-locust-2.0.0a4/appian_locust.egg-info/SOURCES.txt` & `appian-locust-2.0.0a5/appian_locust.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 appian_locust/_save_request_builder.py
 appian_locust/_sites.py
 appian_locust/_task_opener.py
 appian_locust/_tasks.py
 appian_locust/_ui_reconciler.py
 appian_locust/actions_info.py
 appian_locust/appianclient.py
+appian_locust/application.py
 appian_locust/application_uiform.py
+appian_locust/design_object.py
 appian_locust/design_object_type.py
 appian_locust/design_object_uiform.py
 appian_locust/design_uiform.py
 appian_locust/exceptions.py
 appian_locust/feature_flag.py
 appian_locust/helper.py
 appian_locust/loadDriverUtils.py
```

### Comparing `appian-locust-2.0.0a4/setup.cfg` & `appian-locust-2.0.0a5/setup.cfg`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/setup.py` & `appian-locust-2.0.0a5/setup.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_actions.py` & `appian-locust-2.0.0a5/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_admin.py` & `appian-locust-2.0.0a5/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_app_importer.py` & `appian-locust-2.0.0a5/tests/test_app_importer.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_appianclient.py` & `appian-locust-2.0.0a5/tests/test_appianclient.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_application_uiform.py` & `appian-locust-2.0.0a5/tests/test_application_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_design.py` & `appian-locust-2.0.0a5/tests/test_design.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_design_object_uiform.py` & `appian-locust-2.0.0a5/tests/test_design_object_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_design_uiform.py` & `appian-locust-2.0.0a5/tests/test_design_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_feature_toggle_helper.py` & `appian-locust-2.0.0a5/tests/test_feature_toggle_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_grid_interactor.py` & `appian-locust-2.0.0a5/tests/test_grid_interactor.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_helper.py` & `appian-locust-2.0.0a5/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_interactor.py` & `appian-locust-2.0.0a5/tests/test_interactor.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_libraries_utils.py` & `appian-locust-2.0.0a5/tests/test_libraries_utils.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_locust_error_handler.py` & `appian-locust-2.0.0a5/tests/test_locust_error_handler.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_news.py` & `appian-locust-2.0.0a5/tests/test_news.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_portals.py` & `appian-locust-2.0.0a5/tests/test_portals.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_record_list_uiform.py` & `appian-locust-2.0.0a5/tests/test_record_list_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_record_uiform.py` & `appian-locust-2.0.0a5/tests/test_record_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_records.py` & `appian-locust-2.0.0a5/tests/test_records.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_records_helper.py` & `appian-locust-2.0.0a5/tests/test_records_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_reports.py` & `appian-locust-2.0.0a5/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_save_request_builder.py` & `appian-locust-2.0.0a5/tests/test_save_request_builder.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_site_helper.py` & `appian-locust-2.0.0a5/tests/test_site_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_sites.py` & `appian-locust-2.0.0a5/tests/test_sites.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from locust import TaskSet, Locust
 from .mock_client import CustomLocust
 from .mock_reader import read_mock_file
 from requests.exceptions import HTTPError
 from appian_locust import AppianTaskSet
 from appian_locust._interactor import _Interactor
-from appian_locust._sites import _Sites, SiteNotFoundException, PageNotFoundException, PageType
-from appian_locust.uiform import SailUiForm
+from appian_locust._sites import _Sites, PageNotFoundException
+from appian_locust.site_objects import PageType
 import json
-import os
 import unittest
 
 
 class TestSites(unittest.TestCase):
 
     def setUp(self) -> None:
         self.custom_locust = CustomLocust(Locust())
```

### Comparing `appian-locust-2.0.0a4/tests/test_tasks.py` & `appian-locust-2.0.0a5/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_ui_reconciler.py` & `appian-locust-2.0.0a5/tests/test_ui_reconciler.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_uiform.py` & `appian-locust-2.0.0a5/tests/test_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_utils.py` & `appian-locust-2.0.0a5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a4/tests/test_visitor.py` & `appian-locust-2.0.0a5/tests/test_visitor.py`

 * *Files identical despite different names*

