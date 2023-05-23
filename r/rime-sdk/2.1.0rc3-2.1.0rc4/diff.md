# Comparing `tmp/rime_sdk-2.1.0rc3.tar.gz` & `tmp/rime_sdk-2.1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rime_sdk-2.1.0rc3.tar", last modified: Wed May 17 05:16:26 2023, max compression
+gzip compressed data, was "rime_sdk-2.1.0rc4.tar", last modified: Tue May 23 22:16:59 2023, max compression
```

## Comparing `rime_sdk-2.1.0rc3.tar` & `rime_sdk-2.1.0rc4.tar`

### file list

```diff
@@ -1,487 +1,487 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:16:26.863933 rime_sdk-2.1.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-17 05:16:26.859933 rime_sdk-2.1.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:16:26.775933 rime_sdk-2.1.0rc3/rime_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60633 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:16:26.775933 rime_sdk-2.1.0rc3/rime_sdk/data_format_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/data_format_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/data_format_check/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/data_format_check/data_format_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/data_format_check/nlp_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/data_format_check/tabular_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    24471 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/image_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:16:26.779933 rime_sdk-2.1.0rc3/rime_sdk/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/file_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/rest_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/security_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/swagger_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/swagger_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/throttle_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18267 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    61023 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    25145 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:16:26.779933 rime_sdk-2.1.0rc3/rime_sdk/swagger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:16:26.779933 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (123)    46345 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:16:26.783933 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30381 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/config_validator_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25158 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/data_collector_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/detection_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22854 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/file_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/foo_xp_interface_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28249 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/image_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26851 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/integration_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26924 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/job_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21593 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19234 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/model_testing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29422 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19707 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    55776 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/project_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    57282 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/registry_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    64351 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/results_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/rime_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    60397 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25142 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:16:26.859933 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    44319 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    13463 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11773 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/fooexample_foo_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/fooexample_foo_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/model_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_object_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    17717 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/protobuf_any.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rca_rca_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rca_rca_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    18304 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_delta_lake_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_config_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_float_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_foo_task_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_int_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_language.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_named_double.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_foo_task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_foo_task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_str_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_table_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_token_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/role_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schemaregistry_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schematestrun_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/tags_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/user_private_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/user_user_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:16:26.775933 rime_sdk-2.1.0rc3/rime_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-17 05:16:26.000000 rime_sdk-2.1.0rc3/rime_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32082 2023-05-17 05:16:26.000000 rime_sdk-2.1.0rc3/rime_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 05:16:26.000000 rime_sdk-2.1.0rc3/rime_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 05:16:26.000000 rime_sdk-2.1.0rc3/rime_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-17 05:16:26.000000 rime_sdk-2.1.0rc3/rime_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 05:16:26.000000 rime_sdk-2.1.0rc3/rime_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 05:16:26.863933 rime_sdk-2.1.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:16:59.960142 rime_sdk-2.1.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-23 22:16:59.960142 rime_sdk-2.1.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:16:59.868142 rime_sdk-2.1.0rc4/rime_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60561 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:16:59.868142 rime_sdk-2.1.0rc4/rime_sdk/data_format_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/data_format_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/data_format_check/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/data_format_check/data_format_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/data_format_check/nlp_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/data_format_check/tabular_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24472 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/image_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:16:59.872141 rime_sdk-2.1.0rc4/rime_sdk/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/internal/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/internal/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/internal/file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/internal/rest_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/internal/security_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/internal/swagger_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/internal/swagger_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/internal/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/internal/throttle_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18267 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61304 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25145 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:16:59.872141 rime_sdk-2.1.0rc4/rime_sdk/swagger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:16:59.872141 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    46373 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:16:59.876142 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30418 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/config_validator_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25195 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/data_collector_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/detection_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/file_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21540 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/foo_xp_interface_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/image_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26888 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/integration_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26961 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/job_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21630 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19271 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/model_testing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29459 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55813 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/project_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57319 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/registry_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64388 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/results_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/rime_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40185 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60434 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:16:59.960142 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    44347 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16260 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/detection_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/detection_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/fooexample_foo_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/fooexample_foo_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/integration_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/model_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/notification_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/notification_object_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/protobuf_any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rca_rca_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rca_rca_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20573 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_delta_lake_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_config_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_float_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_foo_task_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_int_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_model_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_named_double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_foo_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_foo_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_str_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_table_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_token_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/role_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/tags_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12936 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15198 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/user_private_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/user_user_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-05-23 22:16:55.000000 rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/rime_sdk/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:16:59.868142 rime_sdk-2.1.0rc4/rime_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-23 22:16:59.000000 rime_sdk-2.1.0rc4/rime_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32078 2023-05-23 22:16:59.000000 rime_sdk-2.1.0rc4/rime_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 22:16:59.000000 rime_sdk-2.1.0rc4/rime_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-23 22:16:59.000000 rime_sdk-2.1.0rc4/rime_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-23 22:16:59.000000 rime_sdk-2.1.0rc4/rime_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 22:16:59.000000 rime_sdk-2.1.0rc4/rime_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 22:16:59.960142 rime_sdk-2.1.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-23 22:16:13.000000 rime_sdk-2.1.0rc4/setup.py
```

### Comparing `rime_sdk-2.1.0rc3/LICENSE` & `rime_sdk-2.1.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/PKG-INFO` & `rime_sdk-2.1.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime_sdk
-Version: 2.1.0rc3
+Version: 2.1.0rc4
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.1.0rc3/README.md` & `rime_sdk-2.1.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/__init__.py` & `rime_sdk-2.1.0rc4/rime_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/client.py` & `rime_sdk-2.1.0rc4/rime_sdk/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,21 @@
 
 VALID_MODEL_TASKS = [
     model_task
     for _, model_task in getmembers(RimeModelTask)
     if isinstance(model_task, str) and "MODEL_TASK_" in model_task
 ]
 
+# If the api client receives one of these recoverable status codes, it will retry the request.
+RETRY_HTTP_STATUS = [
+    HTTPStatus.SERVICE_UNAVAILABLE,
+    HTTPStatus.TOO_MANY_REQUESTS,
+    HTTPStatus.GATEWAY_TIMEOUT,
+]
+
 
 class Client:
     """A Client object provides an interface to RIME's \
         services for creating Projects, starting Stress Test Jobs,\
         and querying the backend for current Stress Test Jobs.
 
     To initialize the Client, provide the address of your RIME instance.
@@ -106,22 +113,14 @@
             rime_client = Client("my_vpc.rime.com", "api-key")
     """
 
     # A throttler that limits the number of model tests to roughly 20 every 5 minutes.
     # This is a static variable for Client.
     _throttler = ThrottleQueue(desired_events_per_epoch=20, epoch_duration_sec=300)
 
-    # If the api client receives one of these recoverable status codes, it will retry the request.
-    RETRY_HTTP_STATUS = [
-        HTTPStatus.INTERNAL_SERVER_ERROR,
-        HTTPStatus.SERVICE_UNAVAILABLE,
-        HTTPStatus.TOO_MANY_REQUESTS,
-        HTTPStatus.GATEWAY_TIMEOUT,
-    ]
-
     def __init__(
         self,
         domain: str,
         api_key: str = "",
         channel_timeout: float = 180.0,
         disable_tls: bool = False,
         ssl_ca_cert: Optional[Union[Path, str]] = None,
@@ -155,15 +154,15 @@
         # Prevent race condition in pool.close() triggered by swagger generated code
         atexit.register(self._api_client.pool.close)
         # Sets the timeout and hardcoded retries parameter for the api client.
         self._api_client.rest_client.pool_manager.connection_pool_kw[
             "timeout"
         ] = channel_timeout
         self._api_client.rest_client.pool_manager.connection_pool_kw["retries"] = Retry(
-            total=3, status_forcelist=self.RETRY_HTTP_STATUS
+            total=3, status_forcelist=RETRY_HTTP_STATUS
         )
         self.customer_name = self._check_version()
         self._check_expiration()
 
     def __repr__(self) -> str:
         """Return the string representation of the Client."""
         return f"Client(domain={self._domain})"
@@ -920,15 +919,15 @@
               test_run_config=config, project_id="123-456-789"
            )
         """
         self._check_stress_test_limit()
         # TODO(blaine): Add config validation service.
         if not isinstance(test_run_config, dict):
             raise ValueError("The configuration must be a dictionary")
-        # TODO (VAL-316): do proper runtime validation of all of the types in the config
+        # TODO(VAL-316): do proper runtime validation of all of the types in the config
         if project_id and not self._project_exists(project_id):
             raise ValueError("Project id {} does not exist".format(project_id))
         if "model_id" in test_run_config:
             if isinstance(test_run_config["model_id"], str):
                 test_run_config["model_id"] = _get_uuid(test_run_config["model_id"])
         if "run_time_info" in test_run_config:
             if "agent_id" in test_run_config["run_time_info"]:
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/data_collector.py` & `rime_sdk-2.1.0rc4/rime_sdk/data_collector.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/data_format_check/cli.py` & `rime_sdk-2.1.0rc4/rime_sdk/data_format_check/cli.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/data_format_check/data_format_checker.py` & `rime_sdk-2.1.0rc4/rime_sdk/data_format_check/data_format_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/data_format_check/nlp_checker.py` & `rime_sdk-2.1.0rc4/rime_sdk/data_format_check/nlp_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
             raise ValueError(
                 ERROR_UNKNOWN_INPUT.format(input_type=input_type, accepted=INPUT_TYPES)
             )
 
     print(f"\nInspecting '{file_path}':")
     for i in tqdm(range(0, len(list_data))):
         try:
-            # TODO add manual non-null/non-empty check?
+            # TODO(RAT-1940): add manual non-null/non-empty check
             schema.validate(list_data[i])
         except SchemaError as e:
             schema_str_trimmed = str(schema).replace("Schema(", "").replace(")", "")
             schema_msg = (
                 f"\n\n---\n\nInputs for task '{task}' must adhere to the "
                 f"following structure:\n\n{schema_str_trimmed}"
             )
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/data_format_check/tabular_checker.py` & `rime_sdk-2.1.0rc4/rime_sdk/data_format_check/tabular_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import numpy as np
 import pandas as pd
 
 from rime_sdk.data_format_check.data_format_checker import DataFormatChecker
 
 # Tabular Tasks
-# TODO add Ranking
+# TODO(RAT-1942): add Ranking
 BINARY_CLASSIFICATION = "Binary Classification"
 REGRESSION = "Regression"
 MULTI_CLASS_CLASSIFICATION = "Multi-class Classification"
 TABULAR_TASKS = {BINARY_CLASSIFICATION, REGRESSION, MULTI_CLASS_CLASSIFICATION}
 
 # Accepted formats for the "timestamp" column
 FORMAT_SECONDS = "%Y-%m-%d %H:%M:%S"
@@ -79,15 +79,14 @@
         pred_col_name: Optional[str],
         timestamp_col_name: Optional[str] = None,
     ) -> None:
         """Perform multiple checks against the given file."""
         if not filename.exists():
             raise ValueError(f"File {filename} does not exist")
 
-        # TODO decide if this should be wrapped and re-thrown, for clarity?
         if filename.suffix == ".csv":
             df = pd.read_csv(filename)
         elif filename.suffix == ".parquet":
             df = pd.read_parquet(filename)
         else:
             raise ValueError(
                 f"Invalid file type '{filename.suffix}'. File must be one of "
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/detection_event.py` & `rime_sdk-2.1.0rc4/rime_sdk/detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/firewall.py` & `rime_sdk-2.1.0rc4/rime_sdk/firewall.py`

 * *Files 1% similar despite different names*

```diff
@@ -341,15 +341,15 @@
     ) -> pd.DataFrame:
         """Get a dataframe of Detected Events for the given Firewall.
 
         Monitors detect Events when degradations occur.
         For example, a Monitor for the metric "Accuracy" will detect an Event
         when the value of the model performance metric drops below a threshold.
         """
-        # TODO [Wombat]: allow user to specify a time interval to query over.
+        # TODO(RAT-1943): allow user to specify a time interval to query over.
         detection_api = DetectionApi(self._api_client)
         next_page_token = ""
         has_more = True
         all_events = []
         while has_more:
             kwargs: Dict[str, Any] = {}
             if len(next_page_token) > 0:
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/image_builder.py` & `rime_sdk-2.1.0rc4/rime_sdk/image_builder.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/internal/config_parser.py` & `rime_sdk-2.1.0rc4/rime_sdk/internal/config_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 
 from rime_sdk.swagger.swagger_client.models import (
     DataParamsFeatureIntersection,
     DataParamsRankingInfo,
     RegistryConnectionInfo,
     RegistryDataCollectorInfo,
     RegistryDataFileInfo,
+    RegistryDataInfo,
     RegistryDataLoadingInfo,
     RegistryDataParams,
     RegistryDeltaLakeInfo,
     RegistryHuggingFaceDataInfo,
     RegistryHuggingFaceModelInfo,
     RegistryModelInfo,
     RegistryModelPathInfo,
     RegistryPredictionParams,
     RegistryPredInfo,
     RimeUUID,
-    SchemaregistryDataInfo,
 )
 
 DEFAULT_DO_SAMPLING = True
 CONNECTION_INFO_TYPE_SWAGGER = Union[
     RegistryDataFileInfo,
     RegistryDataLoadingInfo,
     RegistryDataCollectorInfo,
@@ -290,15 +290,15 @@
     connection_swagger = process_connection_info_to_swagger(
         connection_info, config_type, _path
     )
     return connection_swagger, config_type
 
 
 @validate_types
-def convert_single_data_info_to_swagger(data_config: dict) -> SchemaregistryDataInfo:
+def convert_single_data_info_to_swagger(data_config: dict) -> RegistryDataInfo:
     """Convert a dictionary to a `DataInfo` Swagger message."""
     _config = deepcopy(data_config)
     if "connection_info" not in _config:
         raise ValueError(
             "Missing required key `connection_info` in data info config."
             f"\nGot: {list(_config)}"
         )
@@ -309,19 +309,19 @@
     )
     params_dict = _config.pop("data_params", {})
     data_params = convert_data_params_to_swagger(params_dict)
     if _config:
         raise ValueError(
             f"Found parameters in the data info config for {path} that do not"
             f" belong: {list(_config)}."
-            f" Expected parameters: {list(SchemaregistryDataInfo.swagger_types)}."
+            f" Expected parameters: {list(RegistryDataInfo.swagger_types)}."
         )
     connection_info = RegistryConnectionInfo()
     setattr(connection_info, field, connection_swagger)
-    return SchemaregistryDataInfo(
+    return RegistryDataInfo(
         data_params=data_params,
         connection_info=connection_info,
     )
 
 
 @validate_types
 def convert_model_info_to_swagger(model_config: dict) -> RegistryModelInfo:
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/internal/constants.py` & `rime_sdk-2.1.0rc4/rime_sdk/internal/constants.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/internal/decorators.py` & `rime_sdk-2.1.0rc4/rime_sdk/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/internal/file_upload.py` & `rime_sdk-2.1.0rc4/rime_sdk/internal/file_upload.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/internal/rest_error_handler.py` & `rime_sdk-2.1.0rc4/rime_sdk/internal/rest_error_handler.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/internal/security_config_parser.py` & `rime_sdk-2.1.0rc4/rime_sdk/internal/security_config_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/internal/swagger_parser.py` & `rime_sdk-2.1.0rc4/rime_sdk/internal/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/internal/swagger_utils.py` & `rime_sdk-2.1.0rc4/rime_sdk/internal/swagger_utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/internal/test_helpers.py` & `rime_sdk-2.1.0rc4/rime_sdk/internal/test_helpers.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/internal/throttle_queue.py` & `rime_sdk-2.1.0rc4/rime_sdk/internal/throttle_queue.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/internal/utils.py` & `rime_sdk-2.1.0rc4/rime_sdk/internal/utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/job.py` & `rime_sdk-2.1.0rc4/rime_sdk/job.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/monitor.py` & `rime_sdk-2.1.0rc4/rime_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/project.py` & `rime_sdk-2.1.0rc4/rime_sdk/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,37 +201,43 @@
         """
         api = swagger_client.ProjectServiceApi(self._api_client)
         with RESTErrorHandler():
             response = api.project_service_get_project(self._project_id)
             return response.project.project
 
     @deprecated
-    def foo_example_cross_plane_task(self) -> Optional[datetime]:
+    def foo_example_cross_plane_task(
+        self, should_fail: bool = False
+    ) -> Optional[datetime]:
         """Do the Foo toy example for the given project.
 
         This makes a CrossPlane call to the DataPlane and returns the current
         time on the agent side.
         This may fail at certain times :)
         """
         # TODO(RAT-1738): remove this method, only for internal testing.
         api = swagger_client.FooXPInterfaceApi(self._api_client)
         with RESTErrorHandler():
-            req = RimeStartFooTaskRequest(project_id=RimeUUID(self._project_id))
+            req = RimeStartFooTaskRequest(
+                project_id=RimeUUID(self._project_id), req={"should_fail": should_fail}
+            )
             res: RimeStartFooTaskResponse = api.foo_xp_interface_start_foo_task(req)
             job_id: str = res.job_id.uuid
             job = CrossPlaneTask(self._api_client, job_id)
-            status = job.get_status(
-                verbose=True, wait_until_finish=True, poll_rate_sec=1
+            job_res = job.get_status(
+                verbose=False, wait_until_finish=True, poll_rate_sec=1
             )
-
-            if status.get("status") == StatedbJobStatus.SUCCEEDED:
+            final_status = job_res.get("status")
+            if final_status == StatedbJobStatus.SUCCEEDED:
                 get_res: RimeGetFooTaskStatusResponse = (
                     api.foo_xp_interface_get_foo_task_status(job_id)
                 )
                 return get_res.res.receive_time
+            elif final_status == StatedbJobStatus.FAILED:
+                raise ValueError(f"Job failed: {job_res.get('error_msg')}")
 
             return None
 
     @property
     def info(self) -> ProjectInfo:
         """Return description, use case and ethical consideration of the Project."""
         project = self._get_project()
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/registry.py` & `rime_sdk-2.1.0rc4/rime_sdk/registry.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/__init__.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 # flake8: noqa
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
@@ -171,14 +171,15 @@
 from rime_sdk.swagger.swagger_client.models.rca_rca_result import RcaRCAResult
 from rime_sdk.swagger.swagger_client.models.rca_rca_role import RcaRCARole
 from rime_sdk.swagger.swagger_client.models.rca_test_case_cause import RcaTestCaseCause
 from rime_sdk.swagger.swagger_client.models.rca_test_case_id import RcaTestCaseID
 from rime_sdk.swagger.swagger_client.models.registry_connection_info import RegistryConnectionInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_collector_info import RegistryDataCollectorInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_file_info import RegistryDataFileInfo
+from rime_sdk.swagger.swagger_client.models.registry_data_info import RegistryDataInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_loading_info import RegistryDataLoadingInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_params import RegistryDataParams
 from rime_sdk.swagger.swagger_client.models.registry_delta_lake_info import RegistryDeltaLakeInfo
 from rime_sdk.swagger.swagger_client.models.registry_hugging_face_data_info import RegistryHuggingFaceDataInfo
 from rime_sdk.swagger.swagger_client.models.registry_hugging_face_model_info import RegistryHuggingFaceModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_metadata import RegistryMetadata
 from rime_sdk.swagger.swagger_client.models.registry_model_info import RegistryModelInfo
@@ -385,16 +386,14 @@
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_custom_image_type import RuntimeinfoCustomImageType
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_resource_request import RuntimeinfoResourceRequest
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_run_time_info import RuntimeinfoRunTimeInfo
 from rime_sdk.swagger.swagger_client.models.schemadatacollector_prediction import SchemadatacollectorPrediction
 from rime_sdk.swagger.swagger_client.models.schemaintegration_integration_variable import SchemaintegrationIntegrationVariable
 from rime_sdk.swagger.swagger_client.models.schemamonitor_config import SchemamonitorConfig
 from rime_sdk.swagger.swagger_client.models.schemanotification_config import SchemanotificationConfig
-from rime_sdk.swagger.swagger_client.models.schemaregistry_data_info import SchemaregistryDataInfo
-from rime_sdk.swagger.swagger_client.models.schematestrun_data_info import SchematestrunDataInfo
 from rime_sdk.swagger.swagger_client.models.security_event_details_flagged_datapoint import SecurityEventDetailsFlaggedDatapoint
 from rime_sdk.swagger.swagger_client.models.security_event_details_security_event_type import SecurityEventDetailsSecurityEventType
 from rime_sdk.swagger.swagger_client.models.statedb_archived_job_logs import StatedbArchivedJobLogs
 from rime_sdk.swagger.swagger_client.models.statedb_job_status import StatedbJobStatus
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_datapoints_response import StreamResultOfRimeGetDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_latest_logs_response import StreamResultOfRimeGetLatestLogsResponse
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_predictions_response import StreamResultOfRimeGetPredictionsResponse
@@ -405,14 +404,15 @@
 from rime_sdk.swagger.swagger_client.models.test_run_progress_test_batch_progress import TestRunProgressTestBatchProgress
 from rime_sdk.swagger.swagger_client.models.testrun_annotated_test_config import TestrunAnnotatedTestConfig
 from rime_sdk.swagger.swagger_client.models.testrun_custom_metric import TestrunCustomMetric
 from rime_sdk.swagger.swagger_client.models.testrun_data_profiling import TestrunDataProfiling
 from rime_sdk.swagger.swagger_client.models.testrun_generative_test_run_config import TestrunGenerativeTestRunConfig
 from rime_sdk.swagger.swagger_client.models.testrun_model_profiling import TestrunModelProfiling
 from rime_sdk.swagger.swagger_client.models.testrun_profiling_config import TestrunProfilingConfig
+from rime_sdk.swagger.swagger_client.models.testrun_ref_eval_datasets import TestrunRefEvalDatasets
 from rime_sdk.swagger.swagger_client.models.testrun_test_category_type import TestrunTestCategoryType
 from rime_sdk.swagger.swagger_client.models.testrun_test_run_config import TestrunTestRunConfig
 from rime_sdk.swagger.swagger_client.models.testrun_test_run_incremental_config import TestrunTestRunIncrementalConfig
 from rime_sdk.swagger.swagger_client.models.testrun_test_sensitivity import TestrunTestSensitivity
 from rime_sdk.swagger.swagger_client.models.testrun_test_suite_config import TestrunTestSuiteConfig
 from rime_sdk.swagger.swagger_client.models.testrunresult_get_batch_result_response import TestrunresultGetBatchResultResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_get_feature_result_response import TestrunresultGetFeatureResultResponse
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/__init__.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/agent_manager_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/agent_manager_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/config_validator_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/config_validator_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/data_collector_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/data_collector_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/detection_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/detection_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
@@ -31,15 +31,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def detection_list_detection_events(self, project_id_uuid, **kwargs):  # noqa: E501
         """ListDetectionEvents  # noqa: E501
 
-        List out events for a given project. Detection events represent problems RIME detects in different risk categories, such as performance degradation or security risk. This is a paginated method.  # noqa: E501
+        List out events for a given project. Detection events represent problems Robust Intelligence detects in different risk categories, such as performance degradation or security risk. This is a paginated method.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.detection_list_detection_events(project_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str project_id_uuid: Unique object ID. (required)
@@ -64,15 +64,15 @@
         else:
             (data) = self.detection_list_detection_events_with_http_info(project_id_uuid, **kwargs)  # noqa: E501
             return data
 
     def detection_list_detection_events_with_http_info(self, project_id_uuid, **kwargs):  # noqa: E501
         """ListDetectionEvents  # noqa: E501
 
-        List out events for a given project. Detection events represent problems RIME detects in different risk categories, such as performance degradation or security risk. This is a paginated method.  # noqa: E501
+        List out events for a given project. Detection events represent problems Robust Intelligence detects in different risk categories, such as performance degradation or security risk. This is a paginated method.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.detection_list_detection_events_with_http_info(project_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str project_id_uuid: Unique object ID. (required)
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/feature_flag_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/feature_flag_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/file_scanning_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/file_scanning_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/file_upload_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/file_upload_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/firewall_service_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/firewall_service_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
@@ -320,15 +320,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def firewall_service_get_url(self, firewall_id_uuid, **kwargs):  # noqa: E501
         """GetURL  # noqa: E501
 
-        Returns the URL for the specified Firewall in the RIME web application.  # noqa: E501
+        Returns the URL for the specified Firewall in the Robust Intelligence web application.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.firewall_service_get_url(firewall_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str firewall_id_uuid: Unique object ID. (required)
@@ -342,15 +342,15 @@
         else:
             (data) = self.firewall_service_get_url_with_http_info(firewall_id_uuid, **kwargs)  # noqa: E501
             return data
 
     def firewall_service_get_url_with_http_info(self, firewall_id_uuid, **kwargs):  # noqa: E501
         """GetURL  # noqa: E501
 
-        Returns the URL for the specified Firewall in the RIME web application.  # noqa: E501
+        Returns the URL for the specified Firewall in the Robust Intelligence web application.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.firewall_service_get_url_with_http_info(firewall_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str firewall_id_uuid: Unique object ID. (required)
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/foo_xp_interface_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/foo_xp_interface_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/image_registry_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/image_registry_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/integration_service_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/integration_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/job_reader_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/job_reader_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/model_card_service_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/model_card_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/model_testing_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/model_testing_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/monitor_service_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/monitor_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/notification_setting_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/notification_setting_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/project_service_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/project_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/registry_service_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/registry_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/results_reader_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/results_reader_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/rime_info_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/rime_info_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
@@ -31,15 +31,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def r_ime_info_get_rime_info(self, **kwargs):  # noqa: E501
         """GetRIMEInfo  # noqa: E501
 
-        Returns information about the RIME cluster you are querying.  # noqa: E501
+        Returns information about the Robust Intelligence cluster you are querying.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.r_ime_info_get_rime_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :return: RimeGetRIMEInfoResponse
@@ -52,15 +52,15 @@
         else:
             (data) = self.r_ime_info_get_rime_info_with_http_info(**kwargs)  # noqa: E501
             return data
 
     def r_ime_info_get_rime_info_with_http_info(self, **kwargs):  # noqa: E501
         """GetRIMEInfo  # noqa: E501
 
-        Returns information about the RIME cluster you are querying.  # noqa: E501
+        Returns information about the Robust Intelligence cluster you are querying.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.r_ime_info_get_rime_info_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :return: RimeGetRIMEInfoResponse
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/user_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/workspace_service_api.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api/workspace_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api_client.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/configuration.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/__init__.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 
 # flake8: noqa
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
@@ -144,14 +144,15 @@
 from rime_sdk.swagger.swagger_client.models.rca_rca_result import RcaRCAResult
 from rime_sdk.swagger.swagger_client.models.rca_rca_role import RcaRCARole
 from rime_sdk.swagger.swagger_client.models.rca_test_case_cause import RcaTestCaseCause
 from rime_sdk.swagger.swagger_client.models.rca_test_case_id import RcaTestCaseID
 from rime_sdk.swagger.swagger_client.models.registry_connection_info import RegistryConnectionInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_collector_info import RegistryDataCollectorInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_file_info import RegistryDataFileInfo
+from rime_sdk.swagger.swagger_client.models.registry_data_info import RegistryDataInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_loading_info import RegistryDataLoadingInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_params import RegistryDataParams
 from rime_sdk.swagger.swagger_client.models.registry_delta_lake_info import RegistryDeltaLakeInfo
 from rime_sdk.swagger.swagger_client.models.registry_hugging_face_data_info import RegistryHuggingFaceDataInfo
 from rime_sdk.swagger.swagger_client.models.registry_hugging_face_model_info import RegistryHuggingFaceModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_metadata import RegistryMetadata
 from rime_sdk.swagger.swagger_client.models.registry_model_info import RegistryModelInfo
@@ -358,16 +359,14 @@
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_custom_image_type import RuntimeinfoCustomImageType
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_resource_request import RuntimeinfoResourceRequest
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_run_time_info import RuntimeinfoRunTimeInfo
 from rime_sdk.swagger.swagger_client.models.schemadatacollector_prediction import SchemadatacollectorPrediction
 from rime_sdk.swagger.swagger_client.models.schemaintegration_integration_variable import SchemaintegrationIntegrationVariable
 from rime_sdk.swagger.swagger_client.models.schemamonitor_config import SchemamonitorConfig
 from rime_sdk.swagger.swagger_client.models.schemanotification_config import SchemanotificationConfig
-from rime_sdk.swagger.swagger_client.models.schemaregistry_data_info import SchemaregistryDataInfo
-from rime_sdk.swagger.swagger_client.models.schematestrun_data_info import SchematestrunDataInfo
 from rime_sdk.swagger.swagger_client.models.security_event_details_flagged_datapoint import SecurityEventDetailsFlaggedDatapoint
 from rime_sdk.swagger.swagger_client.models.security_event_details_security_event_type import SecurityEventDetailsSecurityEventType
 from rime_sdk.swagger.swagger_client.models.statedb_archived_job_logs import StatedbArchivedJobLogs
 from rime_sdk.swagger.swagger_client.models.statedb_job_status import StatedbJobStatus
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_datapoints_response import StreamResultOfRimeGetDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_latest_logs_response import StreamResultOfRimeGetLatestLogsResponse
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_predictions_response import StreamResultOfRimeGetPredictionsResponse
@@ -378,14 +377,15 @@
 from rime_sdk.swagger.swagger_client.models.test_run_progress_test_batch_progress import TestRunProgressTestBatchProgress
 from rime_sdk.swagger.swagger_client.models.testrun_annotated_test_config import TestrunAnnotatedTestConfig
 from rime_sdk.swagger.swagger_client.models.testrun_custom_metric import TestrunCustomMetric
 from rime_sdk.swagger.swagger_client.models.testrun_data_profiling import TestrunDataProfiling
 from rime_sdk.swagger.swagger_client.models.testrun_generative_test_run_config import TestrunGenerativeTestRunConfig
 from rime_sdk.swagger.swagger_client.models.testrun_model_profiling import TestrunModelProfiling
 from rime_sdk.swagger.swagger_client.models.testrun_profiling_config import TestrunProfilingConfig
+from rime_sdk.swagger.swagger_client.models.testrun_ref_eval_datasets import TestrunRefEvalDatasets
 from rime_sdk.swagger.swagger_client.models.testrun_test_category_type import TestrunTestCategoryType
 from rime_sdk.swagger.swagger_client.models.testrun_test_run_config import TestrunTestRunConfig
 from rime_sdk.swagger.swagger_client.models.testrun_test_run_incremental_config import TestrunTestRunIncrementalConfig
 from rime_sdk.swagger.swagger_client.models.testrun_test_sensitivity import TestrunTestSensitivity
 from rime_sdk.swagger.swagger_client.models.testrun_test_suite_config import TestrunTestSuiteConfig
 from rime_sdk.swagger.swagger_client.models.testrunresult_get_batch_result_response import TestrunresultGetBatchResultResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_get_feature_result_response import TestrunresultGetFeatureResultResponse
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
@@ -25,15 +25,15 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'eval_data_integration_id': 'RimeUUID',
-        'eval_data_info': 'SchemaregistryDataInfo',
+        'eval_data_info': 'RegistryDataInfo',
         'eval_pred_integration_id': 'RimeUUID',
         'eval_pred_info': 'RegistryPredInfo',
         'rolling_window': 'str'
     }
 
     attribute_map = {
         'eval_data_integration_id': 'evalDataIntegrationId',
@@ -85,25 +85,25 @@
 
     @property
     def eval_data_info(self):
         """Gets the eval_data_info of this CreateFirewallRequestScheduledCTParameters.  # noqa: E501
 
 
         :return: The eval_data_info of this CreateFirewallRequestScheduledCTParameters.  # noqa: E501
-        :rtype: SchemaregistryDataInfo
+        :rtype: RegistryDataInfo
         """
         return self._eval_data_info
 
     @eval_data_info.setter
     def eval_data_info(self, eval_data_info):
         """Sets the eval_data_info of this CreateFirewallRequestScheduledCTParameters.
 
 
         :param eval_data_info: The eval_data_info of this CreateFirewallRequestScheduledCTParameters.  # noqa: E501
-        :type: SchemaregistryDataInfo
+        :type: RegistryDataInfo
         """
 
         self._eval_data_info = eval_data_info
 
     @property
     def eval_pred_integration_id(self):
         """Gets the eval_pred_integration_id of this CreateFirewallRequestScheduledCTParameters.  # noqa: E501
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/dataset_dataset.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/dataset_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
@@ -31,15 +31,15 @@
         'name': 'str',
         'dataset_id': 'str',
         'project_ids': 'list[RimeUUID]',
         'creator_id': 'RimeUUID',
         'creation_time': 'datetime',
         'user_metadata': 'RegistryMetadata',
         'integration_id': 'RimeUUID',
-        'data_info': 'SchemaregistryDataInfo',
+        'data_info': 'RegistryDataInfo',
         'ct_info': 'DatasetCTInfo',
         'validity_status': 'RegistryValidityStatus',
         'marked_for_delete_at': 'datetime'
     }
 
     attribute_map = {
         'name': 'name',
@@ -245,25 +245,25 @@
 
     @property
     def data_info(self):
         """Gets the data_info of this DatasetDataset.  # noqa: E501
 
 
         :return: The data_info of this DatasetDataset.  # noqa: E501
-        :rtype: SchemaregistryDataInfo
+        :rtype: RegistryDataInfo
         """
         return self._data_info
 
     @data_info.setter
     def data_info(self, data_info):
         """Sets the data_info of this DatasetDataset.
 
 
         :param data_info: The data_info of this DatasetDataset.  # noqa: E501
-        :type: SchemaregistryDataInfo
+        :type: RegistryDataInfo
         """
 
         self._data_info = data_info
 
     @property
     def ct_info(self):
         """Gets the ct_info of this DatasetDataset.  # noqa: E501
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_detection_event.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/detection_detection_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_event_detail.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/detection_event_detail.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_event_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,44 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class DetectionEventType(object):
+class RimeDeletePredictionSetResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
-
-    """
-    allowed enum values
-    """
-    UNSPECIFIED = "EVENT_TYPE_UNSPECIFIED"
-    METRIC_DEGRADATION = "EVENT_TYPE_METRIC_DEGRADATION"
-    SECURITY = "EVENT_TYPE_SECURITY"
-    STRESS_TEST = "EVENT_TYPE_STRESS_TEST"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """DetectionEventType - a model defined in Swagger"""  # noqa: E501
+        """RimeDeletePredictionSetResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -62,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(DetectionEventType, dict):
+        if issubclass(RimeDeletePredictionSetResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, DetectionEventType):
+        if not isinstance(other, RimeDeletePredictionSetResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_resolution.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/detection_resolution.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/firewall_firewall.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/firewall_firewall.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
@@ -25,15 +25,15 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'eval_data_integration_id': 'RimeUUID',
-        'eval_data_info': 'SchemaregistryDataInfo',
+        'eval_data_info': 'RegistryDataInfo',
         'eval_pred_integration_id': 'RimeUUID',
         'eval_pred_info': 'RegistryPredInfo',
         'rolling_window': 'str',
         'last_ct_scheduled': 'datetime',
         'activated_time': 'datetime',
         'disable_scheduled_ct': 'bool'
     }
@@ -100,25 +100,25 @@
 
     @property
     def eval_data_info(self):
         """Gets the eval_data_info of this FirewallScheduledCTInfo.  # noqa: E501
 
 
         :return: The eval_data_info of this FirewallScheduledCTInfo.  # noqa: E501
-        :rtype: SchemaregistryDataInfo
+        :rtype: RegistryDataInfo
         """
         return self._eval_data_info
 
     @eval_data_info.setter
     def eval_data_info(self, eval_data_info):
         """Sets the eval_data_info of this FirewallScheduledCTInfo.
 
 
         :param eval_data_info: The eval_data_info of this FirewallScheduledCTInfo.  # noqa: E501
-        :type: SchemaregistryDataInfo
+        :type: RegistryDataInfo
         """
 
         self._eval_data_info = eval_data_info
 
     @property
     def eval_pred_integration_id(self):
         """Gets the eval_pred_integration_id of this FirewallScheduledCTInfo.  # noqa: E501
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/fooexample_foo_request.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/user_role.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class FooexampleFooRequest(object):
+class UserRole(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
+
+    """
+    allowed enum values
+    """
+    UNSPECIFIED = "ROLE_UNSPECIFIED"
+    ADMIN = "ROLE_ADMIN"
+    TRIAL_USER = "ROLE_TRIAL_USER"
+    SUPPORT = "ROLE_SUPPORT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """FooexampleFooRequest - a model defined in Swagger"""  # noqa: E501
+        """UserRole - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(FooexampleFooRequest, dict):
+        if issubclass(UserRole, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +78,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FooexampleFooRequest):
+        if not isinstance(other, UserRole):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/fooexample_foo_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/fooexample_foo_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/googlerpc_status.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/googlerpc_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/integration_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_level.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/integration_integration_level.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/integration_integration_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/model_model.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/model_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_token_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,51 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class MonitorAggregationType(object):
+class RimeTokenType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "AGGREGATION_TYPE_UNSPECIFIED"
-    AVG = "AGGREGATION_TYPE_AVG"
-    MIN = "AGGREGATION_TYPE_MIN"
-    MAX = "AGGREGATION_TYPE_MAX"
-    SUM = "AGGREGATION_TYPE_SUM"
+    UNSPECIFIED = "TOKEN_TYPE_UNSPECIFIED"
+    USER = "TOKEN_TYPE_USER"
+    AGENT = "TOKEN_TYPE_AGENT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """MonitorAggregationType - a model defined in Swagger"""  # noqa: E501
+        """RimeTokenType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -63,15 +61,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(MonitorAggregationType, dict):
+        if issubclass(RimeTokenType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -79,15 +77,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MonitorAggregationType):
+        if not isinstance(other, RimeTokenType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_monitor.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_threshold.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_threshold.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/notification_object_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class MonitorThresholdType(object):
+class NotificationObjectType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "TYPE_UNSPECIFIED"
-    UPPER_BOUND = "TYPE_UPPER_BOUND"
-    LOWER_BOUND = "TYPE_LOWER_BOUND"
+    UNSPECIFIED = "OBJECT_TYPE_UNSPECIFIED"
+    PROJECT = "OBJECT_TYPE_PROJECT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """MonitorThresholdType - a model defined in Swagger"""  # noqa: E501
+        """NotificationObjectType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -61,15 +60,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(MonitorThresholdType, dict):
+        if issubclass(NotificationObjectType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -77,15 +76,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MonitorThresholdType):
+        if not isinstance(other, NotificationObjectType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_transform.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_digest_config.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/notification_digest_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class NotificationJobActionConfig(object):
+class ProtobufNullValue(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
+
+    """
+    allowed enum values
+    """
+    NULL_VALUE = "NULL_VALUE"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """NotificationJobActionConfig - a model defined in Swagger"""  # noqa: E501
+        """ProtobufNullValue - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +59,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(NotificationJobActionConfig, dict):
+        if issubclass(ProtobufNullValue, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +75,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, NotificationJobActionConfig):
+        if not isinstance(other, ProtobufNullValue):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_notification.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/notification_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_notification_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_view.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class NotificationNotificationType(object):
+class RimeJobView(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "NOTIFICATION_TYPE_UNSPECIFIED"
-    DIGEST = "NOTIFICATION_TYPE_DIGEST"
-    JOB_ACTION = "NOTIFICATION_TYPE_JOB_ACTION"
-    MONITORING = "NOTIFICATION_TYPE_MONITORING"
+    UNSPECIFIED = "JOB_VIEW_UNSPECIFIED"
+    BASIC = "JOB_VIEW_BASIC"
+    FULL = "JOB_VIEW_FULL"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """NotificationNotificationType - a model defined in Swagger"""  # noqa: E501
+        """RimeJobView - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -62,15 +61,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(NotificationNotificationType, dict):
+        if issubclass(RimeJobView, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,15 +77,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, NotificationNotificationType):
+        if not isinstance(other, RimeJobView):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_object_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,44 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class NotificationObjectType(object):
+class RimeUpdateBuildInfoResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
-
-    """
-    allowed enum values
-    """
-    UNSPECIFIED = "OBJECT_TYPE_UNSPECIFIED"
-    PROJECT = "OBJECT_TYPE_PROJECT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """NotificationObjectType - a model defined in Swagger"""  # noqa: E501
+        """RimeUpdateBuildInfoResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -60,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(NotificationObjectType, dict):
+        if issubclass(RimeUpdateBuildInfoResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -76,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, NotificationObjectType):
+        if not isinstance(other, RimeUpdateBuildInfoResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_create_project_request.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_create_project_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_create_project_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_create_project_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_get_project_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_get_project_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
@@ -28,15 +28,15 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'project_id': 'object',
         'name': 'str',
         'metadata': 'RegistryMetadata',
         'integration_id': 'RimeUUID',
-        'data_info': 'SchemaregistryDataInfo',
+        'data_info': 'RegistryDataInfo',
         'ct_info': 'DatasetCTInfo'
     }
 
     attribute_map = {
         'project_id': 'projectId',
         'name': 'name',
         'metadata': 'metadata',
@@ -158,25 +158,25 @@
 
     @property
     def data_info(self):
         """Gets the data_info of this ProjectIdUuidDatasetBody.  # noqa: E501
 
 
         :return: The data_info of this ProjectIdUuidDatasetBody.  # noqa: E501
-        :rtype: SchemaregistryDataInfo
+        :rtype: RegistryDataInfo
         """
         return self._data_info
 
     @data_info.setter
     def data_info(self, data_info):
         """Sets the data_info of this ProjectIdUuidDatasetBody.
 
 
         :param data_info: The data_info of this ProjectIdUuidDatasetBody.  # noqa: E501
-        :type: SchemaregistryDataInfo
+        :type: RegistryDataInfo
         """
 
         self._data_info = data_info
 
     @property
     def ct_info(self):
         """Gets the ct_info of this ProjectIdUuidDatasetBody.  # noqa: E501
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_owner_details.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_owner_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_project.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_project_with_details.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_project_with_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_update_project_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_update_project_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ProjectUpdateUserOfProjectResponse(object):
+class RimeUpdateUserOfWorkspaceResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """ProjectUpdateUserOfProjectResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeUpdateUserOfWorkspaceResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ProjectUpdateUserOfProjectResponse, dict):
+        if issubclass(RimeUpdateUserOfWorkspaceResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ProjectUpdateUserOfProjectResponse):
+        if not isinstance(other, RimeUpdateUserOfWorkspaceResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/protobuf_any.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/protobuf_any.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ProtobufNullValue(object):
+class RimeValidateTestConfigResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
-
-    """
-    allowed enum values
-    """
-    NULL_VALUE = "NULL_VALUE"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """ProtobufNullValue - a model defined in Swagger"""  # noqa: E501
+        """RimeValidateTestConfigResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -59,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ProtobufNullValue, dict):
+        if issubclass(RimeValidateTestConfigResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -75,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ProtobufNullValue):
+        if not isinstance(other, RimeValidateTestConfigResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rca_rca_result.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rca_rca_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rca_rca_role.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rca_rca_role.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_connection_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_connection_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_params.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_params.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
@@ -36,18 +36,20 @@
         'nrows_per_time_bin': 'str',
         'sample': 'bool',
         'categorical_features': 'list[str]',
         'protected_features': 'list[str]',
         'features_not_in_model': 'list[str]',
         'text_features': 'list[str]',
         'image_features': 'list[str]',
+        'prompt_col': 'str',
         'intersections': 'list[DataParamsFeatureIntersection]',
         'loading_kwargs': 'str',
         'feature_type_path': 'str',
-        'image_load_path': 'str'
+        'image_load_path': 'str',
+        'experimental_fields': 'dict(str, object)'
     }
 
     attribute_map = {
         'label_col': 'labelCol',
         'timestamp_col': 'timestampCol',
         'class_names': 'classNames',
         'ranking_info': 'rankingInfo',
@@ -55,38 +57,42 @@
         'nrows_per_time_bin': 'nrowsPerTimeBin',
         'sample': 'sample',
         'categorical_features': 'categoricalFeatures',
         'protected_features': 'protectedFeatures',
         'features_not_in_model': 'featuresNotInModel',
         'text_features': 'textFeatures',
         'image_features': 'imageFeatures',
+        'prompt_col': 'promptCol',
         'intersections': 'intersections',
         'loading_kwargs': 'loadingKwargs',
         'feature_type_path': 'featureTypePath',
-        'image_load_path': 'imageLoadPath'
+        'image_load_path': 'imageLoadPath',
+        'experimental_fields': 'experimentalFields'
     }
 
-    def __init__(self, label_col=None, timestamp_col=None, class_names=None, ranking_info=None, nrows=None, nrows_per_time_bin=None, sample=None, categorical_features=None, protected_features=None, features_not_in_model=None, text_features=None, image_features=None, intersections=None, loading_kwargs=None, feature_type_path=None, image_load_path=None):  # noqa: E501
+    def __init__(self, label_col=None, timestamp_col=None, class_names=None, ranking_info=None, nrows=None, nrows_per_time_bin=None, sample=None, categorical_features=None, protected_features=None, features_not_in_model=None, text_features=None, image_features=None, prompt_col=None, intersections=None, loading_kwargs=None, feature_type_path=None, image_load_path=None, experimental_fields=None):  # noqa: E501
         """RegistryDataParams - a model defined in Swagger"""  # noqa: E501
         self._label_col = None
         self._timestamp_col = None
         self._class_names = None
         self._ranking_info = None
         self._nrows = None
         self._nrows_per_time_bin = None
         self._sample = None
         self._categorical_features = None
         self._protected_features = None
         self._features_not_in_model = None
         self._text_features = None
         self._image_features = None
+        self._prompt_col = None
         self._intersections = None
         self._loading_kwargs = None
         self._feature_type_path = None
         self._image_load_path = None
+        self._experimental_fields = None
         self.discriminator = None
         if label_col is not None:
             self.label_col = label_col
         if timestamp_col is not None:
             self.timestamp_col = timestamp_col
         if class_names is not None:
             self.class_names = class_names
@@ -104,22 +110,26 @@
             self.protected_features = protected_features
         if features_not_in_model is not None:
             self.features_not_in_model = features_not_in_model
         if text_features is not None:
             self.text_features = text_features
         if image_features is not None:
             self.image_features = image_features
+        if prompt_col is not None:
+            self.prompt_col = prompt_col
         if intersections is not None:
             self.intersections = intersections
         if loading_kwargs is not None:
             self.loading_kwargs = loading_kwargs
         if feature_type_path is not None:
             self.feature_type_path = feature_type_path
         if image_load_path is not None:
             self.image_load_path = image_load_path
+        if experimental_fields is not None:
+            self.experimental_fields = experimental_fields
 
     @property
     def label_col(self):
         """Gets the label_col of this RegistryDataParams.  # noqa: E501
 
         Naming of special columns.  # noqa: E501
 
@@ -386,14 +396,37 @@
         :param image_features: The image_features of this RegistryDataParams.  # noqa: E501
         :type: list[str]
         """
 
         self._image_features = image_features
 
     @property
+    def prompt_col(self):
+        """Gets the prompt_col of this RegistryDataParams.  # noqa: E501
+
+        Prompt template column for Generative tasks.  # noqa: E501
+
+        :return: The prompt_col of this RegistryDataParams.  # noqa: E501
+        :rtype: str
+        """
+        return self._prompt_col
+
+    @prompt_col.setter
+    def prompt_col(self, prompt_col):
+        """Sets the prompt_col of this RegistryDataParams.
+
+        Prompt template column for Generative tasks.  # noqa: E501
+
+        :param prompt_col: The prompt_col of this RegistryDataParams.  # noqa: E501
+        :type: str
+        """
+
+        self._prompt_col = prompt_col
+
+    @property
     def intersections(self):
         """Gets the intersections of this RegistryDataParams.  # noqa: E501
 
         A list of arrays of features. Each array represents the intersection of features on which certain subset and fairness tests are run.  # noqa: E501
 
         :return: The intersections of this RegistryDataParams.  # noqa: E501
         :rtype: list[DataParamsFeatureIntersection]
@@ -477,14 +510,37 @@
 
         :param image_load_path: The image_load_path of this RegistryDataParams.  # noqa: E501
         :type: str
         """
 
         self._image_load_path = image_load_path
 
+    @property
+    def experimental_fields(self):
+        """Gets the experimental_fields of this RegistryDataParams.  # noqa: E501
+
+        Fields that enable experimental functionality.  WARNING: these fields are experimental; ie, their functionality may not be reliable or backwards-compatible. Do not use these fields in production.  # noqa: E501
+
+        :return: The experimental_fields of this RegistryDataParams.  # noqa: E501
+        :rtype: dict(str, object)
+        """
+        return self._experimental_fields
+
+    @experimental_fields.setter
+    def experimental_fields(self, experimental_fields):
+        """Sets the experimental_fields of this RegistryDataParams.
+
+        Fields that enable experimental functionality.  WARNING: these fields are experimental; ie, their functionality may not be reliable or backwards-compatible. Do not use these fields in production.  # noqa: E501
+
+        :param experimental_fields: The experimental_fields of this RegistryDataParams.  # noqa: E501
+        :type: dict(str, object)
+        """
+
+        self._experimental_fields = experimental_fields
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_delta_lake_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_delta_lake_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_metadata.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_model_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_model_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_pred_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_pred_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,123 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RegistryPredictionParams(object):
+class RimeListAPITokensResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'pred_col': 'str',
-        'timestamp_col': 'str'
+        'api_token_infos': 'list[RimeAPITokenInfo]',
+        'next_page_token': 'str',
+        'has_more': 'bool'
     }
 
     attribute_map = {
-        'pred_col': 'predCol',
-        'timestamp_col': 'timestampCol'
+        'api_token_infos': 'apiTokenInfos',
+        'next_page_token': 'nextPageToken',
+        'has_more': 'hasMore'
     }
 
-    def __init__(self, pred_col=None, timestamp_col=None):  # noqa: E501
-        """RegistryPredictionParams - a model defined in Swagger"""  # noqa: E501
-        self._pred_col = None
-        self._timestamp_col = None
+    def __init__(self, api_token_infos=None, next_page_token=None, has_more=None):  # noqa: E501
+        """RimeListAPITokensResponse - a model defined in Swagger"""  # noqa: E501
+        self._api_token_infos = None
+        self._next_page_token = None
+        self._has_more = None
         self.discriminator = None
-        if pred_col is not None:
-            self.pred_col = pred_col
-        if timestamp_col is not None:
-            self.timestamp_col = timestamp_col
+        if api_token_infos is not None:
+            self.api_token_infos = api_token_infos
+        if next_page_token is not None:
+            self.next_page_token = next_page_token
+        if has_more is not None:
+            self.has_more = has_more
 
     @property
-    def pred_col(self):
-        """Gets the pred_col of this RegistryPredictionParams.  # noqa: E501
+    def api_token_infos(self):
+        """Gets the api_token_infos of this RimeListAPITokensResponse.  # noqa: E501
 
-        Column used for predictions.  # noqa: E501
 
-        :return: The pred_col of this RegistryPredictionParams.  # noqa: E501
-        :rtype: str
+        :return: The api_token_infos of this RimeListAPITokensResponse.  # noqa: E501
+        :rtype: list[RimeAPITokenInfo]
         """
-        return self._pred_col
+        return self._api_token_infos
 
-    @pred_col.setter
-    def pred_col(self, pred_col):
-        """Sets the pred_col of this RegistryPredictionParams.
+    @api_token_infos.setter
+    def api_token_infos(self, api_token_infos):
+        """Sets the api_token_infos of this RimeListAPITokensResponse.
 
-        Column used for predictions.  # noqa: E501
 
-        :param pred_col: The pred_col of this RegistryPredictionParams.  # noqa: E501
-        :type: str
+        :param api_token_infos: The api_token_infos of this RimeListAPITokensResponse.  # noqa: E501
+        :type: list[RimeAPITokenInfo]
         """
 
-        self._pred_col = pred_col
+        self._api_token_infos = api_token_infos
 
     @property
-    def timestamp_col(self):
-        """Gets the timestamp_col of this RegistryPredictionParams.  # noqa: E501
+    def next_page_token(self):
+        """Gets the next_page_token of this RimeListAPITokensResponse.  # noqa: E501
 
-        Column used for CT timestamp.  # noqa: E501
 
-        :return: The timestamp_col of this RegistryPredictionParams.  # noqa: E501
+        :return: The next_page_token of this RimeListAPITokensResponse.  # noqa: E501
         :rtype: str
         """
-        return self._timestamp_col
+        return self._next_page_token
 
-    @timestamp_col.setter
-    def timestamp_col(self, timestamp_col):
-        """Sets the timestamp_col of this RegistryPredictionParams.
+    @next_page_token.setter
+    def next_page_token(self, next_page_token):
+        """Sets the next_page_token of this RimeListAPITokensResponse.
 
-        Column used for CT timestamp.  # noqa: E501
 
-        :param timestamp_col: The timestamp_col of this RegistryPredictionParams.  # noqa: E501
+        :param next_page_token: The next_page_token of this RimeListAPITokensResponse.  # noqa: E501
         :type: str
         """
 
-        self._timestamp_col = timestamp_col
+        self._next_page_token = next_page_token
+
+    @property
+    def has_more(self):
+        """Gets the has_more of this RimeListAPITokensResponse.  # noqa: E501
+
+
+        :return: The has_more of this RimeListAPITokensResponse.  # noqa: E501
+        :rtype: bool
+        """
+        return self._has_more
+
+    @has_more.setter
+    def has_more(self, has_more):
+        """Sets the has_more of this RimeListAPITokensResponse.
+
+
+        :param has_more: The has_more of this RimeListAPITokensResponse.  # noqa: E501
+        :type: bool
+        """
+
+        self._has_more = has_more
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -110,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RegistryPredictionParams, dict):
+        if issubclass(RimeListAPITokensResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -126,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RegistryPredictionParams):
+        if not isinstance(other, RimeListAPITokensResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_validity_status.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_validity_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_actor_role.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_actor_role.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_agent.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_agent_status.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_agent_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
@@ -121,26 +121,26 @@
 
         self._name = name
 
     @property
     def suffix(self):
         """Gets the suffix of this RimeAPITokenInfo.  # noqa: E501
 
-        The suffix of the API token, which is visible in the RIME UI.  # noqa: E501
+        The suffix of the API token, which is visible in the Robust Intelligence web application.  # noqa: E501
 
         :return: The suffix of this RimeAPITokenInfo.  # noqa: E501
         :rtype: str
         """
         return self._suffix
 
     @suffix.setter
     def suffix(self, suffix):
         """Sets the suffix of this RimeAPITokenInfo.
 
-        The suffix of the API token, which is visible in the RIME UI.  # noqa: E501
+        The suffix of the API token, which is visible in the Robust Intelligence web application.  # noqa: E501
 
         :param suffix: The suffix of this RimeAPITokenInfo.  # noqa: E501
         :type: str
         """
 
         self._suffix = suffix
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeCancelJobResponse(object):
+class RimeDeleteImageResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeCancelJobResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeDeleteImageResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeCancelJobResponse, dict):
+        if issubclass(RimeDeleteImageResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeCancelJobResponse):
+        if not isinstance(other, RimeDeleteImageResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_category_metric.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_category_metric.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_config_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,53 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeConfigType(object):
+class RimeTableColumnType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "CONFIG_TYPE_UNSPECIFIED"
-    TEST_RUN = "CONFIG_TYPE_TEST_RUN"
-    TEST_SUITE = "CONFIG_TYPE_TEST_SUITE"
-    TEST_RUN_INCREMENTAL = "CONFIG_TYPE_TEST_RUN_INCREMENTAL"
-    PROFILING = "CONFIG_TYPE_PROFILING"
-    DATA_PROFILING = "CONFIG_TYPE_DATA_PROFILING"
-    MODEL_PROFILING = "CONFIG_TYPE_MODEL_PROFILING"
+    UNSPECIFIED = "TABLE_COLUMN_TYPE_UNSPECIFIED"
+    STRING = "TABLE_COLUMN_TYPE_STRING"
+    NUMERICAL = "TABLE_COLUMN_TYPE_NUMERICAL"
+    DATE = "TABLE_COLUMN_TYPE_DATE"
+    PICKABLE = "TABLE_COLUMN_TYPE_PICKABLE"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeConfigType - a model defined in Swagger"""  # noqa: E501
+        """RimeTableColumnType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -65,15 +63,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeConfigType, dict):
+        if issubclass(RimeTableColumnType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -81,15 +79,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeConfigType):
+        if not isinstance(other, RimeTableColumnType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeConfigureIntegrationResponse(object):
+class RimeGetIntegrationResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,36 +32,36 @@
     }
 
     attribute_map = {
         'integration_info': 'integrationInfo'
     }
 
     def __init__(self, integration_info=None):  # noqa: E501
-        """RimeConfigureIntegrationResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeGetIntegrationResponse - a model defined in Swagger"""  # noqa: E501
         self._integration_info = None
         self.discriminator = None
         if integration_info is not None:
             self.integration_info = integration_info
 
     @property
     def integration_info(self):
-        """Gets the integration_info of this RimeConfigureIntegrationResponse.  # noqa: E501
+        """Gets the integration_info of this RimeGetIntegrationResponse.  # noqa: E501
 
 
-        :return: The integration_info of this RimeConfigureIntegrationResponse.  # noqa: E501
+        :return: The integration_info of this RimeGetIntegrationResponse.  # noqa: E501
         :rtype: RimeIntegrationInfo
         """
         return self._integration_info
 
     @integration_info.setter
     def integration_info(self, integration_info):
-        """Sets the integration_info of this RimeConfigureIntegrationResponse.
+        """Sets the integration_info of this RimeGetIntegrationResponse.
 
 
-        :param integration_info: The integration_info of this RimeConfigureIntegrationResponse.  # noqa: E501
+        :param integration_info: The integration_info of this RimeGetIntegrationResponse.  # noqa: E501
         :type: RimeIntegrationInfo
         """
 
         self._integration_info = integration_info
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeConfigureIntegrationResponse, dict):
+        if issubclass(RimeGetIntegrationResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeConfigureIntegrationResponse):
+        if not isinstance(other, RimeGetIntegrationResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeCreateIntegrationRequest(object):
+class RimeCreateIntegrationResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'integration': 'IntegrationIntegration'
+        'integration_info': 'RimeIntegrationInfo'
     }
 
     attribute_map = {
-        'integration': 'integration'
+        'integration_info': 'integrationInfo'
     }
 
-    def __init__(self, integration=None):  # noqa: E501
-        """RimeCreateIntegrationRequest - a model defined in Swagger"""  # noqa: E501
-        self._integration = None
+    def __init__(self, integration_info=None):  # noqa: E501
+        """RimeCreateIntegrationResponse - a model defined in Swagger"""  # noqa: E501
+        self._integration_info = None
         self.discriminator = None
-        if integration is not None:
-            self.integration = integration
+        if integration_info is not None:
+            self.integration_info = integration_info
 
     @property
-    def integration(self):
-        """Gets the integration of this RimeCreateIntegrationRequest.  # noqa: E501
+    def integration_info(self):
+        """Gets the integration_info of this RimeCreateIntegrationResponse.  # noqa: E501
 
 
-        :return: The integration of this RimeCreateIntegrationRequest.  # noqa: E501
-        :rtype: IntegrationIntegration
+        :return: The integration_info of this RimeCreateIntegrationResponse.  # noqa: E501
+        :rtype: RimeIntegrationInfo
         """
-        return self._integration
+        return self._integration_info
 
-    @integration.setter
-    def integration(self, integration):
-        """Sets the integration of this RimeCreateIntegrationRequest.
+    @integration_info.setter
+    def integration_info(self, integration_info):
+        """Sets the integration_info of this RimeCreateIntegrationResponse.
 
 
-        :param integration: The integration of this RimeCreateIntegrationRequest.  # noqa: E501
-        :type: IntegrationIntegration
+        :param integration_info: The integration_info of this RimeCreateIntegrationResponse.  # noqa: E501
+        :type: RimeIntegrationInfo
         """
 
-        self._integration = integration
+        self._integration_info = integration_info
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeCreateIntegrationRequest, dict):
+        if issubclass(RimeCreateIntegrationResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeCreateIntegrationRequest):
+        if not isinstance(other, RimeCreateIntegrationResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeCreateIntegrationResponse(object):
+class RimeUpdateIntegrationResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,36 +32,36 @@
     }
 
     attribute_map = {
         'integration_info': 'integrationInfo'
     }
 
     def __init__(self, integration_info=None):  # noqa: E501
-        """RimeCreateIntegrationResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeUpdateIntegrationResponse - a model defined in Swagger"""  # noqa: E501
         self._integration_info = None
         self.discriminator = None
         if integration_info is not None:
             self.integration_info = integration_info
 
     @property
     def integration_info(self):
-        """Gets the integration_info of this RimeCreateIntegrationResponse.  # noqa: E501
+        """Gets the integration_info of this RimeUpdateIntegrationResponse.  # noqa: E501
 
 
-        :return: The integration_info of this RimeCreateIntegrationResponse.  # noqa: E501
+        :return: The integration_info of this RimeUpdateIntegrationResponse.  # noqa: E501
         :rtype: RimeIntegrationInfo
         """
         return self._integration_info
 
     @integration_info.setter
     def integration_info(self, integration_info):
-        """Sets the integration_info of this RimeCreateIntegrationResponse.
+        """Sets the integration_info of this RimeUpdateIntegrationResponse.
 
 
-        :param integration_info: The integration_info of this RimeCreateIntegrationResponse.  # noqa: E501
+        :param integration_info: The integration_info of this RimeUpdateIntegrationResponse.  # noqa: E501
         :type: RimeIntegrationInfo
         """
 
         self._integration_info = integration_info
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeCreateIntegrationResponse, dict):
+        if issubclass(RimeUpdateIntegrationResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeCreateIntegrationResponse):
+        if not isinstance(other, RimeUpdateIntegrationResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_language.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeDeactivateAgentResponse(object):
+class RimeLanguage(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
+
+    """
+    allowed enum values
+    """
+    UNSPECIFIED = "LANGUAGE_UNSPECIFIED"
+    EN = "LANGUAGE_EN"
+    JA = "LANGUAGE_JA"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeDeactivateAgentResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeLanguage - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +61,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeDeactivateAgentResponse, dict):
+        if issubclass(RimeLanguage, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +77,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeDeactivateAgentResponse):
+        if not isinstance(other, RimeLanguage):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeDeleteCustomMonitorResponse(object):
+class RimeDeleteUploadedFileURLResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeDeleteCustomMonitorResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeDeleteUploadedFileURLResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeDeleteCustomMonitorResponse, dict):
+        if issubclass(RimeDeleteUploadedFileURLResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeDeleteCustomMonitorResponse):
+        if not isinstance(other, RimeDeleteUploadedFileURLResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeDeleteFirewallResponse(object):
+class RimeDeleteWorkspaceTagResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeDeleteFirewallResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeDeleteWorkspaceTagResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeDeleteFirewallResponse, dict):
+        if issubclass(RimeDeleteWorkspaceTagResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeDeleteFirewallResponse):
+        if not isinstance(other, RimeDeleteWorkspaceTagResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeDeleteImageResponse(object):
+class RimeEnsureImageExistenceResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeDeleteImageResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeEnsureImageExistenceResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeDeleteImageResponse, dict):
+        if issubclass(RimeEnsureImageExistenceResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeDeleteImageResponse):
+        if not isinstance(other, RimeEnsureImageExistenceResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeDeleteIntegrationResponse(object):
+class RimeSendRIEmailResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeDeleteIntegrationResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeSendRIEmailResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeDeleteIntegrationResponse, dict):
+        if issubclass(RimeSendRIEmailResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeDeleteIntegrationResponse):
+        if not isinstance(other, RimeSendRIEmailResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeDeleteModelResponse(object):
+class RimeCancelJobResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeDeleteModelResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeCancelJobResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeDeleteModelResponse, dict):
+        if issubclass(RimeCancelJobResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeDeleteModelResponse):
+        if not isinstance(other, RimeCancelJobResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeDeletePredictionSetResponse(object):
+class RimeUpdateUserResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeDeletePredictionSetResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeUpdateUserResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeDeletePredictionSetResponse, dict):
+        if issubclass(RimeUpdateUserResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeDeletePredictionSetResponse):
+        if not isinstance(other, RimeUpdateUserResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeDeleteUploadedFileURLResponse(object):
+class RimeListWorkspacesRequestQuery(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeDeleteUploadedFileURLResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeListWorkspacesRequestQuery - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeDeleteUploadedFileURLResponse, dict):
+        if issubclass(RimeListWorkspacesRequestQuery, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeDeleteUploadedFileURLResponse):
+        if not isinstance(other, RimeListWorkspacesRequestQuery):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeDeleteWorkspaceTagResponse(object):
+class RimeUpdateWorkspaceResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeDeleteWorkspaceTagResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeUpdateWorkspaceResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeDeleteWorkspaceTagResponse, dict):
+        if issubclass(RimeUpdateWorkspaceResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeDeleteWorkspaceTagResponse):
+        if not isinstance(other, RimeUpdateWorkspaceResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeEnsureImageExistenceResponse(object):
+class RimeHeartbeatResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeEnsureImageExistenceResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeHeartbeatResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeEnsureImageExistenceResponse, dict):
+        if issubclass(RimeHeartbeatResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeEnsureImageExistenceResponse):
+        if not isinstance(other, RimeHeartbeatResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_failing_row.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_failing_row.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_feature_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_feature_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_float_list.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_float_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_foo_task_status_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_foo_task_status_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,45 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeGetImageResponse(object):
+class RimeUpdateWorkspaceTagResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'image': 'RimeManagedImage'
     }
 
     attribute_map = {
-        'image': 'image'
     }
 
-    def __init__(self, image=None):  # noqa: E501
-        """RimeGetImageResponse - a model defined in Swagger"""  # noqa: E501
-        self._image = None
+    def __init__(self):  # noqa: E501
+        """RimeUpdateWorkspaceTagResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
-        if image is not None:
-            self.image = image
-
-    @property
-    def image(self):
-        """Gets the image of this RimeGetImageResponse.  # noqa: E501
-
-
-        :return: The image of this RimeGetImageResponse.  # noqa: E501
-        :rtype: RimeManagedImage
-        """
-        return self._image
-
-    @image.setter
-    def image(self, image):
-        """Sets the image of this RimeGetImageResponse.
-
-
-        :param image: The image of this RimeGetImageResponse.  # noqa: E501
-        :type: RimeManagedImage
-        """
-
-        self._image = image
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeGetImageResponse, dict):
+        if issubclass(RimeUpdateWorkspaceTagResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeGetImageResponse):
+        if not isinstance(other, RimeUpdateWorkspaceTagResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeGetIntegrationResponse(object):
+class RimeConfigureIntegrationResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,36 +32,36 @@
     }
 
     attribute_map = {
         'integration_info': 'integrationInfo'
     }
 
     def __init__(self, integration_info=None):  # noqa: E501
-        """RimeGetIntegrationResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeConfigureIntegrationResponse - a model defined in Swagger"""  # noqa: E501
         self._integration_info = None
         self.discriminator = None
         if integration_info is not None:
             self.integration_info = integration_info
 
     @property
     def integration_info(self):
-        """Gets the integration_info of this RimeGetIntegrationResponse.  # noqa: E501
+        """Gets the integration_info of this RimeConfigureIntegrationResponse.  # noqa: E501
 
 
-        :return: The integration_info of this RimeGetIntegrationResponse.  # noqa: E501
+        :return: The integration_info of this RimeConfigureIntegrationResponse.  # noqa: E501
         :rtype: RimeIntegrationInfo
         """
         return self._integration_info
 
     @integration_info.setter
     def integration_info(self, integration_info):
-        """Sets the integration_info of this RimeGetIntegrationResponse.
+        """Sets the integration_info of this RimeConfigureIntegrationResponse.
 
 
-        :param integration_info: The integration_info of this RimeGetIntegrationResponse.  # noqa: E501
+        :param integration_info: The integration_info of this RimeConfigureIntegrationResponse.  # noqa: E501
         :type: RimeIntegrationInfo
         """
 
         self._integration_info = integration_info
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeGetIntegrationResponse, dict):
+        if issubclass(RimeConfigureIntegrationResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeGetIntegrationResponse):
+        if not isinstance(other, RimeConfigureIntegrationResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeGetModelCardResponse(object):
+class RimeUpdateModelCardResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,36 +32,36 @@
     }
 
     attribute_map = {
         'model_card': 'modelCard'
     }
 
     def __init__(self, model_card=None):  # noqa: E501
-        """RimeGetModelCardResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeUpdateModelCardResponse - a model defined in Swagger"""  # noqa: E501
         self._model_card = None
         self.discriminator = None
         if model_card is not None:
             self.model_card = model_card
 
     @property
     def model_card(self):
-        """Gets the model_card of this RimeGetModelCardResponse.  # noqa: E501
+        """Gets the model_card of this RimeUpdateModelCardResponse.  # noqa: E501
 
 
-        :return: The model_card of this RimeGetModelCardResponse.  # noqa: E501
+        :return: The model_card of this RimeUpdateModelCardResponse.  # noqa: E501
         :rtype: RimeModelCard
         """
         return self._model_card
 
     @model_card.setter
     def model_card(self, model_card):
-        """Sets the model_card of this RimeGetModelCardResponse.
+        """Sets the model_card of this RimeUpdateModelCardResponse.
 
 
-        :param model_card: The model_card of this RimeGetModelCardResponse.  # noqa: E501
+        :param model_card: The model_card of this RimeUpdateModelCardResponse.  # noqa: E501
         :type: RimeModelCard
         """
 
         self._model_card = model_card
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeGetModelCardResponse, dict):
+        if issubclass(RimeUpdateModelCardResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeGetModelCardResponse):
+        if not isinstance(other, RimeUpdateModelCardResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
@@ -67,26 +67,26 @@
         if build_version is not None:
             self.build_version = build_version
 
     @property
     def cluster_info_version(self):
         """Gets the cluster_info_version of this RimeGetRIMEInfoResponse.  # noqa: E501
 
-        Version of the RIME cluster control plane.  # noqa: E501
+        Version of the Robust Intelligence cluster control plane.  # noqa: E501
 
         :return: The cluster_info_version of this RimeGetRIMEInfoResponse.  # noqa: E501
         :rtype: str
         """
         return self._cluster_info_version
 
     @cluster_info_version.setter
     def cluster_info_version(self, cluster_info_version):
         """Sets the cluster_info_version of this RimeGetRIMEInfoResponse.
 
-        Version of the RIME cluster control plane.  # noqa: E501
+        Version of the Robust Intelligence cluster control plane.  # noqa: E501
 
         :param cluster_info_version: The cluster_info_version of this RimeGetRIMEInfoResponse.  # noqa: E501
         :type: str
         """
 
         self._cluster_info_version = cluster_info_version
 
@@ -180,26 +180,26 @@
 
         self._ri_plan = ri_plan
 
     @property
     def build_version(self):
         """Gets the build_version of this RimeGetRIMEInfoResponse.  # noqa: E501
 
-        Annotated version of the RIME cluster control plane, including the timestamp corresponding to the build.  # noqa: E501
+        Annotated version of the Robust Intelligence cluster control plane, including the timestamp corresponding to the build.  # noqa: E501
 
         :return: The build_version of this RimeGetRIMEInfoResponse.  # noqa: E501
         :rtype: str
         """
         return self._build_version
 
     @build_version.setter
     def build_version(self, build_version):
         """Sets the build_version of this RimeGetRIMEInfoResponse.
 
-        Annotated version of the RIME cluster control plane, including the timestamp corresponding to the build.  # noqa: E501
+        Annotated version of the Robust Intelligence cluster control plane, including the timestamp corresponding to the build.  # noqa: E501
 
         :param build_version: The build_version of this RimeGetRIMEInfoResponse.  # noqa: E501
         :type: str
         """
 
         self._build_version = build_version
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeHeartbeatResponse(object):
+class RimeUpsertFeatureFlagsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeHeartbeatResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeUpsertFeatureFlagsResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeHeartbeatResponse, dict):
+        if issubclass(RimeUpsertFeatureFlagsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeHeartbeatResponse):
+        if not isinstance(other, RimeUpsertFeatureFlagsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_image_reference.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_image_reference.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_int_list.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_int_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_integration_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_integration_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_data.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_view.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_subject_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeJobView(object):
+class RimeSubjectType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "JOB_VIEW_UNSPECIFIED"
-    BASIC = "JOB_VIEW_BASIC"
-    FULL = "JOB_VIEW_FULL"
+    UNSPECIFIED = "SUBJECT_TYPE_UNSPECIFIED"
+    ORGANIZATION = "SUBJECT_TYPE_ORGANIZATION"
+    WORKSPACE = "SUBJECT_TYPE_WORKSPACE"
+    PROJECT = "SUBJECT_TYPE_PROJECT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeJobView - a model defined in Swagger"""  # noqa: E501
+        """RimeSubjectType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -61,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeJobView, dict):
+        if issubclass(RimeSubjectType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -77,15 +78,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeJobView):
+        if not isinstance(other, RimeSubjectType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_language.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeLanguage(object):
+class RimeLimitStatusStatus(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "LANGUAGE_UNSPECIFIED"
-    EN = "LANGUAGE_EN"
-    JA = "LANGUAGE_JA"
+    UNSPECIFIED = "STATUS_UNSPECIFIED"
+    OK = "STATUS_OK"
+    WARN = "STATUS_WARN"
+    ERROR = "STATUS_ERROR"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeLanguage - a model defined in Swagger"""  # noqa: E501
+        """RimeLimitStatusStatus - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -61,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeLanguage, dict):
+        if issubclass(RimeLimitStatusStatus, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -77,15 +78,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeLanguage):
+        if not isinstance(other, RimeLimitStatusStatus):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_license_feature.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_license_feature.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_license_limit.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeLicenseLimit(object):
+class TestrunTestSensitivity(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "LICENSE_LIMIT_UNSPECIFIED"
-    EXPIRATION = "LICENSE_LIMIT_EXPIRATION"
-    STRESS_TEST_RUNS = "LICENSE_LIMIT_STRESS_TEST_RUNS"
-    FIREWALL = "LICENSE_LIMIT_FIREWALL"
+    UNSPECIFIED = "TEST_SENSITIVITY_UNSPECIFIED"
+    LESS_SENSITIVE = "TEST_SENSITIVITY_LESS_SENSITIVE"
+    DEFAULT = "TEST_SENSITIVITY_DEFAULT"
+    MORE_SENSITIVE = "TEST_SENSITIVITY_MORE_SENSITIVE"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeLicenseLimit - a model defined in Swagger"""  # noqa: E501
+        """TestrunTestSensitivity - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -62,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeLicenseLimit, dict):
+        if issubclass(TestrunTestSensitivity, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,15 +78,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeLicenseLimit):
+        if not isinstance(other, TestrunTestSensitivity):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_limit_status.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_limit_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_license_limit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeLimitStatusStatus(object):
+class RimeLicenseLimit(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "STATUS_UNSPECIFIED"
-    OK = "STATUS_OK"
-    WARN = "STATUS_WARN"
-    ERROR = "STATUS_ERROR"
+    UNSPECIFIED = "LICENSE_LIMIT_UNSPECIFIED"
+    EXPIRATION = "LICENSE_LIMIT_EXPIRATION"
+    STRESS_TEST_RUNS = "LICENSE_LIMIT_STRESS_TEST_RUNS"
+    FIREWALL = "LICENSE_LIMIT_FIREWALL"
+    WORKSPACES = "LICENSE_LIMIT_WORKSPACES"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeLimitStatusStatus - a model defined in Swagger"""  # noqa: E501
+        """RimeLicenseLimit - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -62,15 +63,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeLimitStatusStatus, dict):
+        if issubclass(RimeLicenseLimit, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,15 +79,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeLimitStatusStatus):
+        if not isinstance(other, RimeLicenseLimit):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,119 +1,119 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeListAPITokensResponse(object):
+class RimeListDatasetsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'api_token_infos': 'list[RimeAPITokenInfo]',
+        'datasets': 'list[DatasetDataset]',
         'next_page_token': 'str',
         'has_more': 'bool'
     }
 
     attribute_map = {
-        'api_token_infos': 'apiTokenInfos',
+        'datasets': 'datasets',
         'next_page_token': 'nextPageToken',
         'has_more': 'hasMore'
     }
 
-    def __init__(self, api_token_infos=None, next_page_token=None, has_more=None):  # noqa: E501
-        """RimeListAPITokensResponse - a model defined in Swagger"""  # noqa: E501
-        self._api_token_infos = None
+    def __init__(self, datasets=None, next_page_token=None, has_more=None):  # noqa: E501
+        """RimeListDatasetsResponse - a model defined in Swagger"""  # noqa: E501
+        self._datasets = None
         self._next_page_token = None
         self._has_more = None
         self.discriminator = None
-        if api_token_infos is not None:
-            self.api_token_infos = api_token_infos
+        if datasets is not None:
+            self.datasets = datasets
         if next_page_token is not None:
             self.next_page_token = next_page_token
         if has_more is not None:
             self.has_more = has_more
 
     @property
-    def api_token_infos(self):
-        """Gets the api_token_infos of this RimeListAPITokensResponse.  # noqa: E501
+    def datasets(self):
+        """Gets the datasets of this RimeListDatasetsResponse.  # noqa: E501
 
 
-        :return: The api_token_infos of this RimeListAPITokensResponse.  # noqa: E501
-        :rtype: list[RimeAPITokenInfo]
+        :return: The datasets of this RimeListDatasetsResponse.  # noqa: E501
+        :rtype: list[DatasetDataset]
         """
-        return self._api_token_infos
+        return self._datasets
 
-    @api_token_infos.setter
-    def api_token_infos(self, api_token_infos):
-        """Sets the api_token_infos of this RimeListAPITokensResponse.
+    @datasets.setter
+    def datasets(self, datasets):
+        """Sets the datasets of this RimeListDatasetsResponse.
 
 
-        :param api_token_infos: The api_token_infos of this RimeListAPITokensResponse.  # noqa: E501
-        :type: list[RimeAPITokenInfo]
+        :param datasets: The datasets of this RimeListDatasetsResponse.  # noqa: E501
+        :type: list[DatasetDataset]
         """
 
-        self._api_token_infos = api_token_infos
+        self._datasets = datasets
 
     @property
     def next_page_token(self):
-        """Gets the next_page_token of this RimeListAPITokensResponse.  # noqa: E501
+        """Gets the next_page_token of this RimeListDatasetsResponse.  # noqa: E501
 
 
-        :return: The next_page_token of this RimeListAPITokensResponse.  # noqa: E501
+        :return: The next_page_token of this RimeListDatasetsResponse.  # noqa: E501
         :rtype: str
         """
         return self._next_page_token
 
     @next_page_token.setter
     def next_page_token(self, next_page_token):
-        """Sets the next_page_token of this RimeListAPITokensResponse.
+        """Sets the next_page_token of this RimeListDatasetsResponse.
 
 
-        :param next_page_token: The next_page_token of this RimeListAPITokensResponse.  # noqa: E501
+        :param next_page_token: The next_page_token of this RimeListDatasetsResponse.  # noqa: E501
         :type: str
         """
 
         self._next_page_token = next_page_token
 
     @property
     def has_more(self):
-        """Gets the has_more of this RimeListAPITokensResponse.  # noqa: E501
+        """Gets the has_more of this RimeListDatasetsResponse.  # noqa: E501
 
 
-        :return: The has_more of this RimeListAPITokensResponse.  # noqa: E501
+        :return: The has_more of this RimeListDatasetsResponse.  # noqa: E501
         :rtype: bool
         """
         return self._has_more
 
     @has_more.setter
     def has_more(self, has_more):
-        """Sets the has_more of this RimeListAPITokensResponse.
+        """Sets the has_more of this RimeListDatasetsResponse.
 
 
-        :param has_more: The has_more of this RimeListAPITokensResponse.  # noqa: E501
+        :param has_more: The has_more of this RimeListDatasetsResponse.  # noqa: E501
         :type: bool
         """
 
         self._has_more = has_more
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -132,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeListAPITokensResponse, dict):
+        if issubclass(RimeListDatasetsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeListAPITokensResponse):
+        if not isinstance(other, RimeListDatasetsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,119 +1,119 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeListDatasetsResponse(object):
+class RimeListPredictionSetsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'datasets': 'list[DatasetDataset]',
+        'predictions': 'list[RegistrypredictionPrediction]',
         'next_page_token': 'str',
         'has_more': 'bool'
     }
 
     attribute_map = {
-        'datasets': 'datasets',
+        'predictions': 'predictions',
         'next_page_token': 'nextPageToken',
         'has_more': 'hasMore'
     }
 
-    def __init__(self, datasets=None, next_page_token=None, has_more=None):  # noqa: E501
-        """RimeListDatasetsResponse - a model defined in Swagger"""  # noqa: E501
-        self._datasets = None
+    def __init__(self, predictions=None, next_page_token=None, has_more=None):  # noqa: E501
+        """RimeListPredictionSetsResponse - a model defined in Swagger"""  # noqa: E501
+        self._predictions = None
         self._next_page_token = None
         self._has_more = None
         self.discriminator = None
-        if datasets is not None:
-            self.datasets = datasets
+        if predictions is not None:
+            self.predictions = predictions
         if next_page_token is not None:
             self.next_page_token = next_page_token
         if has_more is not None:
             self.has_more = has_more
 
     @property
-    def datasets(self):
-        """Gets the datasets of this RimeListDatasetsResponse.  # noqa: E501
+    def predictions(self):
+        """Gets the predictions of this RimeListPredictionSetsResponse.  # noqa: E501
 
 
-        :return: The datasets of this RimeListDatasetsResponse.  # noqa: E501
-        :rtype: list[DatasetDataset]
+        :return: The predictions of this RimeListPredictionSetsResponse.  # noqa: E501
+        :rtype: list[RegistrypredictionPrediction]
         """
-        return self._datasets
+        return self._predictions
 
-    @datasets.setter
-    def datasets(self, datasets):
-        """Sets the datasets of this RimeListDatasetsResponse.
+    @predictions.setter
+    def predictions(self, predictions):
+        """Sets the predictions of this RimeListPredictionSetsResponse.
 
 
-        :param datasets: The datasets of this RimeListDatasetsResponse.  # noqa: E501
-        :type: list[DatasetDataset]
+        :param predictions: The predictions of this RimeListPredictionSetsResponse.  # noqa: E501
+        :type: list[RegistrypredictionPrediction]
         """
 
-        self._datasets = datasets
+        self._predictions = predictions
 
     @property
     def next_page_token(self):
-        """Gets the next_page_token of this RimeListDatasetsResponse.  # noqa: E501
+        """Gets the next_page_token of this RimeListPredictionSetsResponse.  # noqa: E501
 
 
-        :return: The next_page_token of this RimeListDatasetsResponse.  # noqa: E501
+        :return: The next_page_token of this RimeListPredictionSetsResponse.  # noqa: E501
         :rtype: str
         """
         return self._next_page_token
 
     @next_page_token.setter
     def next_page_token(self, next_page_token):
-        """Sets the next_page_token of this RimeListDatasetsResponse.
+        """Sets the next_page_token of this RimeListPredictionSetsResponse.
 
 
-        :param next_page_token: The next_page_token of this RimeListDatasetsResponse.  # noqa: E501
+        :param next_page_token: The next_page_token of this RimeListPredictionSetsResponse.  # noqa: E501
         :type: str
         """
 
         self._next_page_token = next_page_token
 
     @property
     def has_more(self):
-        """Gets the has_more of this RimeListDatasetsResponse.  # noqa: E501
+        """Gets the has_more of this RimeListPredictionSetsResponse.  # noqa: E501
 
 
-        :return: The has_more of this RimeListDatasetsResponse.  # noqa: E501
+        :return: The has_more of this RimeListPredictionSetsResponse.  # noqa: E501
         :rtype: bool
         """
         return self._has_more
 
     @has_more.setter
     def has_more(self, has_more):
-        """Sets the has_more of this RimeListDatasetsResponse.
+        """Sets the has_more of this RimeListPredictionSetsResponse.
 
 
-        :param has_more: The has_more of this RimeListDatasetsResponse.  # noqa: E501
+        :param has_more: The has_more of this RimeListPredictionSetsResponse.  # noqa: E501
         :type: bool
         """
 
         self._has_more = has_more
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -132,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeListDatasetsResponse, dict):
+        if issubclass(RimeListPredictionSetsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeListDatasetsResponse):
+        if not isinstance(other, RimeListPredictionSetsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,121 +1,119 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeListJobsForProjectResponse(object):
+class RimeListModelsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'jobs': 'list[RimeJobMetadata]',
+        'models': 'list[RimeModelWithOwnerDetails]',
         'next_page_token': 'str',
         'has_more': 'bool'
     }
 
     attribute_map = {
-        'jobs': 'jobs',
+        'models': 'models',
         'next_page_token': 'nextPageToken',
         'has_more': 'hasMore'
     }
 
-    def __init__(self, jobs=None, next_page_token=None, has_more=None):  # noqa: E501
-        """RimeListJobsForProjectResponse - a model defined in Swagger"""  # noqa: E501
-        self._jobs = None
+    def __init__(self, models=None, next_page_token=None, has_more=None):  # noqa: E501
+        """RimeListModelsResponse - a model defined in Swagger"""  # noqa: E501
+        self._models = None
         self._next_page_token = None
         self._has_more = None
         self.discriminator = None
-        if jobs is not None:
-            self.jobs = jobs
+        if models is not None:
+            self.models = models
         if next_page_token is not None:
             self.next_page_token = next_page_token
         if has_more is not None:
             self.has_more = has_more
 
     @property
-    def jobs(self):
-        """Gets the jobs of this RimeListJobsForProjectResponse.  # noqa: E501
+    def models(self):
+        """Gets the models of this RimeListModelsResponse.  # noqa: E501
 
 
-        :return: The jobs of this RimeListJobsForProjectResponse.  # noqa: E501
-        :rtype: list[RimeJobMetadata]
+        :return: The models of this RimeListModelsResponse.  # noqa: E501
+        :rtype: list[RimeModelWithOwnerDetails]
         """
-        return self._jobs
+        return self._models
 
-    @jobs.setter
-    def jobs(self, jobs):
-        """Sets the jobs of this RimeListJobsForProjectResponse.
+    @models.setter
+    def models(self, models):
+        """Sets the models of this RimeListModelsResponse.
 
 
-        :param jobs: The jobs of this RimeListJobsForProjectResponse.  # noqa: E501
-        :type: list[RimeJobMetadata]
+        :param models: The models of this RimeListModelsResponse.  # noqa: E501
+        :type: list[RimeModelWithOwnerDetails]
         """
 
-        self._jobs = jobs
+        self._models = models
 
     @property
     def next_page_token(self):
-        """Gets the next_page_token of this RimeListJobsForProjectResponse.  # noqa: E501
+        """Gets the next_page_token of this RimeListModelsResponse.  # noqa: E501
 
-        Use this page token in your next ListJobs call to access the next page of results.  # noqa: E501
 
-        :return: The next_page_token of this RimeListJobsForProjectResponse.  # noqa: E501
+        :return: The next_page_token of this RimeListModelsResponse.  # noqa: E501
         :rtype: str
         """
         return self._next_page_token
 
     @next_page_token.setter
     def next_page_token(self, next_page_token):
-        """Sets the next_page_token of this RimeListJobsForProjectResponse.
+        """Sets the next_page_token of this RimeListModelsResponse.
 
-        Use this page token in your next ListJobs call to access the next page of results.  # noqa: E501
 
-        :param next_page_token: The next_page_token of this RimeListJobsForProjectResponse.  # noqa: E501
+        :param next_page_token: The next_page_token of this RimeListModelsResponse.  # noqa: E501
         :type: str
         """
 
         self._next_page_token = next_page_token
 
     @property
     def has_more(self):
-        """Gets the has_more of this RimeListJobsForProjectResponse.  # noqa: E501
+        """Gets the has_more of this RimeListModelsResponse.  # noqa: E501
 
 
-        :return: The has_more of this RimeListJobsForProjectResponse.  # noqa: E501
+        :return: The has_more of this RimeListModelsResponse.  # noqa: E501
         :rtype: bool
         """
         return self._has_more
 
     @has_more.setter
     def has_more(self, has_more):
-        """Sets the has_more of this RimeListJobsForProjectResponse.
+        """Sets the has_more of this RimeListModelsResponse.
 
 
-        :param has_more: The has_more of this RimeListJobsForProjectResponse.  # noqa: E501
+        :param has_more: The has_more of this RimeListModelsResponse.  # noqa: E501
         :type: bool
         """
 
         self._has_more = has_more
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -134,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeListJobsForProjectResponse, dict):
+        if issubclass(RimeListModelsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -150,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeListJobsForProjectResponse):
+        if not isinstance(other, RimeListModelsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,119 +1,119 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeListModelsResponse(object):
+class RimeListWorkspacesResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'models': 'list[RimeModelWithOwnerDetails]',
+        'workspaces': 'list[RimeWorkspace]',
         'next_page_token': 'str',
         'has_more': 'bool'
     }
 
     attribute_map = {
-        'models': 'models',
+        'workspaces': 'workspaces',
         'next_page_token': 'nextPageToken',
         'has_more': 'hasMore'
     }
 
-    def __init__(self, models=None, next_page_token=None, has_more=None):  # noqa: E501
-        """RimeListModelsResponse - a model defined in Swagger"""  # noqa: E501
-        self._models = None
+    def __init__(self, workspaces=None, next_page_token=None, has_more=None):  # noqa: E501
+        """RimeListWorkspacesResponse - a model defined in Swagger"""  # noqa: E501
+        self._workspaces = None
         self._next_page_token = None
         self._has_more = None
         self.discriminator = None
-        if models is not None:
-            self.models = models
+        if workspaces is not None:
+            self.workspaces = workspaces
         if next_page_token is not None:
             self.next_page_token = next_page_token
         if has_more is not None:
             self.has_more = has_more
 
     @property
-    def models(self):
-        """Gets the models of this RimeListModelsResponse.  # noqa: E501
+    def workspaces(self):
+        """Gets the workspaces of this RimeListWorkspacesResponse.  # noqa: E501
 
 
-        :return: The models of this RimeListModelsResponse.  # noqa: E501
-        :rtype: list[RimeModelWithOwnerDetails]
+        :return: The workspaces of this RimeListWorkspacesResponse.  # noqa: E501
+        :rtype: list[RimeWorkspace]
         """
-        return self._models
+        return self._workspaces
 
-    @models.setter
-    def models(self, models):
-        """Sets the models of this RimeListModelsResponse.
+    @workspaces.setter
+    def workspaces(self, workspaces):
+        """Sets the workspaces of this RimeListWorkspacesResponse.
 
 
-        :param models: The models of this RimeListModelsResponse.  # noqa: E501
-        :type: list[RimeModelWithOwnerDetails]
+        :param workspaces: The workspaces of this RimeListWorkspacesResponse.  # noqa: E501
+        :type: list[RimeWorkspace]
         """
 
-        self._models = models
+        self._workspaces = workspaces
 
     @property
     def next_page_token(self):
-        """Gets the next_page_token of this RimeListModelsResponse.  # noqa: E501
+        """Gets the next_page_token of this RimeListWorkspacesResponse.  # noqa: E501
 
 
-        :return: The next_page_token of this RimeListModelsResponse.  # noqa: E501
+        :return: The next_page_token of this RimeListWorkspacesResponse.  # noqa: E501
         :rtype: str
         """
         return self._next_page_token
 
     @next_page_token.setter
     def next_page_token(self, next_page_token):
-        """Sets the next_page_token of this RimeListModelsResponse.
+        """Sets the next_page_token of this RimeListWorkspacesResponse.
 
 
-        :param next_page_token: The next_page_token of this RimeListModelsResponse.  # noqa: E501
+        :param next_page_token: The next_page_token of this RimeListWorkspacesResponse.  # noqa: E501
         :type: str
         """
 
         self._next_page_token = next_page_token
 
     @property
     def has_more(self):
-        """Gets the has_more of this RimeListModelsResponse.  # noqa: E501
+        """Gets the has_more of this RimeListWorkspacesResponse.  # noqa: E501
 
 
-        :return: The has_more of this RimeListModelsResponse.  # noqa: E501
+        :return: The has_more of this RimeListWorkspacesResponse.  # noqa: E501
         :rtype: bool
         """
         return self._has_more
 
     @has_more.setter
     def has_more(self, has_more):
-        """Sets the has_more of this RimeListModelsResponse.
+        """Sets the has_more of this RimeListWorkspacesResponse.
 
 
-        :param has_more: The has_more of this RimeListModelsResponse.  # noqa: E501
+        :param has_more: The has_more of this RimeListWorkspacesResponse.  # noqa: E501
         :type: bool
         """
 
         self._has_more = has_more
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -132,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeListModelsResponse, dict):
+        if issubclass(RimeListWorkspacesResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeListModelsResponse):
+        if not isinstance(other, RimeListWorkspacesResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,119 +1,125 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeListPredictionSetsResponse(object):
+class TestrunresultListTestRunsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'predictions': 'list[RegistrypredictionPrediction]',
+        'test_runs': 'list[TestrunresultTestRunDetail]',
         'next_page_token': 'str',
         'has_more': 'bool'
     }
 
     attribute_map = {
-        'predictions': 'predictions',
+        'test_runs': 'testRuns',
         'next_page_token': 'nextPageToken',
         'has_more': 'hasMore'
     }
 
-    def __init__(self, predictions=None, next_page_token=None, has_more=None):  # noqa: E501
-        """RimeListPredictionSetsResponse - a model defined in Swagger"""  # noqa: E501
-        self._predictions = None
+    def __init__(self, test_runs=None, next_page_token=None, has_more=None):  # noqa: E501
+        """TestrunresultListTestRunsResponse - a model defined in Swagger"""  # noqa: E501
+        self._test_runs = None
         self._next_page_token = None
         self._has_more = None
         self.discriminator = None
-        if predictions is not None:
-            self.predictions = predictions
+        if test_runs is not None:
+            self.test_runs = test_runs
         if next_page_token is not None:
             self.next_page_token = next_page_token
         if has_more is not None:
             self.has_more = has_more
 
     @property
-    def predictions(self):
-        """Gets the predictions of this RimeListPredictionSetsResponse.  # noqa: E501
+    def test_runs(self):
+        """Gets the test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
 
+        The details of the test runs.  # noqa: E501
 
-        :return: The predictions of this RimeListPredictionSetsResponse.  # noqa: E501
-        :rtype: list[RegistrypredictionPrediction]
+        :return: The test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
+        :rtype: list[TestrunresultTestRunDetail]
         """
-        return self._predictions
+        return self._test_runs
 
-    @predictions.setter
-    def predictions(self, predictions):
-        """Sets the predictions of this RimeListPredictionSetsResponse.
+    @test_runs.setter
+    def test_runs(self, test_runs):
+        """Sets the test_runs of this TestrunresultListTestRunsResponse.
 
+        The details of the test runs.  # noqa: E501
 
-        :param predictions: The predictions of this RimeListPredictionSetsResponse.  # noqa: E501
-        :type: list[RegistrypredictionPrediction]
+        :param test_runs: The test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
+        :type: list[TestrunresultTestRunDetail]
         """
 
-        self._predictions = predictions
+        self._test_runs = test_runs
 
     @property
     def next_page_token(self):
-        """Gets the next_page_token of this RimeListPredictionSetsResponse.  # noqa: E501
+        """Gets the next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
 
+        A token representing the next page from the list returned by a ListTestRuns query.  # noqa: E501
 
-        :return: The next_page_token of this RimeListPredictionSetsResponse.  # noqa: E501
+        :return: The next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
         :rtype: str
         """
         return self._next_page_token
 
     @next_page_token.setter
     def next_page_token(self, next_page_token):
-        """Sets the next_page_token of this RimeListPredictionSetsResponse.
+        """Sets the next_page_token of this TestrunresultListTestRunsResponse.
 
+        A token representing the next page from the list returned by a ListTestRuns query.  # noqa: E501
 
-        :param next_page_token: The next_page_token of this RimeListPredictionSetsResponse.  # noqa: E501
+        :param next_page_token: The next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
         :type: str
         """
 
         self._next_page_token = next_page_token
 
     @property
     def has_more(self):
-        """Gets the has_more of this RimeListPredictionSetsResponse.  # noqa: E501
+        """Gets the has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
 
+        A Boolean that specifies whether there are more test runs to return.  # noqa: E501
 
-        :return: The has_more of this RimeListPredictionSetsResponse.  # noqa: E501
+        :return: The has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
         :rtype: bool
         """
         return self._has_more
 
     @has_more.setter
     def has_more(self, has_more):
-        """Sets the has_more of this RimeListPredictionSetsResponse.
+        """Sets the has_more of this TestrunresultListTestRunsResponse.
 
+        A Boolean that specifies whether there are more test runs to return.  # noqa: E501
 
-        :param has_more: The has_more of this RimeListPredictionSetsResponse.  # noqa: E501
+        :param has_more: The has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
         :type: bool
         """
 
         self._has_more = has_more
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -132,15 +138,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeListPredictionSetsResponse, dict):
+        if issubclass(TestrunresultListTestRunsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +154,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeListPredictionSetsResponse):
+        if not isinstance(other, TestrunresultListTestRunsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeListUsersRequestQuery(object):
+class ProjectUpdateUserOfProjectResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeListUsersRequestQuery - a model defined in Swagger"""  # noqa: E501
+        """ProjectUpdateUserOfProjectResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeListUsersRequestQuery, dict):
+        if issubclass(ProjectUpdateUserOfProjectResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeListUsersRequestQuery):
+        if not isinstance(other, ProjectUpdateUserOfProjectResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeListWorkspacesRequestQuery(object):
+class RimeListUsersRequestQuery(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeListWorkspacesRequestQuery - a model defined in Swagger"""  # noqa: E501
+        """RimeListUsersRequestQuery - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeListWorkspacesRequestQuery, dict):
+        if issubclass(RimeListUsersRequestQuery, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeListWorkspacesRequestQuery):
+        if not isinstance(other, RimeListUsersRequestQuery):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,119 +1,125 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeListWorkspacesResponse(object):
+class TestrunresultListTestCasesResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'workspaces': 'list[RimeWorkspace]',
+        'test_cases': 'list[TestrunresultTestCase]',
         'next_page_token': 'str',
         'has_more': 'bool'
     }
 
     attribute_map = {
-        'workspaces': 'workspaces',
+        'test_cases': 'testCases',
         'next_page_token': 'nextPageToken',
         'has_more': 'hasMore'
     }
 
-    def __init__(self, workspaces=None, next_page_token=None, has_more=None):  # noqa: E501
-        """RimeListWorkspacesResponse - a model defined in Swagger"""  # noqa: E501
-        self._workspaces = None
+    def __init__(self, test_cases=None, next_page_token=None, has_more=None):  # noqa: E501
+        """TestrunresultListTestCasesResponse - a model defined in Swagger"""  # noqa: E501
+        self._test_cases = None
         self._next_page_token = None
         self._has_more = None
         self.discriminator = None
-        if workspaces is not None:
-            self.workspaces = workspaces
+        if test_cases is not None:
+            self.test_cases = test_cases
         if next_page_token is not None:
             self.next_page_token = next_page_token
         if has_more is not None:
             self.has_more = has_more
 
     @property
-    def workspaces(self):
-        """Gets the workspaces of this RimeListWorkspacesResponse.  # noqa: E501
+    def test_cases(self):
+        """Gets the test_cases of this TestrunresultListTestCasesResponse.  # noqa: E501
 
+        The list of test cases.  # noqa: E501
 
-        :return: The workspaces of this RimeListWorkspacesResponse.  # noqa: E501
-        :rtype: list[RimeWorkspace]
+        :return: The test_cases of this TestrunresultListTestCasesResponse.  # noqa: E501
+        :rtype: list[TestrunresultTestCase]
         """
-        return self._workspaces
+        return self._test_cases
 
-    @workspaces.setter
-    def workspaces(self, workspaces):
-        """Sets the workspaces of this RimeListWorkspacesResponse.
+    @test_cases.setter
+    def test_cases(self, test_cases):
+        """Sets the test_cases of this TestrunresultListTestCasesResponse.
 
+        The list of test cases.  # noqa: E501
 
-        :param workspaces: The workspaces of this RimeListWorkspacesResponse.  # noqa: E501
-        :type: list[RimeWorkspace]
+        :param test_cases: The test_cases of this TestrunresultListTestCasesResponse.  # noqa: E501
+        :type: list[TestrunresultTestCase]
         """
 
-        self._workspaces = workspaces
+        self._test_cases = test_cases
 
     @property
     def next_page_token(self):
-        """Gets the next_page_token of this RimeListWorkspacesResponse.  # noqa: E501
+        """Gets the next_page_token of this TestrunresultListTestCasesResponse.  # noqa: E501
 
+        A token representing the next page from the list returned by a ListTestCases query.  # noqa: E501
 
-        :return: The next_page_token of this RimeListWorkspacesResponse.  # noqa: E501
+        :return: The next_page_token of this TestrunresultListTestCasesResponse.  # noqa: E501
         :rtype: str
         """
         return self._next_page_token
 
     @next_page_token.setter
     def next_page_token(self, next_page_token):
-        """Sets the next_page_token of this RimeListWorkspacesResponse.
+        """Sets the next_page_token of this TestrunresultListTestCasesResponse.
 
+        A token representing the next page from the list returned by a ListTestCases query.  # noqa: E501
 
-        :param next_page_token: The next_page_token of this RimeListWorkspacesResponse.  # noqa: E501
+        :param next_page_token: The next_page_token of this TestrunresultListTestCasesResponse.  # noqa: E501
         :type: str
         """
 
         self._next_page_token = next_page_token
 
     @property
     def has_more(self):
-        """Gets the has_more of this RimeListWorkspacesResponse.  # noqa: E501
+        """Gets the has_more of this TestrunresultListTestCasesResponse.  # noqa: E501
 
+        A Boolean flag that specifies whether there are more test cases to return.  # noqa: E501
 
-        :return: The has_more of this RimeListWorkspacesResponse.  # noqa: E501
+        :return: The has_more of this TestrunresultListTestCasesResponse.  # noqa: E501
         :rtype: bool
         """
         return self._has_more
 
     @has_more.setter
     def has_more(self, has_more):
-        """Sets the has_more of this RimeListWorkspacesResponse.
+        """Sets the has_more of this TestrunresultListTestCasesResponse.
 
+        A Boolean flag that specifies whether there are more test cases to return.  # noqa: E501
 
-        :param has_more: The has_more of this RimeListWorkspacesResponse.  # noqa: E501
+        :param has_more: The has_more of this TestrunresultListTestCasesResponse.  # noqa: E501
         :type: bool
         """
 
         self._has_more = has_more
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -132,15 +138,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeListWorkspacesResponse, dict):
+        if issubclass(TestrunresultListTestCasesResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +154,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeListWorkspacesResponse):
+        if not isinstance(other, TestrunresultListTestCasesResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_managed_image.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_managed_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
@@ -316,26 +316,26 @@
 
         self._pip_libraries = pip_libraries
 
     @property
     def python_version(self):
         """Gets the python_version of this RimeManagedImage.  # noqa: E501
 
-        The version of Python used to build the RIME image.  # noqa: E501
+        The version of Python used to build the Robust Intelligence image.  # noqa: E501
 
         :return: The python_version of this RimeManagedImage.  # noqa: E501
         :rtype: str
         """
         return self._python_version
 
     @python_version.setter
     def python_version(self, python_version):
         """Sets the python_version of this RimeManagedImage.
 
-        The version of Python used to build the RIME image.  # noqa: E501
+        The version of Python used to build the Robust Intelligence image.  # noqa: E501
 
         :param python_version: The python_version of this RimeManagedImage.  # noqa: E501
         :type: str
         """
 
         self._python_version = python_version
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_card.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_model_card.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_task.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_model_task.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
@@ -30,14 +30,15 @@
     MULTICLASS_CLASSIFICATION = "MODEL_TASK_MULTICLASS_CLASSIFICATION"
     NAMED_ENTITY_RECOGNITION = "MODEL_TASK_NAMED_ENTITY_RECOGNITION"
     RANKING = "MODEL_TASK_RANKING"
     OBJECT_DETECTION = "MODEL_TASK_OBJECT_DETECTION"
     NATURAL_LANGUAGE_INFERENCE = "MODEL_TASK_NATURAL_LANGUAGE_INFERENCE"
     FILL_MASK = "MODEL_TASK_FILL_MASK"
     QUESTION_ANSWERING = "MODEL_TASK_QUESTION_ANSWERING"
+    ANOMALY_DETECTION = "MODEL_TASK_ANOMALY_DETECTION"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_named_double.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_named_double.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_order.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_order.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeResetPasswordResponse(object):
+class RimeDeleteModelResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeResetPasswordResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeDeleteModelResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeResetPasswordResponse, dict):
+        if issubclass(RimeDeleteModelResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeResetPasswordResponse):
+        if not isinstance(other, RimeDeleteModelResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeResolveDetectionEventResponse(object):
+class NotificationJobActionConfig(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeResolveDetectionEventResponse - a model defined in Swagger"""  # noqa: E501
+        """NotificationJobActionConfig - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeResolveDetectionEventResponse, dict):
+        if issubclass(NotificationJobActionConfig, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeResolveDetectionEventResponse):
+        if not isinstance(other, NotificationJobActionConfig):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_safe_url.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_safe_url.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeSendRIEmailResponse(object):
+class RimeDeleteCustomMonitorResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeSendRIEmailResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeDeleteCustomMonitorResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeSendRIEmailResponse, dict):
+        if issubclass(RimeDeleteCustomMonitorResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeSendRIEmailResponse):
+        if not isinstance(other, RimeDeleteCustomMonitorResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_severity.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_severity.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_foo_task_request.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_foo_task_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_foo_task_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_foo_task_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_str_list.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_str_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_subject_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeSubjectType(object):
+class RimeTestType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "SUBJECT_TYPE_UNSPECIFIED"
-    ORGANIZATION = "SUBJECT_TYPE_ORGANIZATION"
-    WORKSPACE = "SUBJECT_TYPE_WORKSPACE"
-    PROJECT = "SUBJECT_TYPE_PROJECT"
+    STRESS_TESTING_UNSPECIFIED = "TEST_TYPE_STRESS_TESTING_UNSPECIFIED"
+    CONTINUOUS_TESTING = "TEST_TYPE_CONTINUOUS_TESTING"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeSubjectType - a model defined in Swagger"""  # noqa: E501
+        """RimeTestType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -62,15 +60,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeSubjectType, dict):
+        if issubclass(RimeTestType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,15 +76,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeSubjectType):
+        if not isinstance(other, RimeTestType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_suggestion.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_suggestion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_table_column.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_table_column.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeTableColumnType(object):
+class MonitorAggregationType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "TABLE_COLUMN_TYPE_UNSPECIFIED"
-    STRING = "TABLE_COLUMN_TYPE_STRING"
-    NUMERICAL = "TABLE_COLUMN_TYPE_NUMERICAL"
-    DATE = "TABLE_COLUMN_TYPE_DATE"
-    PICKABLE = "TABLE_COLUMN_TYPE_PICKABLE"
+    UNSPECIFIED = "AGGREGATION_TYPE_UNSPECIFIED"
+    AVG = "AGGREGATION_TYPE_AVG"
+    MIN = "AGGREGATION_TYPE_MIN"
+    MAX = "AGGREGATION_TYPE_MAX"
+    SUM = "AGGREGATION_TYPE_SUM"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeTableColumnType - a model defined in Swagger"""  # noqa: E501
+        """MonitorAggregationType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -63,15 +63,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeTableColumnType, dict):
+        if issubclass(MonitorAggregationType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -79,15 +79,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeTableColumnType):
+        if not isinstance(other, MonitorAggregationType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_tag.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_metric.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_metric.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/detection_event_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeTestType(object):
+class DetectionEventType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    STRESS_TESTING_UNSPECIFIED = "TEST_TYPE_STRESS_TESTING_UNSPECIFIED"
-    CONTINUOUS_TESTING = "TEST_TYPE_CONTINUOUS_TESTING"
+    UNSPECIFIED = "EVENT_TYPE_UNSPECIFIED"
+    METRIC_DEGRADATION = "EVENT_TYPE_METRIC_DEGRADATION"
+    SECURITY = "EVENT_TYPE_SECURITY"
+    STRESS_TEST = "EVENT_TYPE_STRESS_TEST"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeTestType - a model defined in Swagger"""  # noqa: E501
+        """DetectionEventType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -60,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeTestType, dict):
+        if issubclass(DetectionEventType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -76,15 +78,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeTestType):
+        if not isinstance(other, DetectionEventType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_time_interval.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_time_interval.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_token_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeTokenType(object):
+class SecurityEventDetailsSecurityEventType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "TOKEN_TYPE_UNSPECIFIED"
-    USER = "TOKEN_TYPE_USER"
-    AGENT = "TOKEN_TYPE_AGENT"
+    UNSPECIFIED = "SECURITY_EVENT_TYPE_UNSPECIFIED"
+    DATA_POISONING = "SECURITY_EVENT_TYPE_DATA_POISONING"
+    MODEL_EVASION = "SECURITY_EVENT_TYPE_MODEL_EVASION"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeTokenType - a model defined in Swagger"""  # noqa: E501
+        """SecurityEventDetailsSecurityEventType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -61,15 +61,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeTokenType, dict):
+        if issubclass(SecurityEventDetailsSecurityEventType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -77,15 +77,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeTokenType):
+        if not isinstance(other, SecurityEventDetailsSecurityEventType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeUpdateBuildInfoResponse(object):
+class RimeDeleteIntegrationResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeUpdateBuildInfoResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeDeleteIntegrationResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeUpdateBuildInfoResponse, dict):
+        if issubclass(RimeDeleteIntegrationResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeUpdateBuildInfoResponse):
+        if not isinstance(other, RimeDeleteIntegrationResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeUpdateIntegrationResponse(object):
+class RimeCreateIntegrationRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'integration_info': 'RimeIntegrationInfo'
+        'integration': 'IntegrationIntegration'
     }
 
     attribute_map = {
-        'integration_info': 'integrationInfo'
+        'integration': 'integration'
     }
 
-    def __init__(self, integration_info=None):  # noqa: E501
-        """RimeUpdateIntegrationResponse - a model defined in Swagger"""  # noqa: E501
-        self._integration_info = None
+    def __init__(self, integration=None):  # noqa: E501
+        """RimeCreateIntegrationRequest - a model defined in Swagger"""  # noqa: E501
+        self._integration = None
         self.discriminator = None
-        if integration_info is not None:
-            self.integration_info = integration_info
+        if integration is not None:
+            self.integration = integration
 
     @property
-    def integration_info(self):
-        """Gets the integration_info of this RimeUpdateIntegrationResponse.  # noqa: E501
+    def integration(self):
+        """Gets the integration of this RimeCreateIntegrationRequest.  # noqa: E501
 
 
-        :return: The integration_info of this RimeUpdateIntegrationResponse.  # noqa: E501
-        :rtype: RimeIntegrationInfo
+        :return: The integration of this RimeCreateIntegrationRequest.  # noqa: E501
+        :rtype: IntegrationIntegration
         """
-        return self._integration_info
+        return self._integration
 
-    @integration_info.setter
-    def integration_info(self, integration_info):
-        """Sets the integration_info of this RimeUpdateIntegrationResponse.
+    @integration.setter
+    def integration(self, integration):
+        """Sets the integration of this RimeCreateIntegrationRequest.
 
 
-        :param integration_info: The integration_info of this RimeUpdateIntegrationResponse.  # noqa: E501
-        :type: RimeIntegrationInfo
+        :param integration: The integration of this RimeCreateIntegrationRequest.  # noqa: E501
+        :type: IntegrationIntegration
         """
 
-        self._integration_info = integration_info
+        self._integration = integration
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeUpdateIntegrationResponse, dict):
+        if issubclass(RimeCreateIntegrationRequest, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeUpdateIntegrationResponse):
+        if not isinstance(other, RimeCreateIntegrationRequest):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeUpdateModelCardResponse(object):
+class RimeGetModelCardResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,36 +32,36 @@
     }
 
     attribute_map = {
         'model_card': 'modelCard'
     }
 
     def __init__(self, model_card=None):  # noqa: E501
-        """RimeUpdateModelCardResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeGetModelCardResponse - a model defined in Swagger"""  # noqa: E501
         self._model_card = None
         self.discriminator = None
         if model_card is not None:
             self.model_card = model_card
 
     @property
     def model_card(self):
-        """Gets the model_card of this RimeUpdateModelCardResponse.  # noqa: E501
+        """Gets the model_card of this RimeGetModelCardResponse.  # noqa: E501
 
 
-        :return: The model_card of this RimeUpdateModelCardResponse.  # noqa: E501
+        :return: The model_card of this RimeGetModelCardResponse.  # noqa: E501
         :rtype: RimeModelCard
         """
         return self._model_card
 
     @model_card.setter
     def model_card(self, model_card):
-        """Sets the model_card of this RimeUpdateModelCardResponse.
+        """Sets the model_card of this RimeGetModelCardResponse.
 
 
-        :param model_card: The model_card of this RimeUpdateModelCardResponse.  # noqa: E501
+        :param model_card: The model_card of this RimeGetModelCardResponse.  # noqa: E501
         :type: RimeModelCard
         """
 
         self._model_card = model_card
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeUpdateModelCardResponse, dict):
+        if issubclass(RimeGetModelCardResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeUpdateModelCardResponse):
+        if not isinstance(other, RimeGetModelCardResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,71 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeUpdateUserOfWorkspaceResponse(object):
+class RimeGetImageResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'image': 'RimeManagedImage'
     }
 
     attribute_map = {
+        'image': 'image'
     }
 
-    def __init__(self):  # noqa: E501
-        """RimeUpdateUserOfWorkspaceResponse - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, image=None):  # noqa: E501
+        """RimeGetImageResponse - a model defined in Swagger"""  # noqa: E501
+        self._image = None
         self.discriminator = None
+        if image is not None:
+            self.image = image
+
+    @property
+    def image(self):
+        """Gets the image of this RimeGetImageResponse.  # noqa: E501
+
+
+        :return: The image of this RimeGetImageResponse.  # noqa: E501
+        :rtype: RimeManagedImage
+        """
+        return self._image
+
+    @image.setter
+    def image(self, image):
+        """Sets the image of this RimeGetImageResponse.
+
+
+        :param image: The image of this RimeGetImageResponse.  # noqa: E501
+        :type: RimeManagedImage
+        """
+
+        self._image = image
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -54,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeUpdateUserOfWorkspaceResponse, dict):
+        if issubclass(RimeGetImageResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeUpdateUserOfWorkspaceResponse):
+        if not isinstance(other, RimeGetImageResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeUpdateUserResponse(object):
+class RimeResolveDetectionEventResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeUpdateUserResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeResolveDetectionEventResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeUpdateUserResponse, dict):
+        if issubclass(RimeResolveDetectionEventResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeUpdateUserResponse):
+        if not isinstance(other, RimeResolveDetectionEventResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeUpdateWorkspaceResponse(object):
+class MonitorThresholdType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
+
+    """
+    allowed enum values
+    """
+    UNSPECIFIED = "TYPE_UNSPECIFIED"
+    UPPER_BOUND = "TYPE_UPPER_BOUND"
+    LOWER_BOUND = "TYPE_LOWER_BOUND"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeUpdateWorkspaceResponse - a model defined in Swagger"""  # noqa: E501
+        """MonitorThresholdType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +61,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeUpdateWorkspaceResponse, dict):
+        if issubclass(MonitorThresholdType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +77,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeUpdateWorkspaceResponse):
+        if not isinstance(other, MonitorThresholdType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/statedb_job_status.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,55 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeUpdateWorkspaceTagResponse(object):
+class StatedbJobStatus(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
+
+    """
+    allowed enum values
+    """
+    UNSPECIFIED = "JOB_STATUS_UNSPECIFIED"
+    PENDING = "JOB_STATUS_PENDING"
+    RUNNING = "JOB_STATUS_RUNNING"
+    FAILED = "JOB_STATUS_FAILED"
+    SUCCEEDED = "JOB_STATUS_SUCCEEDED"
+    REQUESTED = "JOB_STATUS_REQUESTED"
+    CANCELLED = "JOB_STATUS_CANCELLED"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeUpdateWorkspaceTagResponse - a model defined in Swagger"""  # noqa: E501
+        """StatedbJobStatus - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +65,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeUpdateWorkspaceTagResponse, dict):
+        if issubclass(StatedbJobStatus, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +81,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeUpdateWorkspaceTagResponse):
+        if not isinstance(other, StatedbJobStatus):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/notification_notification_type.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeUpsertFeatureFlagsResponse(object):
+class NotificationNotificationType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
+
+    """
+    allowed enum values
+    """
+    UNSPECIFIED = "NOTIFICATION_TYPE_UNSPECIFIED"
+    DIGEST = "NOTIFICATION_TYPE_DIGEST"
+    JOB_ACTION = "NOTIFICATION_TYPE_JOB_ACTION"
+    MONITORING = "NOTIFICATION_TYPE_MONITORING"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeUpsertFeatureFlagsResponse - a model defined in Swagger"""  # noqa: E501
+        """NotificationNotificationType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeUpsertFeatureFlagsResponse, dict):
+        if issubclass(NotificationNotificationType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +78,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeUpsertFeatureFlagsResponse):
+        if not isinstance(other, NotificationNotificationType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_role.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_role.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_uuid.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_uuid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeValidateTestConfigResponse(object):
+class RimeDeleteFirewallResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeValidateTestConfigResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeDeleteFirewallResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeValidateTestConfigResponse, dict):
+        if issubclass(RimeDeleteFirewallResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeValidateTestConfigResponse):
+        if not isinstance(other, RimeDeleteFirewallResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_workspace.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/role_users_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/role_users_body.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/role_workspace_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/role_workspace_body.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schemanotification_config.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/schemanotification_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schemaregistry_data_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class SchemaregistryDataInfo(object):
+class RegistryDataInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -34,60 +34,60 @@
 
     attribute_map = {
         'connection_info': 'connectionInfo',
         'data_params': 'dataParams'
     }
 
     def __init__(self, connection_info=None, data_params=None):  # noqa: E501
-        """SchemaregistryDataInfo - a model defined in Swagger"""  # noqa: E501
+        """RegistryDataInfo - a model defined in Swagger"""  # noqa: E501
         self._connection_info = None
         self._data_params = None
         self.discriminator = None
         if connection_info is not None:
             self.connection_info = connection_info
         if data_params is not None:
             self.data_params = data_params
 
     @property
     def connection_info(self):
-        """Gets the connection_info of this SchemaregistryDataInfo.  # noqa: E501
+        """Gets the connection_info of this RegistryDataInfo.  # noqa: E501
 
 
-        :return: The connection_info of this SchemaregistryDataInfo.  # noqa: E501
+        :return: The connection_info of this RegistryDataInfo.  # noqa: E501
         :rtype: RegistryConnectionInfo
         """
         return self._connection_info
 
     @connection_info.setter
     def connection_info(self, connection_info):
-        """Sets the connection_info of this SchemaregistryDataInfo.
+        """Sets the connection_info of this RegistryDataInfo.
 
 
-        :param connection_info: The connection_info of this SchemaregistryDataInfo.  # noqa: E501
+        :param connection_info: The connection_info of this RegistryDataInfo.  # noqa: E501
         :type: RegistryConnectionInfo
         """
 
         self._connection_info = connection_info
 
     @property
     def data_params(self):
-        """Gets the data_params of this SchemaregistryDataInfo.  # noqa: E501
+        """Gets the data_params of this RegistryDataInfo.  # noqa: E501
 
 
-        :return: The data_params of this SchemaregistryDataInfo.  # noqa: E501
+        :return: The data_params of this RegistryDataInfo.  # noqa: E501
         :rtype: RegistryDataParams
         """
         return self._data_params
 
     @data_params.setter
     def data_params(self, data_params):
-        """Sets the data_params of this SchemaregistryDataInfo.
+        """Sets the data_params of this RegistryDataInfo.
 
 
-        :param data_params: The data_params of this SchemaregistryDataInfo.  # noqa: E501
+        :param data_params: The data_params of this RegistryDataInfo.  # noqa: E501
         :type: RegistryDataParams
         """
 
         self._data_params = data_params
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(SchemaregistryDataInfo, dict):
+        if issubclass(RegistryDataInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SchemaregistryDataInfo):
+        if not isinstance(other, RegistryDataInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schematestrun_data_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class SchematestrunDataInfo(object):
+class TestrunRefEvalDatasets(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -34,64 +34,64 @@
 
     attribute_map = {
         'ref_dataset_id': 'refDatasetId',
         'eval_dataset_id': 'evalDatasetId'
     }
 
     def __init__(self, ref_dataset_id=None, eval_dataset_id=None):  # noqa: E501
-        """SchematestrunDataInfo - a model defined in Swagger"""  # noqa: E501
+        """TestrunRefEvalDatasets - a model defined in Swagger"""  # noqa: E501
         self._ref_dataset_id = None
         self._eval_dataset_id = None
         self.discriminator = None
         self.ref_dataset_id = ref_dataset_id
         self.eval_dataset_id = eval_dataset_id
 
     @property
     def ref_dataset_id(self):
-        """Gets the ref_dataset_id of this SchematestrunDataInfo.  # noqa: E501
+        """Gets the ref_dataset_id of this TestrunRefEvalDatasets.  # noqa: E501
 
         Uniquely specifies a reference Dataset.  # noqa: E501
 
-        :return: The ref_dataset_id of this SchematestrunDataInfo.  # noqa: E501
+        :return: The ref_dataset_id of this TestrunRefEvalDatasets.  # noqa: E501
         :rtype: str
         """
         return self._ref_dataset_id
 
     @ref_dataset_id.setter
     def ref_dataset_id(self, ref_dataset_id):
-        """Sets the ref_dataset_id of this SchematestrunDataInfo.
+        """Sets the ref_dataset_id of this TestrunRefEvalDatasets.
 
         Uniquely specifies a reference Dataset.  # noqa: E501
 
-        :param ref_dataset_id: The ref_dataset_id of this SchematestrunDataInfo.  # noqa: E501
+        :param ref_dataset_id: The ref_dataset_id of this TestrunRefEvalDatasets.  # noqa: E501
         :type: str
         """
         if ref_dataset_id is None:
             raise ValueError("Invalid value for `ref_dataset_id`, must not be `None`")  # noqa: E501
 
         self._ref_dataset_id = ref_dataset_id
 
     @property
     def eval_dataset_id(self):
-        """Gets the eval_dataset_id of this SchematestrunDataInfo.  # noqa: E501
+        """Gets the eval_dataset_id of this TestrunRefEvalDatasets.  # noqa: E501
 
         Uniquely specifies an evaluation Dataset.  # noqa: E501
 
-        :return: The eval_dataset_id of this SchematestrunDataInfo.  # noqa: E501
+        :return: The eval_dataset_id of this TestrunRefEvalDatasets.  # noqa: E501
         :rtype: str
         """
         return self._eval_dataset_id
 
     @eval_dataset_id.setter
     def eval_dataset_id(self, eval_dataset_id):
-        """Sets the eval_dataset_id of this SchematestrunDataInfo.
+        """Sets the eval_dataset_id of this TestrunRefEvalDatasets.
 
         Uniquely specifies an evaluation Dataset.  # noqa: E501
 
-        :param eval_dataset_id: The eval_dataset_id of this SchematestrunDataInfo.  # noqa: E501
+        :param eval_dataset_id: The eval_dataset_id of this TestrunRefEvalDatasets.  # noqa: E501
         :type: str
         """
         if eval_dataset_id is None:
             raise ValueError("Invalid value for `eval_dataset_id`, must not be `None`")  # noqa: E501
 
         self._eval_dataset_id = eval_dataset_id
 
@@ -112,15 +112,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(SchematestrunDataInfo, dict):
+        if issubclass(TestrunRefEvalDatasets, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -128,15 +128,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SchematestrunDataInfo):
+        if not isinstance(other, TestrunRefEvalDatasets):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,61 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class SecurityEventDetailsSecurityEventType(object):
+class TestrunTestCategoryType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "SECURITY_EVENT_TYPE_UNSPECIFIED"
-    DATA_POISONING = "SECURITY_EVENT_TYPE_DATA_POISONING"
-    MODEL_EVASION = "SECURITY_EVENT_TYPE_MODEL_EVASION"
+    UNSPECIFIED = "TEST_CATEGORY_TYPE_UNSPECIFIED"
+    ABNORMAL_INPUTS = "TEST_CATEGORY_TYPE_ABNORMAL_INPUTS"
+    ADVERSARIAL = "TEST_CATEGORY_TYPE_ADVERSARIAL"
+    BIAS_AND_FAIRNESS = "TEST_CATEGORY_TYPE_BIAS_AND_FAIRNESS"
+    DATA_CLEANLINESS = "TEST_CATEGORY_TYPE_DATA_CLEANLINESS"
+    DRIFT = "TEST_CATEGORY_TYPE_DRIFT"
+    MODEL_PERFORMANCE = "TEST_CATEGORY_TYPE_MODEL_PERFORMANCE"
+    DATA_POISONING_DETECTION = "TEST_CATEGORY_TYPE_DATA_POISONING_DETECTION"
+    SUBSET_PERFORMANCE = "TEST_CATEGORY_TYPE_SUBSET_PERFORMANCE"
+    SUBSET_PERFORMANCE_DEGRADATION = "TEST_CATEGORY_TYPE_SUBSET_PERFORMANCE_DEGRADATION"
+    TRANSFORMATIONS = "TEST_CATEGORY_TYPE_TRANSFORMATIONS"
+    EVASION_ATTACK_DETECTION = "TEST_CATEGORY_TYPE_EVASION_ATTACK_DETECTION"
+    CUSTOM = "TEST_CATEGORY_TYPE_CUSTOM"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """SecurityEventDetailsSecurityEventType - a model defined in Swagger"""  # noqa: E501
+        """TestrunTestCategoryType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -61,15 +71,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(SecurityEventDetailsSecurityEventType, dict):
+        if issubclass(TestrunTestCategoryType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -77,15 +87,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SecurityEventDetailsSecurityEventType):
+        if not isinstance(other, TestrunTestCategoryType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/statedb_job_status.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_config_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class StatedbJobStatus(object):
+class RimeConfigType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "JOB_STATUS_UNSPECIFIED"
-    PENDING = "JOB_STATUS_PENDING"
-    RUNNING = "JOB_STATUS_RUNNING"
-    FAILED = "JOB_STATUS_FAILED"
-    SUCCEEDED = "JOB_STATUS_SUCCEEDED"
-    REQUESTED = "JOB_STATUS_REQUESTED"
-    CANCELLED = "JOB_STATUS_CANCELLED"
+    UNSPECIFIED = "CONFIG_TYPE_UNSPECIFIED"
+    TEST_RUN = "CONFIG_TYPE_TEST_RUN"
+    TEST_SUITE = "CONFIG_TYPE_TEST_SUITE"
+    TEST_RUN_INCREMENTAL = "CONFIG_TYPE_TEST_RUN_INCREMENTAL"
+    PROFILING = "CONFIG_TYPE_PROFILING"
+    DATA_PROFILING = "CONFIG_TYPE_DATA_PROFILING"
+    MODEL_PROFILING = "CONFIG_TYPE_MODEL_PROFILING"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """StatedbJobStatus - a model defined in Swagger"""  # noqa: E501
+        """RimeConfigType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -65,15 +65,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(StatedbJobStatus, dict):
+        if issubclass(RimeConfigType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -81,15 +81,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, StatedbJobStatus):
+        if not isinstance(other, RimeConfigType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/tags_name_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/tags_name_body.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,44 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunTestCategoryType(object):
+class RimeDeactivateAgentResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
-
-    """
-    allowed enum values
-    """
-    UNSPECIFIED = "TEST_CATEGORY_TYPE_UNSPECIFIED"
-    ABNORMAL_INPUTS = "TEST_CATEGORY_TYPE_ABNORMAL_INPUTS"
-    ADVERSARIAL = "TEST_CATEGORY_TYPE_ADVERSARIAL"
-    BIAS_AND_FAIRNESS = "TEST_CATEGORY_TYPE_BIAS_AND_FAIRNESS"
-    DATA_CLEANLINESS = "TEST_CATEGORY_TYPE_DATA_CLEANLINESS"
-    DRIFT = "TEST_CATEGORY_TYPE_DRIFT"
-    MODEL_PERFORMANCE = "TEST_CATEGORY_TYPE_MODEL_PERFORMANCE"
-    DATA_POISONING_DETECTION = "TEST_CATEGORY_TYPE_DATA_POISONING_DETECTION"
-    SUBSET_PERFORMANCE = "TEST_CATEGORY_TYPE_SUBSET_PERFORMANCE"
-    SUBSET_PERFORMANCE_DEGRADATION = "TEST_CATEGORY_TYPE_SUBSET_PERFORMANCE_DEGRADATION"
-    TRANSFORMATIONS = "TEST_CATEGORY_TYPE_TRANSFORMATIONS"
-    EVASION_ATTACK_DETECTION = "TEST_CATEGORY_TYPE_EVASION_ATTACK_DETECTION"
-    CUSTOM = "TEST_CATEGORY_TYPE_CUSTOM"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """TestrunTestCategoryType - a model defined in Swagger"""  # noqa: E501
+        """RimeDeactivateAgentResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -71,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunTestCategoryType, dict):
+        if issubclass(RimeDeactivateAgentResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -87,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunTestCategoryType):
+        if not isinstance(other, RimeDeactivateAgentResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
@@ -26,15 +26,15 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'run_name': 'str',
         'model_id': 'RimeUUID',
-        'data_info': 'SchematestrunDataInfo',
+        'data_info': 'TestrunRefEvalDatasets',
         'run_time_info': 'RuntimeinfoRunTimeInfo',
         'profiling_config': 'TestrunProfilingConfig',
         'test_suite_config': 'TestrunTestSuiteConfig',
         'categories': 'list[TestrunTestCategoryType]'
     }
 
     attribute_map = {
@@ -119,25 +119,25 @@
 
     @property
     def data_info(self):
         """Gets the data_info of this TestrunTestRunConfig.  # noqa: E501
 
 
         :return: The data_info of this TestrunTestRunConfig.  # noqa: E501
-        :rtype: SchematestrunDataInfo
+        :rtype: TestrunRefEvalDatasets
         """
         return self._data_info
 
     @data_info.setter
     def data_info(self, data_info):
         """Sets the data_info of this TestrunTestRunConfig.
 
 
         :param data_info: The data_info of this TestrunTestRunConfig.  # noqa: E501
-        :type: SchematestrunDataInfo
+        :type: TestrunRefEvalDatasets
         """
         if data_info is None:
             raise ValueError("Invalid value for `data_info`, must not be `None`")  # noqa: E501
 
         self._data_info = data_info
 
     @property
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,71 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunTestSensitivity(object):
+class TestrunresultGetTestRunResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
-
-    """
-    allowed enum values
-    """
-    UNSPECIFIED = "TEST_SENSITIVITY_UNSPECIFIED"
-    LESS_SENSITIVE = "TEST_SENSITIVITY_LESS_SENSITIVE"
-    DEFAULT = "TEST_SENSITIVITY_DEFAULT"
-    MORE_SENSITIVE = "TEST_SENSITIVITY_MORE_SENSITIVE"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'test_run': 'TestrunresultTestRunDetail'
     }
 
     attribute_map = {
+        'test_run': 'testRun'
     }
 
-    def __init__(self):  # noqa: E501
-        """TestrunTestSensitivity - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, test_run=None):  # noqa: E501
+        """TestrunresultGetTestRunResponse - a model defined in Swagger"""  # noqa: E501
+        self._test_run = None
         self.discriminator = None
+        if test_run is not None:
+            self.test_run = test_run
+
+    @property
+    def test_run(self):
+        """Gets the test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
+
+
+        :return: The test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
+        :rtype: TestrunresultTestRunDetail
+        """
+        return self._test_run
+
+    @test_run.setter
+    def test_run(self, test_run):
+        """Sets the test_run of this TestrunresultGetTestRunResponse.
+
+
+        :param test_run: The test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
+        :type: TestrunresultTestRunDetail
+        """
+
+        self._test_run = test_run
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -62,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunTestSensitivity, dict):
+        if issubclass(TestrunresultGetTestRunResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunTestSensitivity):
+        if not isinstance(other, TestrunresultGetTestRunResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunresultGetTestRunResponse(object):
+class TestrunresultRenameTestRunResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,36 +32,36 @@
     }
 
     attribute_map = {
         'test_run': 'testRun'
     }
 
     def __init__(self, test_run=None):  # noqa: E501
-        """TestrunresultGetTestRunResponse - a model defined in Swagger"""  # noqa: E501
+        """TestrunresultRenameTestRunResponse - a model defined in Swagger"""  # noqa: E501
         self._test_run = None
         self.discriminator = None
         if test_run is not None:
             self.test_run = test_run
 
     @property
     def test_run(self):
-        """Gets the test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
+        """Gets the test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
 
 
-        :return: The test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
+        :return: The test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
         :rtype: TestrunresultTestRunDetail
         """
         return self._test_run
 
     @test_run.setter
     def test_run(self, test_run):
-        """Sets the test_run of this TestrunresultGetTestRunResponse.
+        """Sets the test_run of this TestrunresultRenameTestRunResponse.
 
 
-        :param test_run: The test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
+        :param test_run: The test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
         :type: TestrunresultTestRunDetail
         """
 
         self._test_run = test_run
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunresultGetTestRunResponse, dict):
+        if issubclass(TestrunresultRenameTestRunResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunresultGetTestRunResponse):
+        if not isinstance(other, TestrunresultRenameTestRunResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,129 +1,127 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunresultListTestCasesResponse(object):
+class TestrunresultTestCaseDisplay(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'test_cases': 'list[TestrunresultTestCase]',
-        'next_page_token': 'str',
-        'has_more': 'bool'
+        'table_info': 'str',
+        'details': 'str',
+        'details_layout': 'list[str]'
     }
 
     attribute_map = {
-        'test_cases': 'testCases',
-        'next_page_token': 'nextPageToken',
-        'has_more': 'hasMore'
+        'table_info': 'tableInfo',
+        'details': 'details',
+        'details_layout': 'detailsLayout'
     }
 
-    def __init__(self, test_cases=None, next_page_token=None, has_more=None):  # noqa: E501
-        """TestrunresultListTestCasesResponse - a model defined in Swagger"""  # noqa: E501
-        self._test_cases = None
-        self._next_page_token = None
-        self._has_more = None
+    def __init__(self, table_info=None, details=None, details_layout=None):  # noqa: E501
+        """TestrunresultTestCaseDisplay - a model defined in Swagger"""  # noqa: E501
+        self._table_info = None
+        self._details = None
+        self._details_layout = None
         self.discriminator = None
-        if test_cases is not None:
-            self.test_cases = test_cases
-        if next_page_token is not None:
-            self.next_page_token = next_page_token
-        if has_more is not None:
-            self.has_more = has_more
+        if table_info is not None:
+            self.table_info = table_info
+        if details is not None:
+            self.details = details
+        if details_layout is not None:
+            self.details_layout = details_layout
 
     @property
-    def test_cases(self):
-        """Gets the test_cases of this TestrunresultListTestCasesResponse.  # noqa: E501
+    def table_info(self):
+        """Gets the table_info of this TestrunresultTestCaseDisplay.  # noqa: E501
 
-        The list of test cases.  # noqa: E501
+        Table info contains information for displaying the test case in a table in the FE.  # noqa: E501
 
-        :return: The test_cases of this TestrunresultListTestCasesResponse.  # noqa: E501
-        :rtype: list[TestrunresultTestCase]
+        :return: The table_info of this TestrunresultTestCaseDisplay.  # noqa: E501
+        :rtype: str
         """
-        return self._test_cases
+        return self._table_info
 
-    @test_cases.setter
-    def test_cases(self, test_cases):
-        """Sets the test_cases of this TestrunresultListTestCasesResponse.
+    @table_info.setter
+    def table_info(self, table_info):
+        """Sets the table_info of this TestrunresultTestCaseDisplay.
 
-        The list of test cases.  # noqa: E501
+        Table info contains information for displaying the test case in a table in the FE.  # noqa: E501
 
-        :param test_cases: The test_cases of this TestrunresultListTestCasesResponse.  # noqa: E501
-        :type: list[TestrunresultTestCase]
+        :param table_info: The table_info of this TestrunresultTestCaseDisplay.  # noqa: E501
+        :type: str
         """
 
-        self._test_cases = test_cases
+        self._table_info = table_info
 
     @property
-    def next_page_token(self):
-        """Gets the next_page_token of this TestrunresultListTestCasesResponse.  # noqa: E501
+    def details(self):
+        """Gets the details of this TestrunresultTestCaseDisplay.  # noqa: E501
 
-        A token representing the next page from the list returned by a ListTestCases query.  # noqa: E501
+        Details includes ML-specified details for the test case. This can include graphs, HTML, etc.  # noqa: E501
 
-        :return: The next_page_token of this TestrunresultListTestCasesResponse.  # noqa: E501
+        :return: The details of this TestrunresultTestCaseDisplay.  # noqa: E501
         :rtype: str
         """
-        return self._next_page_token
+        return self._details
 
-    @next_page_token.setter
-    def next_page_token(self, next_page_token):
-        """Sets the next_page_token of this TestrunresultListTestCasesResponse.
+    @details.setter
+    def details(self, details):
+        """Sets the details of this TestrunresultTestCaseDisplay.
 
-        A token representing the next page from the list returned by a ListTestCases query.  # noqa: E501
+        Details includes ML-specified details for the test case. This can include graphs, HTML, etc.  # noqa: E501
 
-        :param next_page_token: The next_page_token of this TestrunresultListTestCasesResponse.  # noqa: E501
+        :param details: The details of this TestrunresultTestCaseDisplay.  # noqa: E501
         :type: str
         """
 
-        self._next_page_token = next_page_token
+        self._details = details
 
     @property
-    def has_more(self):
-        """Gets the has_more of this TestrunresultListTestCasesResponse.  # noqa: E501
+    def details_layout(self):
+        """Gets the details_layout of this TestrunresultTestCaseDisplay.  # noqa: E501
 
-        A Boolean flag that specifies whether there are more test cases to return.  # noqa: E501
 
-        :return: The has_more of this TestrunresultListTestCasesResponse.  # noqa: E501
-        :rtype: bool
+        :return: The details_layout of this TestrunresultTestCaseDisplay.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._has_more
+        return self._details_layout
 
-    @has_more.setter
-    def has_more(self, has_more):
-        """Sets the has_more of this TestrunresultListTestCasesResponse.
+    @details_layout.setter
+    def details_layout(self, details_layout):
+        """Sets the details_layout of this TestrunresultTestCaseDisplay.
 
-        A Boolean flag that specifies whether there are more test cases to return.  # noqa: E501
 
-        :param has_more: The has_more of this TestrunresultListTestCasesResponse.  # noqa: E501
-        :type: bool
+        :param details_layout: The details_layout of this TestrunresultTestCaseDisplay.  # noqa: E501
+        :type: list[str]
         """
 
-        self._has_more = has_more
+        self._details_layout = details_layout
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -138,15 +136,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunresultListTestCasesResponse, dict):
+        if issubclass(TestrunresultTestCaseDisplay, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -154,15 +152,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunresultListTestCasesResponse):
+        if not isinstance(other, TestrunresultTestCaseDisplay):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,129 +1,185 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunresultListTestRunsResponse(object):
+class TestrunresultResultSummaryCounts(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'test_runs': 'list[TestrunresultTestRunDetail]',
-        'next_page_token': 'str',
-        'has_more': 'bool'
+        'total': 'str',
+        '_pass': 'str',
+        'warning': 'str',
+        'fail': 'str',
+        'skip': 'str'
     }
 
     attribute_map = {
-        'test_runs': 'testRuns',
-        'next_page_token': 'nextPageToken',
-        'has_more': 'hasMore'
+        'total': 'total',
+        '_pass': 'pass',
+        'warning': 'warning',
+        'fail': 'fail',
+        'skip': 'skip'
     }
 
-    def __init__(self, test_runs=None, next_page_token=None, has_more=None):  # noqa: E501
-        """TestrunresultListTestRunsResponse - a model defined in Swagger"""  # noqa: E501
-        self._test_runs = None
-        self._next_page_token = None
-        self._has_more = None
+    def __init__(self, total=None, _pass=None, warning=None, fail=None, skip=None):  # noqa: E501
+        """TestrunresultResultSummaryCounts - a model defined in Swagger"""  # noqa: E501
+        self._total = None
+        self.__pass = None
+        self._warning = None
+        self._fail = None
+        self._skip = None
         self.discriminator = None
-        if test_runs is not None:
-            self.test_runs = test_runs
-        if next_page_token is not None:
-            self.next_page_token = next_page_token
-        if has_more is not None:
-            self.has_more = has_more
+        if total is not None:
+            self.total = total
+        if _pass is not None:
+            self._pass = _pass
+        if warning is not None:
+            self.warning = warning
+        if fail is not None:
+            self.fail = fail
+        if skip is not None:
+            self.skip = skip
 
     @property
-    def test_runs(self):
-        """Gets the test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
+    def total(self):
+        """Gets the total of this TestrunresultResultSummaryCounts.  # noqa: E501
 
-        The details of the test runs.  # noqa: E501
+        The total number of tests.  # noqa: E501
 
-        :return: The test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
-        :rtype: list[TestrunresultTestRunDetail]
+        :return: The total of this TestrunresultResultSummaryCounts.  # noqa: E501
+        :rtype: str
+        """
+        return self._total
+
+    @total.setter
+    def total(self, total):
+        """Sets the total of this TestrunresultResultSummaryCounts.
+
+        The total number of tests.  # noqa: E501
+
+        :param total: The total of this TestrunresultResultSummaryCounts.  # noqa: E501
+        :type: str
+        """
+
+        self._total = total
+
+    @property
+    def _pass(self):
+        """Gets the _pass of this TestrunresultResultSummaryCounts.  # noqa: E501
+
+        The number of tests that pass.  # noqa: E501
+
+        :return: The _pass of this TestrunresultResultSummaryCounts.  # noqa: E501
+        :rtype: str
+        """
+        return self.__pass
+
+    @_pass.setter
+    def _pass(self, _pass):
+        """Sets the _pass of this TestrunresultResultSummaryCounts.
+
+        The number of tests that pass.  # noqa: E501
+
+        :param _pass: The _pass of this TestrunresultResultSummaryCounts.  # noqa: E501
+        :type: str
+        """
+
+        self.__pass = _pass
+
+    @property
+    def warning(self):
+        """Gets the warning of this TestrunresultResultSummaryCounts.  # noqa: E501
+
+        The number of tests that raise a warning.  # noqa: E501
+
+        :return: The warning of this TestrunresultResultSummaryCounts.  # noqa: E501
+        :rtype: str
         """
-        return self._test_runs
+        return self._warning
 
-    @test_runs.setter
-    def test_runs(self, test_runs):
-        """Sets the test_runs of this TestrunresultListTestRunsResponse.
+    @warning.setter
+    def warning(self, warning):
+        """Sets the warning of this TestrunresultResultSummaryCounts.
 
-        The details of the test runs.  # noqa: E501
+        The number of tests that raise a warning.  # noqa: E501
 
-        :param test_runs: The test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
-        :type: list[TestrunresultTestRunDetail]
+        :param warning: The warning of this TestrunresultResultSummaryCounts.  # noqa: E501
+        :type: str
         """
 
-        self._test_runs = test_runs
+        self._warning = warning
 
     @property
-    def next_page_token(self):
-        """Gets the next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
+    def fail(self):
+        """Gets the fail of this TestrunresultResultSummaryCounts.  # noqa: E501
 
-        A token representing the next page from the list returned by a ListTestRuns query.  # noqa: E501
+        The number of tests that fail.  # noqa: E501
 
-        :return: The next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
+        :return: The fail of this TestrunresultResultSummaryCounts.  # noqa: E501
         :rtype: str
         """
-        return self._next_page_token
+        return self._fail
 
-    @next_page_token.setter
-    def next_page_token(self, next_page_token):
-        """Sets the next_page_token of this TestrunresultListTestRunsResponse.
+    @fail.setter
+    def fail(self, fail):
+        """Sets the fail of this TestrunresultResultSummaryCounts.
 
-        A token representing the next page from the list returned by a ListTestRuns query.  # noqa: E501
+        The number of tests that fail.  # noqa: E501
 
-        :param next_page_token: The next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
+        :param fail: The fail of this TestrunresultResultSummaryCounts.  # noqa: E501
         :type: str
         """
 
-        self._next_page_token = next_page_token
+        self._fail = fail
 
     @property
-    def has_more(self):
-        """Gets the has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
+    def skip(self):
+        """Gets the skip of this TestrunresultResultSummaryCounts.  # noqa: E501
 
-        A Boolean that specifies whether there are more test runs to return.  # noqa: E501
+        The number of tests that are skipped.  # noqa: E501
 
-        :return: The has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
-        :rtype: bool
+        :return: The skip of this TestrunresultResultSummaryCounts.  # noqa: E501
+        :rtype: str
         """
-        return self._has_more
+        return self._skip
 
-    @has_more.setter
-    def has_more(self, has_more):
-        """Sets the has_more of this TestrunresultListTestRunsResponse.
+    @skip.setter
+    def skip(self, skip):
+        """Sets the skip of this TestrunresultResultSummaryCounts.
 
-        A Boolean that specifies whether there are more test runs to return.  # noqa: E501
+        The number of tests that are skipped.  # noqa: E501
 
-        :param has_more: The has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
-        :type: bool
+        :param skip: The skip of this TestrunresultResultSummaryCounts.  # noqa: E501
+        :type: str
         """
 
-        self._has_more = has_more
+        self._skip = skip
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -138,15 +194,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunresultListTestRunsResponse, dict):
+        if issubclass(TestrunresultResultSummaryCounts, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -154,15 +210,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunresultListTestRunsResponse):
+        if not isinstance(other, TestrunresultResultSummaryCounts):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/user_private_info.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunresultRenameTestRunResponse(object):
+class UserPrivateInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'test_run': 'TestrunresultTestRunDetail'
+        'favorite_projects': 'list[UserFavoriteProjects]'
     }
 
     attribute_map = {
-        'test_run': 'testRun'
+        'favorite_projects': 'favoriteProjects'
     }
 
-    def __init__(self, test_run=None):  # noqa: E501
-        """TestrunresultRenameTestRunResponse - a model defined in Swagger"""  # noqa: E501
-        self._test_run = None
+    def __init__(self, favorite_projects=None):  # noqa: E501
+        """UserPrivateInfo - a model defined in Swagger"""  # noqa: E501
+        self._favorite_projects = None
         self.discriminator = None
-        if test_run is not None:
-            self.test_run = test_run
+        if favorite_projects is not None:
+            self.favorite_projects = favorite_projects
 
     @property
-    def test_run(self):
-        """Gets the test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
+    def favorite_projects(self):
+        """Gets the favorite_projects of this UserPrivateInfo.  # noqa: E501
 
 
-        :return: The test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
-        :rtype: TestrunresultTestRunDetail
+        :return: The favorite_projects of this UserPrivateInfo.  # noqa: E501
+        :rtype: list[UserFavoriteProjects]
         """
-        return self._test_run
+        return self._favorite_projects
 
-    @test_run.setter
-    def test_run(self, test_run):
-        """Sets the test_run of this TestrunresultRenameTestRunResponse.
+    @favorite_projects.setter
+    def favorite_projects(self, favorite_projects):
+        """Sets the favorite_projects of this UserPrivateInfo.
 
 
-        :param test_run: The test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
-        :type: TestrunresultTestRunDetail
+        :param favorite_projects: The favorite_projects of this UserPrivateInfo.  # noqa: E501
+        :type: list[UserFavoriteProjects]
         """
 
-        self._test_run = test_run
+        self._favorite_projects = favorite_projects
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunresultRenameTestRunResponse, dict):
+        if issubclass(UserPrivateInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunresultRenameTestRunResponse):
+        if not isinstance(other, UserPrivateInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
@@ -420,26 +420,26 @@
 
         self._progress = progress
 
     @property
     def rime_version(self):
         """Gets the rime_version of this TestrunresultTestRunDetail.  # noqa: E501
 
-        The version of RIME that ran this test.  # noqa: E501
+        The version of Robust Intelligence that ran this test.  # noqa: E501
 
         :return: The rime_version of this TestrunresultTestRunDetail.  # noqa: E501
         :rtype: str
         """
         return self._rime_version
 
     @rime_version.setter
     def rime_version(self, rime_version):
         """Sets the rime_version of this TestrunresultTestRunDetail.
 
-        The version of RIME that ran this test.  # noqa: E501
+        The version of Robust Intelligence that ran this test.  # noqa: E501
 
         :param rime_version: The rime_version of this TestrunresultTestRunDetail.  # noqa: E501
         :type: str
         """
 
         self._rime_version = rime_version
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/user_private_info.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,45 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UserPrivateInfo(object):
+class RimeResetPasswordResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'favorite_projects': 'list[UserFavoriteProjects]'
     }
 
     attribute_map = {
-        'favorite_projects': 'favoriteProjects'
     }
 
-    def __init__(self, favorite_projects=None):  # noqa: E501
-        """UserPrivateInfo - a model defined in Swagger"""  # noqa: E501
-        self._favorite_projects = None
+    def __init__(self):  # noqa: E501
+        """RimeResetPasswordResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
-        if favorite_projects is not None:
-            self.favorite_projects = favorite_projects
-
-    @property
-    def favorite_projects(self):
-        """Gets the favorite_projects of this UserPrivateInfo.  # noqa: E501
-
-
-        :return: The favorite_projects of this UserPrivateInfo.  # noqa: E501
-        :rtype: list[UserFavoriteProjects]
-        """
-        return self._favorite_projects
-
-    @favorite_projects.setter
-    def favorite_projects(self, favorite_projects):
-        """Sets the favorite_projects of this UserPrivateInfo.
-
-
-        :param favorite_projects: The favorite_projects of this UserPrivateInfo.  # noqa: E501
-        :type: list[UserFavoriteProjects]
-        """
-
-        self._favorite_projects = favorite_projects
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UserPrivateInfo, dict):
+        if issubclass(RimeResetPasswordResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UserPrivateInfo):
+        if not isinstance(other, RimeResetPasswordResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/user_role.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,97 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UserRole(object):
+class UsersUserIdUuidBody(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
-
-    """
-    allowed enum values
-    """
-    UNSPECIFIED = "ROLE_UNSPECIFIED"
-    ADMIN = "ROLE_ADMIN"
-    TRIAL_USER = "ROLE_TRIAL_USER"
-    SUPPORT = "ROLE_SUPPORT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'user': 'V1usersuserIdUuidUser',
+        'mask': 'RimeUserWriteMask'
     }
 
     attribute_map = {
+        'user': 'user',
+        'mask': 'mask'
     }
 
-    def __init__(self):  # noqa: E501
-        """UserRole - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, user=None, mask=None):  # noqa: E501
+        """UsersUserIdUuidBody - a model defined in Swagger"""  # noqa: E501
+        self._user = None
+        self._mask = None
         self.discriminator = None
+        if user is not None:
+            self.user = user
+        if mask is not None:
+            self.mask = mask
+
+    @property
+    def user(self):
+        """Gets the user of this UsersUserIdUuidBody.  # noqa: E501
+
+
+        :return: The user of this UsersUserIdUuidBody.  # noqa: E501
+        :rtype: V1usersuserIdUuidUser
+        """
+        return self._user
+
+    @user.setter
+    def user(self, user):
+        """Sets the user of this UsersUserIdUuidBody.
+
+
+        :param user: The user of this UsersUserIdUuidBody.  # noqa: E501
+        :type: V1usersuserIdUuidUser
+        """
+
+        self._user = user
+
+    @property
+    def mask(self):
+        """Gets the mask of this UsersUserIdUuidBody.  # noqa: E501
+
+
+        :return: The mask of this UsersUserIdUuidBody.  # noqa: E501
+        :rtype: RimeUserWriteMask
+        """
+        return self._mask
+
+    @mask.setter
+    def mask(self, mask):
+        """Sets the mask of this UsersUserIdUuidBody.
+
+
+        :param mask: The mask of this UsersUserIdUuidBody.  # noqa: E501
+        :type: RimeUserWriteMask
+        """
+
+        self._mask = mask
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -62,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UserRole, dict):
+        if issubclass(UsersUserIdUuidBody, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UserRole):
+        if not isinstance(other, UsersUserIdUuidBody):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/user_user_detail.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/user_user_detail.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,97 +1,99 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UsersUserIdUuidBody(object):
+class UsersUserUserIdUuidBody1(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'user': 'V1usersuserIdUuidUser',
-        'mask': 'RimeUserWriteMask'
+        'workspace_id': 'object',
+        'user': 'V1projectsprojectIdUuidroleusersuserUserIdUuidUser'
     }
 
     attribute_map = {
-        'user': 'user',
-        'mask': 'mask'
+        'workspace_id': 'workspaceId',
+        'user': 'user'
     }
 
-    def __init__(self, user=None, mask=None):  # noqa: E501
-        """UsersUserIdUuidBody - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, workspace_id=None, user=None):  # noqa: E501
+        """UsersUserUserIdUuidBody1 - a model defined in Swagger"""  # noqa: E501
+        self._workspace_id = None
         self._user = None
-        self._mask = None
         self.discriminator = None
+        if workspace_id is not None:
+            self.workspace_id = workspace_id
         if user is not None:
             self.user = user
-        if mask is not None:
-            self.mask = mask
 
     @property
-    def user(self):
-        """Gets the user of this UsersUserIdUuidBody.  # noqa: E501
+    def workspace_id(self):
+        """Gets the workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
 
+        Unique ID of an object in RIME.  # noqa: E501
 
-        :return: The user of this UsersUserIdUuidBody.  # noqa: E501
-        :rtype: V1usersuserIdUuidUser
+        :return: The workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :rtype: object
         """
-        return self._user
+        return self._workspace_id
 
-    @user.setter
-    def user(self, user):
-        """Sets the user of this UsersUserIdUuidBody.
+    @workspace_id.setter
+    def workspace_id(self, workspace_id):
+        """Sets the workspace_id of this UsersUserUserIdUuidBody1.
 
+        Unique ID of an object in RIME.  # noqa: E501
 
-        :param user: The user of this UsersUserIdUuidBody.  # noqa: E501
-        :type: V1usersuserIdUuidUser
+        :param workspace_id: The workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :type: object
         """
 
-        self._user = user
+        self._workspace_id = workspace_id
 
     @property
-    def mask(self):
-        """Gets the mask of this UsersUserIdUuidBody.  # noqa: E501
+    def user(self):
+        """Gets the user of this UsersUserUserIdUuidBody1.  # noqa: E501
 
 
-        :return: The mask of this UsersUserIdUuidBody.  # noqa: E501
-        :rtype: RimeUserWriteMask
+        :return: The user of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :rtype: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
         """
-        return self._mask
+        return self._user
 
-    @mask.setter
-    def mask(self, mask):
-        """Sets the mask of this UsersUserIdUuidBody.
+    @user.setter
+    def user(self, user):
+        """Sets the user of this UsersUserUserIdUuidBody1.
 
 
-        :param mask: The mask of this UsersUserIdUuidBody.  # noqa: E501
-        :type: RimeUserWriteMask
+        :param user: The user of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :type: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
         """
 
-        self._mask = mask
+        self._user = user
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UsersUserIdUuidBody, dict):
+        if issubclass(UsersUserUserIdUuidBody1, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UsersUserIdUuidBody):
+        if not isinstance(other, UsersUserUserIdUuidBody1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,99 +1,99 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UsersUserUserIdUuidBody1(object):
+class V1projectsprojectIdUuidroleusersuserUserIdUuidUser(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'workspace_id': 'object',
-        'user': 'V1projectsprojectIdUuidroleusersuserUserIdUuidUser'
+        'user_id': 'object',
+        'user_role': 'RimeActorRole'
     }
 
     attribute_map = {
-        'workspace_id': 'workspaceId',
-        'user': 'user'
+        'user_id': 'userId',
+        'user_role': 'userRole'
     }
 
-    def __init__(self, workspace_id=None, user=None):  # noqa: E501
-        """UsersUserUserIdUuidBody1 - a model defined in Swagger"""  # noqa: E501
-        self._workspace_id = None
-        self._user = None
+    def __init__(self, user_id=None, user_role=None):  # noqa: E501
+        """V1projectsprojectIdUuidroleusersuserUserIdUuidUser - a model defined in Swagger"""  # noqa: E501
+        self._user_id = None
+        self._user_role = None
         self.discriminator = None
-        if workspace_id is not None:
-            self.workspace_id = workspace_id
-        if user is not None:
-            self.user = user
+        if user_id is not None:
+            self.user_id = user_id
+        if user_role is not None:
+            self.user_role = user_role
 
     @property
-    def workspace_id(self):
-        """Gets the workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+    def user_id(self):
+        """Gets the user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
 
         Unique ID of an object in RIME.  # noqa: E501
 
-        :return: The workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :return: The user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
         :rtype: object
         """
-        return self._workspace_id
+        return self._user_id
 
-    @workspace_id.setter
-    def workspace_id(self, workspace_id):
-        """Sets the workspace_id of this UsersUserUserIdUuidBody1.
+    @user_id.setter
+    def user_id(self, user_id):
+        """Sets the user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.
 
         Unique ID of an object in RIME.  # noqa: E501
 
-        :param workspace_id: The workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :param user_id: The user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
         :type: object
         """
 
-        self._workspace_id = workspace_id
+        self._user_id = user_id
 
     @property
-    def user(self):
-        """Gets the user of this UsersUserUserIdUuidBody1.  # noqa: E501
+    def user_role(self):
+        """Gets the user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
 
 
-        :return: The user of this UsersUserUserIdUuidBody1.  # noqa: E501
-        :rtype: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
+        :return: The user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
+        :rtype: RimeActorRole
         """
-        return self._user
+        return self._user_role
 
-    @user.setter
-    def user(self, user):
-        """Sets the user of this UsersUserUserIdUuidBody1.
+    @user_role.setter
+    def user_role(self, user_role):
+        """Sets the user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.
 
 
-        :param user: The user of this UsersUserUserIdUuidBody1.  # noqa: E501
-        :type: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
+        :param user_role: The user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
+        :type: RimeActorRole
         """
 
-        self._user = user
+        self._user_role = user_role
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -108,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UsersUserUserIdUuidBody1, dict):
+        if issubclass(V1projectsprojectIdUuidroleusersuserUserIdUuidUser, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -124,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UsersUserUserIdUuidBody1):
+        if not isinstance(other, V1projectsprojectIdUuidroleusersuserUserIdUuidUser):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/rest.py` & `rime_sdk-2.1.0rc4/rime_sdk/swagger/swagger_client/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    RIME Rest API
+    Robust Intelligence REST API
 
-    API methods for RIME. Must be authenticated with `rime-api-key` header.  # noqa: E501
+    API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/test_batch.py` & `rime_sdk-2.1.0rc4/rime_sdk/test_batch.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk/test_run.py` & `rime_sdk-2.1.0rc4/rime_sdk/test_run.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc3/rime_sdk.egg-info/PKG-INFO` & `rime_sdk-2.1.0rc4/rime_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime-sdk
-Version: 2.1.0rc3
+Version: 2.1.0rc4
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.1.0rc3/rime_sdk.egg-info/SOURCES.txt` & `rime_sdk-2.1.0rc4/rime_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,15 @@
 rime_sdk/swagger/swagger_client/models/rca_rca_result.py
 rime_sdk/swagger/swagger_client/models/rca_rca_role.py
 rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py
 rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
 rime_sdk/swagger/swagger_client/models/registry_connection_info.py
 rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
 rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
+rime_sdk/swagger/swagger_client/models/registry_data_info.py
 rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
 rime_sdk/swagger/swagger_client/models/registry_data_params.py
 rime_sdk/swagger/swagger_client/models/registry_delta_lake_info.py
 rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
 rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
 rime_sdk/swagger/swagger_client/models/registry_metadata.py
 rime_sdk/swagger/swagger_client/models/registry_model_info.py
@@ -409,16 +410,14 @@
 rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
 rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
 rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
 rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
 rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
 rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
 rime_sdk/swagger/swagger_client/models/schemanotification_config.py
-rime_sdk/swagger/swagger_client/models/schemaregistry_data_info.py
-rime_sdk/swagger/swagger_client/models/schematestrun_data_info.py
 rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
 rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
 rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
 rime_sdk/swagger/swagger_client/models/statedb_job_status.py
 rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
 rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
 rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
@@ -429,14 +428,15 @@
 rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
 rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
 rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
 rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
 rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py
 rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
 rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
+rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py
 rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
 rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
 rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
 rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
 rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
 rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
 rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
```

### Comparing `rime_sdk-2.1.0rc3/setup.py` & `rime_sdk-2.1.0rc4/setup.py`

 * *Files identical despite different names*

