# Comparing `tmp/nista_library-4.0.2.tar.gz` & `tmp/nista_library-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nista_library-4.0.2.tar", max compression
+gzip compressed data, was "nista_library-4.0.3.tar", max compression
```

## Comparing `nista_library-4.0.2.tar` & `nista_library-4.0.3.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0     1117 2023-05-18 13:57:43.917467 nista_library-4.0.2/LICENSE.md
--rw-r--r--   0        0        0     6428 2023-05-18 13:57:43.917467 nista_library-4.0.2/README.md
--rw-r--r--   0        0        0      153 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/__init__.py
--rw-r--r--   0        0        0       47 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_export/__init__.py
--rw-r--r--   0        0        0     5330 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_export/data_export_create_csv_export.py
--rw-r--r--   0        0        0        0 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/__init__.py
--rw-r--r--   0        0        0     5482 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_append_execution_result_data.py
--rw-r--r--   0        0        0     5376 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_append_time_series_data.py
--rw-r--r--   0        0        0     5768 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_create_area.py
--rw-r--r--   0        0        0     6225 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_create_area_message.py
--rw-r--r--   0        0        0     5323 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_create_chiller_samples.py
--rw-r--r--   0        0        0     5441 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_create_data_point.py
--rw-r--r--   0        0        0     4789 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_delete_area.py
--rw-r--r--   0        0        0     4473 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_delete_data_point.py
--rw-r--r--   0        0        0     4478 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py
--rw-r--r--   0        0        0     5168 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_delete_message.py
--rw-r--r--   0        0        0     5472 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_get_data.py
--rw-r--r--   0        0        0     5005 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_get_data_point.py
--rw-r--r--   0        0        0     5326 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_get_data_point_by_version.py
--rw-r--r--   0        0        0     8928 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_get_data_points.py
--rw-r--r--   0        0        0     7699 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_get_tags.py
--rw-r--r--   0        0        0     4805 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_get_tags_2.py
--rw-r--r--   0        0        0     5296 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_list_areas.py
--rw-r--r--   0        0        0     5769 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_update_area.py
--rw-r--r--   0        0        0     5397 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_update_constant_data.py
--rw-r--r--   0        0        0     5442 2023-05-18 13:57:43.919467 nista_library-4.0.2/data_point_client/api/data_point/data_point_update_data_point.py
--rw-r--r--   0        0        0     5518 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py
--rw-r--r--   0        0        0     5262 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/api/data_point/data_point_update_data_point_unit.py
--rw-r--r--   0        0        0     5369 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/api/data_point/data_point_update_day_period_data.py
--rw-r--r--   0        0        0     6226 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/api/data_point/data_point_update_message.py
--rw-r--r--   0        0        0     5381 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/api/data_point/data_point_update_time_series_data.py
--rw-r--r--   0        0        0     5381 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/api/data_point/data_point_update_week_period_data.py
--rw-r--r--   0        0        0     2817 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/client.py
--rw-r--r--   0        0        0      470 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/errors.py
--rw-r--r--   0        0        0     4795 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/__init__.py
--rw-r--r--   0        0        0     1965 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/append_execution_result_data_request.py
--rw-r--r--   0        0        0     1618 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/append_time_series_request.py
--rw-r--r--   0        0        0     4359 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/area_of_interest_response.py
--rw-r--r--   0        0        0     1858 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/calculation_origin.py
--rw-r--r--   0        0        0     7547 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/constant_data_bucket.py
--rw-r--r--   0        0        0     2965 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/constant_data_point_data.py
--rw-r--r--   0        0        0     2597 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/continuous_location_rest.py
--rw-r--r--   0        0        0      923 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/create_area_message_request.py
--rw-r--r--   0        0        0     2319 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/create_area_request.py
--rw-r--r--   0        0        0     5874 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/data_bucket_base.py
--rw-r--r--   0        0        0     2054 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/data_export_request.py
--rw-r--r--   0        0        0     2702 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/data_point_comment_message_response.py
--rw-r--r--   0        0        0     2016 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/data_point_data_base.py
--rw-r--r--   0        0        0     2418 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/data_point_data_response.py
--rw-r--r--   0        0        0      779 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/data_point_origin.py
--rw-r--r--   0        0        0     3212 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/data_point_request.py
--rw-r--r--   0        0        0     7362 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/data_point_response_base.py
--rw-r--r--   0        0        0     7281 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/day_data_by_hour_transfer.py
--rw-r--r--   0        0        0     7564 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/day_period_data_bucket.py
--rw-r--r--   0        0        0     4321 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/day_period_data_point_data.py
--rw-r--r--   0        0        0      191 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/en_area_type_rest.py
--rw-r--r--   0        0        0      192 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/en_data_bucket_state.py
--rw-r--r--   0        0        0      208 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/en_data_point_existence_dto.py
--rw-r--r--   0        0        0      214 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/en_data_point_state_dto.py
--rw-r--r--   0        0        0      192 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/en_data_point_status.py
--rw-r--r--   0        0        0      250 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/en_data_point_type.py
--rw-r--r--   0        0        0      181 2023-05-18 13:57:43.920467 nista_library-4.0.2/data_point_client/models/en_operator.py
--rw-r--r--   0        0        0     2375 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/file_origin.py
--rw-r--r--   0        0        0     2579 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/get_constant_response.py
--rw-r--r--   0        0        0     3472 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/get_data_request.py
--rw-r--r--   0        0        0      779 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/get_data_response.py
--rw-r--r--   0        0        0     3900 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/get_day_period_response.py
--rw-r--r--   0        0        0     2529 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/get_series_response.py
--rw-r--r--   0        0        0     3227 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/get_week_period_response.py
--rw-r--r--   0        0        0     1176 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/gnista_unit_response.py
--rw-r--r--   0        0        0     1810 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/live_data_origin.py
--rw-r--r--   0        0        0      765 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/location_rest.py
--rw-r--r--   0        0        0     2045 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/point_location_rest.py
--rw-r--r--   0        0        0     3377 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/problem_details.py
--rw-r--r--   0        0        0     1215 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/problem_details_extensions.py
--rw-r--r--   0        0        0     1449 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/remote_origin.py
--rw-r--r--   0        0        0     1247 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/rule.py
--rw-r--r--   0        0        0     9273 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/series_data_bucket.py
--rw-r--r--   0        0        0     3058 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/series_data_point_data.py
--rw-r--r--   0        0        0     1446 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/sub_series_request.py
--rw-r--r--   0        0        0     1214 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/sub_series_request_values.py
--rw-r--r--   0        0        0     1631 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/time_series_period.py
--rw-r--r--   0        0        0     2675 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/time_series_response.py
--rw-r--r--   0        0        0     1219 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/time_series_response_curve.py
--rw-r--r--   0        0        0      923 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/update_area_message_request.py
--rw-r--r--   0        0        0     2674 2023-05-18 13:57:43.921466 nista_library-4.0.2/data_point_client/models/update_area_request.py
--rw-r--r--   0        0        0     1401 2023-05-18 13:57:43.922467 nista_library-4.0.2/data_point_client/models/update_constant_data_request.py
--rw-r--r--   0        0        0     2725 2023-05-18 13:57:43.922467 nista_library-4.0.2/data_point_client/models/update_day_period_request.py
--rw-r--r--   0        0        0     3346 2023-05-18 13:57:43.922467 nista_library-4.0.2/data_point_client/models/update_time_series_request.py
--rw-r--r--   0        0        0     2052 2023-05-18 13:57:43.922467 nista_library-4.0.2/data_point_client/models/update_week_period_request.py
--rw-r--r--   0        0        0     7478 2023-05-18 13:57:43.922467 nista_library-4.0.2/data_point_client/models/week_data_transfere.py
--rw-r--r--   0        0        0     7576 2023-05-18 13:57:43.922467 nista_library-4.0.2/data_point_client/models/week_period_data_bucket.py
--rw-r--r--   0        0        0     3648 2023-05-18 13:57:43.922467 nista_library-4.0.2/data_point_client/models/week_period_data_point_data.py
--rw-r--r--   0        0        0       25 2023-05-18 13:57:43.922467 nista_library-4.0.2/data_point_client/py.typed
--rw-r--r--   0        0        0      974 2023-05-18 13:57:43.922467 nista_library-4.0.2/data_point_client/types.py
--rw-r--r--   0        0        0     1007 2023-05-18 13:57:43.923467 nista_library-4.0.2/nista_library/__init__.py
--rw-r--r--   0        0        0    11406 2023-05-18 13:57:43.923467 nista_library-4.0.2/nista_library/nista_connetion.py
--rw-r--r--   0        0        0     1049 2023-05-18 13:57:43.923467 nista_library-4.0.2/nista_library/nista_credential_manager.py
--rw-r--r--   0        0        0    15802 2023-05-18 13:57:43.923467 nista_library-4.0.2/nista_library/nista_data_point.py
--rw-r--r--   0        0        0     1997 2023-05-18 13:57:43.923467 nista_library-4.0.2/nista_library/nista_data_points.py
--rw-r--r--   0        0        0     1383 2023-05-18 13:57:43.925466 nista_library-4.0.2/pyproject.toml
--rw-r--r--   0        0        0     7471 1970-01-01 00:00:00.000000 nista_library-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1117 2023-05-24 14:17:43.509786 nista_library-4.0.3/LICENSE.md
+-rw-r--r--   0        0        0     6428 2023-05-24 14:17:43.510786 nista_library-4.0.3/README.md
+-rw-r--r--   0        0        0      153 2023-05-24 14:17:43.511786 nista_library-4.0.3/data_point_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-24 14:17:43.511786 nista_library-4.0.3/data_point_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 14:17:43.511786 nista_library-4.0.3/data_point_client/api/data_export/__init__.py
+-rw-r--r--   0        0        0     5330 2023-05-24 14:17:43.511786 nista_library-4.0.3/data_point_client/api/data_export/data_export_create_csv_export.py
+-rw-r--r--   0        0        0        0 2023-05-24 14:17:43.511786 nista_library-4.0.3/data_point_client/api/data_point/__init__.py
+-rw-r--r--   0        0        0     5482 2023-05-24 14:17:43.511786 nista_library-4.0.3/data_point_client/api/data_point/data_point_append_execution_result_data.py
+-rw-r--r--   0        0        0     5376 2023-05-24 14:17:43.511786 nista_library-4.0.3/data_point_client/api/data_point/data_point_append_time_series_data.py
+-rw-r--r--   0        0        0     5768 2023-05-24 14:17:43.511786 nista_library-4.0.3/data_point_client/api/data_point/data_point_create_area.py
+-rw-r--r--   0        0        0     6225 2023-05-24 14:17:43.511786 nista_library-4.0.3/data_point_client/api/data_point/data_point_create_area_message.py
+-rw-r--r--   0        0        0     5323 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_create_chiller_samples.py
+-rw-r--r--   0        0        0     5441 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_create_data_point.py
+-rw-r--r--   0        0        0     4789 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_delete_area.py
+-rw-r--r--   0        0        0     4473 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_delete_data_point.py
+-rw-r--r--   0        0        0     4478 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py
+-rw-r--r--   0        0        0     5168 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_delete_message.py
+-rw-r--r--   0        0        0     5472 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_get_data.py
+-rw-r--r--   0        0        0     5005 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_get_data_point.py
+-rw-r--r--   0        0        0     5326 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_get_data_point_by_version.py
+-rw-r--r--   0        0        0     8928 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_get_data_points.py
+-rw-r--r--   0        0        0     7699 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_get_tags.py
+-rw-r--r--   0        0        0     4805 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_get_tags_2.py
+-rw-r--r--   0        0        0     5296 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_list_areas.py
+-rw-r--r--   0        0        0     5769 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_update_area.py
+-rw-r--r--   0        0        0     5397 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_update_constant_data.py
+-rw-r--r--   0        0        0     5442 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_update_data_point.py
+-rw-r--r--   0        0        0     5518 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py
+-rw-r--r--   0        0        0     5262 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_update_data_point_unit.py
+-rw-r--r--   0        0        0     5369 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_update_day_period_data.py
+-rw-r--r--   0        0        0     6226 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_update_message.py
+-rw-r--r--   0        0        0     5381 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_update_time_series_data.py
+-rw-r--r--   0        0        0     5381 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_update_week_period_data.py
+-rw-r--r--   0        0        0     2817 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/client.py
+-rw-r--r--   0        0        0      470 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/errors.py
+-rw-r--r--   0        0        0     4795 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/__init__.py
+-rw-r--r--   0        0        0     1965 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/append_execution_result_data_request.py
+-rw-r--r--   0        0        0     1906 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/append_time_series_request.py
+-rw-r--r--   0        0        0     4359 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/area_of_interest_response.py
+-rw-r--r--   0        0        0     1858 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/calculation_origin.py
+-rw-r--r--   0        0        0     7547 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/constant_data_bucket.py
+-rw-r--r--   0        0        0     2965 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/constant_data_point_data.py
+-rw-r--r--   0        0        0     2597 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/continuous_location_rest.py
+-rw-r--r--   0        0        0      923 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/create_area_message_request.py
+-rw-r--r--   0        0        0     2319 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/create_area_request.py
+-rw-r--r--   0        0        0     5874 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/data_bucket_base.py
+-rw-r--r--   0        0        0     2054 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/data_export_request.py
+-rw-r--r--   0        0        0     2702 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/data_point_comment_message_response.py
+-rw-r--r--   0        0        0     2016 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/data_point_data_base.py
+-rw-r--r--   0        0        0     2418 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/data_point_data_response.py
+-rw-r--r--   0        0        0      779 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/data_point_origin.py
+-rw-r--r--   0        0        0     3212 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/data_point_request.py
+-rw-r--r--   0        0        0     7362 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/data_point_response_base.py
+-rw-r--r--   0        0        0     7281 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/day_data_by_hour_transfer.py
+-rw-r--r--   0        0        0     7564 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/day_period_data_bucket.py
+-rw-r--r--   0        0        0     4321 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/day_period_data_point_data.py
+-rw-r--r--   0        0        0      191 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/en_area_type_rest.py
+-rw-r--r--   0        0        0      192 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/en_data_bucket_state.py
+-rw-r--r--   0        0        0      208 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/en_data_point_existence_dto.py
+-rw-r--r--   0        0        0      214 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/en_data_point_state_dto.py
+-rw-r--r--   0        0        0      192 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/en_data_point_status.py
+-rw-r--r--   0        0        0      250 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/en_data_point_type.py
+-rw-r--r--   0        0        0      181 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/en_operator.py
+-rw-r--r--   0        0        0     2375 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/file_origin.py
+-rw-r--r--   0        0        0     2579 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/get_constant_response.py
+-rw-r--r--   0        0        0     3472 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/get_data_request.py
+-rw-r--r--   0        0        0      779 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/get_data_response.py
+-rw-r--r--   0        0        0     3900 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/get_day_period_response.py
+-rw-r--r--   0        0        0     2529 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/get_series_response.py
+-rw-r--r--   0        0        0     3227 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/get_week_period_response.py
+-rw-r--r--   0        0        0     1176 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/gnista_unit_response.py
+-rw-r--r--   0        0        0     1810 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/live_data_origin.py
+-rw-r--r--   0        0        0      765 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/location_rest.py
+-rw-r--r--   0        0        0     2045 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/point_location_rest.py
+-rw-r--r--   0        0        0     3377 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/problem_details.py
+-rw-r--r--   0        0        0     1215 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/problem_details_extensions.py
+-rw-r--r--   0        0        0     1449 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/remote_origin.py
+-rw-r--r--   0        0        0     1247 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/rule.py
+-rw-r--r--   0        0        0     9273 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/series_data_bucket.py
+-rw-r--r--   0        0        0     3058 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/series_data_point_data.py
+-rw-r--r--   0        0        0     1446 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/sub_series_request.py
+-rw-r--r--   0        0        0     1214 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/sub_series_request_values.py
+-rw-r--r--   0        0        0     1631 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/time_series_period.py
+-rw-r--r--   0        0        0     2675 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/time_series_response.py
+-rw-r--r--   0        0        0     1219 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/time_series_response_curve.py
+-rw-r--r--   0        0        0      923 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/update_area_message_request.py
+-rw-r--r--   0        0        0     2674 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/update_area_request.py
+-rw-r--r--   0        0        0     1401 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/update_constant_data_request.py
+-rw-r--r--   0        0        0     2725 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/update_day_period_request.py
+-rw-r--r--   0        0        0     3346 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/update_time_series_request.py
+-rw-r--r--   0        0        0     2052 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/update_week_period_request.py
+-rw-r--r--   0        0        0     7478 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/week_data_transfere.py
+-rw-r--r--   0        0        0     7576 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/week_period_data_bucket.py
+-rw-r--r--   0        0        0     3648 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/week_period_data_point_data.py
+-rw-r--r--   0        0        0       25 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/py.typed
+-rw-r--r--   0        0        0      993 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/types.py
+-rw-r--r--   0        0        0     1007 2023-05-24 14:17:43.515786 nista_library-4.0.3/nista_library/__init__.py
+-rw-r--r--   0        0        0    11406 2023-05-24 14:17:43.515786 nista_library-4.0.3/nista_library/nista_connetion.py
+-rw-r--r--   0        0        0     1049 2023-05-24 14:17:43.515786 nista_library-4.0.3/nista_library/nista_credential_manager.py
+-rw-r--r--   0        0        0    15802 2023-05-24 14:17:43.515786 nista_library-4.0.3/nista_library/nista_data_point.py
+-rw-r--r--   0        0        0     1997 2023-05-24 14:17:43.515786 nista_library-4.0.3/nista_library/nista_data_points.py
+-rw-r--r--   0        0        0     1383 2023-05-24 14:17:43.517786 nista_library-4.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7471 1970-01-01 00:00:00.000000 nista_library-4.0.3/PKG-INFO
```

### Comparing `nista_library-4.0.2/LICENSE.md` & `nista_library-4.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/README.md` & `nista_library-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_export/data_export_create_csv_export.py` & `nista_library-4.0.3/data_point_client/api/data_export/data_export_create_csv_export.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_append_execution_result_data.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_append_execution_result_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_append_time_series_data.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_append_time_series_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_create_area.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_create_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_create_area_message.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_create_area_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_create_chiller_samples.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_create_chiller_samples.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_create_data_point.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_create_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_delete_area.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_delete_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_delete_data_point.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_delete_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_delete_message.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_delete_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_get_data.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_get_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_get_data_point.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_get_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_get_data_point_by_version.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_get_data_point_by_version.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_get_data_points.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_get_data_points.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_get_tags.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_get_tags.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_get_tags_2.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_get_tags_2.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_list_areas.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_list_areas.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_update_area.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_update_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_update_constant_data.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_update_constant_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_update_data_point.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_update_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_update_data_point_unit.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_update_data_point_unit.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_update_day_period_data.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_update_day_period_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_update_message.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_update_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_update_time_series_data.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_update_time_series_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/api/data_point/data_point_update_week_period_data.py` & `nista_library-4.0.3/data_point_client/api/data_point/data_point_update_week_period_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/client.py` & `nista_library-4.0.3/data_point_client/client.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/__init__.py` & `nista_library-4.0.3/data_point_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/append_execution_result_data_request.py` & `nista_library-4.0.3/data_point_client/models/append_execution_result_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/area_of_interest_response.py` & `nista_library-4.0.3/data_point_client/models/area_of_interest_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/calculation_origin.py` & `nista_library-4.0.3/data_point_client/models/calculation_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/constant_data_bucket.py` & `nista_library-4.0.3/data_point_client/models/constant_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/constant_data_point_data.py` & `nista_library-4.0.3/data_point_client/models/constant_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/continuous_location_rest.py` & `nista_library-4.0.3/data_point_client/models/continuous_location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/create_area_message_request.py` & `nista_library-4.0.3/data_point_client/models/create_area_message_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/create_area_request.py` & `nista_library-4.0.3/data_point_client/models/create_area_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/data_bucket_base.py` & `nista_library-4.0.3/data_point_client/models/data_bucket_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/data_export_request.py` & `nista_library-4.0.3/data_point_client/models/data_export_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/data_point_comment_message_response.py` & `nista_library-4.0.3/data_point_client/models/data_point_comment_message_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/data_point_data_base.py` & `nista_library-4.0.3/data_point_client/models/data_point_data_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/data_point_data_response.py` & `nista_library-4.0.3/data_point_client/models/data_point_data_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/data_point_origin.py` & `nista_library-4.0.3/data_point_client/models/data_point_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/data_point_request.py` & `nista_library-4.0.3/data_point_client/models/data_point_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/data_point_response_base.py` & `nista_library-4.0.3/data_point_client/models/data_point_response_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/day_data_by_hour_transfer.py` & `nista_library-4.0.3/data_point_client/models/day_data_by_hour_transfer.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/day_period_data_bucket.py` & `nista_library-4.0.3/data_point_client/models/day_period_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/day_period_data_point_data.py` & `nista_library-4.0.3/data_point_client/models/day_period_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/file_origin.py` & `nista_library-4.0.3/data_point_client/models/file_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/get_constant_response.py` & `nista_library-4.0.3/data_point_client/models/get_constant_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/get_data_request.py` & `nista_library-4.0.3/data_point_client/models/get_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/get_data_response.py` & `nista_library-4.0.3/data_point_client/models/get_data_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/get_day_period_response.py` & `nista_library-4.0.3/data_point_client/models/get_day_period_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/get_series_response.py` & `nista_library-4.0.3/data_point_client/models/get_series_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/get_week_period_response.py` & `nista_library-4.0.3/data_point_client/models/get_week_period_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/gnista_unit_response.py` & `nista_library-4.0.3/data_point_client/models/gnista_unit_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/live_data_origin.py` & `nista_library-4.0.3/data_point_client/models/live_data_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/location_rest.py` & `nista_library-4.0.3/data_point_client/models/location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/point_location_rest.py` & `nista_library-4.0.3/data_point_client/models/point_location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/problem_details.py` & `nista_library-4.0.3/data_point_client/models/problem_details.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/problem_details_extensions.py` & `nista_library-4.0.3/data_point_client/models/problem_details_extensions.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/remote_origin.py` & `nista_library-4.0.3/data_point_client/models/remote_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/rule.py` & `nista_library-4.0.3/data_point_client/models/rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/series_data_bucket.py` & `nista_library-4.0.3/data_point_client/models/series_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/series_data_point_data.py` & `nista_library-4.0.3/data_point_client/models/series_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/sub_series_request.py` & `nista_library-4.0.3/data_point_client/models/sub_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/sub_series_request_values.py` & `nista_library-4.0.3/data_point_client/models/sub_series_request_values.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/time_series_period.py` & `nista_library-4.0.3/data_point_client/models/time_series_period.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/time_series_response.py` & `nista_library-4.0.3/data_point_client/models/time_series_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/time_series_response_curve.py` & `nista_library-4.0.3/data_point_client/models/time_series_response_curve.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/update_area_message_request.py` & `nista_library-4.0.3/data_point_client/models/update_area_message_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/update_area_request.py` & `nista_library-4.0.3/data_point_client/models/update_area_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/update_constant_data_request.py` & `nista_library-4.0.3/data_point_client/models/update_constant_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/update_day_period_request.py` & `nista_library-4.0.3/data_point_client/models/update_day_period_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/update_time_series_request.py` & `nista_library-4.0.3/data_point_client/models/update_time_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/update_week_period_request.py` & `nista_library-4.0.3/data_point_client/models/update_week_period_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/week_data_transfere.py` & `nista_library-4.0.3/data_point_client/models/week_data_transfere.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/week_period_data_bucket.py` & `nista_library-4.0.3/data_point_client/models/week_period_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/models/week_period_data_point_data.py` & `nista_library-4.0.3/data_point_client/models/week_period_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/data_point_client/types.py` & `nista_library-4.0.3/data_point_client/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """ Contains some shared types for properties """
 from http import HTTPStatus
-from typing import BinaryIO, Generic, MutableMapping, Optional, Tuple, TypeVar
+from typing import BinaryIO, Generic, Literal, MutableMapping, Optional, Tuple, TypeVar
 
 import attr
 
 
 class Unset:
-    def __bool__(self) -> bool:
+    def __bool__(self) -> Literal[False]:
         return False
 
 
 UNSET: Unset = Unset()
 
 FileJsonType = Tuple[Optional[str], BinaryIO, Optional[str]]
```

### Comparing `nista_library-4.0.2/nista_library/__init__.py` & `nista_library-4.0.3/nista_library/__init__.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/nista_library/nista_connetion.py` & `nista_library-4.0.3/nista_library/nista_connetion.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/nista_library/nista_credential_manager.py` & `nista_library-4.0.3/nista_library/nista_credential_manager.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/nista_library/nista_data_point.py` & `nista_library-4.0.3/nista_library/nista_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/nista_library/nista_data_points.py` & `nista_library-4.0.3/nista_library/nista_data_points.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.2/pyproject.toml` & `nista_library-4.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nista-library"
-version = "4.0.2"
+version = "4.0.3"
 description = "A client library for accessing nista.io"
 license = "MIT"
 
 authors = ["Markus Hoffmann <markus.hoffmann@nista.io>"]
 
 readme = "README.md"
 homepage = "https://nista.io"
```

### Comparing `nista_library-4.0.2/PKG-INFO` & `nista_library-4.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nista-library
-Version: 4.0.2
+Version: 4.0.3
 Summary: A client library for accessing nista.io
 Home-page: https://nista.io
 License: MIT
 Author: Markus Hoffmann
 Author-email: markus.hoffmann@nista.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

