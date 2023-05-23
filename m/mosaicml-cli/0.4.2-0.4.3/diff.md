# Comparing `tmp/mosaicml-cli-0.4.2.tar.gz` & `tmp/mosaicml-cli-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.4.2.tar", last modified: Wed May 17 17:05:29 2023, max compression
+gzip compressed data, was "mosaicml-cli-0.4.3.tar", last modified: Tue May 23 23:31:36 2023, max compression
```

## Comparing `mosaicml-cli-0.4.2.tar` & `mosaicml-cli-0.4.3.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.791059 mosaicml-cli-0.4.2/
--rw-r--r--   0 anna       (501) staff       (20)      696 2023-05-17 17:05:29.790904 mosaicml-cli-0.4.2/PKG-INFO
--rw-r--r--   0 anna       (501) staff       (20)     7199 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/README.md
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.764117 mosaicml-cli-0.4.2/mcli/
--rw-r--r--   0 anna       (501) staff       (20)     1794 2023-05-17 17:01:42.000000 mosaicml-cli-0.4.2/mcli/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.764661 mosaicml-cli-0.4.2/mcli/api/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/api/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.765215 mosaicml-cli-0.4.2/mcli/api/cluster/
--rw-r--r--   0 anna       (501) staff       (20)      134 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/api/cluster/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4237 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.765555 mosaicml-cli-0.4.2/mcli/api/engine/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/api/engine/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)    25914 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/api/engine/engine.py
--rw-r--r--   0 anna       (501) staff       (20)    10685 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/api/exceptions.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.767232 mosaicml-cli-0.4.2/mcli/api/inference_deployments/
--rw-r--r--   0 anna       (501) staff       (20)     1023 2023-05-17 17:01:42.000000 mosaicml-cli-0.4.2/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     3301 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 anna       (501) staff       (20)     3179 2023-05-17 17:01:42.000000 mosaicml-cli-0.4.2/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     3582 2023-05-17 17:01:42.000000 mosaicml-cli-0.4.2/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
--rw-r--r--   0 anna       (501) staff       (20)     6138 2023-05-17 17:01:42.000000 mosaicml-cli-0.4.2/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     1319 2023-05-17 17:01:49.000000 mosaicml-cli-0.4.2/mcli/api/inference_deployments/api_ping_inference_deployment.py
--rw-r--r--   0 anna       (501) staff       (20)     1603 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/api/inference_deployments/api_predict_inference_deployment.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.767752 mosaicml-cli-0.4.2/mcli/api/mint/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/api/mint/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     7759 2023-05-09 21:37:54.000000 mosaicml-cli-0.4.2/mcli/api/mint/shell.py
--rw-r--r--   0 anna       (501) staff       (20)     2676 2023-05-09 21:37:54.000000 mosaicml-cli-0.4.2/mcli/api/mint/tty.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.768581 mosaicml-cli-0.4.2/mcli/api/model/
--rw-r--r--   0 anna       (501) staff       (20)     1114 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/api/model/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     6322 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/api/model/cluster_details.py
--rw-r--r--   0 anna       (501) staff       (20)     2992 2023-05-09 21:34:29.000000 mosaicml-cli-0.4.2/mcli/api/model/inference_deployment.py
--rw-r--r--   0 anna       (501) staff       (20)    10439 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/api/model/run.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.770118 mosaicml-cli-0.4.2/mcli/api/runs/
--rw-r--r--   0 anna       (501) staff       (20)     1199 2023-05-09 21:34:29.000000 mosaicml-cli-0.4.2/mcli/api/runs/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2804 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/api/runs/api_create_run.py
--rw-r--r--   0 anna       (501) staff       (20)     4211 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     8405 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 anna       (501) staff       (20)    10933 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     5213 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/api/runs/api_start_run.py
--rw-r--r--   0 anna       (501) staff       (20)     5405 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     3937 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.2/mcli/api/runs/api_update_run_metadata.py
--rw-r--r--   0 anna       (501) staff       (20)    10619 2023-05-09 23:22:09.000000 mosaicml-cli-0.4.2/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.770567 mosaicml-cli-0.4.2/mcli/api/schema/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/api/schema/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)      636 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.771554 mosaicml-cli-0.4.2/mcli/api/secrets/
--rw-r--r--   0 anna       (501) staff       (20)      309 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/api/secrets/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2386 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 anna       (501) staff       (20)     3019 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 anna       (501) staff       (20)     3718 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 anna       (501) staff       (20)     2354 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/api/typing_future.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.771879 mosaicml-cli-0.4.2/mcli/api/users/
--rw-r--r--   0 anna       (501) staff       (20)      139 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/api/users/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2715 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/api/users/api_get_users.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.772139 mosaicml-cli-0.4.2/mcli/cli/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/__init__.py
--rwxr-xr-x   0 anna       (501) staff       (20)     6387 2023-05-17 17:01:49.000000 mosaicml-cli-0.4.2/mcli/cli/cli.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.772619 mosaicml-cli-0.4.2/mcli/cli/common/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/common/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2461 2023-05-09 21:37:54.000000 mosaicml-cli-0.4.2/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 anna       (501) staff       (20)     6874 2023-05-17 17:04:38.000000 mosaicml-cli-0.4.2/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.772961 mosaicml-cli-0.4.2/mcli/cli/m_connect/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1694 2023-05-09 21:37:54.000000 mosaicml-cli-0.4.2/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.773355 mosaicml-cli-0.4.2/mcli/cli/m_create/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/m_create/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2385 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/cli/m_create/m_create.py
--rw-r--r--   0 anna       (501) staff       (20)    16874 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.773909 mosaicml-cli-0.4.2/mcli/cli/m_delete/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     6184 2023-05-17 17:01:49.000000 mosaicml-cli-0.4.2/mcli/cli/m_delete/delete.py
--rw-r--r--   0 anna       (501) staff       (20)     5805 2023-05-17 17:04:38.000000 mosaicml-cli-0.4.2/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.774255 mosaicml-cli-0.4.2/mcli/cli/m_deploy/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     3896 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.774981 mosaicml-cli-0.4.2/mcli/cli/m_describe/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4274 2023-05-17 17:01:42.000000 mosaicml-cli-0.4.2/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     9999 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     2002 2023-05-09 21:37:54.000000 mosaicml-cli-0.4.2/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.776757 mosaicml-cli-0.4.2/mcli/cli/m_get/
--rw-r--r--   0 anna       (501) staff       (20)      467 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/cli/m_get/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     6226 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/cli/m_get/clusters.py
--rw-r--r--   0 anna       (501) staff       (20)     6452 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/m_get/display.py
--rw-r--r--   0 anna       (501) staff       (20)     5642 2023-05-17 17:04:38.000000 mosaicml-cli-0.4.2/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     4803 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/cli/m_get/m_get.py
--rw-r--r--   0 anna       (501) staff       (20)     9790 2023-05-17 17:04:38.000000 mosaicml-cli-0.4.2/mcli/cli/m_get/runs.py
--rw-r--r--   0 anna       (501) staff       (20)     2189 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/cli/m_get/secrets.py
--rw-r--r--   0 anna       (501) staff       (20)     1580 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/m_get/users.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.776992 mosaicml-cli-0.4.2/mcli/cli/m_init/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/m_init/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4115 2023-05-09 21:34:29.000000 mosaicml-cli-0.4.2/mcli/cli/m_init/m_init.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.777854 mosaicml-cli-0.4.2/mcli/cli/m_interactive/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     9325 2023-05-09 21:37:54.000000 mosaicml-cli-0.4.2/mcli/cli/m_interactive/interactive.py
--rw-r--r--   0 anna       (501) staff       (20)    44284 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/cli/m_interactive/kube_config.py
--rw-r--r--   0 anna       (501) staff       (20)     9321 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/cli/m_interactive/m_interactive.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.778735 mosaicml-cli-0.4.2/mcli/cli/m_kube/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-05-17 17:01:49.000000 mosaicml-cli-0.4.2/mcli/cli/m_kube/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     5523 2023-05-17 17:01:49.000000 mosaicml-cli-0.4.2/mcli/cli/m_kube/m_get_config.py
--rw-r--r--   0 anna       (501) staff       (20)     1398 2023-05-17 17:01:49.000000 mosaicml-cli-0.4.2/mcli/cli/m_kube/m_kube.py
--rw-r--r--   0 anna       (501) staff       (20)     2050 2023-05-17 17:01:49.000000 mosaicml-cli-0.4.2/mcli/cli/m_kube/m_merge_config.py
--rw-r--r--   0 anna       (501) staff       (20)     6946 2023-05-17 17:01:49.000000 mosaicml-cli-0.4.2/mcli/cli/m_kube/utils.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.778993 mosaicml-cli-0.4.2/mcli/cli/m_log/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/m_log/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)    10180 2023-05-17 15:15:36.000000 mosaicml-cli-0.4.2/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.779344 mosaicml-cli-0.4.2/mcli/cli/m_ping/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2115 2023-05-17 17:01:42.000000 mosaicml-cli-0.4.2/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.779683 mosaicml-cli-0.4.2/mcli/cli/m_predict/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2610 2023-05-09 21:37:54.000000 mosaicml-cli-0.4.2/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.779914 mosaicml-cli-0.4.2/mcli/cli/m_root/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/m_root/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)      536 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.780160 mosaicml-cli-0.4.2/mcli/cli/m_run/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/m_run/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     8099 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.781138 mosaicml-cli-0.4.2/mcli/cli/m_set_unset/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2973 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.2/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 anna       (501) staff       (20)     1802 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/cli/m_set_unset/feature_flag.py
--rw-r--r--   0 anna       (501) staff       (20)     1940 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 anna       (501) staff       (20)     1421 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 anna       (501) staff       (20)      881 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.781432 mosaicml-cli-0.4.2/mcli/cli/m_stop/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4047 2023-05-17 17:04:38.000000 mosaicml-cli-0.4.2/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.781826 mosaicml-cli-0.4.2/mcli/cli/m_util/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/cli/m_util/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)      797 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/cli/m_util/m_util.py
--rw-r--r--   0 anna       (501) staff       (20)     6837 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/cli/m_util/util.py
--rw-r--r--   0 anna       (501) staff       (20)    12743 2023-05-16 00:10:24.000000 mosaicml-cli-0.4.2/mcli/config.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.782888 mosaicml-cli-0.4.2/mcli/models/
--rw-r--r--   0 anna       (501) staff       (20)     1047 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/models/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2103 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/models/gpu_type.py
--rw-r--r--   0 anna       (501) staff       (20)    10321 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/models/inference_deployment_config.py
--rw-r--r--   0 anna       (501) staff       (20)      427 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/models/mcli_cluster.py
--rw-r--r--   0 anna       (501) staff       (20)      456 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/models/mcli_envvar.py
--rw-r--r--   0 anna       (501) staff       (20)     6724 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/models/mcli_secret.py
--rw-r--r--   0 anna       (501) staff       (20)    19547 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/models/run_config.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.783098 mosaicml-cli-0.4.2/mcli/objects/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/objects/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.784459 mosaicml-cli-0.4.2/mcli/objects/secrets/
--rw-r--r--   0 anna       (501) staff       (20)     1090 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/objects/secrets/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.785670 mosaicml-cli-0.4.2/mcli/objects/secrets/create/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1646 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/objects/secrets/create/base.py
--rw-r--r--   0 anna       (501) staff       (20)     2244 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 anna       (501) staff       (20)     2408 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 anna       (501) staff       (20)     6377 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 anna       (501) staff       (20)     3858 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 anna       (501) staff       (20)     3001 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 anna       (501) staff       (20)     5342 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 anna       (501) staff       (20)      783 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 anna       (501) staff       (20)     1017 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/objects/secrets/env_var.py
--rw-r--r--   0 anna       (501) staff       (20)      556 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/objects/secrets/gcp.py
--rw-r--r--   0 anna       (501) staff       (20)     1267 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/objects/secrets/mounted.py
--rw-r--r--   0 anna       (501) staff       (20)      967 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/objects/secrets/oci.py
--rw-r--r--   0 anna       (501) staff       (20)      961 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/objects/secrets/s3.py
--rw-r--r--   0 anna       (501) staff       (20)     1718 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.785907 mosaicml-cli-0.4.2/mcli/proto/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.2/mcli/proto/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1477 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.2/mcli/proto/mint_pb2.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.786147 mosaicml-cli-0.4.2/mcli/sdk/
--rw-r--r--   0 anna       (501) staff       (20)     1786 2023-05-17 17:01:42.000000 mosaicml-cli-0.4.2/mcli/sdk/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.789224 mosaicml-cli-0.4.2/mcli/utils/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/utils/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     5306 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/utils/utils_cli.py
--rw-r--r--   0 anna       (501) staff       (20)     6073 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.2/mcli/utils/utils_config.py
--rw-r--r--   0 anna       (501) staff       (20)      740 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/utils/utils_date.py
--rw-r--r--   0 anna       (501) staff       (20)    10749 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/utils/utils_docker.py
--rw-r--r--   0 anna       (501) staff       (20)     2225 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/utils/utils_epilog.py
--rw-r--r--   0 anna       (501) staff       (20)    10774 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/utils/utils_interactive.py
--rw-r--r--   0 anna       (501) staff       (20)     4527 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/utils/utils_logging.py
--rw-r--r--   0 anna       (501) staff       (20)     2160 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.2/mcli/utils/utils_message_decoding.py
--rw-r--r--   0 anna       (501) staff       (20)     6614 2023-05-06 11:02:40.000000 mosaicml-cli-0.4.2/mcli/utils/utils_pypi.py
--rw-r--r--   0 anna       (501) staff       (20)     3115 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/utils/utils_rich.py
--rw-r--r--   0 anna       (501) staff       (20)     5035 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/utils/utils_run_status.py
--rw-r--r--   0 anna       (501) staff       (20)     4350 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/utils/utils_serializable_dataclass.py
--rw-r--r--   0 anna       (501) staff       (20)     1103 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/utils/utils_spinner.py
--rw-r--r--   0 anna       (501) staff       (20)    10751 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/utils/utils_string_functions.py
--rw-r--r--   0 anna       (501) staff       (20)     1677 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/mcli/utils/utils_types.py
--rw-r--r--   0 anna       (501) staff       (20)     1001 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/mcli/utils/utils_yaml.py
--rw-r--r--   0 anna       (501) staff       (20)     3885 2023-05-17 17:04:45.000000 mosaicml-cli-0.4.2/mcli/version.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.789978 mosaicml-cli-0.4.2/mosaicml_cli.egg-info/
--rw-r--r--   0 anna       (501) staff       (20)      696 2023-05-17 17:05:29.000000 mosaicml-cli-0.4.2/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 anna       (501) staff       (20)     4822 2023-05-17 17:05:29.000000 mosaicml-cli-0.4.2/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 anna       (501) staff       (20)        1 2023-05-17 17:05:29.000000 mosaicml-cli-0.4.2/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 anna       (501) staff       (20)       75 2023-05-17 17:05:29.000000 mosaicml-cli-0.4.2/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 anna       (501) staff       (20)     1621 2023-05-17 17:05:29.000000 mosaicml-cli-0.4.2/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 anna       (501) staff       (20)        5 2023-05-17 17:05:29.000000 mosaicml-cli-0.4.2/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 anna       (501) staff       (20)    31087 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/pyproject.toml
--rw-r--r--   0 anna       (501) staff       (20)       38 2023-05-17 17:05:29.791099 mosaicml-cli-0.4.2/setup.cfg
--rw-r--r--   0 anna       (501) staff       (20)     3033 2023-05-17 17:01:49.000000 mosaicml-cli-0.4.2/setup.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-05-17 17:05:29.790613 mosaicml-cli-0.4.2/tests/
--rw-r--r--   0 anna       (501) staff       (20)     5991 2023-05-11 23:18:27.000000 mosaicml-cli-0.4.2/tests/test_config.py
--rw-r--r--   0 anna       (501) staff       (20)       62 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/tests/test_simple.py
--rw-r--r--   0 anna       (501) staff       (20)     6116 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.2/tests/test_upgrade.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.594446 mosaicml-cli-0.4.3/
+-rw-r--r--   0 jeffchen   (501) staff       (20)      696 2023-05-23 23:31:36.594271 mosaicml-cli-0.4.3/PKG-INFO
+-rw-r--r--   0 jeffchen   (501) staff       (20)     7187 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.3/README.md
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.557662 mosaicml-cli-0.4.3/mcli/
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1918 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.3/mcli/__init__.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.558260 mosaicml-cli-0.4.3/mcli/api/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.3/mcli/api/__init__.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.558797 mosaicml-cli-0.4.3/mcli/api/cluster/
+-rw-r--r--   0 jeffchen   (501) staff       (20)      134 2022-10-27 20:22:32.000000 mosaicml-cli-0.4.3/mcli/api/cluster/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4237 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.559241 mosaicml-cli-0.4.3/mcli/api/engine/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.3/mcli/api/engine/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    25914 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/api/engine/engine.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    10685 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/api/exceptions.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.561046 mosaicml-cli-0.4.3/mcli/api/inference_deployments/
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1237 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.3/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3301 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     5105 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.3/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3603 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.3/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     8458 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.3/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1277 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.3/mcli/api/inference_deployments/api_ping.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1603 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/api/inference_deployments/api_predict_inference_deployment.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.561546 mosaicml-cli-0.4.3/mcli/api/mint/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.3/mcli/api/mint/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     7759 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/api/mint/shell.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2676 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/api/mint/tty.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.562388 mosaicml-cli-0.4.3/mcli/api/model/
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1114 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/api/model/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6322 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/api/model/cluster_details.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4611 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.3/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    10439 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/api/model/run.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.564108 mosaicml-cli-0.4.3/mcli/api/runs/
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1199 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/api/runs/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2804 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4211 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     8405 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    10933 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     5213 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.3/mcli/api/runs/api_start_run.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     5405 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.3/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3937 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.3/mcli/api/runs/api_update_run_metadata.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    10619 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.3/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.564521 mosaicml-cli-0.4.3/mcli/api/schema/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.3/mcli/api/schema/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      636 2022-11-11 00:18:38.000000 mosaicml-cli-0.4.3/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.565532 mosaicml-cli-0.4.3/mcli/api/secrets/
+-rw-r--r--   0 jeffchen   (501) staff       (20)      309 2022-09-19 22:17:10.000000 mosaicml-cli-0.4.3/mcli/api/secrets/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2386 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3019 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3718 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2354 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.3/mcli/api/typing_future.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.566058 mosaicml-cli-0.4.3/mcli/api/users/
+-rw-r--r--   0 jeffchen   (501) staff       (20)      139 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.3/mcli/api/users/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2715 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/api/users/api_get_users.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.566395 mosaicml-cli-0.4.3/mcli/cli/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.3/mcli/cli/__init__.py
+-rwxr-xr-x   0 jeffchen   (501) staff       (20)     6387 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/cli.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.568638 mosaicml-cli-0.4.3/mcli/cli/common/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-02-01 21:37:29.000000 mosaicml-cli-0.4.3/mcli/cli/common/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2461 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6874 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.568997 mosaicml-cli-0.4.3/mcli/cli/m_connect/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.3/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1694 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.569586 mosaicml-cli-0.4.3/mcli/cli/m_create/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.3/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2385 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    16874 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.570265 mosaicml-cli-0.4.3/mcli/cli/m_delete/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.3/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6184 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     5805 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.570718 mosaicml-cli-0.4.3/mcli/cli/m_deploy/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.3/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3896 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.3/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.571753 mosaicml-cli-0.4.3/mcli/cli/m_describe/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-01-26 01:45:43.000000 mosaicml-cli-0.4.3/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3902 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.3/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     9999 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2002 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.573731 mosaicml-cli-0.4.3/mcli/cli/m_get/
+-rw-r--r--   0 jeffchen   (501) staff       (20)      467 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6226 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6447 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.3/mcli/cli/m_get/display.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     5642 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4803 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     9790 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_get/runs.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2189 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1580 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.3/mcli/cli/m_get/users.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.574371 mosaicml-cli-0.4.3/mcli/cli/m_init/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.3/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4115 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_init/m_init.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.575637 mosaicml-cli-0.4.3/mcli/cli/m_interactive/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.3/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     9325 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_interactive/interactive.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    44284 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_interactive/kube_config.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     9321 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_interactive/m_interactive.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.576810 mosaicml-cli-0.4.3/mcli/cli/m_kube/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_kube/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     5523 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_kube/m_get_config.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1398 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_kube/m_kube.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2050 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_kube/m_merge_config.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6946 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_kube/utils.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.577203 mosaicml-cli-0.4.3/mcli/cli/m_log/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.3/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    10380 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.3/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.577588 mosaicml-cli-0.4.3/mcli/cli/m_ping/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.3/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2091 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.3/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.577956 mosaicml-cli-0.4.3/mcli/cli/m_predict/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.3/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2610 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.578350 mosaicml-cli-0.4.3/mcli/cli/m_root/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.3/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      536 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.578730 mosaicml-cli-0.4.3/mcli/cli/m_run/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.3/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     8099 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.580103 mosaicml-cli-0.4.3/mcli/cli/m_set_unset/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-10-06 23:40:35.000000 mosaicml-cli-0.4.3/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2973 2023-04-18 22:36:16.000000 mosaicml-cli-0.4.3/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1802 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_set_unset/feature_flag.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1940 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1421 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      881 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.3/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.580437 mosaicml-cli-0.4.3/mcli/cli/m_stop/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-27 01:04:20.000000 mosaicml-cli-0.4.3/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4047 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.581574 mosaicml-cli-0.4.3/mcli/cli/m_util/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.3/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      797 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6837 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/cli/m_util/util.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    12590 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.3/mcli/config.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.583050 mosaicml-cli-0.4.3/mcli/models/
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1047 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/models/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2103 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/models/gpu_type.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    10321 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      427 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/models/mcli_cluster.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      456 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/models/mcli_envvar.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6724 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/models/mcli_secret.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    19547 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/models/run_config.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.583337 mosaicml-cli-0.4.3/mcli/objects/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.3/mcli/objects/__init__.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.585514 mosaicml-cli-0.4.3/mcli/objects/secrets/
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1090 2022-12-09 18:28:49.000000 mosaicml-cli-0.4.3/mcli/objects/secrets/__init__.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.587413 mosaicml-cli-0.4.3/mcli/objects/secrets/create/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.3/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1646 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2244 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2408 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6377 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3858 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3001 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     5342 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      783 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1017 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      556 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1267 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      967 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/objects/secrets/oci.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      961 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/objects/secrets/s3.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1718 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.587774 mosaicml-cli-0.4.3/mcli/proto/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/proto/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1477 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/proto/mint_pb2.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.587962 mosaicml-cli-0.4.3/mcli/sdk/
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1744 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.3/mcli/sdk/__init__.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.591942 mosaicml-cli-0.4.3/mcli/utils/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.3/mcli/utils/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     5306 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.3/mcli/utils/utils_cli.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6073 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/utils/utils_config.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      740 2022-09-23 00:37:17.000000 mosaicml-cli-0.4.3/mcli/utils/utils_date.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    10749 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/utils/utils_docker.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2225 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/utils/utils_epilog.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    10774 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/utils/utils_interactive.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4527 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/utils/utils_logging.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2160 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/utils/utils_message_decoding.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6614 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.3/mcli/utils/utils_pypi.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3115 2022-09-08 17:54:07.000000 mosaicml-cli-0.4.3/mcli/utils/utils_rich.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     5035 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/utils/utils_run_status.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4350 2022-09-09 21:35:49.000000 mosaicml-cli-0.4.3/mcli/utils/utils_serializable_dataclass.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1103 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.3/mcli/utils/utils_spinner.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    10751 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1677 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/mcli/utils/utils_types.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1001 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.3/mcli/utils/utils_yaml.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3885 2023-05-23 23:30:13.000000 mosaicml-cli-0.4.3/mcli/version.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.593010 mosaicml-cli-0.4.3/mosaicml_cli.egg-info/
+-rw-r--r--   0 jeffchen   (501) staff       (20)      696 2023-05-23 23:31:36.000000 mosaicml-cli-0.4.3/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4801 2023-05-23 23:31:36.000000 mosaicml-cli-0.4.3/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffchen   (501) staff       (20)        1 2023-05-23 23:31:36.000000 mosaicml-cli-0.4.3/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffchen   (501) staff       (20)       75 2023-05-23 23:31:36.000000 mosaicml-cli-0.4.3/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1655 2023-05-23 23:31:36.000000 mosaicml-cli-0.4.3/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 jeffchen   (501) staff       (20)        5 2023-05-23 23:31:36.000000 mosaicml-cli-0.4.3/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 jeffchen   (501) staff       (20)    31087 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/pyproject.toml
+-rw-r--r--   0 jeffchen   (501) staff       (20)       38 2023-05-23 23:31:36.594504 mosaicml-cli-0.4.3/setup.cfg
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3057 2023-05-23 23:29:40.000000 mosaicml-cli-0.4.3/setup.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-05-23 23:31:36.593849 mosaicml-cli-0.4.3/tests/
+-rw-r--r--   0 jeffchen   (501) staff       (20)     5991 2023-05-23 23:11:05.000000 mosaicml-cli-0.4.3/tests/test_config.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)       62 2022-09-07 04:52:30.000000 mosaicml-cli-0.4.3/tests/test_simple.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6116 2023-04-05 00:11:39.000000 mosaicml-cli-0.4.3/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.4.2/PKG-INFO` & `mosaicml-cli-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.2
+Version: 0.4.3
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.2/README.md` & `mosaicml-cli-0.4.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -132,16 +132,16 @@
 - To get back into your virtual environment: `$ source venv/bin/activate`
 
 ## Running against mcloud as a developer
 
 There are currently 6 MCLI Modes. To use a mode other than the default `PROD`, set your local environment variable `MCLI_MODE` or specify the mode when you run MCLI commands (e.g. `MCLI_MODE=DEV mcli get runs`)
 
 | Mode       | Used By         | MAPI Endpoint                            | Use cases                                              | API Key                                                      |
-| ---------- | --------------- | ---------------------------------------- | ------------------------------------------------------ | ------------------------------------------------------------ | --- |
-| `PROD`     | Default         | https://api.mosaicml.com/graphql         | Demos, simulating customer behavior, integration tests | Create one [here](https://console.mosaicml.com/account#)     |     |
+| ---------- | --------------- | ---------------------------------------- | ------------------------------------------------------ | ------------------------------------------------------------ |
+| `PROD`     | Default         | https://api.mosaicml.com/graphql         | Demos, simulating customer behavior, integration tests | Create one [here](https://console.mosaicml.com/account#)     |
 | `INTERNAL` | Internal users  | https://api.mosaicml.com/graphql         | Internal/alpha features in a prod environment          | Create one [here](https://console.mosaicml.com/account#)     |
 | `STAGING`  | Developers only | https://staging.api.mosaicml.com/graphql | Test changes queued for prod release                   | Testing api key                                              |
 | `DEV`      | Developers only | https://dev.api.mosaicml.com/graphql     | Test against dev branch of mcloud                      | Create one [here](https://dev.console.mosaicml.com/account#) |
 | `LOCAL`    | Developers only | http://localhost:3001/graphql            | Test local mcloud changes                              | Testing api key                                              |
 
 Note for almost all of these modes, you need to set an api key to talk to MAPI:
```

### Comparing `mosaicml-cli-0.4.2/mcli/__init__.py` & `mosaicml-cli-0.4.3/mcli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 """ MCLI Package """
 
 from mcli.api.cluster import get_clusters
 from mcli.api.exceptions import MAPIException
 from mcli.api.inference_deployments import (InferenceDeployment, InferenceDeploymentConfig, create_inference_deployment,
-                                            delete_inference_deployments, get_inference_deployment_logs,
-                                            get_inference_deployments, ping_inference_deployment, predict)
+                                            delete_inference_deployment, delete_inference_deployments,
+                                            get_inference_deployment, get_inference_deployment_logs,
+                                            get_inference_deployments, ping, predict)
 from mcli.api.runs import (FinalRunConfig, Run, RunConfig, RunStatus, create_run, delete_run, delete_runs,
                            follow_run_logs, get_run, get_run_logs, get_runs, start_run, start_runs, stop_run, stop_runs,
                            update_run_metadata, wait_for_run_status, watch_run_status)
 from mcli.api.secrets import create_secret, delete_secrets, get_secrets
 from mcli.cli.m_init.m_init import initialize
 from mcli.cli.m_set_unset.api_key import set_api_key
 from mcli.config import FeatureFlag, MCLIConfig
 
 from .version import __version__
 
 __all__ = [
-    'get_clusters',
-    'MAPIException',
-    'InferenceDeployment',
-    'InferenceDeploymentConfig',
     'create_inference_deployment',
+    'create_run',
+    'create_secret',
+    'delete_inference_deployment',
     'delete_inference_deployments',
+    'delete_run',
+    'delete_runs',
+    'delete_secrets',
+    'FeatureFlag',
+    'FinalRunConfig',
+    'follow_run_logs',
+    'get_clusters',
     'get_inference_deployment_logs',
+    'get_inference_deployment',
     'get_inference_deployments',
-    'ping_inference_deployment',
+    'get_run_logs',
+    'get_run',
+    'get_runs',
+    'get_secrets',
+    'InferenceDeployment',
+    'InferenceDeploymentConfig',
+    'initialize',
+    'MAPIException',
+    'MCLIConfig',
+    'ping',
     'predict',
-    'FinalRunConfig',
     'Run',
     'RunConfig',
     'RunStatus',
-    'create_run',
-    'delete_run',
-    'delete_runs',
-    'follow_run_logs',
-    'get_run',
-    'get_run_logs',
-    'get_runs',
+    'set_api_key',
     'start_run',
     'start_runs',
     'stop_run',
     'stop_runs',
     'update_run_metadata',
     'wait_for_run_status',
     'watch_run_status',
-    'create_secret',
-    'delete_secrets',
-    'get_secrets',
-    'initialize',
-    'set_api_key',
-    'FeatureFlag',
-    'MCLIConfig',
 ]
```

### Comparing `mosaicml-cli-0.4.2/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.4.3/mcli/api/cluster/api_get_clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/engine/engine.py` & `mosaicml-cli-0.4.3/mcli/api/engine/engine.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/exceptions.py` & `mosaicml-cli-0.4.3/mcli/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.4.3/mcli/api/inference_deployments/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 """ API calls for deployment management """
 from mcli.api.inference_deployments.api_create_inference_deployment import create_inference_deployment
-from mcli.api.inference_deployments.api_delete_inference_deployments import delete_inference_deployments
+from mcli.api.inference_deployments.api_delete_inference_deployments import (delete_inference_deployment,
+                                                                             delete_inference_deployments)
 from mcli.api.inference_deployments.api_get_inference_deployment_logs import get_inference_deployment_logs
-from mcli.api.inference_deployments.api_get_inference_deployments import get_inference_deployments
-from mcli.api.inference_deployments.api_ping_inference_deployment import ping_inference_deployment
+from mcli.api.inference_deployments.api_get_inference_deployments import (get_inference_deployment,
+                                                                          get_inference_deployments)
+from mcli.api.inference_deployments.api_ping import ping
 from mcli.api.inference_deployments.api_predict_inference_deployment import predict
 from mcli.api.model.inference_deployment import InferenceDeployment
 from mcli.models import InferenceDeploymentConfig
 
 __all__ = [
-    "InferenceDeployment",
-    "InferenceDeploymentConfig",
     "create_inference_deployment",
+    "delete_inference_deployment",
     "delete_inference_deployments",
-    "get_inference_deployments",
-    "ping_inference_deployment",
     "get_inference_deployment_logs",
+    "get_inference_deployment",
+    "get_inference_deployments",
+    "InferenceDeployment",
+    "InferenceDeploymentConfig",
+    "ping",
     "predict",
 ]
```

### Comparing `mosaicml-cli-0.4.2/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.4.3/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.4.3/mcli/api/inference_deployments/api_get_inference_deployment_logs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,97 +1,91 @@
-""" Delete a deployment. """
+""" Get an inference deployment's logs from the MosaicML platform"""
 from __future__ import annotations
 
 from concurrent.futures import Future
-from typing import List, Optional, Union, overload
+from typing import Any, Dict, Generator, Optional, Union, overload
 
 from typing_extensions import Literal
 
-from mcli.api.engine.engine import get_return_response, run_plural_mapi_request
 from mcli.api.model.inference_deployment import InferenceDeployment
-from mcli.config import MCLIConfig
+from mcli.api.runs.api_get_run_logs import _get_logs
 
-QUERY_FUNCTION = 'deleteInferenceDeployments'
-VARIABLE_DATA_NAME = 'getInferenceDeploymentsData'
+QUERY_FUNCTION = 'getInferenceDeploymentLogs'
+VARIABLE_DATA_NAME = 'getInferenceDeploymentLogsInput'
 QUERY = f"""
-mutation DeleteInferenceDeployments(${VARIABLE_DATA_NAME}: GetInferenceDeploymentsInput!) {{
-  {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
-    id
-    name
-    inferenceDeploymentInput
-    originalInferenceDeploymentInput
-    status
-    createdAt
-    updatedAt
-    deletedAt
-    publicDNS
-    createdByEmail
-  }}
+subscription Subscription(${VARIABLE_DATA_NAME}: GetInferenceDeploymentLogsInput!) {{
+    {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME})
 }}"""
 
-__all__ = ['delete_inference_deployments']
-
 
 @overload
-def delete_inference_deployments(
-    deployments: Union[List[str], List[InferenceDeployment]],
+def get_inference_deployment_logs(
+    deployment: Union[str, InferenceDeployment],
     *,
-    timeout: Optional[float] = 10,
+    restart: Optional[int] = None,
+    timeout: Optional[float] = None,
     future: Literal[False] = False,
-) -> List[InferenceDeployment]:
+) -> Generator[str, None, None]:
     ...
 
 
 @overload
-def delete_inference_deployments(
-    deployments: Union[List[str], List[InferenceDeployment]],
+def get_inference_deployment_logs(
+    deployment: Union[str, InferenceDeployment],
     *,
+    restart: Optional[int] = None,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
-) -> Future[List[InferenceDeployment]]:
+) -> Generator[Future[str], None, None]:
     ...
 
 
-def delete_inference_deployments(
-    deployments: Union[List[str], List[InferenceDeployment]],
+def get_inference_deployment_logs(
+    deployment: Union[str, InferenceDeployment],
     *,
-    timeout: Optional[float] = 10,
+    restart: Optional[int] = None,
+    timeout: Optional[float] = None,
     future: bool = False,
-):
-    """Delete a list of inference deployments in the MosaicML Cloud
-    Any deployments that are currently running will first be stopped.
+) -> Union[Generator[str, None, None], Generator[Future[str], None, None]]:
+    """Get the current logs for an active or completed inference deployment
+
+    Get the current logs for an active or completed inference deployment in the MosaicML platform.
+    This returns the full logs as a ``str``, as they exist at the time the request is
+    made.
+
     Args:
-        deploymnets: A list of inference deployments or inference deployment names to delete
-        timeout: Time, in seconds, in which the call should complete. If the call
-            takes too long, a TimeoutError will be raised. If ``future`` is ``True``, this
-            value will be ignored.
-        future: Return the output as a :type concurrent.futures.Future:. If True, the
-            call to `delete_inference_deployments` will return immediately and the request will be
+        deployment (:obj:`str` | :class:`~mcli.api.model.inference_deployment.InferenceDeployment`): The
+            inference deployment to get logs for. If a name is provided, the remaining required deployment details
+            will be queried with :func:`~mcli.get_inference_deployments`.
+        restart (``Optional[int]``): Which restart of a inference deployment to get logs for. Defaults to the most
+            recent deployment restart.
+        timeout (``Optional[float]``): Time, in seconds, in which the call should complete.
+            If the the call takes too long, a :exc:`~concurrent.futures.TimeoutError`
+            will be raised. If ``future`` is ``True``, this value will be ignored.
+        future (``bool``): Return the output as a :class:`~concurrent.futures.Future` . If True, the
+            call to :func:`get_inference_deployment_logs` will return immediately and the request will be
             processed in the background. This takes precedence over the ``timeout``
-            argument. To get the :type InferenceDeployment: output, use ``return_value.result()``
-            with an optional ``timeout`` argument.
+            argument. To get the log text, use ``return_value.result()`` with an optional
+            ``timeout`` argument.
+
     Returns:
-        A list of :type InferenceDeployment: for the inference deployments that were deleted
+        If future is False:
+            The full log text for a inference deployment at the time of the request as a :obj:`str`
+        Otherwise:
+            A :class:`~concurrent.futures.Future` for the log text
     """
-    # Extract run names
-    deployment_names = [d.name if isinstance(d, InferenceDeployment) else d for d in deployments]
-
-    filters = {}
-    if deployment_names:
-        filters['name'] = {'in': deployment_names}
-
-    variables = {VARIABLE_DATA_NAME: {'filters': filters}}
-
-    cfg = MCLIConfig.load_config(safe=True)
-    if cfg.user_id:
-        variables[VARIABLE_DATA_NAME]['entity'] = {
-            'userIds': [cfg.user_id],
-        }
-
-    response = run_plural_mapi_request(
-        query=QUERY,
-        query_function=QUERY_FUNCTION,
-        return_model_type=InferenceDeployment,
-        variables=variables,
-    )
+    # Convert to strings
+    deployment_name = deployment.name if isinstance(deployment, InferenceDeployment) else deployment
 
-    return get_return_response(response, future=future, timeout=timeout)
+    filters: Dict[str, Any] = {'name': deployment_name}
+    if restart:
+        filters['restartCount'] = restart
+
+    variables = {VARIABLE_DATA_NAME: filters}
+    for message in _get_logs(QUERY, variables, QUERY_FUNCTION):
+        if not future:
+            try:
+                yield message.result(timeout)
+            except StopAsyncIteration:
+                break
+        else:
+            yield message
```

### Comparing `mosaicml-cli-0.4.2/mcli/api/inference_deployments/api_ping_inference_deployment.py` & `mosaicml-cli-0.4.3/mcli/api/inference_deployments/api_ping.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from typing import Optional, Union
 
 import requests
 from requests import Response
 
 from mcli.api.model.inference_deployment import InferenceDeployment
 
-__all__ = ['ping_inference_deployment']
+__all__ = ['ping']
 
 
-def ping_inference_deployment(
+def ping(
     deployment: Union[InferenceDeployment, str],
     *,
     timeout: Optional[float] = 10,
 ) -> dict:
     """Pings an inference deployment that has been launched in the MosaicML platform
     and returns the status of the deployment. The deployment must have a '/ping' endpoint
     defined.
```

### Comparing `mosaicml-cli-0.4.2/mcli/api/inference_deployments/api_predict_inference_deployment.py` & `mosaicml-cli-0.4.3/mcli/api/inference_deployments/api_predict_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/mint/shell.py` & `mosaicml-cli-0.4.3/mcli/api/mint/shell.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/mint/tty.py` & `mosaicml-cli-0.4.3/mcli/api/mint/tty.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/model/__init__.py` & `mosaicml-cli-0.4.3/mcli/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.4.3/mcli/api/model/cluster_details.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.4.3/mcli/cli/m_predict/m_predict.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,74 @@
-"""GraphQL representaion of Deployment"""
-from dataclasses import dataclass
-from datetime import datetime
-from http import HTTPStatus
-from typing import Any, Dict, Optional, Tuple
+"""mcli predict entrypoint"""
+import argparse
+import logging
+from pprint import pprint
+from typing import Any, Callable, Dict, Union, cast
 
-from mcli.api.exceptions import MAPIException
-from mcli.api.schema.generic_model import DeserializableModel, convert_datetime
-from mcli.models.inference_deployment_config import FinalInferenceDeploymentConfig, InferenceDeploymentConfig
+import validators
+import yaml
 
+from mcli.api.exceptions import MAPIException
+from mcli.api.model.inference_deployment import InferenceDeployment
+from mcli.cli.common.deployment_filters import get_deployments_with_filters
+from mcli.sdk import predict
+from mcli.utils.utils_logging import FAIL, err_console
+
+logger = logging.getLogger(__name__)
+
+
+def predict_cli(
+    inputs: Dict[str, Any],
+    deployment: str,
+    **kwargs,
+) -> int:
+    del kwargs
+    try:
+        deployment_obj_or_url: Union[InferenceDeployment, str] = deployment
+        validate_url = cast(Callable[[str], bool], validators.url)
+        if not deployment_obj_or_url or not validate_url(deployment):
+            # if a url is not passed in then lookup the deployment and get the name
+            deployment_objs = get_deployments_with_filters(name_filter=[deployment])
+            if len(deployment_objs) == 0:
+                if not deployment:
+                    err_console.print("No inference deployments found.")
+                else:
+                    err_console.print(f'No inference deployment found with name {deployment}.')
+                return 1
+
+            deployment_obj_or_url = deployment_objs[0]
+
+        resp = predict(deployment_obj_or_url, inputs=inputs)
+        name_or_url = deployment_obj_or_url if isinstance(deployment_obj_or_url, str) else deployment_obj_or_url.name
+        print(f'{name_or_url}\'s prediction results:')
+        pprint(resp)
+        return 0
+    except RuntimeError as e:
+        logger.error(f'{FAIL} {e}')
+        return 1
+    except MAPIException as e:
+        logger.error(f'{FAIL} {e}')
+        return 1
+
+
+def add_predict_parser(subparser: argparse._SubParsersAction):
+    predict_parser: argparse.ArgumentParser = subparser.add_parser(
+        'predict',
+        help='Run prediction on a model in the MosaicML Cloud with given inputs. Returns forward pass result',
+    )
+    predict_parser.add_argument('deployment',
+                                metavar='DEPLOYMENT',
+                                help='The name or url of the deployment to run inference on')
+
+    predict_parser.add_argument(
+        '--input',
+        '--inputs',
+        '-i',
+        dest='inputs',
+        required=True,
+        nargs="?",
+        type=yaml.safe_load,
+        metavar='INPUT',
+        help='Input values to run forward pass on. Input values must be JSON-serializable and have string keys.',
+    )
 
-@dataclass
-class InferenceDeployment(DeserializableModel):
-    """A deployment that has been launched on the MosaicML Cloud
-    
-    Args:
-        deployment_uid (`str`): Unique identifier for the deployment
-        name (`str`): User-defined name of the deployment
-        status (:class:`~mcli.utils.utils_deployment_status.DeploymentStatus`): Status of the deployment
-        at a moment in time
-        created_at (`datetime`): Date and time when the deployment was created
-        updated_at (`datetime`): Date and time when the deployment was last updated
-        config (:class:`~mcli.models.deployment_config.DeploymentConfig`): The
-            :class:`deployment configuration <mcli.models.deployment_config.DeploymentConfig>` that was
-            used to launch to the deployment
-    """
-
-    deployment_uid: str
-    name: str
-    status: str
-    created_at: datetime
-    updated_at: datetime
-    config: FinalInferenceDeploymentConfig
-    created_by: str
-    public_dns: str = ""
-
-    deleted_at: Optional[datetime] = None
-    submitted_config: Optional[InferenceDeploymentConfig] = None
-
-    _required_properties: Tuple[str] = tuple(
-        ['id', 'name', 'status', 'createdAt', 'updatedAt', 'inferenceDeploymentInput', 'publicDNS'])
-
-    @classmethod
-    def from_mapi_response(cls, response: Dict[str, Any]):
-        missing = set(cls._required_properties) - set(response)
-        if missing:
-            raise MAPIException(
-                status=HTTPStatus.BAD_REQUEST,
-                message=f'Missing required key(s) in response to deserialize Deployment object: {", ".join(missing)}',
-            )
-
-        deleted_at = None
-        if response['deletedAt'] is not None:
-            deleted_at = convert_datetime(response['deletedAt'])
-
-        submit_config = None
-        if response.get('originalInferenceDeploymentInput', {}):
-            submit_config = InferenceDeploymentConfig.from_mapi_response(response['originalInferenceDeploymentInput'])
-
-        return cls(deployment_uid=response['id'],
-                   name=response['name'],
-                   created_at=convert_datetime(response['createdAt']),
-                   updated_at=convert_datetime(response['updatedAt']),
-                   deleted_at=deleted_at,
-                   status=response['status'],
-                   public_dns=response['publicDNS'],
-                   created_by=response['createdByEmail'],
-                   config=FinalInferenceDeploymentConfig.from_mapi_response(response['inferenceDeploymentInput']),
-                   submitted_config=submit_config)
+    predict_parser.set_defaults(func=predict_cli)
```

### Comparing `mosaicml-cli-0.4.2/mcli/api/model/run.py` & `mosaicml-cli-0.4.3/mcli/api/model/run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/runs/__init__.py` & `mosaicml-cli-0.4.3/mcli/api/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.4.3/mcli/api/runs/api_create_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.4.3/mcli/api/runs/api_delete_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.4.3/mcli/api/runs/api_get_run_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.4.3/mcli/api/runs/api_get_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/runs/api_start_run.py` & `mosaicml-cli-0.4.3/mcli/api/runs/api_start_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         future (``bool``): Return the output as a :class:`~concurrent.futures.Future`. If True, the
             call to :func:`start_run` will return immediately and the request will be
             processed in the background. This takes precedence over the ``timeout``
             argument. To get the list of :class:`~mcli.api.model.run.Run` output,
             use ``return_value.result()`` with an optional ``timeout`` argument.
 
     Raises:
-        MapiException: Raised if starting the requested runs failed
+        MAPIException: Raised if starting the requested runs failed
             A successfully started run will have the status ```RunStatus.PENDING```
 
     Returns:
         If future is False:
             Started :class:`~mcli.api.model.run.Run` object
         Otherwise:
             A :class:`~concurrent.futures.Future` for the object
@@ -130,15 +130,15 @@
         future (``bool``): Return the output as a :class:`~concurrent.futures.Future`. If True, the
             call to :func:`start_runs` will return immediately and the request will be
             processed in the background. This takes precedence over the ``timeout``
             argument. To get the list of :class:`~mcli.api.model.run.Run` output,
             use ``return_value.result()`` with an optional ``timeout`` argument.
 
     Raises:
-        MapiException: Raised if starting any of the requested runs failed. All
+        MAPIException: Raised if starting any of the requested runs failed. All
             successfully started runs will have the status ```RunStatus.PENDING```. You can
             freely retry any started and started runs if this error is raised due to a
             connection issue.
 
     Returns:
         If future is False:
             A list of started :class:`~mcli.api.model.run.Run` objects
```

### Comparing `mosaicml-cli-0.4.2/mcli/api/runs/api_stop_runs.py` & `mosaicml-cli-0.4.3/mcli/api/runs/api_stop_runs.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         future (``bool``): Return the output as a :class:`~concurrent.futures.Future`. If True, the
             call to :func:`stop_run` will return immediately and the request will be
             processed in the background. This takes precedence over the ``timeout``
             argument. To get the list of :class:`~mcli.api.model.run.Run` output,
             use ``return_value.result()`` with an optional ``timeout`` argument.
 
     Raises:
-        MapiException: Raised if stopping the requested runs failed
+        MAPIException: Raised if stopping the requested runs failed
             A successfully stopped run will have the status ```RunStatus.STOPPED```
 
     Returns:
         If future is False:
             Stopped :class:`~mcli.api.model.run.Run` object
         Otherwise:
             A :class:`~concurrent.futures.Future` for the object
@@ -133,15 +133,15 @@
         future (``bool``): Return the output as a :class:`~concurrent.futures.Future`. If True, the
             call to :func:`stop_runs` will return immediately and the request will be
             processed in the background. This takes precedence over the ``timeout``
             argument. To get the list of :class:`~mcli.api.model.run.Run` output,
             use ``return_value.result()`` with an optional ``timeout`` argument.
 
     Raises:
-        MapiException: Raised if stopping any of the requested runs failed. All
+        MAPIException: Raised if stopping any of the requested runs failed. All
             successfully stopped runs will have the status ```RunStatus.STOPPED```. You can
             freely retry any stopped and unstopped runs if this error is raised due to a
             connection issue.
 
     Returns:
         If future is False:
             A list of stopped :class:`~mcli.api.model.run.Run` objects
```

### Comparing `mosaicml-cli-0.4.2/mcli/api/runs/api_update_run_metadata.py` & `mosaicml-cli-0.4.3/mcli/api/runs/api_update_run_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         future (``bool``): Return the output as a :class:`~concurrent.futures.Future`. If True, the
             call to :func:`update_run_metadata` will return immediately and the request will be
             processed in the background. This takes precedence over the ``timeout``
             argument. To get the list of :class:`~mcli.api.model.run.Run` output,
             use ``return_value.result()`` with an optional ``timeout`` argument.
 
     Raises:
-        MapiException: Raised if updating the requested run failed
+        MAPIException: Raised if updating the requested run failed
 
     Returns:
         If future is False:
             Updated :class:`~mcli.api.model.run.Run` object
         Otherwise:
             A :class:`~concurrent.futures.Future` for the list
     """
```

### Comparing `mosaicml-cli-0.4.2/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.4.3/mcli/api/runs/api_watch_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.4.3/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.4.3/mcli/api/secrets/api_create_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.4.3/mcli/api/secrets/api_delete_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.4.3/mcli/api/secrets/api_get_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/typing_future.py` & `mosaicml-cli-0.4.3/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.4.3/mcli/api/users/api_get_users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/cli.py` & `mosaicml-cli-0.4.3/mcli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.4.3/mcli/cli/common/deployment_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.4.3/mcli/cli/common/run_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.4.3/mcli/cli/m_connect/m_connect.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.4.3/mcli/cli/m_create/m_create.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_create/secret.py` & `mosaicml-cli-0.4.3/mcli/cli/m_create/secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_delete/delete.py` & `mosaicml-cli-0.4.3/mcli/cli/m_delete/delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.4.3/mcli/cli/m_delete/m_delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.4.3/mcli/cli/m_deploy/m_deploy.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.4.3/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 import logging
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Dict, Generator, List, Optional, Tuple
 
 from rich.table import Table
 
-from mcli.api.exceptions import MAPIException, MCLIConfigError
-from mcli.cli.common.deployment_filters import get_deployments_with_filters
+from mcli.api.exceptions import MAPIException
+from mcli.api.inference_deployments.api_get_inference_deployments import get_inference_deployment
 from mcli.cli.m_get.display import MCLIDisplayItem, MCLIGetDisplay, OutputDisplay, create_vertical_display_table
-from mcli.config import MESSAGE
 from mcli.sdk import InferenceDeployment
 from mcli.utils.utils_logging import FAIL, FormatString, format_string
 
 logger = logging.getLogger(__name__)
 
 
 class DescribeDeployMetadataColumns(Enum):
@@ -89,28 +88,20 @@
 
 def describe_deploy(deployment_name: str, output: OutputDisplay = OutputDisplay.TABLE, **kwargs):
     """
     Fetches more details of a Inference Deployment
     """
     del kwargs
 
-    deployments: List[InferenceDeployment] = []
     try:
-        deployments = get_deployments_with_filters(name_filter=[deployment_name])
-    except (MAPIException, RuntimeError) as e:
+        deployment = get_inference_deployment(deployment_name)
+    except MAPIException as e:
         logger.error(f'{FAIL} {e}')
         return 1
-    except MCLIConfigError:
-        logger.error(MESSAGE.MCLI_NOT_INITIALIZED)
 
-    if len(deployments) == 0:
-        logger.error(f'No inference deployments found for name: {deployment_name}')
-        return
-
-    deployment: InferenceDeployment = deployments[0]
     # Deployment metadata section
     print(format_string('Inference Deployment Metadata', FormatString.BOLD))
     metadata_display = MCLIDescribeDeploymentMetadataDisplay([deployment])
     metadata_display.print(output)
     print()
 
     # Deployment original input section
```

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.4.3/mcli/cli/m_describe/describe_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.4.3/mcli/cli/m_describe/m_describe.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_get/clusters.py` & `mosaicml-cli-0.4.3/mcli/cli/m_get/clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_get/display.py` & `mosaicml-cli-0.4.3/mcli/cli/m_get/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,30 +135,30 @@
         return items
 
     @abstractmethod
     def __iter__(self) -> Generator[MCLIDisplayItem, None, None]:
         ...
 
 
-def create_vertical_display_table(data: List[Tuple[Any, ...]],
-                                  columns: List,
+def create_vertical_display_table(data: List[Tuple[str]],
+                                  columns: List[str],
                                   padding: Optional[Tuple[int, int]] = None) -> Table:
     final_padding = (0, 5) if not padding else padding
     grid = Table.grid(expand=False, padding=final_padding)
     # left column is header, right column is data
     grid.add_column(justify="left")
     grid.add_column(justify="left")
     for d in data:
         for col, val in zip(columns, d):
             grid.add_row(col, val)
     return grid
 
 
 def create_display_table(names: List[str],
-                         columns: List[Tuple[Any, ...]],
+                         columns: List[Tuple[str]],
                          column_names: List[str],
                          index_label: str = 'NAME') -> Table:
     return create_table(data=columns,
                         indices=names,
                         index_label=index_label,
                         columns=[ss.upper() for ss in column_names],
                         table_kwargs={
```

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.4.3/mcli/cli/m_get/inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_get/m_get.py` & `mosaicml-cli-0.4.3/mcli/cli/m_get/m_get.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.4.3/mcli/cli/m_get/runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_get/secrets.py` & `mosaicml-cli-0.4.3/mcli/cli/m_get/secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_get/users.py` & `mosaicml-cli-0.4.3/mcli/cli/m_get/users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.4.3/mcli/cli/m_init/m_init.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_interactive/interactive.py` & `mosaicml-cli-0.4.3/mcli/cli/m_interactive/interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_interactive/kube_config.py` & `mosaicml-cli-0.4.3/mcli/cli/m_interactive/kube_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_interactive/m_interactive.py` & `mosaicml-cli-0.4.3/mcli/cli/m_interactive/m_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_kube/m_get_config.py` & `mosaicml-cli-0.4.3/mcli/cli/m_kube/m_get_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_kube/m_kube.py` & `mosaicml-cli-0.4.3/mcli/cli/m_kube/m_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_kube/m_merge_config.py` & `mosaicml-cli-0.4.3/mcli/cli/m_kube/m_merge_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_kube/utils.py` & `mosaicml-cli-0.4.3/mcli/cli/m_kube/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_log/m_log.py` & `mosaicml-cli-0.4.3/mcli/cli/m_log/m_log.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,19 @@
 
 def _get_run_logs(
     run: Run,
     follow: bool,
     rank: Optional[int],
     failed: bool,
 ) -> Tuple[Optional[str], int]:
+
+    if run.status == RunStatus.FAILED and not failed and rank is None:
+        logger.info(f'{INFO} Run {run.name} has failed. Defaulting to show the first failed node rank.')
+        failed = True
+
     if follow and run.status.before(RunStatus.RUNNING):
         with CloudEpilogSpinner(run, RunStatus.RUNNING) as watcher:
             run = watcher.follow()
 
     if run.status == RunStatus.FAILED_PULL:
         CommonLog(logger).log_pod_failed_pull(run.name, run.config.image)
         return "", 1
```

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.4.3/mcli/cli/m_ping/m_ping.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """ mcli ping entrypoint """
 import argparse
 import logging
-from pprint import pprint
 from typing import Callable, Union, cast
 
 import validators
 
 from mcli.api.exceptions import MAPIException
+from mcli.api.inference_deployments import ping as api_ping
 from mcli.api.model.inference_deployment import InferenceDeployment
 from mcli.cli.common.deployment_filters import get_deployments_with_filters
-from mcli.sdk import ping_inference_deployment
 from mcli.utils.utils_logging import FAIL, err_console
 
 logger = logging.getLogger(__name__)
 
 
 def ping(
     deployment: str,
@@ -32,18 +31,17 @@
                     err_console.print("No inference deployments found.")
                 else:
                     err_console.log(f'No inference deployment found with name {deployment}.')
                 return 1
 
             deployment_obj_or_url = deployment_objs[0]
 
-        resp = ping_inference_deployment(deployment_obj_or_url)
+        resp = api_ping(deployment_obj_or_url)
         name_or_url = deployment_obj_or_url if isinstance(deployment_obj_or_url, str) else deployment_obj_or_url.name
-        print(f'{name_or_url}\'s status:')
-        pprint(resp)
+        print(f'{name_or_url}\'s status: {resp.get("status", resp)}')
         return 0
     except RuntimeError as e:
         logger.error(f'{FAIL} {e}')
         return 1
     except MAPIException as e:
         logger.error(f'{FAIL} {e}')
         return 1
```

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_root/m_config.py` & `mosaicml-cli-0.4.3/mcli/cli/m_root/m_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_run/m_run.py` & `mosaicml-cli-0.4.3/mcli/cli/m_run/m_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.4.3/mcli/cli/m_set_unset/api_key.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_set_unset/feature_flag.py` & `mosaicml-cli-0.4.3/mcli/cli/m_set_unset/feature_flag.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_set_unset/m_set.py` & `mosaicml-cli-0.4.3/mcli/cli/m_set_unset/m_set.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.4.3/mcli/cli/m_set_unset/m_unset.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.4.3/mcli/cli/m_set_unset/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.4.3/mcli/cli/m_stop/m_stop.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_util/m_util.py` & `mosaicml-cli-0.4.3/mcli/cli/m_util/m_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/cli/m_util/util.py` & `mosaicml-cli-0.4.3/mcli/cli/m_util/util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/config.py` & `mosaicml-cli-0.4.3/mcli/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,22 +105,16 @@
 class MCLIMode(Enum):
     """Enum for mcli user modes
     """
     PROD = 'PROD'
     DEV = 'DEV'
     INTERNAL = 'INTERNAL'
     LOCAL = 'LOCAL'
-    LEGACY = 'LEGACY'
     STAGING = 'STAGING'
 
-    def is_legacy(self) -> bool:
-        """True if this mode is a legacy mode
-        """
-        return self == MCLIMode.LEGACY
-
     def is_internal(self) -> bool:
         """True if this mode is an internal mode
         """
         internal_modes = {MCLIMode.DEV, MCLIMode.INTERNAL, MCLIMode.LOCAL, MCLIMode.STAGING}
         return self in internal_modes
 
     def available_feature_flags(self) -> List[FeatureFlag]:
```

### Comparing `mosaicml-cli-0.4.2/mcli/models/__init__.py` & `mosaicml-cli-0.4.3/mcli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/models/gpu_type.py` & `mosaicml-cli-0.4.3/mcli/models/gpu_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.4.3/mcli/models/inference_deployment_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/models/mcli_secret.py` & `mosaicml-cli-0.4.3/mcli/models/mcli_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/models/run_config.py` & `mosaicml-cli-0.4.3/mcli/models/run_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.4.3/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/objects/secrets/create/base.py` & `mosaicml-cli-0.4.3/mcli/objects/secrets/create/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.4.3/mcli/objects/secrets/create/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.4.3/mcli/objects/secrets/create/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.4.3/mcli/objects/secrets/create/generic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.4.3/mcli/objects/secrets/create/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/objects/secrets/create/s3.py` & `mosaicml-cli-0.4.3/mcli/objects/secrets/create/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.4.3/mcli/objects/secrets/create/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/objects/secrets/docker_registry.py` & `mosaicml-cli-0.4.3/mcli/objects/secrets/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.4.3/mcli/objects/secrets/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/objects/secrets/gcp.py` & `mosaicml-cli-0.4.3/mcli/objects/secrets/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/objects/secrets/mounted.py` & `mosaicml-cli-0.4.3/mcli/objects/secrets/mounted.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/objects/secrets/oci.py` & `mosaicml-cli-0.4.3/mcli/objects/secrets/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/objects/secrets/s3.py` & `mosaicml-cli-0.4.3/mcli/objects/secrets/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/objects/secrets/ssh.py` & `mosaicml-cli-0.4.3/mcli/objects/secrets/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/proto/mint_pb2.py` & `mosaicml-cli-0.4.3/mcli/proto/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/sdk/__init__.py` & `mosaicml-cli-0.4.3/mcli/sdk/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Primary import target for the Python API"""
 
 from mcli.api.cluster import get_clusters
 from mcli.api.exceptions import MAPIException
 from mcli.api.inference_deployments import (InferenceDeployment, InferenceDeploymentConfig, create_inference_deployment,
                                             delete_inference_deployments, get_inference_deployment_logs,
-                                            get_inference_deployments, ping_inference_deployment, predict)
+                                            get_inference_deployments, ping, predict)
 from mcli.api.runs import (FinalRunConfig, Run, RunConfig, RunStatus, create_run, delete_run, delete_runs,
                            follow_run_logs, get_run, get_run_logs, get_runs, start_run, start_runs, stop_run, stop_runs,
                            update_run_metadata, wait_for_run_status, watch_run_status)
 from mcli.api.secrets import create_secret, delete_secrets, get_secrets
 from mcli.cli.m_init.m_init import initialize
 from mcli.cli.m_set_unset.api_key import set_api_key
 from mcli.config import FeatureFlag, MCLIConfig
@@ -18,15 +18,15 @@
     'MAPIException',
     'InferenceDeployment',
     'InferenceDeploymentConfig',
     'create_inference_deployment',
     'delete_inference_deployments',
     'get_inference_deployment_logs',
     'get_inference_deployments',
-    'ping_inference_deployment',
+    'ping',
     'predict',
     'FinalRunConfig',
     'Run',
     'RunConfig',
     'RunStatus',
     'create_run',
     'delete_run',
```

### Comparing `mosaicml-cli-0.4.2/mcli/utils/utils_cli.py` & `mosaicml-cli-0.4.3/mcli/utils/utils_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/utils/utils_config.py` & `mosaicml-cli-0.4.3/mcli/utils/utils_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/utils/utils_date.py` & `mosaicml-cli-0.4.3/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/utils/utils_docker.py` & `mosaicml-cli-0.4.3/mcli/utils/utils_docker.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/utils/utils_epilog.py` & `mosaicml-cli-0.4.3/mcli/utils/utils_epilog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.4.3/mcli/utils/utils_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/utils/utils_logging.py` & `mosaicml-cli-0.4.3/mcli/utils/utils_logging.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/utils/utils_message_decoding.py` & `mosaicml-cli-0.4.3/mcli/utils/utils_message_decoding.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.4.3/mcli/utils/utils_pypi.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/utils/utils_rich.py` & `mosaicml-cli-0.4.3/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/utils/utils_run_status.py` & `mosaicml-cli-0.4.3/mcli/utils/utils_run_status.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/utils/utils_serializable_dataclass.py` & `mosaicml-cli-0.4.3/mcli/utils/utils_serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.4.3/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.4.3/mcli/utils/utils_string_functions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/utils/utils_types.py` & `mosaicml-cli-0.4.3/mcli/utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.4.3/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/mcli/version.py` & `mosaicml-cli-0.4.3/mcli/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,14 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.4.2/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.4.3/mosaicml_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.2
+Version: 0.4.3
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.2/mosaicml_cli.egg-info/SOURCES.txt` & `mosaicml-cli-0.4.3/mosaicml_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 mcli/api/engine/__init__.py
 mcli/api/engine/engine.py
 mcli/api/inference_deployments/__init__.py
 mcli/api/inference_deployments/api_create_inference_deployment.py
 mcli/api/inference_deployments/api_delete_inference_deployments.py
 mcli/api/inference_deployments/api_get_inference_deployment_logs.py
 mcli/api/inference_deployments/api_get_inference_deployments.py
-mcli/api/inference_deployments/api_ping_inference_deployment.py
+mcli/api/inference_deployments/api_ping.py
 mcli/api/inference_deployments/api_predict_inference_deployment.py
 mcli/api/mint/__init__.py
 mcli/api/mint/shell.py
 mcli/api/mint/tty.py
 mcli/api/model/__init__.py
 mcli/api/model/cluster_details.py
 mcli/api/model/inference_deployment.py
```

### Comparing `mosaicml-cli-0.4.2/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.4.3/mosaicml_cli.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,46 +9,47 @@
 questionary>=1.10.0
 rich>=10.16.2
 ruamel.yaml>=0.17.21
 typing_extensions>=4.0.1
 validators>=0.20.0
 
 [all]
-pre-commit>=2.17.0
-sphinx-design
+docutils>=0.17.0
 sphinxcontrib-images>=0.9.4
-build>=0.10.0
-sphinx-markdown-tables==0.0.17
-pytest-cov>=4.0.0
-sphinx_external_toc==0.3.0
-sphinxcontrib-jsmath>=1.0.1
+twine>=4.0.2
+isort>=5.9.3
+furo==2022.9.29
+sphinxcontrib-devhelp>=1.0.2
+yapf>=0.33.0
 sphinx-copybutton==0.5.2
+sphinx-argparse==0.4.0
+sphinxcontrib-qthelp>=1.0.3
+pytest-cov>=4.0.0
 pytest-mock>=3.7.0
-furo==2022.9.29
-sphinxcontrib-applehelp>=1.0.2
 sphinx==4.4.0
-sphinxemoji==0.2.0
+pylint>=2.12.2
+sphinx-panels==0.6.0
+pyright>=1.1.256
+sphinxcontrib-applehelp>=1.0.2
 pytest>=6.2.5
-twine>=4.0.2
-sphinx-rtd-theme==1.0.0
+sphinxcontrib-jsmath>=1.0.1
+sphinxcontrib-htmlhelp>=2.0.0
+sphinx_external_toc==0.3.0
 sphinxext-opengraph==0.8.2
-pyright>=1.1.256
-yapf>=0.33.0
-sphinxcontrib-devhelp>=1.0.2
-radon>=5.1.0
-sphinx-argparse==0.4.0
+sphinx-design
+sphinxemoji==0.2.0
 myst-parser>=0.16.1
-sphinxcontrib-htmlhelp>=2.0.0
-sphinxcontrib-qthelp>=1.0.3
-sphinx-panels==0.6.0
-toml>=0.10.2
-pylint>=2.12.2
+radon>=5.1.0
 sphinxcontrib-serializinghtml==1.1.5
+pre-commit>=2.17.0
+sphinx-rtd-theme==1.0.0
 sphinxcontrib-katex==0.9.4
-isort>=5.9.3
+build>=0.10.0
+toml>=0.10.2
+sphinx-markdown-tables==0.0.17
 
 [dev]
 build>=0.10.0
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
 pyright>=1.1.256
@@ -76,8 +77,9 @@
 sphinxcontrib-jsmath>=1.0.1
 sphinxcontrib-katex==0.9.4
 sphinxcontrib-qthelp>=1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 sphinxemoji==0.2.0
 sphinxext-opengraph==0.8.2
 myst-parser>=0.16.1
+docutils>=0.17.0
 sphinx-design
```

### Comparing `mosaicml-cli-0.4.2/pyproject.toml` & `mosaicml-cli-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/setup.py` & `mosaicml-cli-0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     'sphinxcontrib-jsmath>=1.0.1',
     'sphinxcontrib-katex==0.9.4',
     'sphinxcontrib-qthelp>=1.0.3',
     'sphinxcontrib-serializinghtml==1.1.5',
     'sphinxemoji==0.2.0',
     'sphinxext-opengraph==0.8.2',
     'myst-parser>=0.16.1',
+    'docutils>=0.17.0',
     'sphinx-design',
 ]
 
 
 def package_files(directory: str):
     # from https://stackoverflow.com/a/36693250
     paths = []
```

### Comparing `mosaicml-cli-0.4.2/tests/test_config.py` & `mosaicml-cli-0.4.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.2/tests/test_upgrade.py` & `mosaicml-cli-0.4.3/tests/test_upgrade.py`

 * *Files identical despite different names*

