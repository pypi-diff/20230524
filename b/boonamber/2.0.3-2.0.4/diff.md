# Comparing `tmp/boonamber-2.0.3.tar.gz` & `tmp/boonamber-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boonamber-2.0.3.tar", last modified: Fri May 19 13:52:08 2023, max compression
+gzip compressed data, was "boonamber-2.0.4.tar", last modified: Fri May 19 16:49:13 2023, max compression
```

## Comparing `boonamber-2.0.3.tar` & `boonamber-2.0.4.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 13:52:08.926925 boonamber-2.0.3/
--rw-r--r--   0 jimturnquist   (502) staff       (20)     1072 2023-05-19 12:17:41.000000 boonamber-2.0.3/LICENSE
--rw-r--r--   0 jimturnquist   (502) staff       (20)      845 2023-05-19 13:52:08.926793 boonamber-2.0.3/PKG-INFO
--rw-r--r--   0 jimturnquist   (502) staff       (20)      391 2023-05-19 12:58:46.000000 boonamber-2.0.3/README.md
-drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 13:52:08.913848 boonamber-2.0.3/boonamber/
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2124 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/__init__.py
-drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 13:52:08.914812 boonamber-2.0.3/boonamber/util/
--rw-r--r--   0 jimturnquist   (502) staff       (20)      402 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/util/ambererror.py
-drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 13:52:08.914970 boonamber-2.0.3/boonamber/v1/
--rw-r--r--   0 jimturnquist   (502) staff       (20)    48321 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v1/__init__.py
-drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 13:52:08.916669 boonamber-2.0.3/boonamber/v2/
--rw-r--r--   0 jimturnquist   (502) staff       (20)     4450 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/__init__.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)    23478 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/amber_client.py
-drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 13:52:08.917135 boonamber-2.0.3/boonamber/v2/api/
--rw-r--r--   0 jimturnquist   (502) staff       (20)      139 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/api/__init__.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)    92075 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/api/default_api.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)    24975 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/api_client.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     8168 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/configuration.py
-drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 13:52:08.926576 boonamber-2.0.3/boonamber/v2/models/
--rw-r--r--   0 jimturnquist   (502) staff       (20)     4250 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/__init__.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2477 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/amber_state.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)    11774 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/analytic_results.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3659 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/autotuning.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     6030 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/config_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2663 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/delete_model_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3480 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/error.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     8715 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/feature_config.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3880 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/feature_config_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3986 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/feature_root_cause.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3681 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/fusion_feature.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3046 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/get_models_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2712 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/get_nano_status_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2736 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/get_pretrain_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3220 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/get_root_cause_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2704 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/get_status_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)    31255 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/get_summary_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     8967 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/get_version_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     9710 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_amber_status.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     9591 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_autotune.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     6488 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_buffer_stats.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     6625 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_nano.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     7210 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_nano_backend.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     7188 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_nano_config.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3108 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_pattern_memory.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3780 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_recent_ams.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3852 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_recent_analytics.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3816 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_recent_floats.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3780 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_recent_ids.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3846 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_recent_samples.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3804 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_recent_times.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     9886 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_streaming_parameters.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     6575 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_training.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2326 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/magic_number.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     7172 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/map.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     6827 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/mncp.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     4792 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/model.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     9003 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/model_status.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)    10035 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/nano_status.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2346 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/percent_variation.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     6232 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_config_request.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2732 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_config_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     4149 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_data_request.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3646 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_data_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3032 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_learning_request.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3671 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_learning_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3147 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_model_copy_request.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3131 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_model_request.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2655 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_model_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     4048 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_oauth2_access_request.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     5888 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_oauth2_access_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3326 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_oauth2_refresh_request.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     5908 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_oauth2_refresh_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     4959 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_pretrain_request.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     4189 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_pretrain_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     4077 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/pretrain_status.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     4525 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/put_data_request.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     4330 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/put_data_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3045 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/put_model_request.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2342 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/streaming_window.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     8682 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/training_config.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2334 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/version_number.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)    12835 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/rest.py
-drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 13:52:08.914689 boonamber-2.0.3/boonamber.egg-info/
--rw-r--r--   0 jimturnquist   (502) staff       (20)      845 2023-05-19 13:52:08.000000 boonamber-2.0.3/boonamber.egg-info/PKG-INFO
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2962 2023-05-19 13:52:08.000000 boonamber-2.0.3/boonamber.egg-info/SOURCES.txt
--rw-r--r--   0 jimturnquist   (502) staff       (20)        1 2023-05-19 13:52:08.000000 boonamber-2.0.3/boonamber.egg-info/dependency_links.txt
--rw-r--r--   0 jimturnquist   (502) staff       (20)       15 2023-05-19 13:52:08.000000 boonamber-2.0.3/boonamber.egg-info/requires.txt
--rw-r--r--   0 jimturnquist   (502) staff       (20)       10 2023-05-19 13:52:08.000000 boonamber-2.0.3/boonamber.egg-info/top_level.txt
--rw-r--r--   0 jimturnquist   (502) staff       (20)      835 2023-05-19 13:50:56.000000 boonamber-2.0.3/pyproject.toml
--rw-r--r--   0 jimturnquist   (502) staff       (20)       38 2023-05-19 13:52:08.926961 boonamber-2.0.3/setup.cfg
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 16:49:13.951943 boonamber-2.0.4/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     1072 2023-05-19 12:17:41.000000 boonamber-2.0.4/LICENSE
+-rw-r--r--   0 jimturnquist   (502) staff       (20)      973 2023-05-19 16:49:13.951804 boonamber-2.0.4/PKG-INFO
+-rw-r--r--   0 jimturnquist   (502) staff       (20)      519 2023-05-19 16:46:22.000000 boonamber-2.0.4/README.md
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 16:49:13.931172 boonamber-2.0.4/boonamber/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2124 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/__init__.py
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 16:49:13.938036 boonamber-2.0.4/boonamber/util/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)      402 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/util/ambererror.py
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 16:49:13.938197 boonamber-2.0.4/boonamber/v1/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    48321 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v1/__init__.py
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 16:49:13.939890 boonamber-2.0.4/boonamber/v2/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4450 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/__init__.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    23478 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/amber_client.py
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 16:49:13.940387 boonamber-2.0.4/boonamber/v2/api/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)      139 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/api/__init__.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    92075 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/api/default_api.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    24975 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/api_client.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     8168 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/configuration.py
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 16:49:13.951511 boonamber-2.0.4/boonamber/v2/models/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4250 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/__init__.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2477 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/amber_state.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    11774 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/analytic_results.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3659 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/autotuning.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     6030 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/config_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2663 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/delete_model_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3480 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/error.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     8715 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/feature_config.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3880 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/feature_config_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3986 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/feature_root_cause.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3681 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/fusion_feature.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3046 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/get_models_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2712 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/get_nano_status_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2736 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/get_pretrain_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3220 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/get_root_cause_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2704 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/get_status_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    31255 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/get_summary_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     8967 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/get_version_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     9710 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/m_amber_status.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     9591 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/m_autotune.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     6488 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/m_buffer_stats.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     6625 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/m_nano.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     7210 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/m_nano_backend.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     7188 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/m_nano_config.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3108 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/m_pattern_memory.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3780 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/m_recent_ams.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3852 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/m_recent_analytics.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3816 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/m_recent_floats.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3780 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/m_recent_ids.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3846 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/m_recent_samples.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3804 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/m_recent_times.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     9886 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/m_streaming_parameters.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     6575 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/m_training.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2326 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/magic_number.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     7172 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/map.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     6827 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/mncp.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4792 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/model.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     9003 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/model_status.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    10035 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/nano_status.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2346 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/percent_variation.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     6232 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/post_config_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2732 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/post_config_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4149 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/post_data_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3646 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/post_data_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3032 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/post_learning_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3671 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/post_learning_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3147 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/post_model_copy_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3131 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/post_model_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2655 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/post_model_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4048 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/post_oauth2_access_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     5888 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/post_oauth2_access_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3326 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/post_oauth2_refresh_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     5908 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/post_oauth2_refresh_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4959 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/post_pretrain_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4189 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/post_pretrain_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4077 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/pretrain_status.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4525 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/put_data_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4330 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/put_data_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3045 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/put_model_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2342 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/streaming_window.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     8682 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/training_config.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2334 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/models/version_number.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    12835 2023-05-19 12:17:41.000000 boonamber-2.0.4/boonamber/v2/rest.py
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 16:49:13.937914 boonamber-2.0.4/boonamber.egg-info/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)      973 2023-05-19 16:49:13.000000 boonamber-2.0.4/boonamber.egg-info/PKG-INFO
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2962 2023-05-19 16:49:13.000000 boonamber-2.0.4/boonamber.egg-info/SOURCES.txt
+-rw-r--r--   0 jimturnquist   (502) staff       (20)        1 2023-05-19 16:49:13.000000 boonamber-2.0.4/boonamber.egg-info/dependency_links.txt
+-rw-r--r--   0 jimturnquist   (502) staff       (20)       15 2023-05-19 16:49:13.000000 boonamber-2.0.4/boonamber.egg-info/requires.txt
+-rw-r--r--   0 jimturnquist   (502) staff       (20)       10 2023-05-19 16:49:13.000000 boonamber-2.0.4/boonamber.egg-info/top_level.txt
+-rw-r--r--   0 jimturnquist   (502) staff       (20)      835 2023-05-19 16:47:30.000000 boonamber-2.0.4/pyproject.toml
+-rw-r--r--   0 jimturnquist   (502) staff       (20)       38 2023-05-19 16:49:13.951984 boonamber-2.0.4/setup.cfg
```

### Comparing `boonamber-2.0.3/LICENSE` & `boonamber-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/PKG-INFO` & `boonamber-2.0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,9 @@
-Metadata-Version: 2.1
-Name: boonamber
-Version: 2.0.3
-Summary: An SDK for Boon Amber sensor analytics
-Author: BoonLogic
-Author-email: amber-support@boonlogic.com
-License: MIT
-Project-URL: repository, https://github.com/boonlogic/amber-python-sdk
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-![Logo](docs/BoonLogic.png?raw=true)
+![Logo](https://github.com/boonlogic/amber-python-sdk/blob/master/docs/BoonLogic.png?raw=true)
 
 # Boon Amber Python SDK
 
 Version 2 of Amber Python is Deploying in the spring of 2023.  This SDK will support both v1 and v2 releases.
 v1 users will not see any interface difference when updating to the latest pypi package.
 
-- __Version 1__: [Boon Amber Version 1](boonamber/v1/README.md)
-- __Version 2__: [Boon Amber Version 2](boonamber/v2/README.md)
+- __Version 1__: [Boon Amber Version 1](https://boonlogic.github.io/amber-python-sdk/boonamber/v1)
+- __Version 2__: [Boon Amber Version 2](https://boonlogic.github.io/amber-python-sdk/boonamber/v2)
```

### Comparing `boonamber-2.0.3/boonamber/__init__.py` & `boonamber-2.0.4/boonamber/__init__.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v1/__init__.py` & `boonamber-2.0.4/boonamber/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/__init__.py` & `boonamber-2.0.4/boonamber/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/amber_client.py` & `boonamber-2.0.4/boonamber/v2/amber_client.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/api/default_api.py` & `boonamber-2.0.4/boonamber/v2/api/default_api.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/api_client.py` & `boonamber-2.0.4/boonamber/v2/api_client.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/configuration.py` & `boonamber-2.0.4/boonamber/v2/configuration.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/__init__.py` & `boonamber-2.0.4/boonamber/v2/models/__init__.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/amber_state.py` & `boonamber-2.0.4/boonamber/v2/models/amber_state.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/analytic_results.py` & `boonamber-2.0.4/boonamber/v2/models/analytic_results.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/autotuning.py` & `boonamber-2.0.4/boonamber/v2/models/autotuning.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/config_response.py` & `boonamber-2.0.4/boonamber/v2/models/config_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/delete_model_response.py` & `boonamber-2.0.4/boonamber/v2/models/delete_model_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/error.py` & `boonamber-2.0.4/boonamber/v2/models/error.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/feature_config.py` & `boonamber-2.0.4/boonamber/v2/models/feature_config.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/feature_config_response.py` & `boonamber-2.0.4/boonamber/v2/models/feature_config_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/feature_root_cause.py` & `boonamber-2.0.4/boonamber/v2/models/feature_root_cause.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/fusion_feature.py` & `boonamber-2.0.4/boonamber/v2/models/fusion_feature.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/get_models_response.py` & `boonamber-2.0.4/boonamber/v2/models/get_models_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/get_nano_status_response.py` & `boonamber-2.0.4/boonamber/v2/models/get_nano_status_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/get_pretrain_response.py` & `boonamber-2.0.4/boonamber/v2/models/get_pretrain_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/get_root_cause_response.py` & `boonamber-2.0.4/boonamber/v2/models/get_root_cause_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/get_status_response.py` & `boonamber-2.0.4/boonamber/v2/models/get_status_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/get_summary_response.py` & `boonamber-2.0.4/boonamber/v2/models/get_summary_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/get_version_response.py` & `boonamber-2.0.4/boonamber/v2/models/get_version_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/m_amber_status.py` & `boonamber-2.0.4/boonamber/v2/models/m_amber_status.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/m_autotune.py` & `boonamber-2.0.4/boonamber/v2/models/m_autotune.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/m_buffer_stats.py` & `boonamber-2.0.4/boonamber/v2/models/m_buffer_stats.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/m_nano.py` & `boonamber-2.0.4/boonamber/v2/models/m_nano.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/m_nano_backend.py` & `boonamber-2.0.4/boonamber/v2/models/m_nano_backend.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/m_nano_config.py` & `boonamber-2.0.4/boonamber/v2/models/m_nano_config.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/m_pattern_memory.py` & `boonamber-2.0.4/boonamber/v2/models/m_pattern_memory.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/m_recent_ams.py` & `boonamber-2.0.4/boonamber/v2/models/m_recent_ams.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/m_recent_analytics.py` & `boonamber-2.0.4/boonamber/v2/models/m_recent_analytics.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/m_recent_floats.py` & `boonamber-2.0.4/boonamber/v2/models/m_recent_floats.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/m_recent_ids.py` & `boonamber-2.0.4/boonamber/v2/models/m_recent_ids.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/m_recent_samples.py` & `boonamber-2.0.4/boonamber/v2/models/m_recent_samples.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/m_recent_times.py` & `boonamber-2.0.4/boonamber/v2/models/m_recent_times.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/m_streaming_parameters.py` & `boonamber-2.0.4/boonamber/v2/models/m_streaming_parameters.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/m_training.py` & `boonamber-2.0.4/boonamber/v2/models/m_training.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/magic_number.py` & `boonamber-2.0.4/boonamber/v2/models/magic_number.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/map.py` & `boonamber-2.0.4/boonamber/v2/models/map.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/mncp.py` & `boonamber-2.0.4/boonamber/v2/models/mncp.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/model.py` & `boonamber-2.0.4/boonamber/v2/models/model.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/model_status.py` & `boonamber-2.0.4/boonamber/v2/models/model_status.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/nano_status.py` & `boonamber-2.0.4/boonamber/v2/models/nano_status.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/percent_variation.py` & `boonamber-2.0.4/boonamber/v2/models/percent_variation.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/post_config_request.py` & `boonamber-2.0.4/boonamber/v2/models/post_config_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/post_config_response.py` & `boonamber-2.0.4/boonamber/v2/models/post_config_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/post_data_request.py` & `boonamber-2.0.4/boonamber/v2/models/post_data_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/post_data_response.py` & `boonamber-2.0.4/boonamber/v2/models/post_data_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/post_learning_request.py` & `boonamber-2.0.4/boonamber/v2/models/post_learning_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/post_learning_response.py` & `boonamber-2.0.4/boonamber/v2/models/post_learning_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/post_model_copy_request.py` & `boonamber-2.0.4/boonamber/v2/models/post_model_copy_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/post_model_request.py` & `boonamber-2.0.4/boonamber/v2/models/post_model_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/post_model_response.py` & `boonamber-2.0.4/boonamber/v2/models/post_model_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/post_oauth2_access_request.py` & `boonamber-2.0.4/boonamber/v2/models/post_oauth2_access_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/post_oauth2_access_response.py` & `boonamber-2.0.4/boonamber/v2/models/post_oauth2_access_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/post_oauth2_refresh_request.py` & `boonamber-2.0.4/boonamber/v2/models/post_oauth2_refresh_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/post_oauth2_refresh_response.py` & `boonamber-2.0.4/boonamber/v2/models/post_oauth2_refresh_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/post_pretrain_request.py` & `boonamber-2.0.4/boonamber/v2/models/post_pretrain_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/post_pretrain_response.py` & `boonamber-2.0.4/boonamber/v2/models/post_pretrain_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/pretrain_status.py` & `boonamber-2.0.4/boonamber/v2/models/pretrain_status.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/put_data_request.py` & `boonamber-2.0.4/boonamber/v2/models/put_data_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/put_data_response.py` & `boonamber-2.0.4/boonamber/v2/models/put_data_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/put_model_request.py` & `boonamber-2.0.4/boonamber/v2/models/put_model_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/streaming_window.py` & `boonamber-2.0.4/boonamber/v2/models/streaming_window.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/training_config.py` & `boonamber-2.0.4/boonamber/v2/models/training_config.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/models/version_number.py` & `boonamber-2.0.4/boonamber/v2/models/version_number.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber/v2/rest.py` & `boonamber-2.0.4/boonamber/v2/rest.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/boonamber.egg-info/SOURCES.txt` & `boonamber-2.0.4/boonamber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.3/pyproject.toml` & `boonamber-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "boonamber"
-version = "2.0.3"
+version = "2.0.4"
 authors = [
     {name = "BoonLogic"},
     {email = "amber-support@boonlogic.com"}
 ]
 urls = {repository = "https://github.com/boonlogic/amber-python-sdk"}
 license = {text = "MIT"}
 description = "An SDK for Boon Amber sensor analytics"
```

