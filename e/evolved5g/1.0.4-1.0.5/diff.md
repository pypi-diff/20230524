# Comparing `tmp/evolved5g-1.0.4.tar.gz` & `tmp/evolved5g-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evolved5g-1.0.4.tar", last modified: Thu Apr 27 09:26:00 2023, max compression
+gzip compressed data, was "evolved5g-1.0.5.tar", last modified: Wed May 24 13:46:16 2023, max compression
```

## Comparing `evolved5g-1.0.4.tar` & `evolved5g-1.0.5.tar`

### file list

```diff
@@ -1,122 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:26:00.782917 evolved5g-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-27 09:25:25.000000 evolved5g-1.0.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-04-27 09:25:25.000000 evolved5g-1.0.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-27 09:25:25.000000 evolved5g-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-27 09:25:25.000000 evolved5g-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16434 2023-04-27 09:26:00.782917 evolved5g-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-27 09:25:25.000000 evolved5g-1.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:26:00.754917 evolved5g-1.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:26:00.754917 evolved5g-1.0.4/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/source/cli.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      687 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/source/history.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:26:00.758917 evolved5g-1.0.4/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)    26395 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/source/images/dummy_html_example.png
--rw-r--r--   0 runner    (1001) docker     (123)   416176 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/source/images/generate.gif
--rw-r--r--   0 runner    (1001) docker     (123)    65839 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/source/images/generate_execution.png
--rw-r--r--   0 runner    (1001) docker     (123)    31097 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/source/images/repo_creation.png
--rw-r--r--   0 runner    (1001) docker     (123)    37613 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/source/images/repo_structure.png
--rw-r--r--   0 runner    (1001) docker     (123)   159902 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/source/images/ssh_gpg.png
--rw-r--r--   0 runner    (1001) docker     (123)    19817 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/source/images/ssh_key.png
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/source/images/ssh_key_button.png
--rw-r--r--   0 runner    (1001) docker     (123)    23732 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/source/images/token1.png
--rw-r--r--   0 runner    (1001) docker     (123)    60688 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/source/images/token2.png
--rw-r--r--   0 runner    (1001) docker     (123)    28301 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/source/images/token3.png
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/source/information.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/source/libraries.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/source/pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-27 09:25:25.000000 evolved5g-1.0.4/docs/source/pre_requisites.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:26:00.762917 evolved5g-1.0.4/evolved5g/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/cli_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    88851 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:26:00.762917 evolved5g-1.0.4/evolved5g/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:26:00.766917 evolved5g-1.0.4/evolved5g/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23967 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/api/cells_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19947 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/api/g_n_bs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19983 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/api/location_frontend_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/api/login_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26635 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/api/monitoring_event_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19433 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/api/paths_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/api/qo_s_information_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27983 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/api/session_with_qo_s_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27373 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/api/u_es_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27801 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/api/ui_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26817 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23913 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/api/utils_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25106 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:26:00.782917 evolved5g-1.0.4/evolved5g/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/accumulated_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/all_of_u_es_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/all_of_ue_create_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/all_of_ue_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/all_of_ue_update_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/all_of_user_plane_event_report_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/as_session_with_qo_s_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/as_session_with_qo_s_subscription_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/body_create_user_open_api_v1_users_open_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/body_login_access_token_api_v1_login_access_token_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/body_reset_password_api_v1_reset_password_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/body_update_user_me_api_v1_users_me_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/cell_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/cell_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/gnb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/gnb_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/gnb_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/location_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/monitoring_event_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/monitoring_event_report_received.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/monitoring_event_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/monitoring_event_subscription_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/monitoring_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/monitoring_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/path_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/path_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/qo_s_monitoring_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/qos_monitoring_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/reporting_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/requested_qo_s_monitoring_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/snssai.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    13716 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/u_es.py
--rw-r--r--   0 runner    (1001) docker     (123)    15941 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/ue.py
--rw-r--r--   0 runner    (1001) docker     (123)    14566 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/ue_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/ue_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/usage_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/user_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/user_plane_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/user_plane_event_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/user_plane_notification_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/user_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/swagger_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-27 09:25:25.000000 evolved5g-1.0.4/evolved5g/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:26:00.762917 evolved5g-1.0.4/evolved5g.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16434 2023-04-27 09:26:00.000000 evolved5g-1.0.4/evolved5g.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-27 09:26:00.000000 evolved5g-1.0.4/evolved5g.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:26:00.000000 evolved5g-1.0.4/evolved5g.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-27 09:26:00.000000 evolved5g-1.0.4/evolved5g.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:25:56.000000 evolved5g-1.0.4/evolved5g.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-27 09:26:00.000000 evolved5g-1.0.4/evolved5g.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 09:26:00.000000 evolved5g-1.0.4/evolved5g.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-27 09:25:25.000000 evolved5g-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-27 09:26:00.782917 evolved5g-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-27 09:25:25.000000 evolved5g-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:46:16.501783 evolved5g-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-24 13:45:36.000000 evolved5g-1.0.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-24 13:45:36.000000 evolved5g-1.0.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-24 13:45:36.000000 evolved5g-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-24 13:45:36.000000 evolved5g-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-05-24 13:46:16.501783 evolved5g-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-24 13:45:36.000000 evolved5g-1.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:46:16.489782 evolved5g-1.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:46:16.489782 evolved5g-1.0.5/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/cli.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      687 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/history.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:46:16.493782 evolved5g-1.0.5/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    26395 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/dummy_html_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)   416176 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/generate.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    65839 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/generate_execution.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31097 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/repo_creation.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37613 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/repo_structure.png
+-rw-r--r--   0 runner    (1001) docker     (123)   159902 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/ssh_gpg.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19817 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/ssh_key.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/ssh_key_button.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23732 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/token1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60688 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/token2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28301 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/images/token3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/information.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/libraries.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-24 13:45:36.000000 evolved5g-1.0.5/docs/source/pre_requisites.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:46:16.493782 evolved5g-1.0.5/evolved5g/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17764 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/cli_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12881 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/nef_and_tsn_api_service_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88921 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:46:16.493782 evolved5g-1.0.5/evolved5g/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:46:16.497782 evolved5g-1.0.5/evolved5g/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23967 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/cells_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19947 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/g_n_bs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19983 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/location_frontend_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/login_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26635 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/monitoring_event_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19433 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/paths_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/qo_s_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27983 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/session_with_qo_s_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27373 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/u_es_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27801 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/ui_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26817 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23913 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api/utils_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25106 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:46:16.501783 evolved5g-1.0.5/evolved5g/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/accumulated_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/all_of_u_es_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/all_of_ue_create_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/all_of_ue_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/all_of_ue_update_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/all_of_user_plane_event_report_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/as_session_with_qo_s_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/as_session_with_qo_s_subscription_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/body_create_user_open_api_v1_users_open_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/body_login_access_token_api_v1_login_access_token_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/body_reset_password_api_v1_reset_password_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/body_update_user_me_api_v1_users_me_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/cell_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/cell_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/gnb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/gnb_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/gnb_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/location_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_event_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_event_report_received.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_event_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_event_subscription_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/path_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/path_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/qo_s_monitoring_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/qos_monitoring_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/reporting_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/requested_qo_s_monitoring_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/snssai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13716 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/u_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15941 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/ue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14566 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/ue_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/ue_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/usage_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/user_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/user_plane_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/user_plane_event_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/user_plane_notification_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/user_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/swagger_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-24 13:45:36.000000 evolved5g-1.0.5/evolved5g/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:46:16.493782 evolved5g-1.0.5/evolved5g.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-05-24 13:46:16.000000 evolved5g-1.0.5/evolved5g.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-05-24 13:46:16.000000 evolved5g-1.0.5/evolved5g.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:46:16.000000 evolved5g-1.0.5/evolved5g.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-24 13:46:16.000000 evolved5g-1.0.5/evolved5g.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:46:12.000000 evolved5g-1.0.5/evolved5g.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-24 13:46:16.000000 evolved5g-1.0.5/evolved5g.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 13:46:16.000000 evolved5g-1.0.5/evolved5g.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-24 13:45:36.000000 evolved5g-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-24 13:46:16.505783 evolved5g-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-24 13:45:36.000000 evolved5g-1.0.5/setup.py
```

### Comparing `evolved5g-1.0.4/CONTRIBUTING.rst` & `evolved5g-1.0.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/HISTORY.rst` & `evolved5g-1.0.5/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 =======
 History
 =======
 
 -------------------
+1.0.5 (2023-05-24)
+-------------------
+* Bug fix on CAPIFProviderConnector. When storing the capif_cert_server.pem the port was hardcoded.
+* Improvement on verification pipelines. Required user and password.
+* TSN verification pipeline added.
+* Validation pipeline included.
+ 
+-------------------
 1.0.4 (2023-04-27)
 -------------------
 * Bug fix on ServiceDiscoverer: When creating the security context we now pass OAUTH as prefSecurityMethod
+
 -------------------
 1.0.3 (2023-04-25)
 -------------------
 * New SDK Class CAPIFLogger, that allows a provider (like NEF Emulator) to save Log information, for example capture incoming requests and responses
 * New SDK Class CAPIFAuditor, that allows a provider (like NEF Emulator) to query the Log, for example filter all the Log information for a given Network APP
 * Added examples of usage for CAPIFLogger and CAPIFAuditor class in examples/nef_logger_and_audit_example.py
 * At CAPIFProviderConnector class when using the publish_services() method, a copy of the published to CAPIF api is saved to the local certificates folder. This is useful if you want to retrieve the relevant CAPIF ids for this service like aef_id or api_id.
```

### Comparing `evolved5g-1.0.4/LICENSE` & `evolved5g-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/PKG-INFO` & `evolved5g-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evolved5g
-Version: 1.0.4
+Version: 1.0.5
 Summary: Evolved5G CLI prototype 
 Home-page: https://github.com/EVOLVED-5G/SDK-CLI
 Author: EVOLVED5G project
 License: Apache Software License 2.0
 Description: *******************
         Evolved5G CLI & SDK
         *******************
@@ -54,17 +54,26 @@
         
         
         =======
         History
         =======
         
         -------------------
+        1.0.5 (2023-05-24)
+        -------------------
+        * Bug fix on CAPIFProviderConnector. When storing the capif_cert_server.pem the port was hardcoded.
+        * Improvement on verification pipelines. Required user and password.
+        * TSN verification pipeline added.
+        * Validation pipeline included.
+         
+        -------------------
         1.0.4 (2023-04-27)
         -------------------
         * Bug fix on ServiceDiscoverer: When creating the security context we now pass OAUTH as prefSecurityMethod
+        
         -------------------
         1.0.3 (2023-04-25)
         -------------------
         * New SDK Class CAPIFLogger, that allows a provider (like NEF Emulator) to save Log information, for example capture incoming requests and responses
         * New SDK Class CAPIFAuditor, that allows a provider (like NEF Emulator) to query the Log, for example filter all the Log information for a given Network APP
         * Added examples of usage for CAPIFLogger and CAPIFAuditor class in examples/nef_logger_and_audit_example.py
         * At CAPIFProviderConnector class when using the publish_services() method, a copy of the published to CAPIF api is saved to the local certificates folder. This is useful if you want to retrieve the relevant CAPIF ids for this service like aef_id or api_id.
```

### Comparing `evolved5g-1.0.4/README.rst` & `evolved5g-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/Makefile` & `evolved5g-1.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/make.bat` & `evolved5g-1.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/source/cli.rst` & `evolved5g-1.0.5/docs/source/cli.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/source/conf.py` & `evolved5g-1.0.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/source/images/dummy_html_example.png` & `evolved5g-1.0.5/docs/source/images/dummy_html_example.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/source/images/generate.gif` & `evolved5g-1.0.5/docs/source/images/generate.gif`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/source/images/generate_execution.png` & `evolved5g-1.0.5/docs/source/images/generate_execution.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/source/images/repo_creation.png` & `evolved5g-1.0.5/docs/source/images/repo_creation.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/source/images/repo_structure.png` & `evolved5g-1.0.5/docs/source/images/repo_structure.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/source/images/ssh_gpg.png` & `evolved5g-1.0.5/docs/source/images/ssh_gpg.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/source/images/ssh_key.png` & `evolved5g-1.0.5/docs/source/images/ssh_key.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/source/images/ssh_key_button.png` & `evolved5g-1.0.5/docs/source/images/ssh_key_button.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/source/images/token1.png` & `evolved5g-1.0.5/docs/source/images/token1.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/source/images/token2.png` & `evolved5g-1.0.5/docs/source/images/token2.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/source/images/token3.png` & `evolved5g-1.0.5/docs/source/images/token3.png`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/source/index.rst` & `evolved5g-1.0.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/source/information.rst` & `evolved5g-1.0.5/docs/source/information.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/source/installation.rst` & `evolved5g-1.0.5/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/source/libraries.rst` & `evolved5g-1.0.5/docs/source/libraries.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/source/pipelines.rst` & `evolved5g-1.0.5/docs/source/pipelines.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/docs/source/pre_requisites.rst` & `evolved5g-1.0.5/docs/source/pre_requisites.rst`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/cli.py` & `evolved5g-1.0.5/evolved5g/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,31 +23,36 @@
     ctx.obj["helper"].generate(config_file)
 
 
 @cli.command()
 @click.option(
     "--mode",
     type=click.Choice(
-        ["build", "deploy", "destroy", "capif_nef", "code_analysis", "security_scan"],
+        ["build", "deploy", "destroy", "capif_nef", "capif_tsn", "code_analysis", "security_scan", "validation"],
         case_sensitive=False,
     ),
 )
 @click.option("--repo", type=str, help="Enter repo name")
+@click.option("--user", type=str, help="Enter your username for pipelines")
+@click.option("--passwd", type=str, help="Enter repo password for pipelines")
+
 @click.pass_context
-def run_verification_tests(ctx, mode, repo):
+def run_verification_tests(ctx, mode, repo, user, passwd):
     """Launch different verification tests"""
-    ctx.obj["helper"].run_verification_tests(mode, repo)
+    ctx.obj["helper"].run_verification_tests(mode, repo, user, passwd)
 
 
 @cli.command()
 @click.option("--id", type=int, help="Enter pipeline id")
+@click.option("--user", type=str, help="Enter your username for pipelines")
+@click.option("--passwd", type=str, help="Enter repo password for pipelines")
 @click.pass_context
-def check_job(ctx, id):
+def check_job(ctx, id, user, passwd):
     """Check the status of a pipeline"""
-    ctx.obj["helper"].check_job(id)
+    ctx.obj["helper"].check_job(id, user, passwd)
 
 
 @cli.command()
 @click.option(
     "--config_file_full_path",
     type=str,
     help="""The configuration file used to register and onboard the NetApp to CAPIF
@@ -66,16 +71,16 @@
                 --csr_state_or_province_name: The StateOrProvinceName that will be used in the generated X.509 certificate
                 --csr_country_name: The CountryName that will be used in the generated X.509 certificate
                 --csr_email_address: The email that will be used in the generated X.509 certificate              
               """,
 )
 @click.pass_context
 def register_and_onboard_to_capif(ctx, config_file_full_path: str):
-
     ctx.obj["helper"].register_and_onboard_to_capif(config_file_full_path)
+    # ctx.obj["helper"].test_capif_and_nef_published_to_capif_endpoints(config_file_full_path)
 
 
 @cli.command()
 @click.option(
     "--config_file_full_path",
     type=str,
     help="""The configuration file used to apply Time-Sensitive Network Functionalities to your NetApp.
```

### Comparing `evolved5g-1.0.4/evolved5g/sdk.py` & `evolved5g-1.0.5/evolved5g/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1155,27 +1155,27 @@
         """
         # add the trailing slash if it is not already there using os.path.join
         self.certificates_folder = os.path.join(certificates_folder.strip(), "")
         self.description = description
         self.csr_common_name = capif_netapp_username
         # make sure the parameters are str
         capif_http_port = str(capif_http_port)
-        capif_https_port = str(capif_https_port)
+        self.capif_https_port = str(capif_https_port)
         if len(capif_http_port) == 0 or int(capif_http_port) == 80:
             self.capif_http_url = "http://" + capif_host.strip() + "/"
         else:
             self.capif_http_url = (
                     "http://" + capif_host.strip() + ":" + capif_http_port.strip() + "/"
             )
 
-        if len(capif_https_port) == 0 or int(capif_https_port) == 443:
+        if len(self.capif_https_port ) == 0 or int(self.capif_https_port ) == 443:
             self.capif_https_url = "https://" + capif_host.strip() + "/"
         else:
             self.capif_https_url = (
-                    "https://" + capif_host.strip() + ":" + capif_https_port.strip() + "/"
+                    "https://" + capif_host.strip() + ":" + self.capif_https_port .strip() + "/"
             )
 
         self.capif_host = capif_host.strip()
         self.capif_netapp_username = capif_netapp_username
         self.capif_netapp_password = capif_netapp_password
 
         self.csr_common_name = csr_common_name
@@ -1197,16 +1197,18 @@
             ca_root.write(bytes(response_payload["certificate"], "utf-8"))
 
     def __store_certificate(self) -> None:
         """
         Retrieves and stores the cert_server.pem from CAPIF
         """
         print("Retrieve capif_cert_server.pem , process may take a few minutes")
-        cmd = "openssl s_client -connect {0}:443  | openssl x509 -text > {1}/capif_cert_server.pem".format(
-            self.capif_host, self.certificates_folder
+        cmd = "openssl s_client -connect {0}:{1}  | openssl x509 -text > {2}/capif_cert_server.pem".format(
+            self.capif_host,
+            self.capif_https_port,
+            self.certificates_folder
         )
         os.system(cmd)
         print("cert_server.pem succesfully generated!")
 
     def __create_private_and_public_keys(self, api_prov_func_role) -> bytes:
         """
         Creates 2 keys in folder folder_to_store_certificates. An api_prov_func_role_private.key and a api_prov_func_role_private.public.csr key"
```

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/__init__.py` & `evolved5g-1.0.5/evolved5g/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/api/__init__.py` & `evolved5g-1.0.5/evolved5g/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/api/cells_api.py` & `evolved5g-1.0.5/evolved5g/swagger_client/api/cells_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/api/default_api.py` & `evolved5g-1.0.5/evolved5g/swagger_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/api/g_n_bs_api.py` & `evolved5g-1.0.5/evolved5g/swagger_client/api/g_n_bs_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/api/location_frontend_api.py` & `evolved5g-1.0.5/evolved5g/swagger_client/api/location_frontend_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/api/login_api.py` & `evolved5g-1.0.5/evolved5g/swagger_client/api/login_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/api/monitoring_event_api_api.py` & `evolved5g-1.0.5/evolved5g/swagger_client/api/monitoring_event_api_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/api/paths_api.py` & `evolved5g-1.0.5/evolved5g/swagger_client/api/paths_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/api/qo_s_information_api.py` & `evolved5g-1.0.5/evolved5g/swagger_client/api/qo_s_information_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/api/session_with_qo_s_api_api.py` & `evolved5g-1.0.5/evolved5g/swagger_client/api/session_with_qo_s_api_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/api/u_es_api.py` & `evolved5g-1.0.5/evolved5g/swagger_client/api/u_es_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/api/ui_api.py` & `evolved5g-1.0.5/evolved5g/swagger_client/api/ui_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/api/users_api.py` & `evolved5g-1.0.5/evolved5g/swagger_client/api/users_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/api/utils_api.py` & `evolved5g-1.0.5/evolved5g/swagger_client/api/utils_api.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/api_client.py` & `evolved5g-1.0.5/evolved5g/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/configuration.py` & `evolved5g-1.0.5/evolved5g/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/__init__.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/accumulated_usage.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/accumulated_usage.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/all_of_u_es_speed.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/all_of_u_es_speed.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/all_of_ue_create_speed.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/all_of_ue_create_speed.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/all_of_ue_speed.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/all_of_ue_speed.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/all_of_ue_update_speed.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/all_of_ue_update_speed.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/all_of_user_plane_event_report_event.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/all_of_user_plane_event_report_event.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/as_session_with_qo_s_subscription.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/as_session_with_qo_s_subscription.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/as_session_with_qo_s_subscription_create.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/as_session_with_qo_s_subscription_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/body_create_user_open_api_v1_users_open_post.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/body_create_user_open_api_v1_users_open_post.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/body_login_access_token_api_v1_login_access_token_post.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/body_login_access_token_api_v1_login_access_token_post.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/body_reset_password_api_v1_reset_password_post.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/body_reset_password_api_v1_reset_password_post.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/body_update_user_me_api_v1_users_me_put.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/body_update_user_me_api_v1_users_me_put.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/cell.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/cell.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/cell_create.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/cell_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/cell_update.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/cell_update.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/gnb.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/gnb.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/gnb_create.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/gnb_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/gnb_update.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/gnb_update.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/http_validation_error.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/location_info.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/location_info.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/monitoring_event_report.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_event_report.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/monitoring_event_report_received.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_event_report_received.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/monitoring_event_subscription.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_event_subscription.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/monitoring_event_subscription_create.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_event_subscription_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/monitoring_notification.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_notification.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/monitoring_type.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/monitoring_type.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/msg.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/msg.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/path.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/path.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/path_create.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/path_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/path_update.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/path_update.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/paths.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/paths.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/point.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/point.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/qo_s_monitoring_report.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/qo_s_monitoring_report.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/qos_monitoring_information.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/qos_monitoring_information.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/reporting_frequency.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/reporting_frequency.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/requested_qo_s_monitoring_parameters.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/requested_qo_s_monitoring_parameters.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/snssai.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/snssai.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/speed.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/speed.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/token.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/token.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/u_es.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/u_es.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/ue.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/ue.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/ue_create.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/ue_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/ue_update.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/ue_update.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/usage_threshold.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/usage_threshold.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/user.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/user.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/user_create.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/user_create.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/user_plane_event.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/user_plane_event.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/user_plane_event_report.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/user_plane_event_report.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/user_plane_notification_data.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/user_plane_notification_data.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/user_update.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/user_update.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/models/validation_error.py` & `evolved5g-1.0.5/evolved5g/swagger_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g/swagger_client/rest.py` & `evolved5g-1.0.5/evolved5g/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `evolved5g-1.0.4/evolved5g.egg-info/PKG-INFO` & `evolved5g-1.0.5/evolved5g.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evolved5g
-Version: 1.0.4
+Version: 1.0.5
 Summary: Evolved5G CLI prototype 
 Home-page: https://github.com/EVOLVED-5G/SDK-CLI
 Author: EVOLVED5G project
 License: Apache Software License 2.0
 Description: *******************
         Evolved5G CLI & SDK
         *******************
@@ -54,17 +54,26 @@
         
         
         =======
         History
         =======
         
         -------------------
+        1.0.5 (2023-05-24)
+        -------------------
+        * Bug fix on CAPIFProviderConnector. When storing the capif_cert_server.pem the port was hardcoded.
+        * Improvement on verification pipelines. Required user and password.
+        * TSN verification pipeline added.
+        * Validation pipeline included.
+         
+        -------------------
         1.0.4 (2023-04-27)
         -------------------
         * Bug fix on ServiceDiscoverer: When creating the security context we now pass OAUTH as prefSecurityMethod
+        
         -------------------
         1.0.3 (2023-04-25)
         -------------------
         * New SDK Class CAPIFLogger, that allows a provider (like NEF Emulator) to save Log information, for example capture incoming requests and responses
         * New SDK Class CAPIFAuditor, that allows a provider (like NEF Emulator) to query the Log, for example filter all the Log information for a given Network APP
         * Added examples of usage for CAPIFLogger and CAPIFAuditor class in examples/nef_logger_and_audit_example.py
         * At CAPIFProviderConnector class when using the publish_services() method, a copy of the published to CAPIF api is saved to the local certificates folder. This is useful if you want to retrieve the relevant CAPIF ids for this service like aef_id or api_id.
```

### Comparing `evolved5g-1.0.4/evolved5g.egg-info/SOURCES.txt` & `evolved5g-1.0.5/evolved5g.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 docs/source/images/ssh_key_button.png
 docs/source/images/token1.png
 docs/source/images/token2.png
 docs/source/images/token3.png
 evolved5g/__init__.py
 evolved5g/cli.py
 evolved5g/cli_helper.py
+evolved5g/nef_and_tsn_api_service_tests.py
 evolved5g/sdk.py
 evolved5g/utils.py
 evolved5g.egg-info/PKG-INFO
 evolved5g.egg-info/SOURCES.txt
 evolved5g.egg-info/dependency_links.txt
 evolved5g.egg-info/entry_points.txt
 evolved5g.egg-info/not-zip-safe
```

### Comparing `evolved5g-1.0.4/setup.py` & `evolved5g-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     include_package_data=True,
     keywords="evolved5g",
     name="evolved5g",
     packages=find_packages(include=["evolved5g", "evolved5g.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/EVOLVED-5G/SDK-CLI",
-    version="1.0.4",
+    version="1.0.5",
     zip_safe=False,
 )
```

