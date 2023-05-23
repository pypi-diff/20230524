# Comparing `tmp/lean-1.0.99.tar.gz` & `tmp/lean-1.155.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lean-1.0.99.tar", last modified: Fri Aug 12 22:04:54 2022, max compression
+gzip compressed data, was "lean-1.155.tar", last modified: Tue May 23 22:54:05 2023, max compression
```

## Comparing `lean-1.0.99.tar` & `lean-1.155.tar`

### file list

```diff
@@ -1,157 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-12 22:04:54.000000 lean-1.0.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    72240 2022-08-12 22:04:54.000000 lean-1.0.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4281 2022-08-12 22:04:54.000000 lean-1.0.99/lean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    72240 2022-08-12 22:04:54.000000 lean-1.0.99/lean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-08-12 22:04:54.000000 lean-1.0.99/lean.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-12 22:04:54.000000 lean-1.0.99/lean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-08-12 22:04:54.000000 lean-1.0.99/lean.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-12 22:04:54.000000 lean-1.0.99/lean.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/
--rw-r--r--   0 runner    (1001) docker     (121)     5962 2022-08-12 22:04:48.000000 lean-1.0.99/lean/container.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/commands/
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/whoami.py
--rw-r--r--   0 runner    (1001) docker     (121)    10756 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/create_project.py
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/logout.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/commands/data/
--rw-r--r--   0 runner    (1001) docker     (121)    19544 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/data/download.py
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6286 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/data/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/commands/live/
--rw-r--r--   0 runner    (1001) docker     (121)     2833 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/live/submit_order.py
--rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/live/liquidate.py
--rw-r--r--   0 runner    (1001) docker     (121)    18478 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/live/deploy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3927 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/live/live.py
--rw-r--r--   0 runner    (1001) docker     (121)     3079 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/live/add_security.py
--rw-r--r--   0 runner    (1001) docker     (121)     1580 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/live/cancel_order.py
--rw-r--r--   0 runner    (1001) docker     (121)     2332 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/live/update_order.py
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/live/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/live/stop.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/commands/library/
--rw-r--r--   0 runner    (1001) docker     (121)     5061 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/library/remove.py
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13480 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/library/add.py
--rw-r--r--   0 runner    (1001) docker     (121)     5939 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/init.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/commands/cloud/
--rw-r--r--   0 runner    (1001) docker     (121)     2855 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     2062 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/pull.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/commands/cloud/live/
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/live/liquidate.py
--rw-r--r--   0 runner    (1001) docker     (121)    15301 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/live/deploy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/live/live.py
--rw-r--r--   0 runner    (1001) docker     (121)      944 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/live/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/live/stop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/push.py
--rw-r--r--   0 runner    (1001) docker     (121)    13982 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/optimize.py
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3172 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/cloud/backtest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/commands/config/
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/config/set.py
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/config/list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/config/unset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/config/get.py
--rw-r--r--   0 runner    (1001) docker     (121)    12375 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/optimize.py
--rw-r--r--   0 runner    (1001) docker     (121)     3618 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/logs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2001 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8573 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/research.py
--rw-r--r--   0 runner    (1001) docker     (121)    11361 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/report.py
--rw-r--r--   0 runner    (1001) docker     (121)     8380 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (121)    14681 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/backtest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2364 2022-08-12 22:04:48.000000 lean-1.0.99/lean/commands/login.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/models/
--rw-r--r--   0 runner    (1001) docker     (121)     4381 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/click_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     5972 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/lean_config_configurer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/models/data_providers/
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/data_providers/data_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/data_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/models/brokerages/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/models/brokerages/cloud/
--rw-r--r--   0 runner    (1001) docker     (121)     3529 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/brokerages/cloud/cloud_brokerage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/brokerages/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/models/brokerages/local/
--rw-r--r--   0 runner    (1001) docker     (121)     1780 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/brokerages/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/brokerages/local/local_brokerage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/brokerages/local/data_feed.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/brokerages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3936 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/options.py
--rw-r--r--   0 runner    (1001) docker     (121)    17999 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14294 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/docker.py
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/modules.py
--rw-r--r--   0 runner    (1001) docker     (121)    17459 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1924 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2248 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     8876 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/json_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     1622 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/market_hours_database.py
--rw-r--r--   0 runner    (1001) docker     (121)     1407 2022-08-12 22:04:48.000000 lean-1.0.99/lean/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5856 2022-08-12 22:04:48.000000 lean-1.0.99/lean/main.py
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-08-12 22:04:53.000000 lean-1.0.99/lean/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/ssh/
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-08-12 22:04:48.000000 lean-1.0.99/lean/ssh/key.pub
--rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-08-12 22:04:48.000000 lean-1.0.99/lean/ssh/key
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-08-12 22:04:48.000000 lean-1.0.99/lean/ssh/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/components/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/components/api/
--rw-r--r--   0 runner    (1001) docker     (121)     1387 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/market_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1497 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/service_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4213 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/backtest_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     7716 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3453 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/file_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2250 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/module_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5227 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/project_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/user_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/account_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/organization_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3332 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/node_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4700 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/data_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     8441 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/optimization_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/compile_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5168 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/api/live_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/components/cloud/
--rw-r--r--   0 runner    (1001) docker     (121)     8981 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/cloud/pull_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     7803 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/cloud/cloud_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     4789 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/cloud/cloud_project_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     7506 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/cloud/push_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     7248 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/cloud/data_downloader.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5600 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/cloud/module_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/components/docker/
--rw-r--r--   0 runner    (1001) docker     (121)    35810 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/docker/lean_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23324 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/docker/docker_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/components/config/
--rw-r--r--   0 runner    (1001) docker     (121)     5050 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/config/cli_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    13245 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/config/lean_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     3108 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/config/storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     6255 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/config/output_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    10763 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/config/optimizer_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4130 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/config/project_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 22:04:54.000000 lean-1.0.99/lean/components/util/
--rw-r--r--   0 runner    (1001) docker     (121)     1728 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/click_group_default_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     4455 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/http_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3188 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/path_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/click_custom_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     5676 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     6518 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     4474 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/platform_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     4440 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/task_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22077 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/project_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/xml_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     7677 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/update_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/temp_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/name_extraction.py
--rw-r--r--   0 runner    (1001) docker     (121)     3156 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/name_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3174 2022-08-12 22:04:48.000000 lean-1.0.99/lean/components/util/market_hours_database.py
--rw-r--r--   0 runner    (1001) docker     (121)    11687 2022-08-12 22:04:48.000000 lean-1.0.99/lean/click.py
--rw-r--r--   0 runner    (1001) docker     (121)     4135 2022-08-12 22:04:48.000000 lean-1.0.99/lean/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-08-12 22:04:48.000000 lean-1.0.99/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    59277 2022-08-12 22:04:48.000000 lean-1.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.424809 lean-1.155/
+-rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-05-23 22:54:02.000000 lean-1.155/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    76223 2023-05-23 22:54:05.424809 lean-1.155/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    62508 2023-05-23 22:54:02.000000 lean-1.155/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.392807 lean-1.155/lean/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-23 22:54:04.000000 lean-1.155/lean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12359 2023-05-23 22:54:02.000000 lean-1.155/lean/click.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.396808 lean-1.155/lean/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16597 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/backtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.400808 lean-1.155/lean/commands/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/cloud/backtest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.400808 lean-1.155/lean/commands/cloud/live/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/cloud/live/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19414 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/cloud/live/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/cloud/live/liquidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/cloud/live/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/cloud/live/stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/cloud/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/cloud/pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/cloud/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/cloud/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.400808 lean-1.155/lean/commands/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/config/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/config/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/config/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/config/unset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/create_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.404808 lean-1.155/lean/commands/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18958 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/data/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/data/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/delete_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.404808 lean-1.155/lean/commands/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/lean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.404808 lean-1.155/lean/commands/library/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14002 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/library/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/library/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.408808 lean-1.155/lean/commands/live/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/live/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/live/add_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/live/cancel_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21021 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/live/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/live/liquidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/live/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/live/stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/live/submit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/live/update_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/research.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-23 22:54:02.000000 lean-1.155/lean/commands/whoami.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.408808 lean-1.155/lean/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-23 22:54:02.000000 lean-1.155/lean/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.412808 lean-1.155/lean/components/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-23 22:54:02.000000 lean-1.155/lean/components/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-23 22:54:02.000000 lean-1.155/lean/components/api/account_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-05-23 22:54:02.000000 lean-1.155/lean/components/api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-23 22:54:02.000000 lean-1.155/lean/components/api/backtest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-23 22:54:02.000000 lean-1.155/lean/components/api/compile_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-05-23 22:54:02.000000 lean-1.155/lean/components/api/data_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-23 22:54:02.000000 lean-1.155/lean/components/api/file_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-23 22:54:02.000000 lean-1.155/lean/components/api/lean_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-05-23 22:54:02.000000 lean-1.155/lean/components/api/live_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-23 22:54:02.000000 lean-1.155/lean/components/api/market_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-23 22:54:02.000000 lean-1.155/lean/components/api/module_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-23 22:54:02.000000 lean-1.155/lean/components/api/node_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-05-23 22:54:02.000000 lean-1.155/lean/components/api/optimization_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-23 22:54:02.000000 lean-1.155/lean/components/api/organization_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-05-23 22:54:02.000000 lean-1.155/lean/components/api/project_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-23 22:54:02.000000 lean-1.155/lean/components/api/service_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-23 22:54:02.000000 lean-1.155/lean/components/api/user_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.416808 lean-1.155/lean/components/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-23 22:54:02.000000 lean-1.155/lean/components/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-23 22:54:02.000000 lean-1.155/lean/components/cloud/cloud_project_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-05-23 22:54:02.000000 lean-1.155/lean/components/cloud/cloud_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-05-23 22:54:02.000000 lean-1.155/lean/components/cloud/data_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-05-23 22:54:02.000000 lean-1.155/lean/components/cloud/module_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-05-23 22:54:02.000000 lean-1.155/lean/components/cloud/pull_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-05-23 22:54:02.000000 lean-1.155/lean/components/cloud/push_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.416808 lean-1.155/lean/components/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-23 22:54:02.000000 lean-1.155/lean/components/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-05-23 22:54:02.000000 lean-1.155/lean/components/config/cli_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15703 2023-05-23 22:54:02.000000 lean-1.155/lean/components/config/lean_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-05-23 22:54:02.000000 lean-1.155/lean/components/config/optimizer_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-05-23 22:54:02.000000 lean-1.155/lean/components/config/output_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-23 22:54:02.000000 lean-1.155/lean/components/config/project_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-23 22:54:02.000000 lean-1.155/lean/components/config/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.416808 lean-1.155/lean/components/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-23 22:54:02.000000 lean-1.155/lean/components/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24919 2023-05-23 22:54:02.000000 lean-1.155/lean/components/docker/docker_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37638 2023-05-23 22:54:02.000000 lean-1.155/lean/components/docker/lean_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.420809 lean-1.155/lean/components/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/click_aliased_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/click_custom_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/click_group_default_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/custom_json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/json_modules_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15426 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/library_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/live_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/market_hours_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/name_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/organization_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/path_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/platform_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37999 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/project_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/temp_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/update_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-23 22:54:02.000000 lean-1.155/lean/components/util/xml_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-23 22:54:02.000000 lean-1.155/lean/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-05-23 22:54:02.000000 lean-1.155/lean/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-05-23 22:54:02.000000 lean-1.155/lean/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.420809 lean-1.155/lean/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-23 22:54:02.000000 lean-1.155/lean/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.420809 lean-1.155/lean/models/addon_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-23 22:54:02.000000 lean-1.155/lean/models/addon_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-23 22:54:02.000000 lean-1.155/lean/models/addon_modules/addon_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-05-23 22:54:02.000000 lean-1.155/lean/models/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.420809 lean-1.155/lean/models/brokerages/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-23 22:54:02.000000 lean-1.155/lean/models/brokerages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.424809 lean-1.155/lean/models/brokerages/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-23 22:54:02.000000 lean-1.155/lean/models/brokerages/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-23 22:54:02.000000 lean-1.155/lean/models/brokerages/cloud/cloud_brokerage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.424809 lean-1.155/lean/models/brokerages/local/
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-23 22:54:02.000000 lean-1.155/lean/models/brokerages/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-23 22:54:02.000000 lean-1.155/lean/models/brokerages/local/data_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-23 22:54:02.000000 lean-1.155/lean/models/brokerages/local/local_brokerage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-23 22:54:02.000000 lean-1.155/lean/models/click_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19566 2023-05-23 22:54:02.000000 lean-1.155/lean/models/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17513 2023-05-23 22:54:02.000000 lean-1.155/lean/models/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.424809 lean-1.155/lean/models/data_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-23 22:54:02.000000 lean-1.155/lean/models/data_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-23 22:54:02.000000 lean-1.155/lean/models/data_providers/data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-23 22:54:02.000000 lean-1.155/lean/models/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-23 22:54:02.000000 lean-1.155/lean/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-05-23 22:54:02.000000 lean-1.155/lean/models/json_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-23 22:54:02.000000 lean-1.155/lean/models/lean_config_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-23 22:54:02.000000 lean-1.155/lean/models/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-23 22:54:02.000000 lean-1.155/lean/models/market_hours_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-23 22:54:02.000000 lean-1.155/lean/models/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-23 22:54:02.000000 lean-1.155/lean/models/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-23 22:54:02.000000 lean-1.155/lean/models/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-23 22:54:02.000000 lean-1.155/lean/models/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-23 22:54:02.000000 lean-1.155/lean/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.424809 lean-1.155/lean/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-23 22:54:02.000000 lean-1.155/lean/ssh/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-23 22:54:02.000000 lean-1.155/lean/ssh/key
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-23 22:54:02.000000 lean-1.155/lean/ssh/key.pub
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 22:54:05.392807 lean-1.155/lean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    76223 2023-05-23 22:54:05.000000 lean-1.155/lean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-05-23 22:54:05.000000 lean-1.155/lean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 22:54:05.000000 lean-1.155/lean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-23 22:54:05.000000 lean-1.155/lean.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-23 22:54:05.000000 lean-1.155/lean.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 22:54:05.000000 lean-1.155/lean.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 22:54:05.424809 lean-1.155/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-23 22:54:02.000000 lean-1.155/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lean-1.0.99/PKG-INFO` & `lean-1.155/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: lean
-Version: 1.0.99
+Version: 1.155
 Summary: A CLI aimed at making it easier to run QuantConnect's LEAN engine locally and in the cloud
 Home-page: https://lean.io/cli
 Author: QuantConnect
 Author-email: support@quantconnect.com
 License: UNKNOWN
-Project-URL: Documentation, https://www.lean.io/docs/lean-cli/key-concepts/getting-started
+Project-URL: Documentation, https://www.lean.io/docs/v2/lean-cli/key-concepts/getting-started
 Project-URL: Source, https://github.com/QuantConnect/lean-cli
 Description: ![Lean CLI](http://cdn.quantconnect.com.s3.us-east-1.amazonaws.com/i/github/lean-cli-splash.png)
         
         # QuantConnect Lean CLI
         
         [![Build Status](https://github.com/QuantConnect/lean-cli/workflows/Build/badge.svg)](https://github.com/QuantConnect/lean-cli/actions?query=workflow%3ABuild)
         [![PyPI Version](https://img.shields.io/pypi/v/lean)](https://pypi.org/project/lean/)
         [![Project Status](https://img.shields.io/pypi/status/lean)](https://pypi.org/project/lean/)
         
         The Lean CLI is a cross-platform CLI aimed at making it easier to develop with the LEAN engine locally and in the cloud.
         
-        Visit the [documentation website](https://www.lean.io/docs/lean-cli/key-concepts/getting-started) for comprehensive and up-to-date documentation.
+        Visit the [documentation website](https://www.lean.io/docs/v2/lean-cli/key-concepts/getting-started) for comprehensive and up-to-date documentation.
         
         ## Highlights
         
-        - [Project scaffolding](https://www.lean.io/docs/lean-cli/projects/project-management)
-        - [Local autocomplete](https://www.lean.io/docs/lean-cli/projects/autocomplete)
-        - [Local data downloading](https://www.lean.io/docs/lean-cli/datasets/downloading-quantconnect-data)
-        - [Local backtesting](https://www.lean.io/docs/lean-cli/backtesting/deployment#02-Run-Local-Backtests)
-        - [Local debugging](https://www.lean.io/docs/lean-cli/backtesting/debugging)
-        - [Local research environment](https://www.lean.io/docs/lean-cli/research)
-        - [Local optimization](https://www.lean.io/docs/lean-cli/optimization/deployment#02-Run-Local-Optimizations)
-        - [Local live trading](https://www.lean.io/docs/lean-cli/live-trading/quantconnect-paper-trading#02-Deploy-Local-Algorithms)
-        - [Local backtest report creation](https://www.lean.io/docs/lean-cli/backtesting/report#02-Generate-a-Report)
-        - [Cloud synchronization](https://www.lean.io/docs/lean-cli/projects/cloud-synchronization)
-        - [Cloud backtesting](https://www.lean.io/docs/lean-cli/backtesting/deployment#03-Run-Cloud-Backtests)
-        - [Cloud optimization](https://www.lean.io/docs/lean-cli/optimization/deployment#03-Run-Cloud-Optimizations)
-        - [Cloud live trading](https://www.lean.io/docs/lean-cli/live-trading/quantconnect-paper-trading#03-Deploy-Cloud-Algorithms)
+        - [Project scaffolding](https://www.lean.io/docs/v2/lean-cli/projects/project-management)
+        - [Local autocomplete](https://www.lean.io/docs/v2/lean-cli/projects/autocomplete)
+        - [Local data downloading](https://www.lean.io/docs/v2/lean-cli/datasets/downloading-quantconnect-data)
+        - [Local backtesting](https://www.lean.io/docs/v2/lean-cli/backtesting/deployment#02-Run-Local-Backtests)
+        - [Local debugging](https://www.lean.io/docs/v2/lean-cli/backtesting/debugging)
+        - [Local research environment](https://www.lean.io/docs/v2/lean-cli/research)
+        - [Local optimization](https://www.lean.io/docs/v2/lean-cli/optimization/deployment#02-Run-Local-Optimizations)
+        - [Local live trading](https://www.lean.io/docs/v2/lean-cli/live-trading/quantconnect-paper-trading#02-Deploy-Local-Algorithms)
+        - [Local backtest report creation](https://www.lean.io/docs/v2/lean-cli/backtesting/report#02-Generate-a-Report)
+        - [Cloud synchronization](https://www.lean.io/docs/v2/lean-cli/projects/cloud-synchronization)
+        - [Cloud backtesting](https://www.lean.io/docs/v2/lean-cli/backtesting/deployment#03-Run-Cloud-Backtests)
+        - [Cloud optimization](https://www.lean.io/docs/v2/lean-cli/optimization/deployment#03-Run-Cloud-Optimizations)
+        - [Cloud live trading](https://www.lean.io/docs/v2/lean-cli/live-trading/quantconnect-paper-trading#03-Deploy-Cloud-Algorithms)
         
         ## Installation
         
         The CLI can be installed and updated by running `pip install --upgrade lean`.
         
         Note that many commands in the CLI require Docker to run. See [Get Docker](https://docs.docker.com/get-docker/) for instructions on how to install Docker for your operating system.
         
@@ -71,15 +71,15 @@
         2. Run `lean create-project "Project Name"` to create a new project with some basic code to get you started.
         3. Work on your strategy in `./Project Name`.
         4. Run `lean research "Project Name"` to start a Jupyter Lab session to perform research in.
         5. Run `lean backtest "Project Name"` to run a backtest whenever there's something to test. This runs your strategy in a Docker container containing the same packages as the ones used on QuantConnect.com, but with your own data.
         
         ## Commands
         
-        *Note: the readme only contains the `--help` text of all commands. Visit the [documentation website](https://www.lean.io/docs/lean-cli/key-concepts/getting-started) for more comprehensive documentation.*
+        *Note: the readme only contains the `--help` text of all commands. Visit the [documentation website](https://www.lean.io/docs/v2/lean-cli/key-concepts/getting-started) for more comprehensive documentation.*
         
         <!-- commands start -->
         - [`lean backtest`](#lean-backtest)
         - [`lean build`](#lean-build)
         - [`lean cloud backtest`](#lean-cloud-backtest)
         - [`lean cloud live`](#lean-cloud-live)
         - [`lean cloud live deploy`](#lean-cloud-live-deploy)
@@ -92,14 +92,15 @@
         - [`lean config get`](#lean-config-get)
         - [`lean config list`](#lean-config-list)
         - [`lean config set`](#lean-config-set)
         - [`lean config unset`](#lean-config-unset)
         - [`lean create-project`](#lean-create-project)
         - [`lean data download`](#lean-data-download)
         - [`lean data generate`](#lean-data-generate)
+        - [`lean delete-project`](#lean-delete-project)
         - [`lean init`](#lean-init)
         - [`lean library add`](#lean-library-add)
         - [`lean library remove`](#lean-library-remove)
         - [`lean live`](#lean-live)
         - [`lean live add-security`](#lean-live-add-security)
         - [`lean live cancel-order`](#lean-live-cancel-order)
         - [`lean live deploy`](#lean-live-deploy)
@@ -107,14 +108,16 @@
         - [`lean live stop`](#lean-live-stop)
         - [`lean live submit-order`](#lean-live-submit-order)
         - [`lean live update-order`](#lean-live-update-order)
         - [`lean login`](#lean-login)
         - [`lean logout`](#lean-logout)
         - [`lean logs`](#lean-logs)
         - [`lean optimize`](#lean-optimize)
+        - [`lean project-create`](#lean-project-create)
+        - [`lean project-delete`](#lean-project-delete)
         - [`lean report`](#lean-report)
         - [`lean research`](#lean-research)
         - [`lean whoami`](#lean-whoami)
         
         ### `lean backtest`
         
         Backtest a project locally using Docker.
@@ -124,63 +127,72 @@
         
           Backtest a project locally using Docker.
         
           If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
           If PROJECT is a file, the algorithm in the specified file will be executed.
         
           Go to the following url to learn how to debug backtests locally using the Lean CLI:
-          https://www.lean.io/docs/lean-cli/backtesting/debugging
+          https://www.lean.io/docs/v2/lean-cli/backtesting/debugging
         
           By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
           can set the default engine image for all commands using `lean config set engine-image <image>`.
         
         Options:
           --output DIRECTORY              Directory to store results in (defaults to PROJECT/backtests/TIMESTAMP)
           -d, --detach                    Run the backtest in a detached Docker container and return immediately
-          --debug [pycharm|ptvsd|vsdbg|rider]
+          --debug [pycharm|ptvsd|vsdbg|rider|local-platform]
                                           Enable a certain debugging method (see --help for more information)
-          --data-provider [Terminal Link|QuantConnect|Local]
+          --data-provider [QuantConnect|Local|Terminal Link]
                                           Update the Lean configuration file to retrieve data from the given provider
+          --terminal-link-environment [Production|Beta]
+                                          The environment to run in
+          --terminal-link-server-host TEXT
+                                          The host of the TerminalLink server
+          --terminal-link-server-port INTEGER
+                                          The port of the TerminalLink server
+          --terminal-link-openfigi-api-key TEXT
+                                          The Open FIGI API key to use for mapping options
           --download-data                 Update the Lean configuration file to download data from the QuantConnect API, alias
                                           for --data-provider QuantConnect
           --data-purchase-limit INTEGER   The maximum amount of QCC to spend on downloading data during the backtest when using
                                           QuantConnect as data provider
           --release                       Compile C# projects in release configuration instead of debug
           --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
+          --python-venv TEXT              The path of the python virtual environment to be used
           --update                        Pull the LEAN engine image before running the backtest
           --backtest-name TEXT            Backtest name
+          --no-update                     Use the local LEAN engine image instead of pulling the latest version
           --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
           --verbose                       Enable debug logging
           --help                          Show this message and exit.
         ```
         
         _See code: [lean/commands/backtest.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/backtest.py)_
         
         ### `lean build`
         
-        Build Docker images of your own version of LEAN and the Alpha Streams SDK.
+        Build Docker images of your own version of LEAN.
         
         ```
         Usage: lean build [OPTIONS] [ROOT]
         
-          Build Docker images of your own version of LEAN and the Alpha Streams SDK.
+          Build Docker images of your own version of LEAN.
         
-          ROOT must point to a directory containing the LEAN repository and the Alpha Streams SDK repository:
-          https://github.com/QuantConnect/Lean & https://github.com/QuantConnect/AlphaStreams
+          ROOT must point to a directory containing the LEAN repository:
+          https://github.com/QuantConnect/Lean
         
           When ROOT is not given, the current directory is used as root directory.
         
           This command performs the following actions:
           1. The lean-cli/foundation:latest image is built from Lean/DockerfileLeanFoundation(ARM).
           2. LEAN is compiled in a Docker container using the lean-cli/foundation:latest image.
-          3. The Alpha Streams SDK is compiled in a Docker container using the lean-cli/foundation:latest image.
-          4. The lean-cli/engine:latest image is built from Lean/Dockerfile using lean-cli/foundation:latest as base image.
-          5. The lean-cli/research:latest image is built from Lean/DockerfileJupyter using lean-cli/engine:latest as base image.
-          6. The default engine image is set to lean-cli/engine:latest.
-          7. The default research image is set to lean-cli/research:latest.
+          3. The lean-cli/engine:latest image is built from Lean/Dockerfile using lean-cli/foundation:latest as base image.
+          4. The lean-cli/research:latest image is built from Lean/DockerfileJupyter using lean-cli/engine:latest as base image.
+          5. The default engine image is set to lean-cli/engine:latest.
+          6. The default research image is set to lean-cli/research:latest.
         
           When the foundation Dockerfile is the same as the official foundation Dockerfile, quantconnect/lean:foundation is used
           instead of building a custom foundation image.
         
         Options:
           --tag TEXT  The tag to apply to custom images (defaults to latest)
           --verbose   Enable debug logging
@@ -227,16 +239,14 @@
         
         Commands:
           deploy     Start live trading for a project in the cloud.
           liquidate  Stops live trading and liquidates existing positions for a certain project.
           stop       Stops live trading for a certain project without liquidating existing positions.
         ```
         
-        _See code: [lean/commands/cloud/live.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/live.py)_
-        
         ### `lean cloud live deploy`
         
         Start live trading for a project in the cloud.
         
         ```
         Usage: lean cloud live deploy [OPTIONS] PROJECT
         
@@ -246,44 +256,48 @@
         
           By default an interactive wizard is shown letting you configure the deployment. If --brokerage is given the command
           runs in non-interactive mode. In this mode the CLI does not prompt for input or confirmation. In non-interactive mode
           the options specific to the given brokerage are required, as well as --node, --auto-restart, --notify-order-events and
           --notify-insights.
         
         Options:
-          --brokerage [Paper Trading|Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Kraken|FTX]
+          --brokerage [Paper Trading|Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Trading Technologies|Kraken|TDAmeritrade]
                                           The brokerage to use
           --ib-user-name TEXT             Your Interactive Brokers username
           --ib-account TEXT               Your Interactive Brokers account id
           --ib-password TEXT              Your Interactive Brokers password
+          --ib-weekly-restart-utc-time TEXT
+                                          Weekly restart UTC time (hh:mm:ss). Each week on Sunday your algorithm is restarted at
+                                          this time, and will require 2FA verification. This is required by Interactive Brokers.
+                                          Use this option explicitly to override the default value.
           --ib-data-feed BOOLEAN          Whether the Interactive Brokers price data feed must be used instead of the
                                           QuantConnect price data feed
           --tradier-account-id TEXT       Your Tradier account id
           --tradier-access-token TEXT     Your Tradier access token
           --tradier-environment [live|paper]
                                           Whether the developer sandbox should be used
-          --oanda-environment [Practice|Trade]
-                                          The environment to run in, Practice for fxTrade Practice, Trade for fxTrade
           --oanda-account-id TEXT         Your OANDA account id
           --oanda-access-token TEXT       Your OANDA API token
+          --oanda-environment [Practice|Trade]
+                                          The environment to run in, Practice for fxTrade Practice, Trade for fxTrade
           --bitfinex-api-key TEXT         Your Bitfinex API key
           --bitfinex-api-secret TEXT      Your Bitfinex API secret
-          --gdax-use-sandbox [live|paper]
-                                          Whether the sandbox should be used
           --gdax-api-key TEXT             Your Coinbase Pro API key
           --gdax-api-secret TEXT          Your Coinbase Pro API secret
           --gdax-passphrase TEXT          Your Coinbase Pro API passphrase
+          --gdax-use-sandbox [live|paper]
+                                          Whether the sandbox should be used
           --binance-exchange-name [Binance|BinanceUS]
                                           Binance exchange name [Binance, BinanceUS]
-          --binance-use-testnet [live|paper]
-                                          Whether the testnet should be used
           --binance-api-key TEXT          Your Binance API key
           --binanceus-api-key TEXT        Your Binance API key
           --binance-api-secret TEXT       Your Binance API secret
           --binanceus-api-secret TEXT     Your Binance API secret
+          --binance-use-testnet [live|paper]
+                                          Whether the testnet should be used
           --zerodha-api-key TEXT          Your Kite Connect API key
           --zerodha-access-token TEXT     Your Kite Connect access token
           --zerodha-product-type [mis|cnc|nrml]
                                           MIS if you are targeting intraday products, CNC if you are targeting delivery
                                           products, NRML if you are targeting carry forward products
           --zerodha-trading-segment [equity|commodity]
                                           EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
@@ -295,38 +309,47 @@
           --samco-year-of-birth TEXT      Your year of birth (YYYY) registered with Samco
           --samco-product-type [mis|cnc|nrml]
                                           MIS if you are targeting intraday products, CNC if you are targeting delivery
                                           products, NRML if you are targeting carry forward products
           --samco-trading-segment [equity|commodity]
                                           EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                           commodities on MCX
+          --tt-user-name TEXT             Your Trading Technologies username
+          --tt-session-password TEXT      Your Trading Technologies session password
+          --tt-account-name TEXT          Your Trading Technologies account name
+          --tt-rest-app-key TEXT          Your Trading Technologies REST app key
+          --tt-rest-app-secret TEXT       Your Trading Technologies REST app secret
+          --tt-rest-environment TEXT      The REST environment to run in
+          --tt-order-routing-sender-comp-id TEXT
+                                          The order routing sender comp id to use
           --kraken-api-key TEXT           Your Kraken API key
           --kraken-api-secret TEXT        Your Kraken API secret
           --kraken-verification-tier [Starter|Intermediate|Pro]
                                           Your Kraken Verification Tier
-          --ftx-exchange-name [FTX|FTXUS]
-                                          FTX exchange name [FTX, FTXUS]
-          --ftx-api-key TEXT              Your FTX API key
-          --ftxus-api-key TEXT            Your FTX API key
-          --ftx-api-secret TEXT           Your FTX API secret
-          --ftxus-api-secret TEXT         Your FTX API secret
-          --ftx-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6|VIP1|VIP2|VIP3|MM1|MM2|MM3]
-                                          Your FTX Account Tier
-          --ftxus-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6|Tier7|Tier8|Tier9|VIP1|VIP2|MM1|MM2|MM3]
-                                          Your FTX Account Tier
+          --tdameritrade-api-key TEXT     Your TDAmeritrade API key
+          --tdameritrade-access-token TEXT
+                                          Your TDAmeritrade OAuth Access Token
+          --tdameritrade-account-number TEXT
+                                          Your TDAmeritrade account number
           --node TEXT                     The name or id of the live node to run on
           --auto-restart BOOLEAN          Whether automatic algorithm restarting must be enabled
           --notify-order-events BOOLEAN   Whether notifications must be sent for order events
           --notify-insights BOOLEAN       Whether notifications must be sent for emitted insights
           --notify-emails TEXT            A comma-separated list of 'email:subject' pairs configuring email-notifications
           --notify-webhooks TEXT          A comma-separated list of 'url:HEADER_1=VALUE_1:HEADER_2=VALUE_2:etc' pairs
                                           configuring webhook-notifications
           --notify-sms TEXT               A comma-separated list of phone numbers configuring SMS-notifications
+          --notify-telegram TEXT          A comma-separated list of 'user/group Id:token(optional)' pairs configuring telegram-
+                                          notifications
+          --live-cash-balance TEXT        A comma-separated list of currency:amount pairs of initial cash balance
+          --live-holdings TEXT            A comma-separated list of symbol:symbolId:quantity:averagePrice of initial portfolio
+                                          holdings
           --push                          Push local modifications to the cloud before starting live trading
           --open                          Automatically open the live results in the browser once the deployment starts
+          --show-secrets                  Show secrets as they are input
           --verbose                       Enable debug logging
           --help                          Show this message and exit.
         ```
         
         _See code: [lean/commands/cloud/live/deploy.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/live/deploy.py)_
         
         ### `lean cloud live liquidate`
@@ -432,15 +455,15 @@
         ```
         Usage: lean cloud push [OPTIONS]
         
           Push local projects to QuantConnect.
         
           This command overrides the content of cloud files with the content of their respective local counterparts.
         
-          This command will not delete cloud files which don't have a local counterpart.
+          This command will delete cloud files which don't have a local counterpart.
         
         Options:
           --project DIRECTORY  Path to the local project to push (all local projects if not specified)
           --verbose            Enable debug logging
           --help               Show this message and exit.
         ```
         
@@ -535,15 +558,15 @@
           --help     Show this message and exit.
         ```
         
         _See code: [lean/commands/config/unset.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/config/unset.py)_
         
         ### `lean create-project`
         
-        Create a new project containing starter code.
+        Alias for 'project-create'
         
         ```
         Usage: lean create-project [OPTIONS] NAME
         
           Create a new project containing starter code.
         
           If NAME is a path containing subdirectories those will be created automatically.
@@ -568,26 +591,25 @@
           Purchase and download data from QuantConnect Datasets.
         
           An interactive wizard will show to walk you through the process of selecting data, accepting the CLI API Access and
           Data Agreement and payment. After this wizard the selected data will be downloaded automatically.
         
           If --dataset is given the command runs in non-interactive mode. In this mode the CLI does not prompt for input or
           confirmation but only halts when the agreement must be accepted. In non-interactive mode all options specific to the
-          selected dataset as well as --organization are required.
+          selected dataset are required.
         
           See the following url for the data that can be purchased and downloaded with this command:
           https://www.quantconnect.com/datasets
         
         Options:
-          --dataset TEXT       The name of the dataset to download non-interactively
-          --organization TEXT  The name or id of the organization to purchase and download data with
-          --overwrite          Overwrite existing local data
-          --lean-config FILE   The Lean configuration file that should be used (defaults to the nearest lean.json)
-          --verbose            Enable debug logging
-          --help               Show this message and exit.
+          --dataset TEXT      The name of the dataset to download non-interactively
+          --overwrite         Overwrite existing local data
+          --lean-config FILE  The Lean configuration file that should be used (defaults to the nearest lean.json)
+          --verbose           Enable debug logging
+          --help              Show this message and exit.
         ```
         
         _See code: [lean/commands/data/download.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/data/download.py)_
         
         ### `lean data generate`
         
         Generate random market data.
@@ -622,14 +644,15 @@
           By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
           can set the default engine image for all commands using `lean config set engine-image <image>`.
         
         Options:
           --start [yyyyMMdd]              Start date for the data to generate in yyyyMMdd format  [required]
           --end [yyyyMMdd]                End date for the data to generate in yyyyMMdd format (defaults to today)
           --symbol-count INTEGER RANGE    The number of symbols to generate data for  [x>=0; required]
+          --tickers TEXT                  Comma separated list of tickers to use for generated data
           --security-type [Equity|Forex|Cfd|Future|Crypto|Option]
                                           The security type to generate data for (defaults to Equity)
           --resolution [Tick|Second|Minute|Hour|Daily]
                                           The resolution of the generated data (defaults to Minute)
           --data-density [Dense|Sparse|VerySparse]
                                           The density of the generated data (defaults to Dense)
           --include-coarse BOOLEAN        Whether coarse universe data should be generated for Equity data (defaults to True)
@@ -639,26 +662,46 @@
           --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
           --verbose                       Enable debug logging
           --help                          Show this message and exit.
         ```
         
         _See code: [lean/commands/data/generate.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/data/generate.py)_
         
+        ### `lean delete-project`
+        
+        Alias for 'project-delete'
+        
+        ```
+        Usage: lean delete-project [OPTIONS] PROJECT
+        
+          Delete a project locally and in the cloud if it exists.
+        
+          The project is selected by name or cloud id.
+        
+        Options:
+          --verbose  Enable debug logging
+          --help     Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/delete_project.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/delete_project.py)_
+        
         ### `lean init`
         
         Scaffold a Lean configuration file and data directory.
         
         ```
         Usage: lean init [OPTIONS]
         
           Scaffold a Lean configuration file and data directory.
         
         Options:
-          --verbose  Enable debug logging
-          --help     Show this message and exit.
+          --organization TEXT             The name or id of the organization the Lean CLI will be scaffolded for
+          -l, --language [python|csharp]  The default language to use for new projects
+          --verbose                       Enable debug logging
+          --help                          Show this message and exit.
         ```
         
         _See code: [lean/commands/init.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/init.py)_
         
         ### `lean library add`
         
         Add a custom library to a project.
@@ -666,33 +709,37 @@
         ```
         Usage: lean library add [OPTIONS] PROJECT NAME
         
           Add a custom library to a project.
         
           PROJECT must be the path to the project.
         
-          NAME must be the name of a NuGet package (for C# projects) or of a PyPI package (for Python projects).
+          NAME must be either the name of a NuGet package (for C# projects), a PyPI package (for Python projects), or a path to
+          a Lean CLI library.
         
-          If --version is not given, the package is pinned to the latest compatible version. For C# projects, this is the latest
-          available version. For Python projects, this is the latest version compatible with Python 3.6 (which is what the
-          Docker images use).
+          If --version is not given, and the library is a NuGet or PyPI package the package, it is pinned to the latest
+          compatible version. For C# projects, this is the latest available version. For Python projects, this is the latest
+          version compatible with Python 3.8 (which is what the Docker images use). For Lean CLI library projects, this is
+          ignored.
         
           Custom C# libraries are added to your project's .csproj file, which is then restored if dotnet is on your PATH and the
           --no-local flag has not been given.
         
           Custom Python libraries are added to your project's requirements.txt file and are installed in your local Python
           environment so you get local autocomplete for the library. The last step can be skipped with the --no-local flag.
         
           C# example usage:
           $ lean library add "My CSharp Project" Microsoft.ML
           $ lean library add "My CSharp Project" Microsoft.ML --version 1.5.5
+          $ lean library add "My CSharp Project" "Library/My CSharp Library"
         
           Python example usage:
           $ lean library add "My Python Project" tensorflow
           $ lean library add "My Python Project" tensorflow --version 2.5.0
+          $ lean library add "My Python Project" "Library/My Python Library"
         
         Options:
           --version TEXT  The version of the library to add (defaults to latest compatible version)
           --no-local      Skip making changes to your local environment
           --verbose       Enable debug logging
           --help          Show this message and exit.
         ```
@@ -706,15 +753,16 @@
         ```
         Usage: lean library remove [OPTIONS] PROJECT NAME
         
           Remove a custom library from a project.
         
           PROJECT must be the path to the project directory.
         
-          NAME must be the name of the NuGet package (for C# projects) or of the PyPI package (for Python projects) to remove.
+          NAME must be either the name of the NuGet package (for C# projects), the PyPI package (for Python projects), or the
+          path to the Lean CLI library to remove.
         
           Custom C# libraries are removed from the project's .csproj file, which is then restored if dotnet is on your PATH and
           the --no-local flag has not been given.
         
           Custom Python libraries are removed from the project's requirements.txt file.
         
           C# example usage:
@@ -749,16 +797,14 @@
           deploy        Start live trading a project locally using Docker.
           liquidate     Liquidate the given symbol from the latest deployment of the given project.
           stop          Stop an already running local live trading project.
           submit-order  Represents a command to submit an order to the algorithm.
           update-order  Represents a command to update a specific order by id.
         ```
         
-        _See code: [lean/commands/live.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live.py)_
-        
         ### `lean live add-security`
         
         Represents a command to add a security to the algorithm.
         
         ```
         Usage: lean live add-security [OPTIONS] PROJECT
         
@@ -824,104 +870,89 @@
           By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
           can set the default engine image for all commands using `lean config set engine-image <image>`.
         
         Options:
           --environment TEXT              The environment to use
           --output DIRECTORY              Directory to store results in (defaults to PROJECT/live/TIMESTAMP)
           -d, --detach                    Run the live deployment in a detached Docker container and return immediately
-          --brokerage [Paper Trading|Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Terminal Link|Atreyu|Trading Technologies|Kraken|FTX]
+          --brokerage [Paper Trading|Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Terminal Link|Atreyu|Trading Technologies|Kraken|TDAmeritrade]
                                           The brokerage to use
-          --data-feed [Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Terminal Link|Trading Technologies|Kraken|FTX|IQFeed|Polygon Data Feed|Custom data only]
+          --data-feed [Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Terminal Link|Kraken|TDAmeritrade|IQFeed|Polygon Data Feed|Custom data only]
                                           The data feed to use
-          --data-provider [Terminal Link|QuantConnect|Local]
+          --data-provider [QuantConnect|Local]
                                           Update the Lean configuration file to retrieve data from the given provider
-          --ib-organization TEXT          The name or id of the organization with the Interactive Brokers module subscription
           --ib-user-name TEXT             Your Interactive Brokers username
           --ib-account TEXT               Your Interactive Brokers account id
           --ib-password TEXT              Your Interactive Brokers password
-          --ib-enable-delayed-streaming-data BOOLEAN
-                                          Whether delayed data may be used when your algorithm subscribes to a security you
-                                          don't have a market data subscription for
-          --tradier-organization TEXT     The name or id of the organization with the Tradier module subscription
+          --ib-weekly-restart-utc-time TEXT
+                                          Weekly restart UTC time (hh:mm:ss). Each week on Sunday your algorithm is restarted at
+                                          this time, and will require 2FA verification. This is required by Interactive Brokers.
+                                          Use this option explicitly to override the default value.
           --tradier-account-id TEXT       Your Tradier account id
           --tradier-access-token TEXT     Your Tradier access token
           --tradier-environment [live|paper]
                                           Whether the developer sandbox should be used
-          --oanda-organization TEXT       The name or id of the organization with the Oanda module subscription
-          --oanda-environment [Practice|Trade]
-                                          The environment to run in, Practice for fxTrade Practice, Trade for fxTrade
           --oanda-account-id TEXT         Your OANDA account id
           --oanda-access-token TEXT       Your OANDA API token
-          --bitfinex-organization TEXT    The name or id of the organization with the Bitfinex module subscription
+          --oanda-environment [Practice|Trade]
+                                          The environment to run in, Practice for fxTrade Practice, Trade for fxTrade
           --bitfinex-api-key TEXT         Your Bitfinex API key
           --bitfinex-api-secret TEXT      Your Bitfinex API secret
-          --gdax-organization TEXT        The name or id of the organization with the Coinbase Pro module subscription
-          --gdax-use-sandbox [live|paper]
-                                          Whether the sandbox should be used
           --gdax-api-key TEXT             Your Coinbase Pro API key
           --gdax-api-secret TEXT          Your Coinbase Pro API secret
           --gdax-passphrase TEXT          Your Coinbase Pro API passphrase
-          --binance-organization TEXT     The name or id of the organization with the Binance module subscription
+          --gdax-use-sandbox [live|paper]
+                                          Whether the sandbox should be used
           --binance-exchange-name [Binance|BinanceUS]
                                           Binance exchange name [Binance, BinanceUS]
-          --binance-use-testnet [live|paper]
-                                          Whether the testnet should be used
           --binance-api-key TEXT          Your Binance API key
           --binanceus-api-key TEXT        Your Binance API key
           --binance-api-secret TEXT       Your Binance API secret
           --binanceus-api-secret TEXT     Your Binance API secret
-          --zerodha-organization TEXT     The name or id of the organization with the zerodha module subscription
+          --binance-use-testnet [live|paper]
+                                          Whether the testnet should be used
           --zerodha-api-key TEXT          Your Kite Connect API key
           --zerodha-access-token TEXT     Your Kite Connect access token
           --zerodha-product-type [mis|cnc|nrml]
                                           MIS if you are targeting intraday products, CNC if you are targeting delivery
                                           products, NRML if you are targeting carry forward products
           --zerodha-trading-segment [equity|commodity]
                                           EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                           commodities on MCX
           --zerodha-history-subscription [true|false]
                                           Whether you have a history API subscription for Zerodha
-          --samco-organization TEXT       The name or id of the organization with the samco module subscription
           --samco-client-id TEXT          Your Samco account Client ID
           --samco-client-password TEXT    Your Samco account password
           --samco-year-of-birth TEXT      Your year of birth (YYYY) registered with Samco
           --samco-product-type [mis|cnc|nrml]
                                           MIS if you are targeting intraday products, CNC if you are targeting delivery
                                           products, NRML if you are targeting carry forward products
           --samco-trading-segment [equity|commodity]
                                           EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                           commodities on MCX
-          --terminal-link-organization TEXT
-                                          The name or id of the organization with the Terminal Link module subscription
-          --bloomberg-environment [Production|Beta]
+          --terminal-link-environment [Production|Beta]
                                           The environment to run in
-          --bloomberg-server-host TEXT    The host of the Bloomberg server
-          --bloomberg-server-port INTEGER
-                                          The port of the Bloomberg server
-          --bloomberg-symbol-map-file FILE
-                                          The path to the Bloomberg symbol map file
-          --bloomberg-emsx-broker TEXT    The EMSX broker to use
-          --bloomberg-emsx-user-time-zone TEXT
-                                          The EMSX user timezone to use
-          --bloomberg-emsx-account TEXT   The EMSX account to use
-          --bloomberg-emsx-strategy TEXT  The EMSX strategy to use
-          --bloomberg-emsx-notes TEXT     The EMSX notes to use
-          --bloomberg-emsx-handling TEXT  The EMSX handling to use
-          --bloomberg-allow-modification BOOLEAN
-                                          Whether modification is allowed
-          --atreyu-organization TEXT      The name or id of the organization with the Atreyu module subscription
+          --terminal-link-server-host TEXT
+                                          The host of the TerminalLink server
+          --terminal-link-server-port INTEGER
+                                          The port of the TerminalLink server
+          --terminal-link-emsx-broker TEXT
+                                          The EMSX broker to use
+          --terminal-link-emsx-account TEXT
+                                          The EMSX account to use
+          --terminal-link-openfigi-api-key TEXT
+                                          The Open FIGI API key to use for mapping options
           --atreyu-host TEXT              The host of the Atreyu server
           --atreyu-req-port INTEGER       The Atreyu request port
           --atreyu-sub-port INTEGER       The Atreyu subscribe port
           --atreyu-username TEXT          Your Atreyu username
           --atreyu-password TEXT          Your Atreyu password
           --atreyu-client-id TEXT         Your Atreyu client id
           --atreyu-broker-mpid TEXT       The broker MPID to use
           --atreyu-locate-rqd TEXT        The locate rqd to use
-          --tt-organization TEXT          The name or id of the organization with the Trading Technologies module subscription
           --tt-user-name TEXT             Your Trading Technologies username
           --tt-session-password TEXT      Your Trading Technologies session password
           --tt-account-name TEXT          Your Trading Technologies account name
           --tt-rest-app-key TEXT          Your Trading Technologies REST app key
           --tt-rest-app-secret TEXT       Your Trading Technologies REST app secret
           --tt-rest-environment TEXT      The REST environment to run in
           --tt-market-data-sender-comp-id TEXT
@@ -933,41 +964,41 @@
           --tt-order-routing-sender-comp-id TEXT
                                           The order routing sender comp id to use
           --tt-order-routing-target-comp-id TEXT
                                           The order routing target comp id to use
           --tt-order-routing-host TEXT    The host of the order routing server
           --tt-order-routing-port TEXT    The port of the order routing server
           --tt-log-fix-messages BOOLEAN   Whether FIX messages should be logged
-          --kraken-organization TEXT      The name or id of the organization with the kraken module subscription
           --kraken-api-key TEXT           Your Kraken API key
           --kraken-api-secret TEXT        Your Kraken API secret
           --kraken-verification-tier [Starter|Intermediate|Pro]
                                           Your Kraken Verification Tier
-          --ftx-organization TEXT         The name or id of the organization with the FTX module subscription
-          --ftx-exchange-name [FTX|FTXUS]
-                                          FTX exchange name [FTX, FTXUS]
-          --ftx-api-key TEXT              Your FTX API key
-          --ftxus-api-key TEXT            Your FTX API key
-          --ftx-api-secret TEXT           Your FTX API secret
-          --ftxus-api-secret TEXT         Your FTX API secret
-          --ftx-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6|VIP1|VIP2|VIP3|MM1|MM2|MM3]
-                                          Your FTX Account Tier
-          --ftxus-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6|Tier7|Tier8|Tier9|VIP1|VIP2|MM1|MM2|MM3]
-                                          Your FTX Account Tier
-          --iqfeed-iqconnect FILE         The path to the IQConnect binary
+          --tdameritrade-api-key TEXT     Your TDAmeritrade API key
+          --tdameritrade-access-token TEXT
+                                          Your TDAmeritrade OAuth Access Token
+          --tdameritrade-account-number TEXT
+                                          Your TDAmeritrade account number
+          --ib-enable-delayed-streaming-data BOOLEAN
+                                          Whether delayed data may be used when your algorithm subscribes to a security you
+                                          don't have a market data subscription for
+          --iqfeed-iqconnect TEXT         The path to the IQConnect binary
           --iqfeed-username TEXT          Your IQFeed username
           --iqfeed-password TEXT          Your IQFeed password
           --iqfeed-productName TEXT       The product name of your IQFeed developer account
           --iqfeed-version TEXT           The product version of your IQFeed developer account
           --polygon-api-key TEXT          Your Polygon data feed API Key
-          --quantconnect-organization TEXT
-                                          The name or id of the organization with the QuantConnect datafeed module subscription
           --release                       Compile C# projects in release configuration instead of debug
           --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
+          --python-venv TEXT              The path of the python virtual environment to be used
+          --live-cash-balance TEXT        A comma-separated list of currency:amount pairs of initial cash balance
+          --live-holdings TEXT            A comma-separated list of symbol:symbolId:quantity:averagePrice of initial portfolio
+                                          holdings
           --update                        Pull the LEAN engine image before starting live trading
+          --show-secrets                  Show secrets as they are input
+          --no-update                     Use the local LEAN engine image instead of pulling the latest version
           --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
           --verbose                       Enable debug logging
           --help                          Show this message and exit.
         ```
         
         _See code: [lean/commands/live/deploy.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live/deploy.py)_
         
@@ -1067,14 +1098,15 @@
           If user id or API token is not provided an interactive prompt will show.
         
           Credentials are stored in ~/.lean/credentials and are removed upon running `lean logout`.
         
         Options:
           -u, --user-id TEXT    QuantConnect user id
           -t, --api-token TEXT  QuantConnect API token
+          --show-secrets        Show secrets as they are input
           --verbose             Enable debug logging
           --help                Show this message and exit.
         ```
         
         _See code: [lean/commands/login.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/login.py)_
         
         ### `lean logout`
@@ -1140,14 +1172,17 @@
           - --parameter <name> <min value> <max value> <step size>
           - --parameter my-first-parameter 1 10 0.5 --parameter my-second-parameter 20 30 5
         
           In non-interactive mode the --constraint option can be provided multiple times to configure multiple constraints:
           - --constraint "<statistic> <operator> <value>"
           - --constraint "Sharpe Ratio >= 0.5" --constraint "Drawdown < 0.25"
         
+          If --estimate is given, the optimization will not be executed.
+          The runtime estimate for the optimization will be calculated and outputted.
+        
           By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
           can set the default engine image for all commands using `lean config set engine-image <image>`.
         
         Options:
           --output DIRECTORY              Directory to store results in (defaults to PROJECT/optimizations/TIMESTAMP)
           -d, --detach                    Run the optimization in a detached Docker container and return immediately
           --optimizer-config FILE         The optimizer configuration file that should be used
@@ -1157,21 +1192,64 @@
           --target-direction [min|max]    Whether the target must be minimized or maximized
           --parameter <TEXT FLOAT FLOAT FLOAT>...
                                           The 'parameter min max step' pairs configuring the parameters to optimize
           --constraint TEXT               The 'statistic operator value' pairs configuring the constraints of the optimization
           --release                       Compile C# projects in release configuration instead of debug
           --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
           --update                        Pull the LEAN engine image before running the optimizer
+          --estimate                      Estimate optimization runtime without running it
+          --max-concurrent-backtests INTEGER RANGE
+                                          Maximum number of concurrent backtests to run  [x>=1]
+          --no-update                     Use the local LEAN engine image instead of pulling the latest version
           --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
           --verbose                       Enable debug logging
           --help                          Show this message and exit.
         ```
         
         _See code: [lean/commands/optimize.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/optimize.py)_
         
+        ### `lean project-create`
+        
+        Create a new project containing starter code.
+        
+        ```
+        Usage: lean project-create [OPTIONS] NAME
+        
+          Create a new project containing starter code.
+        
+          If NAME is a path containing subdirectories those will be created automatically.
+        
+          The default language can be set using `lean config set default-language python/csharp`.
+        
+        Options:
+          -l, --language [python|csharp]  The language of the project to create
+          --verbose                       Enable debug logging
+          --help                          Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/project_create.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/project_create.py)_
+        
+        ### `lean project-delete`
+        
+        Delete a project locally and in the cloud if it exists.
+        
+        ```
+        Usage: lean project-delete [OPTIONS] PROJECT
+        
+          Delete a project locally and in the cloud if it exists.
+        
+          The project is selected by name or cloud id.
+        
+        Options:
+          --verbose  Enable debug logging
+          --help     Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/project_delete.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/project_delete.py)_
+        
         ### `lean report`
         
         Generate a report of a backtest.
         
         ```
         Usage: lean report [OPTIONS]
         
@@ -1197,14 +1275,15 @@
           -d, --detach                 Run the report creator in a detached Docker container and return immediately
           --strategy-name TEXT         Name of the strategy, will appear at the top-right corner of each page
           --strategy-version TEXT      Version number of the strategy, will appear next to the project name
           --strategy-description TEXT  Description of the strategy, will appear under the 'Strategy Description' section
           --overwrite                  Overwrite --report-destination if it already contains a file
           --image TEXT                 The LEAN engine image to use (defaults to quantconnect/lean:latest)
           --update                     Pull the LEAN engine image before running the report creator
+          --pdf                        Create a PDF version along with the HTML version of the report
           --lean-config FILE           The Lean configuration file that should be used (defaults to the nearest lean.json)
           --verbose                    Enable debug logging
           --help                       Show this message and exit.
         ```
         
         _See code: [lean/commands/report.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/report.py)_
         
@@ -1218,16 +1297,24 @@
           Run a Jupyter Lab environment locally using Docker.
         
           By default the official LEAN research image is used. You can override this using the --image option. Alternatively you
           can set the default research image using `lean config set research-image <image>`.
         
         Options:
           --port INTEGER                  The port to run Jupyter Lab on (defaults to 8888)
-          --data-provider [Terminal Link|QuantConnect|Local]
+          --data-provider [QuantConnect|Local|Terminal Link]
                                           Update the Lean configuration file to retrieve data from the given provider
+          --terminal-link-environment [Production|Beta]
+                                          The environment to run in
+          --terminal-link-server-host TEXT
+                                          The host of the TerminalLink server
+          --terminal-link-server-port INTEGER
+                                          The port of the TerminalLink server
+          --terminal-link-openfigi-api-key TEXT
+                                          The Open FIGI API key to use for mapping options
           --download-data                 Update the Lean configuration file to download data from the QuantConnect API, alias
                                           for --data-provider QuantConnect
           --data-purchase-limit INTEGER   The maximum amount of QCC to spend on downloading data during the research session
                                           when using QuantConnect as data provider
           -d, --detach                    Run Jupyter Lab in a detached Docker container and return immediately
           --no-open                       Don't open the Jupyter Lab environment in the browser after starting it
           --image TEXT                    The LEAN research image to use (defaults to quantconnect/research:latest)
@@ -1254,15 +1341,15 @@
         ```
         
         _See code: [lean/commands/whoami.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/whoami.py)_
         <!-- commands end -->
         
         ## Development
         
-        To work on the Lean CLI, clone the repository, enter an environment containing Python 3.6+ and run `pip install -r requirements.txt`. This command will install the required dependencies and installs the CLI in editable mode. This means you'll be able to edit the code and immediately see the results the next time you run `lean`.
+        To work on the Lean CLI, clone the repository, enter an environment containing Python 3.7+ and run `pip install -r requirements.txt`. This command will install the required dependencies and installs the CLI in editable mode. This means you'll be able to edit the code and immediately see the results the next time you run `lean`.
         
         If you need to add dependencies, first update `setup.py` (if it is a production dependency) or `requirements.txt` (if it is a development dependency) and then re-run `pip install -r requirements.txt`.
         
         The automated tests can be ran by running `pytest`. The filesystem and HTTP requests are mocked when running tests to make sure they run in an isolated environment.
         
         Can build the lean CLI by running `python setup.py sdist bdist_wheel` from the root of the project and to install it `pip install --force-reinstall dist/lean-dev-py3-none-any.whl`. To update the commands reference part of the readme run `python scripts/readme.py` from the root of the project, after installing the new version.
         
@@ -1270,13 +1357,13 @@
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >= 3.6
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >= 3.7
 Description-Content-Type: text/markdown
```

### Comparing `lean-1.0.99/lean.egg-info/SOURCES.txt` & `lean-1.155/lean.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 lean/__init__.py
 lean/click.py
 lean/constants.py
 lean/container.py
 lean/main.py
@@ -11,15 +12,17 @@
 lean.egg-info/entry_points.txt
 lean.egg-info/requires.txt
 lean.egg-info/top_level.txt
 lean/commands/__init__.py
 lean/commands/backtest.py
 lean/commands/build.py
 lean/commands/create_project.py
+lean/commands/delete_project.py
 lean/commands/init.py
+lean/commands/lean.py
 lean/commands/login.py
 lean/commands/logout.py
 lean/commands/logs.py
 lean/commands/optimize.py
 lean/commands/report.py
 lean/commands/research.py
 lean/commands/whoami.py
@@ -38,14 +41,15 @@
 lean/commands/config/get.py
 lean/commands/config/list.py
 lean/commands/config/set.py
 lean/commands/config/unset.py
 lean/commands/data/__init__.py
 lean/commands/data/download.py
 lean/commands/data/generate.py
+lean/commands/gui/__init__.py
 lean/commands/library/__init__.py
 lean/commands/library/add.py
 lean/commands/library/remove.py
 lean/commands/live/__init__.py
 lean/commands/live/add_security.py
 lean/commands/live/cancel_order.py
 lean/commands/live/deploy.py
@@ -58,14 +62,15 @@
 lean/components/api/__init__.py
 lean/components/api/account_client.py
 lean/components/api/api_client.py
 lean/components/api/backtest_client.py
 lean/components/api/compile_client.py
 lean/components/api/data_client.py
 lean/components/api/file_client.py
+lean/components/api/lean_client.py
 lean/components/api/live_client.py
 lean/components/api/market_client.py
 lean/components/api/module_client.py
 lean/components/api/node_client.py
 lean/components/api/optimization_client.py
 lean/components/api/organization_client.py
 lean/components/api/project_client.py
@@ -85,22 +90,28 @@
 lean/components/config/output_config_manager.py
 lean/components/config/project_config_manager.py
 lean/components/config/storage.py
 lean/components/docker/__init__.py
 lean/components/docker/docker_manager.py
 lean/components/docker/lean_runner.py
 lean/components/util/__init__.py
+lean/components/util/click_aliased_command_group.py
 lean/components/util/click_custom_parameters.py
 lean/components/util/click_group_default_command.py
 lean/components/util/compiler.py
+lean/components/util/custom_json_encoder.py
 lean/components/util/http_client.py
+lean/components/util/json_modules_handler.py
+lean/components/util/library_manager.py
+lean/components/util/live_utils.py
 lean/components/util/logger.py
 lean/components/util/market_hours_database.py
 lean/components/util/name_extraction.py
 lean/components/util/name_generator.py
+lean/components/util/organization_manager.py
 lean/components/util/path_manager.py
 lean/components/util/platform_manager.py
 lean/components/util/project_manager.py
 lean/components/util/task_manager.py
 lean/components/util/temp_manager.py
 lean/components/util/update_manager.py
 lean/components/util/xml_manager.py
@@ -116,14 +127,16 @@
 lean/models/logger.py
 lean/models/market_hours_database.py
 lean/models/modules.py
 lean/models/optimizer.py
 lean/models/options.py
 lean/models/pydantic.py
 lean/models/utils.py
+lean/models/addon_modules/__init__.py
+lean/models/addon_modules/addon_module.py
 lean/models/brokerages/__init__.py
 lean/models/brokerages/cloud/__init__.py
 lean/models/brokerages/cloud/cloud_brokerage.py
 lean/models/brokerages/local/__init__.py
 lean/models/brokerages/local/data_feed.py
 lean/models/brokerages/local/local_brokerage.py
 lean/models/data_providers/__init__.py
```

### Comparing `lean-1.0.99/lean.egg-info/PKG-INFO` & `lean-1.155/lean.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: lean
-Version: 1.0.99
+Version: 1.155
 Summary: A CLI aimed at making it easier to run QuantConnect's LEAN engine locally and in the cloud
 Home-page: https://lean.io/cli
 Author: QuantConnect
 Author-email: support@quantconnect.com
 License: UNKNOWN
-Project-URL: Documentation, https://www.lean.io/docs/lean-cli/key-concepts/getting-started
+Project-URL: Documentation, https://www.lean.io/docs/v2/lean-cli/key-concepts/getting-started
 Project-URL: Source, https://github.com/QuantConnect/lean-cli
 Description: ![Lean CLI](http://cdn.quantconnect.com.s3.us-east-1.amazonaws.com/i/github/lean-cli-splash.png)
         
         # QuantConnect Lean CLI
         
         [![Build Status](https://github.com/QuantConnect/lean-cli/workflows/Build/badge.svg)](https://github.com/QuantConnect/lean-cli/actions?query=workflow%3ABuild)
         [![PyPI Version](https://img.shields.io/pypi/v/lean)](https://pypi.org/project/lean/)
         [![Project Status](https://img.shields.io/pypi/status/lean)](https://pypi.org/project/lean/)
         
         The Lean CLI is a cross-platform CLI aimed at making it easier to develop with the LEAN engine locally and in the cloud.
         
-        Visit the [documentation website](https://www.lean.io/docs/lean-cli/key-concepts/getting-started) for comprehensive and up-to-date documentation.
+        Visit the [documentation website](https://www.lean.io/docs/v2/lean-cli/key-concepts/getting-started) for comprehensive and up-to-date documentation.
         
         ## Highlights
         
-        - [Project scaffolding](https://www.lean.io/docs/lean-cli/projects/project-management)
-        - [Local autocomplete](https://www.lean.io/docs/lean-cli/projects/autocomplete)
-        - [Local data downloading](https://www.lean.io/docs/lean-cli/datasets/downloading-quantconnect-data)
-        - [Local backtesting](https://www.lean.io/docs/lean-cli/backtesting/deployment#02-Run-Local-Backtests)
-        - [Local debugging](https://www.lean.io/docs/lean-cli/backtesting/debugging)
-        - [Local research environment](https://www.lean.io/docs/lean-cli/research)
-        - [Local optimization](https://www.lean.io/docs/lean-cli/optimization/deployment#02-Run-Local-Optimizations)
-        - [Local live trading](https://www.lean.io/docs/lean-cli/live-trading/quantconnect-paper-trading#02-Deploy-Local-Algorithms)
-        - [Local backtest report creation](https://www.lean.io/docs/lean-cli/backtesting/report#02-Generate-a-Report)
-        - [Cloud synchronization](https://www.lean.io/docs/lean-cli/projects/cloud-synchronization)
-        - [Cloud backtesting](https://www.lean.io/docs/lean-cli/backtesting/deployment#03-Run-Cloud-Backtests)
-        - [Cloud optimization](https://www.lean.io/docs/lean-cli/optimization/deployment#03-Run-Cloud-Optimizations)
-        - [Cloud live trading](https://www.lean.io/docs/lean-cli/live-trading/quantconnect-paper-trading#03-Deploy-Cloud-Algorithms)
+        - [Project scaffolding](https://www.lean.io/docs/v2/lean-cli/projects/project-management)
+        - [Local autocomplete](https://www.lean.io/docs/v2/lean-cli/projects/autocomplete)
+        - [Local data downloading](https://www.lean.io/docs/v2/lean-cli/datasets/downloading-quantconnect-data)
+        - [Local backtesting](https://www.lean.io/docs/v2/lean-cli/backtesting/deployment#02-Run-Local-Backtests)
+        - [Local debugging](https://www.lean.io/docs/v2/lean-cli/backtesting/debugging)
+        - [Local research environment](https://www.lean.io/docs/v2/lean-cli/research)
+        - [Local optimization](https://www.lean.io/docs/v2/lean-cli/optimization/deployment#02-Run-Local-Optimizations)
+        - [Local live trading](https://www.lean.io/docs/v2/lean-cli/live-trading/quantconnect-paper-trading#02-Deploy-Local-Algorithms)
+        - [Local backtest report creation](https://www.lean.io/docs/v2/lean-cli/backtesting/report#02-Generate-a-Report)
+        - [Cloud synchronization](https://www.lean.io/docs/v2/lean-cli/projects/cloud-synchronization)
+        - [Cloud backtesting](https://www.lean.io/docs/v2/lean-cli/backtesting/deployment#03-Run-Cloud-Backtests)
+        - [Cloud optimization](https://www.lean.io/docs/v2/lean-cli/optimization/deployment#03-Run-Cloud-Optimizations)
+        - [Cloud live trading](https://www.lean.io/docs/v2/lean-cli/live-trading/quantconnect-paper-trading#03-Deploy-Cloud-Algorithms)
         
         ## Installation
         
         The CLI can be installed and updated by running `pip install --upgrade lean`.
         
         Note that many commands in the CLI require Docker to run. See [Get Docker](https://docs.docker.com/get-docker/) for instructions on how to install Docker for your operating system.
         
@@ -71,15 +71,15 @@
         2. Run `lean create-project "Project Name"` to create a new project with some basic code to get you started.
         3. Work on your strategy in `./Project Name`.
         4. Run `lean research "Project Name"` to start a Jupyter Lab session to perform research in.
         5. Run `lean backtest "Project Name"` to run a backtest whenever there's something to test. This runs your strategy in a Docker container containing the same packages as the ones used on QuantConnect.com, but with your own data.
         
         ## Commands
         
-        *Note: the readme only contains the `--help` text of all commands. Visit the [documentation website](https://www.lean.io/docs/lean-cli/key-concepts/getting-started) for more comprehensive documentation.*
+        *Note: the readme only contains the `--help` text of all commands. Visit the [documentation website](https://www.lean.io/docs/v2/lean-cli/key-concepts/getting-started) for more comprehensive documentation.*
         
         <!-- commands start -->
         - [`lean backtest`](#lean-backtest)
         - [`lean build`](#lean-build)
         - [`lean cloud backtest`](#lean-cloud-backtest)
         - [`lean cloud live`](#lean-cloud-live)
         - [`lean cloud live deploy`](#lean-cloud-live-deploy)
@@ -92,14 +92,15 @@
         - [`lean config get`](#lean-config-get)
         - [`lean config list`](#lean-config-list)
         - [`lean config set`](#lean-config-set)
         - [`lean config unset`](#lean-config-unset)
         - [`lean create-project`](#lean-create-project)
         - [`lean data download`](#lean-data-download)
         - [`lean data generate`](#lean-data-generate)
+        - [`lean delete-project`](#lean-delete-project)
         - [`lean init`](#lean-init)
         - [`lean library add`](#lean-library-add)
         - [`lean library remove`](#lean-library-remove)
         - [`lean live`](#lean-live)
         - [`lean live add-security`](#lean-live-add-security)
         - [`lean live cancel-order`](#lean-live-cancel-order)
         - [`lean live deploy`](#lean-live-deploy)
@@ -107,14 +108,16 @@
         - [`lean live stop`](#lean-live-stop)
         - [`lean live submit-order`](#lean-live-submit-order)
         - [`lean live update-order`](#lean-live-update-order)
         - [`lean login`](#lean-login)
         - [`lean logout`](#lean-logout)
         - [`lean logs`](#lean-logs)
         - [`lean optimize`](#lean-optimize)
+        - [`lean project-create`](#lean-project-create)
+        - [`lean project-delete`](#lean-project-delete)
         - [`lean report`](#lean-report)
         - [`lean research`](#lean-research)
         - [`lean whoami`](#lean-whoami)
         
         ### `lean backtest`
         
         Backtest a project locally using Docker.
@@ -124,63 +127,72 @@
         
           Backtest a project locally using Docker.
         
           If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
           If PROJECT is a file, the algorithm in the specified file will be executed.
         
           Go to the following url to learn how to debug backtests locally using the Lean CLI:
-          https://www.lean.io/docs/lean-cli/backtesting/debugging
+          https://www.lean.io/docs/v2/lean-cli/backtesting/debugging
         
           By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
           can set the default engine image for all commands using `lean config set engine-image <image>`.
         
         Options:
           --output DIRECTORY              Directory to store results in (defaults to PROJECT/backtests/TIMESTAMP)
           -d, --detach                    Run the backtest in a detached Docker container and return immediately
-          --debug [pycharm|ptvsd|vsdbg|rider]
+          --debug [pycharm|ptvsd|vsdbg|rider|local-platform]
                                           Enable a certain debugging method (see --help for more information)
-          --data-provider [Terminal Link|QuantConnect|Local]
+          --data-provider [QuantConnect|Local|Terminal Link]
                                           Update the Lean configuration file to retrieve data from the given provider
+          --terminal-link-environment [Production|Beta]
+                                          The environment to run in
+          --terminal-link-server-host TEXT
+                                          The host of the TerminalLink server
+          --terminal-link-server-port INTEGER
+                                          The port of the TerminalLink server
+          --terminal-link-openfigi-api-key TEXT
+                                          The Open FIGI API key to use for mapping options
           --download-data                 Update the Lean configuration file to download data from the QuantConnect API, alias
                                           for --data-provider QuantConnect
           --data-purchase-limit INTEGER   The maximum amount of QCC to spend on downloading data during the backtest when using
                                           QuantConnect as data provider
           --release                       Compile C# projects in release configuration instead of debug
           --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
+          --python-venv TEXT              The path of the python virtual environment to be used
           --update                        Pull the LEAN engine image before running the backtest
           --backtest-name TEXT            Backtest name
+          --no-update                     Use the local LEAN engine image instead of pulling the latest version
           --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
           --verbose                       Enable debug logging
           --help                          Show this message and exit.
         ```
         
         _See code: [lean/commands/backtest.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/backtest.py)_
         
         ### `lean build`
         
-        Build Docker images of your own version of LEAN and the Alpha Streams SDK.
+        Build Docker images of your own version of LEAN.
         
         ```
         Usage: lean build [OPTIONS] [ROOT]
         
-          Build Docker images of your own version of LEAN and the Alpha Streams SDK.
+          Build Docker images of your own version of LEAN.
         
-          ROOT must point to a directory containing the LEAN repository and the Alpha Streams SDK repository:
-          https://github.com/QuantConnect/Lean & https://github.com/QuantConnect/AlphaStreams
+          ROOT must point to a directory containing the LEAN repository:
+          https://github.com/QuantConnect/Lean
         
           When ROOT is not given, the current directory is used as root directory.
         
           This command performs the following actions:
           1. The lean-cli/foundation:latest image is built from Lean/DockerfileLeanFoundation(ARM).
           2. LEAN is compiled in a Docker container using the lean-cli/foundation:latest image.
-          3. The Alpha Streams SDK is compiled in a Docker container using the lean-cli/foundation:latest image.
-          4. The lean-cli/engine:latest image is built from Lean/Dockerfile using lean-cli/foundation:latest as base image.
-          5. The lean-cli/research:latest image is built from Lean/DockerfileJupyter using lean-cli/engine:latest as base image.
-          6. The default engine image is set to lean-cli/engine:latest.
-          7. The default research image is set to lean-cli/research:latest.
+          3. The lean-cli/engine:latest image is built from Lean/Dockerfile using lean-cli/foundation:latest as base image.
+          4. The lean-cli/research:latest image is built from Lean/DockerfileJupyter using lean-cli/engine:latest as base image.
+          5. The default engine image is set to lean-cli/engine:latest.
+          6. The default research image is set to lean-cli/research:latest.
         
           When the foundation Dockerfile is the same as the official foundation Dockerfile, quantconnect/lean:foundation is used
           instead of building a custom foundation image.
         
         Options:
           --tag TEXT  The tag to apply to custom images (defaults to latest)
           --verbose   Enable debug logging
@@ -227,16 +239,14 @@
         
         Commands:
           deploy     Start live trading for a project in the cloud.
           liquidate  Stops live trading and liquidates existing positions for a certain project.
           stop       Stops live trading for a certain project without liquidating existing positions.
         ```
         
-        _See code: [lean/commands/cloud/live.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/live.py)_
-        
         ### `lean cloud live deploy`
         
         Start live trading for a project in the cloud.
         
         ```
         Usage: lean cloud live deploy [OPTIONS] PROJECT
         
@@ -246,44 +256,48 @@
         
           By default an interactive wizard is shown letting you configure the deployment. If --brokerage is given the command
           runs in non-interactive mode. In this mode the CLI does not prompt for input or confirmation. In non-interactive mode
           the options specific to the given brokerage are required, as well as --node, --auto-restart, --notify-order-events and
           --notify-insights.
         
         Options:
-          --brokerage [Paper Trading|Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Kraken|FTX]
+          --brokerage [Paper Trading|Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Trading Technologies|Kraken|TDAmeritrade]
                                           The brokerage to use
           --ib-user-name TEXT             Your Interactive Brokers username
           --ib-account TEXT               Your Interactive Brokers account id
           --ib-password TEXT              Your Interactive Brokers password
+          --ib-weekly-restart-utc-time TEXT
+                                          Weekly restart UTC time (hh:mm:ss). Each week on Sunday your algorithm is restarted at
+                                          this time, and will require 2FA verification. This is required by Interactive Brokers.
+                                          Use this option explicitly to override the default value.
           --ib-data-feed BOOLEAN          Whether the Interactive Brokers price data feed must be used instead of the
                                           QuantConnect price data feed
           --tradier-account-id TEXT       Your Tradier account id
           --tradier-access-token TEXT     Your Tradier access token
           --tradier-environment [live|paper]
                                           Whether the developer sandbox should be used
-          --oanda-environment [Practice|Trade]
-                                          The environment to run in, Practice for fxTrade Practice, Trade for fxTrade
           --oanda-account-id TEXT         Your OANDA account id
           --oanda-access-token TEXT       Your OANDA API token
+          --oanda-environment [Practice|Trade]
+                                          The environment to run in, Practice for fxTrade Practice, Trade for fxTrade
           --bitfinex-api-key TEXT         Your Bitfinex API key
           --bitfinex-api-secret TEXT      Your Bitfinex API secret
-          --gdax-use-sandbox [live|paper]
-                                          Whether the sandbox should be used
           --gdax-api-key TEXT             Your Coinbase Pro API key
           --gdax-api-secret TEXT          Your Coinbase Pro API secret
           --gdax-passphrase TEXT          Your Coinbase Pro API passphrase
+          --gdax-use-sandbox [live|paper]
+                                          Whether the sandbox should be used
           --binance-exchange-name [Binance|BinanceUS]
                                           Binance exchange name [Binance, BinanceUS]
-          --binance-use-testnet [live|paper]
-                                          Whether the testnet should be used
           --binance-api-key TEXT          Your Binance API key
           --binanceus-api-key TEXT        Your Binance API key
           --binance-api-secret TEXT       Your Binance API secret
           --binanceus-api-secret TEXT     Your Binance API secret
+          --binance-use-testnet [live|paper]
+                                          Whether the testnet should be used
           --zerodha-api-key TEXT          Your Kite Connect API key
           --zerodha-access-token TEXT     Your Kite Connect access token
           --zerodha-product-type [mis|cnc|nrml]
                                           MIS if you are targeting intraday products, CNC if you are targeting delivery
                                           products, NRML if you are targeting carry forward products
           --zerodha-trading-segment [equity|commodity]
                                           EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
@@ -295,38 +309,47 @@
           --samco-year-of-birth TEXT      Your year of birth (YYYY) registered with Samco
           --samco-product-type [mis|cnc|nrml]
                                           MIS if you are targeting intraday products, CNC if you are targeting delivery
                                           products, NRML if you are targeting carry forward products
           --samco-trading-segment [equity|commodity]
                                           EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                           commodities on MCX
+          --tt-user-name TEXT             Your Trading Technologies username
+          --tt-session-password TEXT      Your Trading Technologies session password
+          --tt-account-name TEXT          Your Trading Technologies account name
+          --tt-rest-app-key TEXT          Your Trading Technologies REST app key
+          --tt-rest-app-secret TEXT       Your Trading Technologies REST app secret
+          --tt-rest-environment TEXT      The REST environment to run in
+          --tt-order-routing-sender-comp-id TEXT
+                                          The order routing sender comp id to use
           --kraken-api-key TEXT           Your Kraken API key
           --kraken-api-secret TEXT        Your Kraken API secret
           --kraken-verification-tier [Starter|Intermediate|Pro]
                                           Your Kraken Verification Tier
-          --ftx-exchange-name [FTX|FTXUS]
-                                          FTX exchange name [FTX, FTXUS]
-          --ftx-api-key TEXT              Your FTX API key
-          --ftxus-api-key TEXT            Your FTX API key
-          --ftx-api-secret TEXT           Your FTX API secret
-          --ftxus-api-secret TEXT         Your FTX API secret
-          --ftx-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6|VIP1|VIP2|VIP3|MM1|MM2|MM3]
-                                          Your FTX Account Tier
-          --ftxus-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6|Tier7|Tier8|Tier9|VIP1|VIP2|MM1|MM2|MM3]
-                                          Your FTX Account Tier
+          --tdameritrade-api-key TEXT     Your TDAmeritrade API key
+          --tdameritrade-access-token TEXT
+                                          Your TDAmeritrade OAuth Access Token
+          --tdameritrade-account-number TEXT
+                                          Your TDAmeritrade account number
           --node TEXT                     The name or id of the live node to run on
           --auto-restart BOOLEAN          Whether automatic algorithm restarting must be enabled
           --notify-order-events BOOLEAN   Whether notifications must be sent for order events
           --notify-insights BOOLEAN       Whether notifications must be sent for emitted insights
           --notify-emails TEXT            A comma-separated list of 'email:subject' pairs configuring email-notifications
           --notify-webhooks TEXT          A comma-separated list of 'url:HEADER_1=VALUE_1:HEADER_2=VALUE_2:etc' pairs
                                           configuring webhook-notifications
           --notify-sms TEXT               A comma-separated list of phone numbers configuring SMS-notifications
+          --notify-telegram TEXT          A comma-separated list of 'user/group Id:token(optional)' pairs configuring telegram-
+                                          notifications
+          --live-cash-balance TEXT        A comma-separated list of currency:amount pairs of initial cash balance
+          --live-holdings TEXT            A comma-separated list of symbol:symbolId:quantity:averagePrice of initial portfolio
+                                          holdings
           --push                          Push local modifications to the cloud before starting live trading
           --open                          Automatically open the live results in the browser once the deployment starts
+          --show-secrets                  Show secrets as they are input
           --verbose                       Enable debug logging
           --help                          Show this message and exit.
         ```
         
         _See code: [lean/commands/cloud/live/deploy.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/live/deploy.py)_
         
         ### `lean cloud live liquidate`
@@ -432,15 +455,15 @@
         ```
         Usage: lean cloud push [OPTIONS]
         
           Push local projects to QuantConnect.
         
           This command overrides the content of cloud files with the content of their respective local counterparts.
         
-          This command will not delete cloud files which don't have a local counterpart.
+          This command will delete cloud files which don't have a local counterpart.
         
         Options:
           --project DIRECTORY  Path to the local project to push (all local projects if not specified)
           --verbose            Enable debug logging
           --help               Show this message and exit.
         ```
         
@@ -535,15 +558,15 @@
           --help     Show this message and exit.
         ```
         
         _See code: [lean/commands/config/unset.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/config/unset.py)_
         
         ### `lean create-project`
         
-        Create a new project containing starter code.
+        Alias for 'project-create'
         
         ```
         Usage: lean create-project [OPTIONS] NAME
         
           Create a new project containing starter code.
         
           If NAME is a path containing subdirectories those will be created automatically.
@@ -568,26 +591,25 @@
           Purchase and download data from QuantConnect Datasets.
         
           An interactive wizard will show to walk you through the process of selecting data, accepting the CLI API Access and
           Data Agreement and payment. After this wizard the selected data will be downloaded automatically.
         
           If --dataset is given the command runs in non-interactive mode. In this mode the CLI does not prompt for input or
           confirmation but only halts when the agreement must be accepted. In non-interactive mode all options specific to the
-          selected dataset as well as --organization are required.
+          selected dataset are required.
         
           See the following url for the data that can be purchased and downloaded with this command:
           https://www.quantconnect.com/datasets
         
         Options:
-          --dataset TEXT       The name of the dataset to download non-interactively
-          --organization TEXT  The name or id of the organization to purchase and download data with
-          --overwrite          Overwrite existing local data
-          --lean-config FILE   The Lean configuration file that should be used (defaults to the nearest lean.json)
-          --verbose            Enable debug logging
-          --help               Show this message and exit.
+          --dataset TEXT      The name of the dataset to download non-interactively
+          --overwrite         Overwrite existing local data
+          --lean-config FILE  The Lean configuration file that should be used (defaults to the nearest lean.json)
+          --verbose           Enable debug logging
+          --help              Show this message and exit.
         ```
         
         _See code: [lean/commands/data/download.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/data/download.py)_
         
         ### `lean data generate`
         
         Generate random market data.
@@ -622,14 +644,15 @@
           By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
           can set the default engine image for all commands using `lean config set engine-image <image>`.
         
         Options:
           --start [yyyyMMdd]              Start date for the data to generate in yyyyMMdd format  [required]
           --end [yyyyMMdd]                End date for the data to generate in yyyyMMdd format (defaults to today)
           --symbol-count INTEGER RANGE    The number of symbols to generate data for  [x>=0; required]
+          --tickers TEXT                  Comma separated list of tickers to use for generated data
           --security-type [Equity|Forex|Cfd|Future|Crypto|Option]
                                           The security type to generate data for (defaults to Equity)
           --resolution [Tick|Second|Minute|Hour|Daily]
                                           The resolution of the generated data (defaults to Minute)
           --data-density [Dense|Sparse|VerySparse]
                                           The density of the generated data (defaults to Dense)
           --include-coarse BOOLEAN        Whether coarse universe data should be generated for Equity data (defaults to True)
@@ -639,26 +662,46 @@
           --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
           --verbose                       Enable debug logging
           --help                          Show this message and exit.
         ```
         
         _See code: [lean/commands/data/generate.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/data/generate.py)_
         
+        ### `lean delete-project`
+        
+        Alias for 'project-delete'
+        
+        ```
+        Usage: lean delete-project [OPTIONS] PROJECT
+        
+          Delete a project locally and in the cloud if it exists.
+        
+          The project is selected by name or cloud id.
+        
+        Options:
+          --verbose  Enable debug logging
+          --help     Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/delete_project.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/delete_project.py)_
+        
         ### `lean init`
         
         Scaffold a Lean configuration file and data directory.
         
         ```
         Usage: lean init [OPTIONS]
         
           Scaffold a Lean configuration file and data directory.
         
         Options:
-          --verbose  Enable debug logging
-          --help     Show this message and exit.
+          --organization TEXT             The name or id of the organization the Lean CLI will be scaffolded for
+          -l, --language [python|csharp]  The default language to use for new projects
+          --verbose                       Enable debug logging
+          --help                          Show this message and exit.
         ```
         
         _See code: [lean/commands/init.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/init.py)_
         
         ### `lean library add`
         
         Add a custom library to a project.
@@ -666,33 +709,37 @@
         ```
         Usage: lean library add [OPTIONS] PROJECT NAME
         
           Add a custom library to a project.
         
           PROJECT must be the path to the project.
         
-          NAME must be the name of a NuGet package (for C# projects) or of a PyPI package (for Python projects).
+          NAME must be either the name of a NuGet package (for C# projects), a PyPI package (for Python projects), or a path to
+          a Lean CLI library.
         
-          If --version is not given, the package is pinned to the latest compatible version. For C# projects, this is the latest
-          available version. For Python projects, this is the latest version compatible with Python 3.6 (which is what the
-          Docker images use).
+          If --version is not given, and the library is a NuGet or PyPI package the package, it is pinned to the latest
+          compatible version. For C# projects, this is the latest available version. For Python projects, this is the latest
+          version compatible with Python 3.8 (which is what the Docker images use). For Lean CLI library projects, this is
+          ignored.
         
           Custom C# libraries are added to your project's .csproj file, which is then restored if dotnet is on your PATH and the
           --no-local flag has not been given.
         
           Custom Python libraries are added to your project's requirements.txt file and are installed in your local Python
           environment so you get local autocomplete for the library. The last step can be skipped with the --no-local flag.
         
           C# example usage:
           $ lean library add "My CSharp Project" Microsoft.ML
           $ lean library add "My CSharp Project" Microsoft.ML --version 1.5.5
+          $ lean library add "My CSharp Project" "Library/My CSharp Library"
         
           Python example usage:
           $ lean library add "My Python Project" tensorflow
           $ lean library add "My Python Project" tensorflow --version 2.5.0
+          $ lean library add "My Python Project" "Library/My Python Library"
         
         Options:
           --version TEXT  The version of the library to add (defaults to latest compatible version)
           --no-local      Skip making changes to your local environment
           --verbose       Enable debug logging
           --help          Show this message and exit.
         ```
@@ -706,15 +753,16 @@
         ```
         Usage: lean library remove [OPTIONS] PROJECT NAME
         
           Remove a custom library from a project.
         
           PROJECT must be the path to the project directory.
         
-          NAME must be the name of the NuGet package (for C# projects) or of the PyPI package (for Python projects) to remove.
+          NAME must be either the name of the NuGet package (for C# projects), the PyPI package (for Python projects), or the
+          path to the Lean CLI library to remove.
         
           Custom C# libraries are removed from the project's .csproj file, which is then restored if dotnet is on your PATH and
           the --no-local flag has not been given.
         
           Custom Python libraries are removed from the project's requirements.txt file.
         
           C# example usage:
@@ -749,16 +797,14 @@
           deploy        Start live trading a project locally using Docker.
           liquidate     Liquidate the given symbol from the latest deployment of the given project.
           stop          Stop an already running local live trading project.
           submit-order  Represents a command to submit an order to the algorithm.
           update-order  Represents a command to update a specific order by id.
         ```
         
-        _See code: [lean/commands/live.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live.py)_
-        
         ### `lean live add-security`
         
         Represents a command to add a security to the algorithm.
         
         ```
         Usage: lean live add-security [OPTIONS] PROJECT
         
@@ -824,104 +870,89 @@
           By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
           can set the default engine image for all commands using `lean config set engine-image <image>`.
         
         Options:
           --environment TEXT              The environment to use
           --output DIRECTORY              Directory to store results in (defaults to PROJECT/live/TIMESTAMP)
           -d, --detach                    Run the live deployment in a detached Docker container and return immediately
-          --brokerage [Paper Trading|Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Terminal Link|Atreyu|Trading Technologies|Kraken|FTX]
+          --brokerage [Paper Trading|Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Terminal Link|Atreyu|Trading Technologies|Kraken|TDAmeritrade]
                                           The brokerage to use
-          --data-feed [Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Terminal Link|Trading Technologies|Kraken|FTX|IQFeed|Polygon Data Feed|Custom data only]
+          --data-feed [Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Terminal Link|Kraken|TDAmeritrade|IQFeed|Polygon Data Feed|Custom data only]
                                           The data feed to use
-          --data-provider [Terminal Link|QuantConnect|Local]
+          --data-provider [QuantConnect|Local]
                                           Update the Lean configuration file to retrieve data from the given provider
-          --ib-organization TEXT          The name or id of the organization with the Interactive Brokers module subscription
           --ib-user-name TEXT             Your Interactive Brokers username
           --ib-account TEXT               Your Interactive Brokers account id
           --ib-password TEXT              Your Interactive Brokers password
-          --ib-enable-delayed-streaming-data BOOLEAN
-                                          Whether delayed data may be used when your algorithm subscribes to a security you
-                                          don't have a market data subscription for
-          --tradier-organization TEXT     The name or id of the organization with the Tradier module subscription
+          --ib-weekly-restart-utc-time TEXT
+                                          Weekly restart UTC time (hh:mm:ss). Each week on Sunday your algorithm is restarted at
+                                          this time, and will require 2FA verification. This is required by Interactive Brokers.
+                                          Use this option explicitly to override the default value.
           --tradier-account-id TEXT       Your Tradier account id
           --tradier-access-token TEXT     Your Tradier access token
           --tradier-environment [live|paper]
                                           Whether the developer sandbox should be used
-          --oanda-organization TEXT       The name or id of the organization with the Oanda module subscription
-          --oanda-environment [Practice|Trade]
-                                          The environment to run in, Practice for fxTrade Practice, Trade for fxTrade
           --oanda-account-id TEXT         Your OANDA account id
           --oanda-access-token TEXT       Your OANDA API token
-          --bitfinex-organization TEXT    The name or id of the organization with the Bitfinex module subscription
+          --oanda-environment [Practice|Trade]
+                                          The environment to run in, Practice for fxTrade Practice, Trade for fxTrade
           --bitfinex-api-key TEXT         Your Bitfinex API key
           --bitfinex-api-secret TEXT      Your Bitfinex API secret
-          --gdax-organization TEXT        The name or id of the organization with the Coinbase Pro module subscription
-          --gdax-use-sandbox [live|paper]
-                                          Whether the sandbox should be used
           --gdax-api-key TEXT             Your Coinbase Pro API key
           --gdax-api-secret TEXT          Your Coinbase Pro API secret
           --gdax-passphrase TEXT          Your Coinbase Pro API passphrase
-          --binance-organization TEXT     The name or id of the organization with the Binance module subscription
+          --gdax-use-sandbox [live|paper]
+                                          Whether the sandbox should be used
           --binance-exchange-name [Binance|BinanceUS]
                                           Binance exchange name [Binance, BinanceUS]
-          --binance-use-testnet [live|paper]
-                                          Whether the testnet should be used
           --binance-api-key TEXT          Your Binance API key
           --binanceus-api-key TEXT        Your Binance API key
           --binance-api-secret TEXT       Your Binance API secret
           --binanceus-api-secret TEXT     Your Binance API secret
-          --zerodha-organization TEXT     The name or id of the organization with the zerodha module subscription
+          --binance-use-testnet [live|paper]
+                                          Whether the testnet should be used
           --zerodha-api-key TEXT          Your Kite Connect API key
           --zerodha-access-token TEXT     Your Kite Connect access token
           --zerodha-product-type [mis|cnc|nrml]
                                           MIS if you are targeting intraday products, CNC if you are targeting delivery
                                           products, NRML if you are targeting carry forward products
           --zerodha-trading-segment [equity|commodity]
                                           EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                           commodities on MCX
           --zerodha-history-subscription [true|false]
                                           Whether you have a history API subscription for Zerodha
-          --samco-organization TEXT       The name or id of the organization with the samco module subscription
           --samco-client-id TEXT          Your Samco account Client ID
           --samco-client-password TEXT    Your Samco account password
           --samco-year-of-birth TEXT      Your year of birth (YYYY) registered with Samco
           --samco-product-type [mis|cnc|nrml]
                                           MIS if you are targeting intraday products, CNC if you are targeting delivery
                                           products, NRML if you are targeting carry forward products
           --samco-trading-segment [equity|commodity]
                                           EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                           commodities on MCX
-          --terminal-link-organization TEXT
-                                          The name or id of the organization with the Terminal Link module subscription
-          --bloomberg-environment [Production|Beta]
+          --terminal-link-environment [Production|Beta]
                                           The environment to run in
-          --bloomberg-server-host TEXT    The host of the Bloomberg server
-          --bloomberg-server-port INTEGER
-                                          The port of the Bloomberg server
-          --bloomberg-symbol-map-file FILE
-                                          The path to the Bloomberg symbol map file
-          --bloomberg-emsx-broker TEXT    The EMSX broker to use
-          --bloomberg-emsx-user-time-zone TEXT
-                                          The EMSX user timezone to use
-          --bloomberg-emsx-account TEXT   The EMSX account to use
-          --bloomberg-emsx-strategy TEXT  The EMSX strategy to use
-          --bloomberg-emsx-notes TEXT     The EMSX notes to use
-          --bloomberg-emsx-handling TEXT  The EMSX handling to use
-          --bloomberg-allow-modification BOOLEAN
-                                          Whether modification is allowed
-          --atreyu-organization TEXT      The name or id of the organization with the Atreyu module subscription
+          --terminal-link-server-host TEXT
+                                          The host of the TerminalLink server
+          --terminal-link-server-port INTEGER
+                                          The port of the TerminalLink server
+          --terminal-link-emsx-broker TEXT
+                                          The EMSX broker to use
+          --terminal-link-emsx-account TEXT
+                                          The EMSX account to use
+          --terminal-link-openfigi-api-key TEXT
+                                          The Open FIGI API key to use for mapping options
           --atreyu-host TEXT              The host of the Atreyu server
           --atreyu-req-port INTEGER       The Atreyu request port
           --atreyu-sub-port INTEGER       The Atreyu subscribe port
           --atreyu-username TEXT          Your Atreyu username
           --atreyu-password TEXT          Your Atreyu password
           --atreyu-client-id TEXT         Your Atreyu client id
           --atreyu-broker-mpid TEXT       The broker MPID to use
           --atreyu-locate-rqd TEXT        The locate rqd to use
-          --tt-organization TEXT          The name or id of the organization with the Trading Technologies module subscription
           --tt-user-name TEXT             Your Trading Technologies username
           --tt-session-password TEXT      Your Trading Technologies session password
           --tt-account-name TEXT          Your Trading Technologies account name
           --tt-rest-app-key TEXT          Your Trading Technologies REST app key
           --tt-rest-app-secret TEXT       Your Trading Technologies REST app secret
           --tt-rest-environment TEXT      The REST environment to run in
           --tt-market-data-sender-comp-id TEXT
@@ -933,41 +964,41 @@
           --tt-order-routing-sender-comp-id TEXT
                                           The order routing sender comp id to use
           --tt-order-routing-target-comp-id TEXT
                                           The order routing target comp id to use
           --tt-order-routing-host TEXT    The host of the order routing server
           --tt-order-routing-port TEXT    The port of the order routing server
           --tt-log-fix-messages BOOLEAN   Whether FIX messages should be logged
-          --kraken-organization TEXT      The name or id of the organization with the kraken module subscription
           --kraken-api-key TEXT           Your Kraken API key
           --kraken-api-secret TEXT        Your Kraken API secret
           --kraken-verification-tier [Starter|Intermediate|Pro]
                                           Your Kraken Verification Tier
-          --ftx-organization TEXT         The name or id of the organization with the FTX module subscription
-          --ftx-exchange-name [FTX|FTXUS]
-                                          FTX exchange name [FTX, FTXUS]
-          --ftx-api-key TEXT              Your FTX API key
-          --ftxus-api-key TEXT            Your FTX API key
-          --ftx-api-secret TEXT           Your FTX API secret
-          --ftxus-api-secret TEXT         Your FTX API secret
-          --ftx-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6|VIP1|VIP2|VIP3|MM1|MM2|MM3]
-                                          Your FTX Account Tier
-          --ftxus-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6|Tier7|Tier8|Tier9|VIP1|VIP2|MM1|MM2|MM3]
-                                          Your FTX Account Tier
-          --iqfeed-iqconnect FILE         The path to the IQConnect binary
+          --tdameritrade-api-key TEXT     Your TDAmeritrade API key
+          --tdameritrade-access-token TEXT
+                                          Your TDAmeritrade OAuth Access Token
+          --tdameritrade-account-number TEXT
+                                          Your TDAmeritrade account number
+          --ib-enable-delayed-streaming-data BOOLEAN
+                                          Whether delayed data may be used when your algorithm subscribes to a security you
+                                          don't have a market data subscription for
+          --iqfeed-iqconnect TEXT         The path to the IQConnect binary
           --iqfeed-username TEXT          Your IQFeed username
           --iqfeed-password TEXT          Your IQFeed password
           --iqfeed-productName TEXT       The product name of your IQFeed developer account
           --iqfeed-version TEXT           The product version of your IQFeed developer account
           --polygon-api-key TEXT          Your Polygon data feed API Key
-          --quantconnect-organization TEXT
-                                          The name or id of the organization with the QuantConnect datafeed module subscription
           --release                       Compile C# projects in release configuration instead of debug
           --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
+          --python-venv TEXT              The path of the python virtual environment to be used
+          --live-cash-balance TEXT        A comma-separated list of currency:amount pairs of initial cash balance
+          --live-holdings TEXT            A comma-separated list of symbol:symbolId:quantity:averagePrice of initial portfolio
+                                          holdings
           --update                        Pull the LEAN engine image before starting live trading
+          --show-secrets                  Show secrets as they are input
+          --no-update                     Use the local LEAN engine image instead of pulling the latest version
           --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
           --verbose                       Enable debug logging
           --help                          Show this message and exit.
         ```
         
         _See code: [lean/commands/live/deploy.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live/deploy.py)_
         
@@ -1067,14 +1098,15 @@
           If user id or API token is not provided an interactive prompt will show.
         
           Credentials are stored in ~/.lean/credentials and are removed upon running `lean logout`.
         
         Options:
           -u, --user-id TEXT    QuantConnect user id
           -t, --api-token TEXT  QuantConnect API token
+          --show-secrets        Show secrets as they are input
           --verbose             Enable debug logging
           --help                Show this message and exit.
         ```
         
         _See code: [lean/commands/login.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/login.py)_
         
         ### `lean logout`
@@ -1140,14 +1172,17 @@
           - --parameter <name> <min value> <max value> <step size>
           - --parameter my-first-parameter 1 10 0.5 --parameter my-second-parameter 20 30 5
         
           In non-interactive mode the --constraint option can be provided multiple times to configure multiple constraints:
           - --constraint "<statistic> <operator> <value>"
           - --constraint "Sharpe Ratio >= 0.5" --constraint "Drawdown < 0.25"
         
+          If --estimate is given, the optimization will not be executed.
+          The runtime estimate for the optimization will be calculated and outputted.
+        
           By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
           can set the default engine image for all commands using `lean config set engine-image <image>`.
         
         Options:
           --output DIRECTORY              Directory to store results in (defaults to PROJECT/optimizations/TIMESTAMP)
           -d, --detach                    Run the optimization in a detached Docker container and return immediately
           --optimizer-config FILE         The optimizer configuration file that should be used
@@ -1157,21 +1192,64 @@
           --target-direction [min|max]    Whether the target must be minimized or maximized
           --parameter <TEXT FLOAT FLOAT FLOAT>...
                                           The 'parameter min max step' pairs configuring the parameters to optimize
           --constraint TEXT               The 'statistic operator value' pairs configuring the constraints of the optimization
           --release                       Compile C# projects in release configuration instead of debug
           --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
           --update                        Pull the LEAN engine image before running the optimizer
+          --estimate                      Estimate optimization runtime without running it
+          --max-concurrent-backtests INTEGER RANGE
+                                          Maximum number of concurrent backtests to run  [x>=1]
+          --no-update                     Use the local LEAN engine image instead of pulling the latest version
           --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
           --verbose                       Enable debug logging
           --help                          Show this message and exit.
         ```
         
         _See code: [lean/commands/optimize.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/optimize.py)_
         
+        ### `lean project-create`
+        
+        Create a new project containing starter code.
+        
+        ```
+        Usage: lean project-create [OPTIONS] NAME
+        
+          Create a new project containing starter code.
+        
+          If NAME is a path containing subdirectories those will be created automatically.
+        
+          The default language can be set using `lean config set default-language python/csharp`.
+        
+        Options:
+          -l, --language [python|csharp]  The language of the project to create
+          --verbose                       Enable debug logging
+          --help                          Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/project_create.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/project_create.py)_
+        
+        ### `lean project-delete`
+        
+        Delete a project locally and in the cloud if it exists.
+        
+        ```
+        Usage: lean project-delete [OPTIONS] PROJECT
+        
+          Delete a project locally and in the cloud if it exists.
+        
+          The project is selected by name or cloud id.
+        
+        Options:
+          --verbose  Enable debug logging
+          --help     Show this message and exit.
+        ```
+        
+        _See code: [lean/commands/project_delete.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/project_delete.py)_
+        
         ### `lean report`
         
         Generate a report of a backtest.
         
         ```
         Usage: lean report [OPTIONS]
         
@@ -1197,14 +1275,15 @@
           -d, --detach                 Run the report creator in a detached Docker container and return immediately
           --strategy-name TEXT         Name of the strategy, will appear at the top-right corner of each page
           --strategy-version TEXT      Version number of the strategy, will appear next to the project name
           --strategy-description TEXT  Description of the strategy, will appear under the 'Strategy Description' section
           --overwrite                  Overwrite --report-destination if it already contains a file
           --image TEXT                 The LEAN engine image to use (defaults to quantconnect/lean:latest)
           --update                     Pull the LEAN engine image before running the report creator
+          --pdf                        Create a PDF version along with the HTML version of the report
           --lean-config FILE           The Lean configuration file that should be used (defaults to the nearest lean.json)
           --verbose                    Enable debug logging
           --help                       Show this message and exit.
         ```
         
         _See code: [lean/commands/report.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/report.py)_
         
@@ -1218,16 +1297,24 @@
           Run a Jupyter Lab environment locally using Docker.
         
           By default the official LEAN research image is used. You can override this using the --image option. Alternatively you
           can set the default research image using `lean config set research-image <image>`.
         
         Options:
           --port INTEGER                  The port to run Jupyter Lab on (defaults to 8888)
-          --data-provider [Terminal Link|QuantConnect|Local]
+          --data-provider [QuantConnect|Local|Terminal Link]
                                           Update the Lean configuration file to retrieve data from the given provider
+          --terminal-link-environment [Production|Beta]
+                                          The environment to run in
+          --terminal-link-server-host TEXT
+                                          The host of the TerminalLink server
+          --terminal-link-server-port INTEGER
+                                          The port of the TerminalLink server
+          --terminal-link-openfigi-api-key TEXT
+                                          The Open FIGI API key to use for mapping options
           --download-data                 Update the Lean configuration file to download data from the QuantConnect API, alias
                                           for --data-provider QuantConnect
           --data-purchase-limit INTEGER   The maximum amount of QCC to spend on downloading data during the research session
                                           when using QuantConnect as data provider
           -d, --detach                    Run Jupyter Lab in a detached Docker container and return immediately
           --no-open                       Don't open the Jupyter Lab environment in the browser after starting it
           --image TEXT                    The LEAN research image to use (defaults to quantconnect/research:latest)
@@ -1254,15 +1341,15 @@
         ```
         
         _See code: [lean/commands/whoami.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/whoami.py)_
         <!-- commands end -->
         
         ## Development
         
-        To work on the Lean CLI, clone the repository, enter an environment containing Python 3.6+ and run `pip install -r requirements.txt`. This command will install the required dependencies and installs the CLI in editable mode. This means you'll be able to edit the code and immediately see the results the next time you run `lean`.
+        To work on the Lean CLI, clone the repository, enter an environment containing Python 3.7+ and run `pip install -r requirements.txt`. This command will install the required dependencies and installs the CLI in editable mode. This means you'll be able to edit the code and immediately see the results the next time you run `lean`.
         
         If you need to add dependencies, first update `setup.py` (if it is a production dependency) or `requirements.txt` (if it is a development dependency) and then re-run `pip install -r requirements.txt`.
         
         The automated tests can be ran by running `pytest`. The filesystem and HTTP requests are mocked when running tests to make sure they run in an isolated environment.
         
         Can build the lean CLI by running `python setup.py sdist bdist_wheel` from the root of the project and to install it `pip install --force-reinstall dist/lean-dev-py3-none-any.whl`. To update the commands reference part of the readme run `python scripts/readme.py` from the root of the project, after installing the new version.
         
@@ -1270,13 +1357,13 @@
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >= 3.6
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >= 3.7
 Description-Content-Type: text/markdown
```

### Comparing `lean-1.0.99/lean/commands/whoami.py` & `lean-1.155/lean/commands/whoami.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import click
+from click import command
 
 from lean.click import LeanCommand
 from lean.container import container
 from lean.models.errors import AuthenticationError
 
 
-@click.command(cls=LeanCommand)
+@command(cls=LeanCommand)
 def whoami() -> None:
     """Display who is logged in."""
-    logger = container.logger()
-    api_client = container.api_client()
-    cli_config_manager = container.cli_config_manager()
+    logger = container.logger
+    api_client = container.api_client
+    cli_config_manager = container.cli_config_manager
 
     if cli_config_manager.user_id.get_value() is not None and cli_config_manager.api_token.get_value() is not None:
         try:
             organizations = api_client.organizations.get_all()
             logged_in = True
         except AuthenticationError:
             logged_in = False
```

### Comparing `lean-1.0.99/lean/commands/create_project.py` & `lean-1.155/lean/commands/create_project.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,27 +8,31 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from pathlib import Path
-import click
+from click import Choice, option, argument
+
 from lean.click import LeanCommand
+from lean.commands import lean
 from lean.container import container
 from lean.models.api import QCLanguage
 from lean.models.errors import MoreInfoError
 from lean.components.util.name_extraction import convert_to_class_name
+from lean.components import reserved_names
 
 DEFAULT_PYTHON_MAIN = '''
 from AlgorithmImports import *
 
 
 class $CLASS_NAME$(QCAlgorithm):
     def Initialize(self):
+        # Locally Lean installs free sample data, to download more data please visit https://www.quantconnect.com/docs/v2/lean-cli/datasets/downloading-data
         self.SetStartDate(2013, 10, 7)  # Set Start Date
         self.SetEndDate(2013, 10, 11)  # Set End Date
         self.SetCash(100000)  # Set Strategy Cash
         self.AddEquity("SPY", Resolution.Minute)
 
     def OnData(self, data):
         """OnData event is the primary entry point for your algorithm. Each new data point will be pumped in here.
@@ -77,14 +81,16 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# QuantBook Analysis Tool\\n",
                 "# For more information see https://www.quantconnect.com/docs/research/overview\\n",
                 "qb = QuantBook()\\n",
+                "# Locally Lean installs free sample data, to download more data please visit https://www.quantconnect.com/docs/v2/lean-cli/datasets/downloading-data \\n",
+                "qb.SetStartDate(2013, 10, 11)\\n",
                 "spy = qb.AddEquity(\\"SPY\\")\\n",
                 "history = qb.History(qb.Securities.Keys, 360, Resolution.Daily)\\n",
                 "\\n",
                 "# Indicator Analysis\\n",
                 "ema = qb.Indicator(ExponentialMovingAverage(10), spy.Symbol, 360, Resolution.Daily)\\n",
                 "ema.plot()"
             ]
@@ -109,15 +115,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.6.8"
+            "version": "3.8.13"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
 """.strip() + "\n"
 
@@ -126,14 +132,15 @@
 
 namespace QuantConnect.Algorithm.CSharp
 {
     public class $CLASS_NAME$ : QCAlgorithm
     {
         public override void Initialize()
         {
+            // Locally Lean installs free sample data, to download more data please visit https://www.quantconnect.com/docs/v2/lean-cli/datasets/downloading-data
             SetStartDate(2013, 10, 7); // Set Start Date
             SetEndDate(2013, 10, 11); // Set Start Date
             SetCash(100000); // Set Strategy Cash
             AddEquity("SPY", Resolution.Minute);
         }
 
         /// OnData event is the primary entry point for your algorithm. Each new data point will be pumped in here.
@@ -153,15 +160,15 @@
 LIBRARY_CSHARP_MAIN = """
 namespace QuantConnect
 {
     public class $CLASS_NAME$
     {
         /*
          * To use this library, first add it to a solution and create a project reference in your algorithm project:
-         * https://www.lean.io/docs/lean-cli/projects/libraries/project-libraries#02-C-Libraries
+         * https://www.lean.io/docs/v2/lean-cli/projects/libraries/project-libraries#02-C-Libraries
          *
          * Then add its namespace at the top of the page:
          * using QuantConnect;
          *
          * Then instantiate the class:
          * var x = new $CLASS_NAME$();
          * x.Add(1, 2);
@@ -213,14 +220,16 @@
                 "\\n",
                 "using QuantConnect;\\n",
                 "using QuantConnect.Data;\\n",
                 "using QuantConnect.Research;\\n",
                 "using QuantConnect.Algorithm;\\n",
                 "\\n",
                 "var qb = new QuantBook();\\n",
+                "// Locally Lean installs free sample data, to download more data please visit https://www.quantconnect.com/docs/v2/lean-cli/datasets/downloading-data \\n",
+                "qb.SetStartDate(2013, 10, 11);\\n",
                 "var spy = qb.AddEquity(\\"SPY\\");\\n",
                 "var history = qb.History(qb.Securities.Keys, 360, Resolution.Daily);"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -255,57 +264,76 @@
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
 """.strip() + "\n"
 
-
-@click.command(cls=LeanCommand)
-@click.argument("name", type=str)
-@click.option("--language", "-l",
-              type=click.Choice(container.cli_config_manager().default_language.allowed_values, case_sensitive=False),
+def _not_identifier_char(text):
+    problematic_char = text[-1]
+    for i in range(1, len(text)):
+        substring = text[:i]
+        if not substring.isidentifier():
+            problematic_char = substring[-1]
+            break
+    return problematic_char
+
+@lean.command(cls=LeanCommand, name="project-create", aliases=["create-project"])
+@argument("name", type=str)
+@option("--language", "-l",
+              type=Choice(container.cli_config_manager.default_language.allowed_values, case_sensitive=False),
               help="The language of the project to create")
 def create_project(name: str, language: str) -> None:
     """Create a new project containing starter code.
 
     If NAME is a path containing subdirectories those will be created automatically.
 
     The default language can be set using `lean config set default-language python/csharp`.
     """
-    cli_config_manager = container.cli_config_manager()
+    cli_config_manager = container.cli_config_manager
 
     language = language if language is not None else cli_config_manager.default_language.get_value()
     if language is None:
         raise MoreInfoError(
             "Please specify a language with --language or set the default language using `lean config set default-language python/csharp`",
-            "https://www.lean.io/docs/lean-cli/projects/project-management")
+            "https://www.lean.io/docs/v2/lean-cli/projects/project-management")
 
     full_path = Path.cwd() / name
-
-    if not container.path_manager().is_path_valid(full_path):
-        raise MoreInfoError(f"'{name}' is not a valid path",
-                            "https://www.lean.io/docs/lean-cli/key-concepts/troubleshooting#02-Common-Errors")
+    try:
+        cli_root_dir = container.lean_config_manager.get_cli_root_directory()
+        relative_path = full_path.relative_to(cli_root_dir).as_posix()
+    except MoreInfoError:
+        relative_path = name
+
+    if not container.path_manager.is_cli_path_valid(full_path) or not container.path_manager.is_name_valid(relative_path):
+        raise MoreInfoError(f"Invalid project name. Can only contain letters, numbers & spaces. Can not start with empty char ' ' or be a reserved name [ {', '.join(reserved_names)} ]",
+                         "https://www.lean.io/docs/v2/lean-cli/key-concepts/troubleshooting#02-Common-Errors")
 
     is_library_project = False
     try:
-        library_dir = container.lean_config_manager().get_cli_root_directory() / "Library"
+        library_dir = container.lean_config_manager.get_cli_root_directory() / "Library"
         is_library_project = library_dir in full_path.parents
+        if is_library_project:
+            # Make sure we always use the same casing 'Library' for the library directory
+            full_path = library_dir / full_path.relative_to(library_dir)
     except:
         # get_cli_root_directory() raises an error if there is no such directory
         pass
 
-    if is_library_project and language == "python" and not full_path.name.isidentifier():
+    id_name = full_path.name
+    if is_library_project and language == "python" and not id_name.isidentifier():
+        problematic_char = _not_identifier_char(id_name)
         raise RuntimeError(
-            f"'{full_path.name}' is not a valid Python identifier, which is required for Python library projects to be importable")
+            f"""'{id_name}' is not a valid Python identifier, which is required for Python library projects to be importable.
+Please remove the character '{problematic_char}' and retry""")
 
     if full_path.exists():
         raise RuntimeError(f"A project named '{name}' already exists, please choose a different name")
     else:
-        project_manager = container.project_manager()
+        project_manager = container.project_manager
         project_manager.create_new_project(full_path, QCLanguage.Python if language == "python" else QCLanguage.CSharp)
 
     class_name = convert_to_class_name(full_path)
 
     if language == "python":
         main_name = "main.py"
         main_content = DEFAULT_PYTHON_MAIN if not is_library_project else LIBRARY_PYTHON_MAIN
@@ -315,9 +343,15 @@
 
     with (full_path / main_name).open("w+", encoding="utf-8") as file:
         file.write(main_content.replace("$CLASS_NAME$", class_name).replace("$PROJECT_NAME$", full_path.name))
 
     with (full_path / "research.ipynb").open("w+", encoding="utf-8") as file:
         file.write(DEFAULT_PYTHON_NOTEBOOK if language == "python" else DEFAULT_CSHARP_NOTEBOOK)
 
-    logger = container.logger()
+    if language == "csharp":
+        project_manager = container.project_manager
+        project_csproj_file = project_manager.get_csproj_file_path(full_path)
+        original_csproj_content = project_csproj_file.read_text(encoding="utf-8")
+        project_manager.try_restore_csharp_project(project_csproj_file, original_csproj_content, False)
+
+    logger = container.logger
     logger.info(f"Successfully created {'Python' if language == 'python' else 'C#'} project '{name}'")
```

### Comparing `lean-1.0.99/lean/commands/logout.py` & `lean-1.155/lean/commands/logout.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import click
+from click import command
 
 from lean.click import LeanCommand
 from lean.container import container
 
 
-@click.command(cls=LeanCommand)
+@command(cls=LeanCommand)
 def logout() -> None:
     """Log out and remove stored credentials."""
-    container.credentials_storage().clear()
+    container.credentials_storage.clear()
```

### Comparing `lean-1.0.99/lean/commands/data/download.py` & `lean-1.155/lean/commands/data/download.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,39 +7,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from datetime import datetime
-import itertools
-import re
-from time import sleep
-import webbrowser
-from collections import OrderedDict
 from typing import Iterable, List, Optional
-
-import click
-from rich import box
-from rich.table import Table
+from click import command, option, confirm, pass_context, Context
 
 from lean.click import LeanCommand, ensure_options
 from lean.container import container
 from lean.models.api import QCDataInformation, QCDataVendor, QCFullOrganization, QCDatasetDelivery
 from lean.models.data import Dataset, DataFile, Product
 from lean.models.logger import Option
 
 _data_information: Optional[QCDataInformation] = None
 _presigned_terms="""
 Data Terms of Use has been signed previously.
 Find full agreement at: {link}
 ==========================================================================
 CLI API Access Agreement: On {signed_time} You Agreed:
-- Display or distribution of data obtained through CLI API Access is not permitted. 
+- Display or distribution of data obtained through CLI API Access is not permitted.
 - Data and Third Party Data obtained via CLI API Access can only be used for individual or internal employee's use.
 - Data is provided in LEAN format can not be manipulated for transmission or use in other applications.
 - QuantConnect is not liable for the quality of data received and is not responsible for trading losses.
 ==========================================================================
 """
 
 def _get_data_information(organization: QCFullOrganization) -> QCDataInformation:
@@ -47,15 +38,15 @@
 
     :param organization: the organization to get the information for
     :return: the datasources and prices information
     """
     global _data_information
 
     if _data_information is None:
-        _data_information = container.api_client().data.get_info(organization.id)
+        _data_information = container.api_client.data.get_info(organization.id)
 
     return _data_information
 
 
 def _map_data_files_to_vendors(organization: QCFullOrganization, data_files: Iterable[str]) -> List[DataFile]:
     """Maps a list of data files to the available data vendors.
 
@@ -96,25 +87,29 @@
 def _get_data_files(organization: QCFullOrganization, products: List[Product]) -> List[DataFile]:
     """Returns the unique data files of a list of products mapped to their vendor.
 
     :param organization: the organization to use the price information of
     :param products: the list of products to get the data files from
     :return: the list of unique data files containing the file and vendor for each file for each product
     """
-    unique_data_files = sorted(list(set(itertools.chain(*[product.get_data_files() for product in products]))))
+    from itertools import chain
+    unique_data_files = sorted(list(set(chain(*[product.get_data_files() for product in products]))))
     return _map_data_files_to_vendors(organization, unique_data_files)
 
 
 def _display_products(organization: QCFullOrganization, products: List[Product]) -> None:
     """Previews a list of products in pretty tables.
 
     :param organization: the organization the user selected
     :param products: the products to display
     """
-    logger = container.logger()
+    from rich import box
+    from rich.table import Table
+
+    logger = container.logger
     table = Table(box=box.SQUARE)
 
     for column in ["Dataset", "Vendor", "Details", "File count", "Price"]:
         table.add_column(column, overflow="fold")
 
     summed_price = 0
 
@@ -154,39 +149,32 @@
     if total_price != summed_price:
         logger.warn("The total price is less than the sum of all separate prices because there is overlapping data")
 
     logger.info(f"Total price: {total_price:,.0f} QCC")
     logger.info(f"Organization balance: {organization.credit.balance:,.0f} QCC")
 
 
-def _select_organization() -> QCFullOrganization:
-    """Asks the user for the organization that should be used.
-
-    :return: the selected organization
-    """
-    api_client = container.api_client()
-
-    organizations = api_client.organizations.get_all()
-    options = [Option(id=organization.id, label=organization.name) for organization in organizations]
-
-    logger = container.logger()
-    organization_id = logger.prompt_list("Select the organization to purchase and download data with", options)
-
-    return api_client.organizations.get(organization_id)
+def _get_security_master_warn() -> str:
+    return "\n".join([f"Your organization does not have an active Security Master subscription. Override the Security Master precautions will likely"
+                      f" result in inaccurate and misleading backtest results. Use this override flag at your own risk.",
+                      f"You can add the subscription at https://www.quantconnect.com/datasets/quantconnect-security-master/pricing"
+                      ])
 
 
-def _select_products_interactive(organization: QCFullOrganization, datasets: List[Dataset]) -> List[Product]:
+def _select_products_interactive(organization: QCFullOrganization, datasets: List[Dataset], force: bool) -> List[Product]:
     """Asks the user for the products that should be purchased and downloaded.
 
     :param organization: the organization that will be charged
     :param datasets: the available datasets
     :return: the list of products selected by the user
     """
+    from collections import OrderedDict
+
     products = []
-    logger = container.logger()
+    logger = container.logger
 
     category_options = {}
     for dataset in datasets:
         for category in dataset.categories:
             if category in category_options:
                 continue
 
@@ -202,31 +190,34 @@
         category = logger.prompt_list("Select a category", category_options)
 
         available_datasets = sorted((d for d in datasets if category in d.categories), key=lambda d: d.name)
         dataset: Dataset = logger.prompt_list("Select a dataset",
                                               [Option(id=d, label=d.name) for d in available_datasets])
 
         if dataset.requires_security_master and not organization.has_security_master_subscription():
-            logger.warn("\n".join([
-                f"Your organization needs to have an active Security Master subscription to download data from the '{dataset.name}' dataset",
-                f"You can add the subscription at https://www.quantconnect.com/datasets/quantconnect-security-master/pricing"
-            ]))
-            continue
+            if not force:
+                logger.warn("\n".join([
+                    f"Your organization needs to have an active Security Master subscription to download data from the '{dataset.name}' dataset",
+                    f"You can add the subscription at https://www.quantconnect.com/datasets/quantconnect-security-master/pricing"
+                ]))
+                continue
+            else:
+                logger.warn(_get_security_master_warn())
 
         option_results = OrderedDict()
-        for option in dataset.options:
-            if option.condition is None or option.condition.check(option_results):
-                option_results[option.id] = option.configure_interactive()
+        for dataset_option in dataset.options:
+            if dataset_option.condition is None or dataset_option.condition.check(option_results):
+                option_results[dataset_option.id] = dataset_option.configure_interactive()
 
         products.append(Product(dataset=dataset, option_results=option_results))
 
         logger.info("Selected data:")
         _display_products(organization, products)
 
-        if not click.confirm("Do you want to download more data?"):
+        if not confirm("Do you want to download more data?"):
             break
 
     return products
 
 
 def _confirm_organization_balance(organization: QCFullOrganization, products: List[Product]) -> None:
     """Checks whether the selected organization has enough QCC to download all selected data.
@@ -253,32 +244,36 @@
     If they have, reminds them of the agreement and moves on.
 
     The API will enforce signing the agreement at the end of the day but this is how we keep it in the process of the CLI
 
     :param organization: the organization that the user selected
     :param open_browser: whether the CLI should automatically open the agreement in the browser
     """
-    logger = container.logger()
-    api_client = container.api_client()
+    from webbrowser import open
+    from time import sleep
+    from datetime import datetime
+
+    logger = container.logger
+    api_client = container.api_client
 
     info = api_client.data.get_info(organization.id)
 
     # Is signed
     if organization.data.current:
         logger.info(_presigned_terms.format(link=info.agreement, signed_time=datetime.fromtimestamp(organization.data.signedTime)))
         sleep(1)
     else:
         if open_browser:
-            webbrowser.open(info.agreement)
+            open(info.agreement)
 
         logger.info(f"Go to the following url to accept the CLI API Access and Data Agreement:")
         logger.info(info.agreement)
         logger.info("Waiting until the CLI API Access and Data Agreement has been accepted...")
 
-        container.task_manager().poll(
+        container.task_manager.poll(
             make_request=lambda: api_client.organizations.get(organization.id),
             is_done=lambda data: data.data.current != False
         )
 
 
 def _confirm_payment(organization: QCFullOrganization, products: List[Product]) -> None:
     """Processes payment for the selected products.
@@ -289,66 +284,59 @@
     :param products: the list of products selected by the user
     """
     all_data_files = _get_data_files(organization, products)
     total_price = sum(data_file.vendor.price for data_file in all_data_files)
 
     organization_qcc = organization.credit.balance
 
-    logger = container.logger()
+    logger = container.logger
     logger.info(f"You will be charged {total_price:,.0f} QCC from your organization's QCC balance")
     logger.info(
         f"After downloading all files your organization will have {organization_qcc - total_price:,.0f} QCC left")
 
-    click.confirm("Continue?", abort=True)
+    confirm("Continue?", abort=True)
 
 
-def _get_organization_by_name_or_id(user_input: str) -> QCFullOrganization:
-    """Finds an organization by name or id.
+def _get_organization() -> QCFullOrganization:
+    """Gets the working organization
 
-    Raises an error if no organization with a matching name or id can be found.
-
-    :param user_input: the input given by the user
-    :return: the first organization with the given name or id
+    :return: The working organization in the current Lean CLI folder
     """
-    api_client = container.api_client()
-
-    if re.match("^[a-f0-9]{32}$", user_input) is not None:
-        try:
-            return api_client.organizations.get(user_input)
-        except:
-            pass
-
-    all_organizations = api_client.organizations.get_all()
-    selected_organization = next((o for o in all_organizations if o.id == user_input or o.name == user_input), None)
-
-    if selected_organization is None:
-        raise RuntimeError(f"You are not a member of an organization with name or id '{user_input}'")
+    organization_manager = container.organization_manager
+    organization_id = organization_manager.try_get_working_organization_id()
 
-    return api_client.organizations.get(selected_organization.id)
+    api_client = container.api_client
+    return api_client.organizations.get(organization_id)
 
 
 def _select_products_non_interactive(organization: QCFullOrganization,
                                      datasets: List[Dataset],
-                                     ctx: click.Context) -> List[Product]:
+                                     ctx: Context,
+                                     force: bool) -> List[Product]:
     """Asks the user for the products that should be purchased and downloaded.
 
     :param organization: the organization that will be charged
     :param datasets: the available datasets
     :param ctx: the click context of the invocation
     :return: the list of products selected by the user
     """
+    from collections import OrderedDict
+
     dataset = next((d for d in datasets if d.name.lower() == ctx.params["dataset"].lower()), None)
     if dataset is None:
         raise RuntimeError(f"There is no dataset named '{ctx.params['dataset']}'")
 
     if dataset.requires_security_master and not organization.has_security_master_subscription():
-        raise RuntimeError("\n".join([
-            f"Your organization needs to have an active Security Master subscription to download data from the '{dataset.name}' dataset",
-            f"You can add the subscription at https://www.quantconnect.com/datasets/quantconnect-security-master/pricing"
-        ]))
+        if not force:
+            raise RuntimeError("\n".join([
+                f"Your organization needs to have an active Security Master subscription to download data from the '{dataset.name}' dataset",
+                f"You can add the subscription at https://www.quantconnect.com/datasets/quantconnect-security-master/pricing"
+            ]))
+        else:
+            container.logger.warn(_get_security_master_warn())
 
     option_results = OrderedDict()
     invalid_options = []
     missing_options = []
 
     for option in dataset.options:
         if option.condition is not None and not option.condition.check(option_results):
@@ -372,89 +360,85 @@
                 joined_lines = "\n".join(lines)
                 blocks.append(f"{label}{'s' if len(lines) > 1 else ''}:\n{joined_lines}")
 
         raise RuntimeError("\n\n".join(blocks))
 
     products = [Product(dataset=dataset, option_results=option_results)]
 
-    container.logger().info("Data that will be purchased and downloaded:")
+    container.logger.info("Data that will be purchased and downloaded:")
     _display_products(organization, products)
 
     return products
 
 
 def _get_available_datasets(organization: QCFullOrganization) -> List[Dataset]:
     """Retrieves the available datasets.
 
     :param organization: the organization that will be charged
     :return: the datasets which data can be downloaded from
     """
-    cloud_datasets = container.api_client().market.list_datasets()
+    cloud_datasets = container.api_client.market.list_datasets()
     data_information = _get_data_information(organization)
 
     available_datasets = []
     for cloud_dataset in cloud_datasets:
         if cloud_dataset.delivery == QCDatasetDelivery.CloudOnly:
             continue
 
         datasource = data_information.datasources.get(str(cloud_dataset.id), None)
         if datasource is None or isinstance(datasource, list):
             if cloud_dataset.name != "Template Data Source Product":
                 name = cloud_dataset.name.strip()
                 vendor = cloud_dataset.vendorName.strip()
-                container.logger().debug(
+                container.logger.debug(
                     f"There is no datasources entry for {name} by {vendor} (id {cloud_dataset.id})")
             continue
 
         available_datasets.append(Dataset(name=cloud_dataset.name.strip(),
                                           vendor=cloud_dataset.vendorName.strip(),
                                           categories=[tag.name.strip() for tag in cloud_dataset.tags],
                                           options=datasource["options"],
                                           paths=datasource["paths"],
                                           requires_security_master=datasource["requiresSecurityMaster"]))
 
     return available_datasets
 
-@click.command(cls=LeanCommand, requires_lean_config=True, allow_unknown_options=True)
-@click.option("--dataset", type=str, help="The name of the dataset to download non-interactively")
-@click.option("--organization", type=str, help="The name or id of the organization to purchase and download data with")
-@click.option("--overwrite", is_flag=True, default=False, help="Overwrite existing local data")
-@click.pass_context
-def download(ctx: click.Context,
-             dataset: Optional[str],
-             organization: Optional[str],
-             overwrite: bool,
-             **kwargs) -> None:
+
+@command(cls=LeanCommand, requires_lean_config=True, allow_unknown_options=True)
+@option("--dataset", type=str, help="The name of the dataset to download non-interactively")
+@option("--overwrite", is_flag=True, default=False, help="Overwrite existing local data")
+@option("--force", is_flag=True, default=False, hidden=True)
+@pass_context
+def download(ctx: Context, dataset: Optional[str], overwrite: bool, force: bool, **kwargs) -> None:
     """Purchase and download data from QuantConnect Datasets.
 
     An interactive wizard will show to walk you through the process of selecting data,
     accepting the CLI API Access and Data Agreement and payment.
     After this wizard the selected data will be downloaded automatically.
 
     If --dataset is given the command runs in non-interactive mode.
     In this mode the CLI does not prompt for input or confirmation but only halts when the agreement must be accepted.
-    In non-interactive mode all options specific to the selected dataset as well as --organization are required.
+    In non-interactive mode all options specific to the selected dataset are required.
 
     \b
     See the following url for the data that can be purchased and downloaded with this command:
     https://www.quantconnect.com/datasets
     """
-    is_interactive = dataset is None and organization is None
+    organization = _get_organization()
 
+    is_interactive = dataset is None
     if not is_interactive:
-        ensure_options(["dataset", "organization"])
-        selected_organization = _get_organization_by_name_or_id(organization)
-        datasets = _get_available_datasets(selected_organization)
-        products = _select_products_non_interactive(selected_organization, datasets, ctx)
+        ensure_options(["dataset"])
+        datasets = _get_available_datasets(organization)
+        products = _select_products_non_interactive(organization, datasets, ctx, force)
     else:
-        selected_organization = _select_organization()
-        datasets = _get_available_datasets(selected_organization)
-        products = _select_products_interactive(selected_organization, datasets)
+        datasets = _get_available_datasets(organization)
+        products = _select_products_interactive(organization, datasets, force)
 
-    _confirm_organization_balance(selected_organization, products)
-    _verify_accept_agreement(selected_organization, is_interactive)
+    _confirm_organization_balance(organization, products)
+    _verify_accept_agreement(organization, is_interactive)
 
     if is_interactive:
-        _confirm_payment(selected_organization, products)
+        _confirm_payment(organization, products)
 
-    all_data_files = _get_data_files(selected_organization, products)
-    container.data_downloader().download_files(all_data_files, overwrite, selected_organization.id)
+    all_data_files = _get_data_files(organization, products)
+    container.data_downloader.download_files(all_data_files, overwrite, organization.id)
```

### Comparing `lean-1.0.99/lean/commands/data/__init__.py` & `lean-1.155/lean/commands/data/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import click
+from click import group
 
 from lean.commands.data.download import download
 from lean.commands.data.generate import generate
 
 
-@click.group()
+@group()
 def data() -> None:
     """Download or generate data for local use."""
     # This method is intentionally empty
     # It is used as the command group for all `lean data <command>` commands
     pass
```

### Comparing `lean-1.0.99/lean/commands/data/generate.py` & `lean-1.155/lean/commands/data/generate.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,64 +10,70 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from datetime import datetime
 from typing import Optional
 
-import click
+from click import command, option, Choice, IntRange
 
 from lean.click import DateParameter, LeanCommand
 from lean.constants import DEFAULT_ENGINE_IMAGE
 from lean.container import container
 
 
-@click.command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
-@click.option("--start",
+@command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
+@option("--start",
               type=DateParameter(),
               required=True,
               help="Start date for the data to generate in yyyyMMdd format")
-@click.option("--end",
+@option("--end",
               type=DateParameter(),
               default=datetime.today().strftime("%Y%m%d"),
               help="End date for the data to generate in yyyyMMdd format (defaults to today)")
-@click.option("--symbol-count",
-              type=click.IntRange(min=0),
+@option("--symbol-count",
+              type=IntRange(min=0),
               required=True,
               help="The number of symbols to generate data for")
-@click.option("--security-type",
-              type=click.Choice(["Equity", "Forex", "Cfd", "Future", "Crypto", "Option"], case_sensitive=False),
+@option("--tickers",
+              type=str,
+              required=False,
+              default="",
+              help="Comma separated list of tickers to use for generated data")
+@option("--security-type",
+              type=Choice(["Equity", "Forex", "Cfd", "Future", "Crypto", "Option"], case_sensitive=False),
               default="Equity",
               help="The security type to generate data for (defaults to Equity)")
-@click.option("--resolution",
-              type=click.Choice(["Tick", "Second", "Minute", "Hour", "Daily"], case_sensitive=False),
+@option("--resolution",
+              type=Choice(["Tick", "Second", "Minute", "Hour", "Daily"], case_sensitive=False),
               default="Minute",
               help="The resolution of the generated data (defaults to Minute)")
-@click.option("--data-density",
-              type=click.Choice(["Dense", "Sparse", "VerySparse"], case_sensitive=False),
+@option("--data-density",
+              type=Choice(["Dense", "Sparse", "VerySparse"], case_sensitive=False),
               default="Dense",
               help="The density of the generated data (defaults to Dense)")
-@click.option("--include-coarse",
+@option("--include-coarse",
               type=bool,
               default=True,
               help="Whether coarse universe data should be generated for Equity data (defaults to True)")
-@click.option("--market",
+@option("--market",
               type=str,
               default="",
               help="The market to generate data for (defaults to standard market for the security type)")
-@click.option("--image",
+@option("--image",
               type=str,
               help=f"The LEAN engine image to use (defaults to {DEFAULT_ENGINE_IMAGE})")
-@click.option("--update",
+@option("--update",
               is_flag=True,
               default=False,
               help="Pull the LEAN engine image before running the generator")
 def generate(start: datetime,
              end: datetime,
              symbol_count: int,
+             tickers: str,
              security_type: str,
              resolution: str,
              data_density: str,
              include_coarse: bool,
              market: str,
              image: Optional[str],
              update: bool) -> None:
@@ -99,38 +105,44 @@
     Example which generates daily data for 100 crypto symbols since 2015-01-01:
     $ lean data generate --start=20150101 --symbol-count=100 --security-type=Crypto --resolution=Daily
 
     By default the official LEAN engine image is used.
     You can override this using the --image option.
     Alternatively you can set the default engine image for all commands using `lean config set engine-image <image>`.
     """
-    lean_config_manager = container.lean_config_manager()
+    lean_config_manager = container.lean_config_manager
     data_dir = lean_config_manager.get_data_directory()
 
+    entrypoint = ["dotnet", "QuantConnect.ToolBox.dll",
+                  "--destination-dir", "/Lean/Data",
+                  "--app", "randomdatagenerator",
+                  "--start", start.strftime("%Y%m%d"),
+                  "--end", end.strftime("%Y%m%d"),
+                  "--symbol-count", str(symbol_count),
+                  "--security-type", security_type,
+                  "--resolution", resolution,
+                  "--data-density", data_density,
+                  "--include-coarse", str(include_coarse).lower(),
+                  "--market", market.lower()]
+
+    # Toolbox uses '--opt=val' as single argument
+    if tickers:
+        entrypoint.append("--tickers=" + tickers)
+
     run_options = {
-        "entrypoint": ["dotnet", "QuantConnect.ToolBox.dll",
-                       "--destination-dir", "/Lean/Data",
-                       "--app", "randomdatagenerator",
-                       "--start", start.strftime("%Y%m%d"),
-                       "--end", end.strftime("%Y%m%d"),
-                       "--symbol-count", str(symbol_count),
-                       "--security-type", security_type,
-                       "--resolution", resolution,
-                       "--data-density", data_density,
-                       "--include-coarse", str(include_coarse).lower(),
-                       "--market", market.lower()],
+        "entrypoint": entrypoint,
         "volumes": {
             str(data_dir): {
                 "bind": "/Lean/Data",
                 "mode": "rw"
             }
         }
     }
 
-    engine_image = container.cli_config_manager().get_engine_image(image)
+    engine_image = container.cli_config_manager.get_engine_image(image)
 
-    container.update_manager().pull_docker_image_if_necessary(engine_image, update)
+    container.update_manager.pull_docker_image_if_necessary(engine_image, update)
 
-    success = container.docker_manager().run_image(engine_image, **run_options)
+    success = container.docker_manager.run_image(engine_image, **run_options)
     if not success:
         raise RuntimeError(
             "Something went wrong while running the random data generator, see the logs above for more information")
```

### Comparing `lean-1.0.99/lean/commands/live/submit_order.py` & `lean-1.155/lean/commands/live/submit_order.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,44 +10,44 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from pathlib import Path
 from typing import Optional
-import uuid
-import click
+
+from click import command, argument, option
 from lean.click import LeanCommand, PathParameter
 from lean.commands.live.live import get_result, send_command
 from lean.components.util.click_custom_parameters import DECIMAL
 
-@click.command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
-@click.argument("project", type=PathParameter(exists=True, file_okay=True, dir_okay=True))
-@click.option("--ticker", type=str, required=True, help="The ticker of the symbol to be submitted")
-@click.option("--market", type=str, required=True, help="The market of the symbol to be submitted")
-@click.option("--security-type", required=True, type=str, help="The security type of the symbol to be submitted")
-@click.option("--order-type", type=str, required=True, help="The order type to be submitted")
-@click.option("--quantity", type=DECIMAL, required=True, help="The number of units to be ordered (directional)")
-@click.option("--limit-price", type=DECIMAL, default=0.0, help="The limit price of the order be submitted")
-@click.option("--stop-price", type=DECIMAL, default=0.0, help="The stop price of the order to be submitted")
-@click.option("--tag", type=str, help="The tag to be attached to the order")
+@command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
+@argument("project", type=PathParameter(exists=True, file_okay=True, dir_okay=True))
+@option("--ticker", type=str, required=True, help="The ticker of the symbol to be submitted")
+@option("--market", type=str, required=True, help="The market of the symbol to be submitted")
+@option("--security-type", required=True, type=str, help="The security type of the symbol to be submitted")
+@option("--order-type", type=str, required=True, help="The order type to be submitted")
+@option("--quantity", type=DECIMAL, required=True, help="The number of units to be ordered (directional)")
+@option("--limit-price", type=DECIMAL, default=0.0, help="The limit price of the order be submitted")
+@option("--stop-price", type=DECIMAL, default=0.0, help="The stop price of the order to be submitted")
+@option("--tag", type=str, help="The tag to be attached to the order")
 def submit_order(project: Path,
                  ticker: str,
                  market: str,
                  security_type: str,
                  order_type: str,
                  quantity: DECIMAL,
                  limit_price: Optional[DECIMAL],
                  stop_price: Optional[DECIMAL],
                  tag: Optional[str]) -> None:
     """
     Represents a command to submit an order to the algorithm.
     """
-
-    command_id = uuid.uuid4().hex
+    from uuid import uuid4
+    command_id = uuid4().hex
 
     data = {
         "$type": "QuantConnect.Commands.OrderCommand, QuantConnect.Common",
         "Id": command_id,
         "Ticker": ticker,
         "Market": market,
         "SecurityType": security_type,
```

### Comparing `lean-1.0.99/lean/commands/live/liquidate.py` & `lean-1.155/lean/commands/live/liquidate.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,34 +10,33 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from pathlib import Path
 from typing import Optional
-import uuid
-import click
+from click import command, argument, option
 from lean.click import LeanCommand, PathParameter
 from lean.commands.live.live import get_result, send_command
 
 
-@click.command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
-@click.argument("project", type=PathParameter(exists=True, file_okay=True, dir_okay=True))
-@click.option("--ticker", type=str, help="The ticker of the symbol to liquidate")
-@click.option("--market", type=str, help="The market of the symbol to liquidate")
-@click.option("--security-type", type=str, default=0, help="The security type of the symbol to liquidate")
+@command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
+@argument("project", type=PathParameter(exists=True, file_okay=True, dir_okay=True))
+@option("--ticker", type=str, help="The ticker of the symbol to liquidate")
+@option("--market", type=str, help="The market of the symbol to liquidate")
+@option("--security-type", type=str, default=0, help="The security type of the symbol to liquidate")
 def liquidate(project: Path,
               ticker: Optional[str],
               market: Optional[str],
               security_type: Optional[str]) -> None:
     """
     Liquidate the given symbol from the latest deployment of the given project.
     """
-
-    command_id = uuid.uuid4().hex
+    from uuid import uuid4
+    command_id = uuid4().hex
 
     data = {
         "$type": "QuantConnect.Commands.LiquidateCommand, QuantConnect.Common",
         "Id": command_id,
         "Ticker": ticker,
         "Market": market,
         "SecurityType": security_type
```

### Comparing `lean-1.0.99/lean/commands/live/deploy.py` & `lean-1.155/lean/commands/live/deploy.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,59 +7,82 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import copy
-import subprocess
-import time
-from datetime import datetime
 from pathlib import Path
-from typing import Any, Dict, List, Optional
-import click
+from typing import Any, Dict, List, Optional, Tuple
+from click import option, argument, Choice
 from lean.click import LeanCommand, PathParameter, ensure_options
 from lean.constants import DEFAULT_ENGINE_IMAGE
 from lean.container import container
 from lean.models.brokerages.local import all_local_brokerages, local_brokerage_data_feeds, all_local_data_feeds
 from lean.models.errors import MoreInfoError
+from lean.models.lean_config_configurer import LeanConfigConfigurer
 from lean.models.logger import Option
-from lean.models.configuration import Configuration, InfoConfiguration, InternalInputUserInput
-from lean.models.click_options import options_from_json
-from lean.models.json_module import JsonModule
+from lean.models.configuration import InternalInputUserInput
+from lean.models.click_options import options_from_json, get_configs_for_options
+from lean.models.json_module import LiveInitialStateInput
 from lean.commands.live.live import live
+from lean.components.util.live_utils import get_last_portfolio_cash_holdings, configure_initial_cash_balance, configure_initial_holdings,\
+                                            _configure_initial_cash_interactively, _configure_initial_holdings_interactively
 from lean.models.data_providers import all_data_providers
+from lean.components.util.json_modules_handler import build_and_configure_modules, get_and_build_module
 
 _environment_skeleton = {
     "live-mode": True,
     "setup-handler": "QuantConnect.Lean.Engine.Setup.BrokerageSetupHandler",
     "result-handler": "QuantConnect.Lean.Engine.Results.LiveTradingResultHandler",
     "data-feed-handler": "QuantConnect.Lean.Engine.DataFeeds.LiveTradingDataFeed",
     "real-time-handler": "QuantConnect.Lean.Engine.RealTime.LiveTradingRealTimeHandler"
 }
 
-def _raise_for_missing_properties(lean_config: Dict[str, Any], environment_name: str, lean_config_path: Path) -> None:
-    """Raises an error if any required properties are missing.
+
+def _get_configurable_modules_from_environment(lean_config: Dict[str, Any], environment_name: str) -> Tuple[LeanConfigConfigurer, List[LeanConfigConfigurer]]:
+    """Returns the configurable modules from the given environment.
 
     :param lean_config: the LEAN configuration that should be used
     :param environment_name: the name of the environment
-    :param lean_config_path: the path to the LEAN configuration file
+    :return: the configurable modules from the given environment
     """
     environment = lean_config["environments"][environment_name]
     for key in ["live-mode-brokerage", "data-queue-handler"]:
         if key not in environment:
             raise MoreInfoError(f"The '{environment_name}' environment does not specify a {key}",
-                                "https://www.lean.io/docs/lean-cli/live-trading")
+                                "https://www.lean.io/docs/v2/lean-cli/live-trading/algorithm-control")
 
     brokerage = environment["live-mode-brokerage"]
     data_queue_handlers = environment["data-queue-handler"]
-
     [brokerage_configurer] = [local_brokerage for local_brokerage in all_local_brokerages if local_brokerage.get_live_name(environment_name) == brokerage]
     data_feed_configurers = [local_data_feed for local_data_feed in all_local_data_feeds if local_data_feed.get_live_name(environment_name) in data_queue_handlers]
+    return brokerage_configurer, data_feed_configurers
+
+
+def _install_modules(modules: List[LeanConfigConfigurer], user_kwargs: Dict[str, Any]) -> None:
+    """Raises an error if any of the given modules are not installed.
+
+    :param modules: the modules to check
+    """
+    for module in modules:
+        if not module._installs:
+            continue
+        organization_id = container.organization_manager.try_get_working_organization_id()
+        module.ensure_module_installed(organization_id)
+
+
+def _raise_for_missing_properties(lean_config: Dict[str, Any], environment_name: str, lean_config_path: Path) -> None:
+    """Raises an error if any required properties are missing.
+
+    :param lean_config: the LEAN configuration that should be used
+    :param environment_name: the name of the environment
+    :param lean_config_path: the path to the LEAN configuration file
+    """
+    brokerage_configurer, data_feed_configurers = _get_configurable_modules_from_environment(lean_config, environment_name)
     brokerage_properties = brokerage_configurer.get_required_properties()
     data_queue_handler_properties = []
     for data_feed_configurer in data_feed_configurers:
         data_queue_handler_properties.extend(data_feed_configurer.get_required_properties())
     required_properties = list(set(brokerage_properties + data_queue_handler_properties))
     missing_properties = [p for p in required_properties if p not in lean_config or lean_config[p] == ""]
     missing_properties = set(missing_properties)
@@ -71,24 +94,26 @@
 
     missing_properties = "\n".join(f"- {p}" for p in missing_properties)
 
     raise RuntimeError(f"""
 Please configure the following missing {properties_str} in {lean_config_path}:
 {missing_properties}
 Go to the following url for documentation on {these_str} {properties_str}:
-https://www.lean.io/docs/lean-cli/live-trading
+https://www.lean.io/docs/v2/lean-cli/live-trading/brokerages/quantconnect-paper-trading
     """.strip())
 
 
 def _start_iqconnect_if_necessary(lean_config: Dict[str, Any], environment_name: str) -> None:
     """Starts IQConnect if the given environment uses IQFeed as data queue handler.
 
     :param lean_config: the LEAN configuration that should be used
     :param environment_name: the name of the environment
     """
+    from subprocess import Popen
+
     environment = lean_config["environments"][environment_name]
     if environment["data-queue-handler"] != "QuantConnect.ToolBox.IQFeed.IQFeedDataQueueHandler":
         return
 
     args = [lean_config["iqfeed-iqconnect"],
             "-product", lean_config["iqfeed-productName"],
             "-version", lean_config["iqfeed-version"]]
@@ -97,194 +122,165 @@
     if username != "":
         args.extend(["-login", username])
 
     password = lean_config.get("iqfeed-password", "")
     if password != "":
         args.extend(["-password", password])
 
-    subprocess.Popen(args)
+    Popen(args)
 
-    container.logger().info("Waiting 10 seconds for IQFeed to start")
-    time.sleep(10)
+    container.logger.info("Waiting 10 seconds for IQFeed to start")
+    from time import sleep
+    sleep(10)
 
 
-def _configure_lean_config_interactively(lean_config: Dict[str, Any], environment_name: str) -> None:
+def _configure_lean_config_interactively(lean_config: Dict[str, Any],
+                                         environment_name: str,
+                                         properties: Dict[str, Any],
+                                         show_secrets: bool) -> None:
     """Interactively configures the Lean config to use.
 
     Asks the user all questions required to set up the Lean config for local live trading.
 
     :param lean_config: the base lean config to use
     :param environment_name: the name of the environment to configure
+    :param properties: the properties to use to configure lean
+    :param show_secrets: whether to show secrets on input
     """
-    logger = container.logger()
+    logger = container.logger
 
     lean_config["environments"] = {
         environment_name: _environment_skeleton
     }
 
     brokerage = logger.prompt_list("Select a brokerage", [
         Option(id=brokerage, label=brokerage.get_name()) for brokerage in all_local_brokerages
     ])
 
-    brokerage.build(lean_config, logger).configure(lean_config, environment_name)
+    brokerage.build(lean_config, logger, properties, hide_input=not show_secrets).configure(lean_config, environment_name)
 
     data_feeds = logger.prompt_list("Select a data feed", [
         Option(id=data_feed, label=data_feed.get_name()) for data_feed in local_brokerage_data_feeds[brokerage]
     ], multiple= True)
     for data_feed in data_feeds:
         if brokerage._id == data_feed._id:
             # update essential properties, so that other dependent values can be fetched.
-            essential_properties_value = {config._id : config._value for config in brokerage.get_essential_configs()}
-            data_feed.update_configs(essential_properties_value)
-            # now required properties can be fetched as per data/filter provider from esssential properties
-            required_properties_value = {config._id : config._value for config in brokerage.get_required_configs([InternalInputUserInput])}
-            data_feed.update_configs(required_properties_value)
-            # mark configs are updated
-            #TODO: create a setter method to set the property instead.
-            setattr(data_feed, '_is_installed_and_build', True)
-        data_feed.build(lean_config, logger).configure(lean_config, environment_name)
-
-
-_cached_organizations = None
-
+            essential_properties_value = {brokerage.convert_lean_key_to_variable(config._id): config._value
+                                          for config in brokerage.get_essential_configs()}
+            properties.update(essential_properties_value)
+            logger.debug(f"live.deploy._configure_lean_config_interactively(): essential_properties_value: {brokerage._id} {essential_properties_value}")
+            # now required properties can be fetched as per data/filter provider from essential properties
+            required_properties_value = {brokerage.convert_lean_key_to_variable(config._id): config._value
+                                         for config in brokerage.get_required_configs([InternalInputUserInput])}
+            properties.update(required_properties_value)
+            logger.debug(f"live.deploy._configure_lean_config_interactively(): required_properties_value: {required_properties_value}")
+        data_feed.build(lean_config, logger, properties, hide_input=not show_secrets).configure(lean_config, environment_name)
 
-def _get_organization_id(given_input: Optional[str], label: str) -> str:
-    """Converts the organization name or id given by the user to an organization id.
-
-    Shows an interactive wizard if no input is given.
-
-    Raises an error if the user is not a member of an organization with the given name or id.
-
-    :param given_input: the input given by the user
-    :param label: the name of the module the organization id is needed for
-    :return: the id of the organization given by the user
-    """
-    global _cached_organizations
-    if _cached_organizations is None:
-        api_client = container.api_client()
-        _cached_organizations = api_client.organizations.get_all()
-
-    if given_input is not None:
-        organization = next((o for o in _cached_organizations if o.id == given_input or o.name == given_input), None)
-        if organization is None:
-            raise RuntimeError(f"You are not a member of an organization with name or id '{given_input}'")
-    else:
-        logger = container.logger()
-        options = [Option(id=organization, label=organization.name) for organization in _cached_organizations]
-        organization = logger.prompt_list(f"Select the organization with the {label} module subscription", options)
-
-    return organization.id
-
-def _get_and_build_module(target_module_name: str, module_list: List[JsonModule], properties: Dict[str, Any]):
-    [target_module] = [module for module in module_list if module.get_name() == target_module_name]
-    # update essential properties from brokerage to datafeed
-    # needs to be updated before fetching required properties
-    essential_properties = [target_module._convert_lean_key_to_variable(prop) for prop in target_module.get_essential_properties()]
-    ensure_options(essential_properties)
-    essential_properties_value = {target_module._convert_variable_to_lean_key(prop) : properties[prop] for prop in essential_properties}
-    target_module.update_configs(essential_properties_value)
-    # now required properties can be fetched as per data/filter provider from esssential properties
-    required_properties: List[str] = []
-    organization_info: Dict[str,str] = {}
-    for config in target_module.get_required_configs([InternalInputUserInput]):
-        if config.is_type_organization_id:
-            organization_info[config._id] = _get_organization_id(properties[target_module._convert_lean_key_to_variable(config._id)], target_module._id)
-            properties[target_module._convert_lean_key_to_variable(config._id)] = organization_info[config._id]
-            # skip organization id from ensure_options() because it is fetched using _get_organization_id()
-            continue
-        required_properties.append(target_module._convert_lean_key_to_variable(config._id)) 
-    ensure_options(required_properties)
-    required_properties_value = {target_module._convert_variable_to_lean_key(prop) : properties[prop] for prop in required_properties}
-    required_properties_value.update(organization_info)
-    target_module.update_configs(required_properties_value)    
-    return target_module
 
 _cached_lean_config = None
 
 
+# being used by lean.models.click_options.get_the_correct_type_default_value()
 def _get_default_value(key: str) -> Optional[Any]:
     """Returns the default value for an option based on the Lean config.
 
     :param key: the name of the property in the Lean config that supplies the default value of an option
     :return: the value of the property in the Lean config, or None if there is none
     """
     global _cached_lean_config
     if _cached_lean_config is None:
-        _cached_lean_config = container.lean_config_manager().get_lean_config()
+        _cached_lean_config = container.lean_config_manager.get_lean_config()
 
     if key not in _cached_lean_config:
         return None
 
     value = _cached_lean_config[key]
     if value == "":
         return None
 
     return value
 
-def _get_configs_for_options() -> List[Configuration]: 
-    run_options: Dict[str, Configuration] = {}
-    config_with_module_id: Dict[str, str] = {}
-    for module in all_local_brokerages + all_local_data_feeds + all_data_providers:
-        for config in module.get_all_input_configs([InternalInputUserInput, InfoConfiguration]):
-            if config._id in run_options:
-                if (config._id in config_with_module_id 
-                    and config_with_module_id[config._id] == module._id):
-                    # config of same module
-                    continue
-                else:
-                    raise ValueError(f'Options names should be unique. Duplicate key present: {config._id}')
-            run_options[config._id] = config
-            config_with_module_id[config._id] = module._id
-    return list(run_options.values())
 
 @live.command(cls=LeanCommand, requires_lean_config=True, requires_docker=True, default_command=True, name="deploy")
-@click.argument("project", type=PathParameter(exists=True, file_okay=True, dir_okay=True))
-@click.option("--environment",
+@argument("project", type=PathParameter(exists=True, file_okay=True, dir_okay=True))
+@option("--environment",
               type=str,
               help="The environment to use")
-@click.option("--output",
+@option("--output",
               type=PathParameter(exists=False, file_okay=False, dir_okay=True),
               help="Directory to store results in (defaults to PROJECT/live/TIMESTAMP)")
-@click.option("--detach", "-d",
+@option("--detach", "-d",
               is_flag=True,
               default=False,
               help="Run the live deployment in a detached Docker container and return immediately")
-@click.option("--brokerage",
-              type=click.Choice([b.get_name() for b in all_local_brokerages], case_sensitive=False),
+@option("--brokerage",
+              type=Choice([b.get_name() for b in all_local_brokerages], case_sensitive=False),
               help="The brokerage to use")
-@click.option("--data-feed",
-              type=click.Choice([d.get_name() for d in all_local_data_feeds], case_sensitive=False),
+@option("--data-feed",
+              type=Choice([d.get_name() for d in all_local_data_feeds], case_sensitive=False),
               multiple=True,
               help="The data feed to use")
-@click.option("--data-provider",
-              type=click.Choice([dp.get_name() for dp in all_data_providers], case_sensitive=False),
+@option("--data-provider",
+              type=Choice([dp.get_name() for dp in all_data_providers if dp._id != "TerminalLinkBrokerage"], case_sensitive=False),
+              default="Local",
               help="Update the Lean configuration file to retrieve data from the given provider")
-@options_from_json(_get_configs_for_options())
-@click.option("--release",
+@options_from_json(get_configs_for_options("live-local"))
+@option("--release",
               is_flag=True,
               default=False,
               help="Compile C# projects in release configuration instead of debug")
-@click.option("--image",
+@option("--image",
               type=str,
               help=f"The LEAN engine image to use (defaults to {DEFAULT_ENGINE_IMAGE})")
-@click.option("--update",
+@option("--python-venv",
+              type=str,
+              help=f"The path of the python virtual environment to be used")
+@option("--live-cash-balance",
+              type=str,
+              default="",
+              help=f"A comma-separated list of currency:amount pairs of initial cash balance")
+@option("--live-holdings",
+              type=str,
+              default="",
+              help=f"A comma-separated list of symbol:symbolId:quantity:averagePrice of initial portfolio holdings")
+@option("--update",
               is_flag=True,
               default=False,
               help="Pull the LEAN engine image before starting live trading")
+@option("--show-secrets", is_flag=True, show_default=True, default=False, help="Show secrets as they are input")
+@option("--addon-module",
+              type=str,
+              multiple=True,
+              hidden=True)
+@option("--extra-config",
+              type=(str, str),
+              multiple=True,
+              hidden=True)
+@option("--no-update",
+              is_flag=True,
+              default=False,
+              help="Use the local LEAN engine image instead of pulling the latest version")
 def deploy(project: Path,
-        environment: Optional[str],
-        output: Optional[Path],
-        detach: bool,
-        brokerage: Optional[str],
-        data_feed: Optional[str],
-        data_provider: Optional[str],
-        release: bool,
-        image: Optional[str],
-        update: bool,
-        **kwargs) -> None:
+           environment: Optional[str],
+           output: Optional[Path],
+           detach: bool,
+           brokerage: Optional[str],
+           data_feed: Optional[str],
+           data_provider: Optional[str],
+           release: bool,
+           image: Optional[str],
+           python_venv: Optional[str],
+           live_cash_balance: Optional[str],
+           live_holdings: Optional[str],
+           update: bool,
+           show_secrets: bool,
+           addon_module: Optional[List[str]],
+           extra_config: Optional[Tuple[str, str]],
+           no_update: bool,
+           **kwargs) -> None:
     """Start live trading a project locally using Docker.
 
     \b
     If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
     If PROJECT is a file, the algorithm in the specified file will be executed.
 
     By default an interactive wizard is shown letting you configure the brokerage and data feed to use.
@@ -297,82 +293,136 @@
     The Lean config is used as fallback when a brokerage/data feed-specific option hasn't been passed in.
     If a required option is not given and cannot be found in the Lean config the command aborts.
 
     By default the official LEAN engine image is used.
     You can override this using the --image option.
     Alternatively you can set the default engine image for all commands using `lean config set engine-image <image>`.
     """
+    from copy import copy
+    from datetime import datetime
     # Reset globals so we reload everything in between tests
-    global _cached_organizations
-    _cached_organizations = None
     global _cached_lean_config
     _cached_lean_config = None
 
-    project_manager = container.project_manager()
+    logger = container.logger
+
+    project_manager = container.project_manager
     algorithm_file = project_manager.find_algorithm_file(Path(project))
 
     if output is None:
         output = algorithm_file.parent / "live" / datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
 
-    lean_config_manager = container.lean_config_manager()
+    lean_config_manager = container.lean_config_manager
 
     if environment is not None and (brokerage is not None or len(data_feed) > 0):
         raise RuntimeError("--environment and --brokerage + --data-feed are mutually exclusive")
 
     if environment is not None:
         environment_name = environment
         lean_config = lean_config_manager.get_complete_lean_config(environment_name, algorithm_file, None)
     elif brokerage is not None or len(data_feed) > 0:
         ensure_options(["brokerage", "data_feed"])
 
         environment_name = "lean-cli"
         lean_config = lean_config_manager.get_complete_lean_config(environment_name, algorithm_file, None)
 
         lean_config["environments"] = {
-            environment_name: copy.copy(_environment_skeleton)
+            environment_name: copy(_environment_skeleton)
         }
 
-        [brokerage_configurer] = [_get_and_build_module(brokerage, all_local_brokerages, kwargs)]
+        [brokerage_configurer] = [get_and_build_module(brokerage, all_local_brokerages, kwargs, logger)]
         brokerage_configurer.configure(lean_config, environment_name)
 
         for df in data_feed:
-            [data_feed_configurer] = [_get_and_build_module(df, all_local_data_feeds, kwargs)]
+            [data_feed_configurer] = [get_and_build_module(df, all_local_data_feeds, kwargs, logger)]
             data_feed_configurer.configure(lean_config, environment_name)
 
     else:
         environment_name = "lean-cli"
         lean_config = lean_config_manager.get_complete_lean_config(environment_name, algorithm_file, None)
-        _configure_lean_config_interactively(lean_config, environment_name)
+        _configure_lean_config_interactively(lean_config, environment_name, kwargs, show_secrets=show_secrets)
 
     if data_provider is not None:
-        [data_provider_configurer] = [_get_and_build_module(data_provider, all_data_providers, kwargs)]
+        [data_provider_configurer] = [get_and_build_module(data_provider, all_data_providers, kwargs, logger)]
         data_provider_configurer.configure(lean_config, environment_name)
 
     if "environments" not in lean_config or environment_name not in lean_config["environments"]:
         lean_config_path = lean_config_manager.get_lean_config_path()
         raise MoreInfoError(f"{lean_config_path} does not contain an environment named '{environment_name}'",
-                            "https://www.lean.io/docs/lean-cli/live-trading")
+                            "https://www.lean.io/docs/v2/lean-cli/live-trading/brokerages/quantconnect-paper-trading")
 
     if not lean_config["environments"][environment_name]["live-mode"]:
         raise MoreInfoError(f"The '{environment_name}' is not a live trading environment (live-mode is set to false)",
-                            "https://www.lean.io/docs/lean-cli/live-trading")
+                            "https://www.lean.io/docs/v2/lean-cli/live-trading/brokerages/quantconnect-paper-trading")
+
+    env_brokerage, env_data_queue_handlers = _get_configurable_modules_from_environment(lean_config, environment_name)
+    _install_modules([env_brokerage] + env_data_queue_handlers, kwargs)
 
     _raise_for_missing_properties(lean_config, environment_name, lean_config_manager.get_lean_config_path())
 
-    project_config_manager = container.project_config_manager()
-    cli_config_manager = container.cli_config_manager()
+    project_config_manager = container.project_config_manager
+    cli_config_manager = container.cli_config_manager
 
     project_config = project_config_manager.get_project_config(algorithm_file.parent)
     engine_image = cli_config_manager.get_engine_image(image or project_config.get("engine-image", None))
 
-    container.update_manager().pull_docker_image_if_necessary(engine_image, update)
+    container.update_manager.pull_docker_image_if_necessary(engine_image, update, no_update)
 
     _start_iqconnect_if_necessary(lean_config, environment_name)
 
     if not output.exists():
         output.mkdir(parents=True)
 
-    output_config_manager = container.output_config_manager()
-    lean_config["algorithm-id"] = f"L-{output_config_manager.get_live_deployment_id(output)}"
+    if python_venv is not None and python_venv != "":
+        lean_config["python-venv"] = f'{"/" if python_venv[0] != "/" else ""}{python_venv}'
+
+    cash_balance_option, holdings_option, last_cash, last_holdings = get_last_portfolio_cash_holdings(container.api_client, env_brokerage,
+                                                                                                      project_config.get("cloud-id", None), project)
+
+    if environment is None and brokerage is None and len(data_feed) == 0:   # condition for using interactive panel
+        if cash_balance_option != LiveInitialStateInput.NotSupported:
+            live_cash_balance = _configure_initial_cash_interactively(logger, cash_balance_option, last_cash)
+
+        if holdings_option != LiveInitialStateInput.NotSupported:
+            live_holdings = _configure_initial_holdings_interactively(logger, holdings_option, last_holdings)
+    else:
+        if cash_balance_option != LiveInitialStateInput.NotSupported:
+            live_cash_balance = configure_initial_cash_balance(logger, cash_balance_option, live_cash_balance, last_cash)
+        elif live_cash_balance is not None and live_cash_balance != "":
+            raise RuntimeError(f"Custom cash balance setting is not available for {brokerage}")
+
+        if holdings_option != LiveInitialStateInput.NotSupported:
+            live_holdings = configure_initial_holdings(logger, holdings_option, live_holdings, last_holdings)
+        elif live_holdings is not None and live_holdings != "":
+            raise RuntimeError(f"Custom portfolio holdings setting is not available for {brokerage}")
+
+    if live_cash_balance:
+        lean_config["live-cash-balance"] = live_cash_balance
+    if live_holdings:
+        lean_config["live-holdings"] = [{
+            "Symbol": {
+                "Value": holding["symbol"],
+                "ID": holding["symbolId"]
+            },
+            "Quantity": holding["quantity"],
+            "AveragePrice": holding["averagePrice"]
+        } for holding in live_holdings]
+
+    if str(engine_image) != DEFAULT_ENGINE_IMAGE:
+        logger.warn(f'A custom engine image: "{engine_image}" is being used!')
+
+    # Set extra config
+    given_algorithm_id = None
+    for key, value in extra_config:
+        if key == "algorithm-id":
+            given_algorithm_id = int(value)
+        else:
+            lean_config[key] = value
+
+    output_config_manager = container.output_config_manager
+    lean_config["algorithm-id"] = f"L-{output_config_manager.get_live_deployment_id(output, given_algorithm_id)}"
+
+    # Configure addon modules
+    build_and_configure_modules(addon_module, container.organization_manager.try_get_working_organization_id(), lean_config, logger, environment_name)
 
-    lean_runner = container.lean_runner()
+    lean_runner = container.lean_runner
     lean_runner.run_lean(lean_config, environment_name, algorithm_file, output, engine_image, None, release, detach)
```

### Comparing `lean-1.0.99/lean/commands/live/live.py` & `lean-1.155/lean/commands/live/live.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,55 +7,55 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import inspect
 from typing import Any, Dict
-import click
+from click import group
 from lean.components.util.click_group_default_command import DefaultCommandGroup
 from lean.constants import COMMAND_FILE_BASENAME, COMMAND_RESULT_FILE_BASENAME
-import time
 from pathlib import Path
 from lean.container import container
 
 
-@click.group(cls=DefaultCommandGroup)
+@group(cls=DefaultCommandGroup)
 def live() -> None:
     """Interact with the local machine."""
     # This method is intentionally empty
     # It is used as the command group for all `lean cloud <command>` commands
     pass
 
 
 def get_command_file_name() -> str:
-    return Path(f'{COMMAND_FILE_BASENAME}-{int(time.time())}.json')
+    from time import time
+
+    return Path(f'{COMMAND_FILE_BASENAME}-{int(time())}.json')
 
 
 def get_result_file_name(command_id: str) -> str:
     return Path(f'{COMMAND_RESULT_FILE_BASENAME}-{command_id}.json')
 
 
 def send_command(project: Path, data: Dict[str, Any]) -> str:
     """send command to the running container of the given project.
 
     :param project: the project path
     :param data: the data to send to the container
     :return: the name of the running docker container of the given project
     """
-    logger = container.logger()
-    live_dir = container.project_config_manager().get_latest_live_directory(project)
-    docker_container_name = container.output_config_manager(
-    ).get_container_name(Path(live_dir))
+    from inspect import stack
+    logger = container.logger
+    live_dir = container.project_config_manager.get_latest_live_directory(project)
+    docker_container_name = container.output_config_manager.get_container_name(Path(live_dir))
     file_name = get_command_file_name()
     logger.info(
-        f"live.send_command(): {inspect.stack()[1].function} - sending command.")
-    container.docker_manager().write_to_file(
+        f"live.send_command(): {stack()[1].function} - sending command.")
+    container.docker_manager.write_to_file(
         docker_container_name, file_name, data)
     return docker_container_name
 
 
 def get_result(command_id: str, docker_container_name: str, container_running_required: bool = True,
                interval: int = 1, timeout: int = 30) -> None:
     """Get the result of a command.
@@ -63,26 +63,27 @@
     :param command_id: command id
     :param docker_container_name: docker container name
     :param container_running_required: should the container be alive after command execution, defaults to True
     :param interval: interval to sleep before retrying, defaults to 1
     :param timeout: time to stop trying to check for result file, defaults to 30
     :raises Exception: When the command is not executed successfully
     """
-    logger = container.logger()
+    from inspect import stack
+    logger = container.logger
     logger.info(
-        f"live.get_result(): {inspect.stack()[1].function} -  waiting for results...")
+        f"live.get_result(): {stack()[1].function} -  waiting for results...")
     result_file_path = get_result_file_name(command_id)
-    result = container.docker_manager().read_from_file(
+    result = container.docker_manager.read_from_file(
         docker_container_name, result_file_path, interval, timeout)
     if "success" in result and result["success"]:
         logger.info(
-            f"live.get_result(): {inspect.stack()[1].function} - Success: The command was executed successfully")
+            f"live.get_result(): {stack()[1].function} - Success: The command was executed successfully")
     elif "container-running" in result and not result["container-running"]:
         if container_running_required:
             raise Exception(
-                f"live.get_result(): {inspect.stack()[1].function} - Failed: The container is not running")
+                f"live.get_result(): {stack()[1].function} - Failed: The container is not running")
         else:
             logger.info(
-                f"live.get_result(): {inspect.stack()[1].function} - Success: The command was executed successfully")
+                f"live.get_result(): {stack()[1].function} - Success: The command was executed successfully")
     else:
-        raise Exception((f"live.get_result(): {inspect.stack()[1].function} - "
+        raise Exception((f"live.get_result(): {stack()[1].function} - "
                         + f"Failed: to execute the command successfully. {result['error']}"))
```

### Comparing `lean-1.0.99/lean/commands/live/add_security.py` & `lean-1.155/lean/commands/live/add_security.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,53 +10,53 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from pathlib import Path
 from typing import Optional
-import uuid
-import click
+from click import command, argument, option
 from lean.click import LeanCommand, PathParameter
 from lean.commands.live.live import get_result, send_command
 from lean.components.util.click_custom_parameters import DECIMAL
 
-@click.command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
-@click.argument("project", type=PathParameter(exists=True, file_okay=True, dir_okay=True))
-@click.option("--ticker", type=str, required=True, help="The ticker of the symbol to add")
-@click.option("--market", type=str, required=True, help="The market of the symbol to add")
-@click.option("--security-type", type=str, required=True, help="The security type of the symbol to add")
-@click.option("--resolution",
+@command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
+@argument("project", type=PathParameter(exists=True, file_okay=True, dir_okay=True))
+@option("--ticker", type=str, required=True, help="The ticker of the symbol to add")
+@option("--market", type=str, required=True, help="The market of the symbol to add")
+@option("--security-type", type=str, required=True, help="The security type of the symbol to add")
+@option("--resolution",
               type=str,
               default="Minute",
               help="The resolution of the symbol to add")
-@click.option("--fill-data-forward",
+@option("--fill-data-forward",
               is_flag=True,
               default=True,
               help="The fill forward behavior, true to fill forward, false otherwise - defaults to true")
-@click.option("--leverage",
+@option("--leverage",
               type=DECIMAL,
               default=0.0,
               help="The leverage for the security, defaults to 2 for equity, 50 for forex, and 1 for everything else")
-@click.option("--extended-market-hours",
+@option("--extended-market-hours",
               is_flag=True,
               default=False,
               help="The extended market hours flag, true to allow pre/post market data, false for only in market data")
 def add_security(project: Path,
                  ticker: str,
                  market: str,
                  security_type: str,
                  resolution: Optional[str],
                  fill_data_forward: Optional[bool],
                  leverage: Optional[DECIMAL],
                  extended_market_hours: Optional[bool]) -> None:
     """
     Represents a command to add a security to the algorithm.
     """
-    command_id = uuid.uuid4().hex
+    from uuid import uuid4
+    command_id = uuid4().hex
 
     data = {
         "$type": "QuantConnect.Commands.AddSecurityCommand, QuantConnect.Common",
         "Id": command_id,
         "Symbol": ticker,
         "Market": market,
         "SecurityType": security_type,
```

### Comparing `lean-1.0.99/lean/commands/live/cancel_order.py` & `lean-1.155/lean/commands/live/cancel_order.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,33 +9,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from pathlib import Path
-import uuid
-import click
+from click import command, argument, option
 from lean.click import LeanCommand, PathParameter
 from lean.commands.live.live import get_result, send_command
 
 
-@click.command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
-@click.argument("project", type=PathParameter(exists=True, file_okay=True, dir_okay=True))
-@click.option("--order-id",
+@command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
+@argument("project", type=PathParameter(exists=True, file_okay=True, dir_okay=True))
+@option("--order-id",
               type=int,
               required=True,
               help="The order id to be cancelled")
 def cancel_order(project: Path,
                  order_id: str) -> None:
     """
     Represents a command to cancel a specific order by id.
     """
-
-    command_id = uuid.uuid4().hex
+    from uuid import uuid4
+    command_id = uuid4().hex
 
     data = {
         "$type": "QuantConnect.Commands.CancelOrderCommand, QuantConnect.Common",
         "Id": command_id,
         "OrderId": order_id
     }
```

### Comparing `lean-1.0.99/lean/commands/live/update_order.py` & `lean-1.155/lean/commands/live/update_order.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,42 +9,43 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from pathlib import Path
-import uuid
-import click
+
+from click import command, argument, option
 from lean.click import LeanCommand, PathParameter
 from typing import Optional
 from lean.commands.live.live import get_result, send_command
 from lean.components.util.click_custom_parameters import DECIMAL
 
-@click.command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
-@click.argument("project", type=PathParameter(exists=True, file_okay=True, dir_okay=True))
-@click.option("--order-id",
+@command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
+@argument("project", type=PathParameter(exists=True, file_okay=True, dir_okay=True))
+@option("--order-id",
               type=int,
               required=True,
               help="The order id to be updated")
-@click.option("--quantity", type=DECIMAL, help="The number of units to be updated (directional)")
-@click.option("--limit-price", type=DECIMAL, help="The limit price of the order to be updated")
-@click.option("--stop-price", type=DECIMAL, help="The stop price of the order to be updated")
-@click.option("--tag", type=str, help="The tag to be attached to the order")
+@option("--quantity", type=DECIMAL, help="The number of units to be updated (directional)")
+@option("--limit-price", type=DECIMAL, help="The limit price of the order to be updated")
+@option("--stop-price", type=DECIMAL, help="The stop price of the order to be updated")
+@option("--tag", type=str, help="The tag to be attached to the order")
 def update_order(project: Path,
                  order_id: str,
                  quantity: Optional[DECIMAL],
                  limit_price: Optional[DECIMAL],
                  stop_price: Optional[DECIMAL],
                  tag: Optional[str]) -> None:
     """
     Represents a command to update a specific order by id.
     """
+    from uuid import uuid4
 
-    command_id = uuid.uuid4().hex
+    command_id = uuid4().hex
 
     data = {
         "$type": "QuantConnect.Commands.UpdateOrderCommand, QuantConnect.Common",
         "Id": command_id,
         "OrderId": order_id,
         "Quantity": quantity,
         "LimitPrice": limit_price,
```

### Comparing `lean-1.0.99/lean/commands/live/__init__.py` & `lean-1.155/lean/commands/live/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/commands/live/stop.py` & `lean-1.155/lean/commands/live/stop.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from pathlib import Path
-import uuid
-import click
+from click import command, argument
 from lean.click import LeanCommand, PathParameter
 from lean.commands.live.live import get_result, send_command
 
 
-@click.command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
-@click.argument("project", type=PathParameter(exists=True, file_okay=True, dir_okay=True))
+@command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
+@argument("project", type=PathParameter(exists=True, file_okay=True, dir_okay=True))
 def stop(project: Path) -> None:
     """
     Stop an already running local live trading project.
     """
-    command_id = uuid.uuid4().hex
+    from uuid import uuid4
+    command_id = uuid4().hex
 
     data = {
         "$type": "QuantConnect.Commands.AlgorithmStatusCommand, QuantConnect.Common",
         "Id": command_id,
         "Status": "Stopped"
     }
```

### Comparing `lean-1.0.99/lean/commands/library/remove.py` & `lean-1.155/lean/commands/library/remove.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,70 +7,71 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import shutil
-import subprocess
 from pathlib import Path
 
-import click
-from pkg_resources import Requirement
+from click import command, argument, option
 
 from lean.click import LeanCommand, PathParameter
 from lean.container import container
 from lean.models.errors import MoreInfoError
 
 
-def _remove_csharp(project_dir: Path, name: str, no_local: bool) -> None:
+def _remove_package_from_csharp_project(project_dir: Path, name: str, no_local: bool) -> None:
     """Removes a custom C# library from a C# project.
 
     Removes the library from the project's .csproj file,
     and restores the project if dotnet is on the user's PATH and no_local is False.
 
     :param project_dir: the path to the project directory
     :param name: the name of the library to remove
     :param no_local:
     """
-    logger = container.logger()
-    path_manager = container.path_manager()
+    from shutil import which
+    from subprocess import run
+    logger = container.logger
+    path_manager = container.path_manager
 
     csproj_file = next(p for p in project_dir.iterdir() if p.name.endswith(".csproj"))
     logger.info(f"Removing {name} from '{path_manager.get_relative_path(csproj_file)}'")
 
-    xml_manager = container.xml_manager()
+    xml_manager = container.xml_manager
     csproj_tree = xml_manager.parse(csproj_file.read_text(encoding="utf-8"))
 
     for package_reference in csproj_tree.findall(".//PackageReference"):
         if package_reference.get("Include", "").lower() == name.lower():
             package_reference.getparent().remove(package_reference)
 
     csproj_file.write_text(xml_manager.to_string(csproj_tree), encoding="utf-8")
 
-    if not no_local and shutil.which("dotnet") is not None:
+    if not no_local and which("dotnet") is not None:
         logger.info(f"Restoring packages in '{path_manager.get_relative_path(project_dir)}'")
 
-        process = subprocess.run(["dotnet", "restore", str(csproj_file)], cwd=project_dir)
+        process = run(["dotnet", "restore", str(csproj_file)], cwd=project_dir)
 
         if process.returncode != 0:
             raise RuntimeError("Something went wrong while restoring packages, see the logs above for more information")
 
 
-def _remove_python(project_dir: Path, name: str) -> None:
+def _remove_pypi_package_from_python_project(project_dir: Path, name: str) -> None:
     """Removes a custom Python library from a Python project.
 
     Removes the library from the project's requirements.txt file.
 
     :param project_dir: the path to the project directory
     :param name: the name of the library to remove
     """
-    logger = container.logger()
-    path_manager = container.path_manager()
+    from pkg_resources import Requirement
+
+    logger = container.logger
+    path_manager = container.path_manager
 
     requirements_file = project_dir / "requirements.txt"
     logger.info(f"Removing {name} from '{path_manager.get_relative_path(requirements_file)}'")
 
     if not requirements_file.is_file():
         return
 
@@ -86,42 +87,51 @@
             new_lines.append(line)
 
     new_content = "\n".join(new_lines).strip()
     new_content = new_content + "\n" if len(new_content) > 0 else new_content
     requirements_file.write_text(new_content, encoding="utf-8")
 
 
-@click.command(cls=LeanCommand, requires_docker=True)
-@click.argument("project", type=PathParameter(exists=True, file_okay=False, dir_okay=True))
-@click.argument("name", type=str)
-@click.option("--no-local", is_flag=True, default=False, help="Skip making changes to your local environment")
+@command(cls=LeanCommand, requires_docker=True)
+@argument("project", type=PathParameter(exists=True, file_okay=False, dir_okay=True))
+@argument("name", type=str)
+@option("--no-local", is_flag=True, default=False, help="Skip making changes to your local environment")
 def remove(project: Path, name: str, no_local: bool) -> None:
     """Remove a custom library from a project.
 
     PROJECT must be the path to the project directory.
 
-    NAME must be the name of the NuGet package (for C# projects) or of the PyPI package (for Python projects) to remove.
+    NAME must be either the name of the NuGet package (for C# projects), the PyPI package (for Python projects),
+    or the path to the Lean CLI library to remove.
 
     Custom C# libraries are removed from the project's .csproj file,
     which is then restored if dotnet is on your PATH and the --no-local flag has not been given.
 
     Custom Python libraries are removed from the project's requirements.txt file.
 
     \b
     C# example usage:
     $ lean library remove "My CSharp Project" Microsoft.ML
 
     \b
     Python example usage:
     $ lean library remove "My Python Project" tensorflow
     """
-    project_config = container.project_config_manager().get_project_config(project)
+    project_config = container.project_config_manager.get_project_config(project)
     project_language = project_config.get("algorithm-language", None)
 
     if project_language is None:
         raise MoreInfoError(f"{project} is not a Lean CLI project",
-                            "https://www.lean.io/docs/lean-cli/projects/project-management#02-Create-Projects")
+                            "https://www.lean.io/docs/v2/lean-cli/projects/project-management#02-Create-Projects")
 
-    if project_language == "CSharp":
-        _remove_csharp(project, name, no_local)
+    library_manager = container.library_manager
+    library_dir = Path(name).expanduser().resolve()
+    if library_manager.is_lean_library(library_dir):
+        if project_language == "CSharp":
+            library_manager.remove_lean_library_from_csharp_project(project, library_dir, no_local)
+        else:
+            library_manager.remove_lean_library_from_python_project(project, library_dir)
     else:
-        _remove_python(project, name)
+        if project_language == "CSharp":
+            _remove_package_from_csharp_project(project, name, no_local)
+        else:
+            _remove_pypi_package_from_python_project(project, name)
```

### Comparing `lean-1.0.99/lean/commands/library/__init__.py` & `lean-1.155/lean/components/api/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,24 +6,7 @@
 # You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-import click
-
-from lean.commands.library.add import add
-from lean.commands.library.remove import remove
-
-
-@click.group()
-def library() -> None:
-    """Manage custom libraries in a project."""
-    # This method is intentionally empty
-    # It is used as the command group for all `lean library <command>` commands
-    pass
-
-
-library.add_command(add)
-library.add_command(remove)
```

### Comparing `lean-1.0.99/lean/commands/library/add.py` & `lean-1.155/lean/commands/library/add.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,55 +7,48 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
-import platform
-import shutil
-import subprocess
-from distutils.version import StrictVersion
 from pathlib import Path
 from typing import Any, Dict, Optional, Tuple
-
-import click
-from dateutil.parser import isoparse
-from lxml import etree
-from pkg_resources import Requirement
+from lean.constants import LEAN_STRICT_PYTHON_VERSION
+from click import command, argument, option
 
 from lean.click import LeanCommand, PathParameter
 from lean.container import container
 from lean.models.errors import MoreInfoError
 
 
 def _get_nuget_package(name: str) -> Tuple[str, str]:
     """Retrieves the properly-capitalized name and the latest version of a package from NuGet.
 
     :param name: the name of the package, case in-sensitive
     :return: a tuple containing the proper name and latest version of the package, excluding pre-release versions
     """
-    http_client = container.http_client()
+    from json import loads
+    http_client = container.http_client
     generic_error = RuntimeError(f"The NuGet API is not responding")
 
     service_index_response = http_client.get("https://api.nuget.org/v3/index.json", raise_for_status=False)
     if not service_index_response.ok:
         raise generic_error
 
-    service_index = json.loads(service_index_response.text)
+    service_index = loads(service_index_response.text)
     query_url = next((x["@id"] for x in service_index["resources"] if x["@type"] == "SearchQueryService"), None)
     if query_url is None:
         raise generic_error
 
     query_response = http_client.get(f"{query_url}?q={name}&prerelease=false", raise_for_status=False)
     if not query_response.ok:
         raise generic_error
 
-    query_results = json.loads(query_response.text)
+    query_results = loads(query_response.text)
     package_data = next((p for p in query_results["data"] if p["id"].lower() == name.lower()), None)
 
     if package_data is None:
         raise RuntimeError(f"NuGet does not have a package named {name}")
 
     return package_data["id"], package_data["versions"][-1]["version"]
 
@@ -63,15 +56,16 @@
 def _add_csharp_package_to_csproj(csproj_file: Path, name: str, version: str) -> None:
     """Adds a NuGet package to a .csproj file, or updates the version if it is already added.
 
     :param csproj_file: the path to the .csproj file
     :param name: the name of the package
     :param version: the version of the package
     """
-    xml_manager = container.xml_manager()
+    from lxml import etree
+    xml_manager = container.xml_manager
     csproj_tree = xml_manager.parse(csproj_file.read_text(encoding="utf-8"))
 
     existing_package_reference = csproj_tree.find(f".//PackageReference[@Include='{name}']")
     if existing_package_reference is not None:
         existing_package_reference.set("Version", version)
     else:
         last_item_group = csproj_tree.find(".//ItemGroup[last()]")
@@ -79,57 +73,49 @@
             last_item_group = etree.SubElement(csproj_tree.find(".//Project"), "ItemGroup")
 
         last_item_group.append(etree.fromstring(f'<PackageReference Include="{name}" Version="{version}" />'))
 
     csproj_file.write_text(xml_manager.to_string(csproj_tree), encoding="utf-8")
 
 
-def _add_csharp(project_dir: Path, name: str, version: Optional[str], no_local: bool) -> None:
-    """Adds a custom C# library to a C# project.
+def _add_nuget_package_to_csharp_project(project_dir: Path, name: str, version: Optional[str], no_local: bool) -> None:
+    """Adds a NuGet package to the project in the given directory.
 
-    Adds the library to the project's .csproj file, and restores the project is dotnet is on the user's PATH.
+    Adds the library to the project's .csproj file, and restores the project if dotnet is on the user's PATH.
 
     :param project_dir: the path to the project directory
     :param name: the name of the library to add
     :param version: the version of the library to use, or None to pin to the latest version
     :param no_local: whether restoring the packages locally must be skipped
     """
-    logger = container.logger()
-    path_manager = container.path_manager()
+    logger = container.logger
 
     if version is None:
         logger.info("Retrieving latest available version from NuGet")
         name, version = _get_nuget_package(name)
 
-    csproj_file = next(p for p in project_dir.iterdir() if p.name.endswith(".csproj"))
+    project_manager = container.project_manager
+    csproj_file = project_manager.get_csproj_file_path(project_dir)
+    path_manager = container.path_manager
     logger.info(f"Adding {name} {version} to '{path_manager.get_relative_path(csproj_file)}'")
 
     original_csproj_content = csproj_file.read_text(encoding="utf-8")
     _add_csharp_package_to_csproj(csproj_file, name, version)
+    project_manager.try_restore_csharp_project(csproj_file, original_csproj_content, no_local)
 
-    if not no_local and shutil.which("dotnet") is not None:
-        logger.info(
-            f"Restoring packages in '{path_manager.get_relative_path(project_dir)}' to provide local autocomplete")
-
-        process = subprocess.run(["dotnet", "restore", str(csproj_file)], cwd=project_dir)
-
-        if process.returncode != 0:
-            logger.warn(f"Reverting the changes to '{path_manager.get_relative_path(csproj_file)}'")
-            csproj_file.write_text(original_csproj_content, encoding="utf-8")
 
-            raise RuntimeError("Something went wrong while restoring packages, see the logs above for more information")
-
-
-def _is_pypi_file_compatible(file: Dict[str, Any], required_python_version: StrictVersion) -> bool:
+def _is_pypi_file_compatible(file: Dict[str, Any], required_python_version) -> bool:
     """Checks whether a file on PyPI is compatible with the Python version in the Docker images.
 
     :param file: the data of a file on PyPI, as returned by its JSON API
     :param required_python_version: the Python version to check compatibility for
     :return: True if the file is compatible with the given Python version, False if not
     """
+    from pkg_resources import Requirement
+
     major, minor, patch = required_python_version.version
     if file["python_version"] not in [f"py{major}", f"py{major}{minor}", f"cp{major}", f"cp{major}{minor}", "source"]:
         return False
 
     if file["requires_python"] is not None:
         requires_python = file["requires_python"].rstrip(",")
         if str(required_python_version) not in Requirement.parse(f"python{requires_python}").specifier:
@@ -143,27 +129,30 @@
 
     If the version is already given, this method checks whether that version is compatible with the Docker images.
 
     :param name: the name of the package, case in-sensitive
     :param version: the version of the package
     :return: a tuple containing the proper name and latest compatible version of the package
     """
-    response = container.http_client().get(f"https://pypi.org/pypi/{name}/json", raise_for_status=False)
+    from json import loads
+    from dateutil.parser import isoparse
+    from distutils.version import StrictVersion
+
+    response = container.http_client.get(f"https://pypi.org/pypi/{name}/json", raise_for_status=False)
 
     if response.status_code == 404:
         raise RuntimeError(f"PyPI does not have a package named {name}")
 
     if not response.ok:
         raise RuntimeError(f"The PyPI API is not responding")
 
-    pypi_data = json.loads(response.text)
+    pypi_data = loads(response.text)
     name = pypi_data["info"]["name"]
 
-    required_python_version = "3.6.7" if platform.machine() in ["arm64", "aarch64"] else "3.6.8"
-    required_python_version = StrictVersion(required_python_version)
+    required_python_version = StrictVersion(LEAN_STRICT_PYTHON_VERSION)
 
     last_compatible_version = None
     last_compatible_version_upload_time = None
 
     if version is not None:
         if version not in pypi_data["releases"]:
             raise RuntimeError(f"Version {version} of the {name} package does not exist")
@@ -194,14 +183,16 @@
 def _add_python_package_to_requirements(requirements_file: Path, name: str, version: str) -> None:
     """Adds a PyPI package to a requirements.txt file, or updates the version if it is already added.
 
     :param requirements_file: the path to the requirements.txt file (created if it does not exist yet)
     :param name: the name of the package
     :param version: the version of the package
     """
+    from pkg_resources import Requirement
+
     if not requirements_file.is_file():
         requirements_file.touch()
 
     requirements_lines = requirements_file.read_text(encoding="utf-8").splitlines()
 
     new_lines = []
     requirement_added = False
@@ -221,86 +212,105 @@
         new_lines.append(f"{name}=={version}")
 
     new_content = "\n".join(new_lines).strip()
     new_content = new_content + "\n" if len(new_content) > 0 else new_content
     requirements_file.write_text(new_content, encoding="utf-8")
 
 
-def _add_python(project_dir: Path, name: str, version: Optional[str], no_local: bool) -> None:
+def _add_pypi_package_to_python_project(project_dir: Path, name: str, version: Optional[str], no_local: bool) -> None:
     """Adds a custom Python library to a Python project.
 
     Adds the library to the project's requirements.txt file,
     and installs it into the local Python environment to provide local autocomplete.
 
     :param project_dir: the path to the project directory
     :param name: the name of the library to add
-    :param version: the version of the library to use, or None to pin to the latest version supporting Python 3.6
+    :param version: the version of the library to use, or None to pin to the latest version supporting Python 3.8
     :param no_local: whether installing the package in the local Python environment must be skipped
     """
-    logger = container.logger()
-    path_manager = container.path_manager()
+    from subprocess import run
+    from shutil import which
+    logger = container.logger
+    path_manager = container.path_manager
 
     if version is not None:
         logger.info(f"Checking compatibility of {name} {version} with the Python version used in the Docker images")
     else:
         logger.info("Retrieving latest compatible version from PyPI")
 
     name, version = _get_pypi_package(name, version)
 
     requirements_file = project_dir / "requirements.txt"
     logger.info(f"Adding {name} {version} to '{path_manager.get_relative_path(requirements_file)}'")
 
     _add_python_package_to_requirements(requirements_file, name, version)
 
-    if not no_local and shutil.which("pip") is not None:
+    if not no_local and which("pip") is not None:
         logger.info(f"Installing {name} {version} in local Python environment to provide local autocomplete")
 
-        process = subprocess.run(["pip", "install", f"{name}=={version}"])
+        process = run(["pip", "install", f"{name}=={version}"])
 
         if process.returncode != 0:
-            raise RuntimeError(
-                f"Something went wrong while installing {name} {version} locally, see the logs above for more information")
+            raise RuntimeError(f"Something went wrong while installing {name} {version} "
+                               "locally, see the logs above for more information")
 
 
-@click.command(cls=LeanCommand)
-@click.argument("project", type=PathParameter(exists=True, file_okay=False, dir_okay=True))
-@click.argument("name", type=str)
-@click.option("--version", type=str, help="The version of the library to add (defaults to latest compatible version)")
-@click.option("--no-local", is_flag=True, default=False, help="Skip making changes to your local environment")
+@command(cls=LeanCommand)
+@argument("project", type=PathParameter(exists=True, file_okay=False, dir_okay=True))
+@argument("name", type=str)
+@option("--version", type=str, help="The version of the library to add (defaults to latest compatible version)")
+@option("--no-local", is_flag=True, default=False, help="Skip making changes to your local environment")
 def add(project: Path, name: str, version: Optional[str], no_local: bool) -> None:
     """Add a custom library to a project.
 
     PROJECT must be the path to the project.
 
-    NAME must be the name of a NuGet package (for C# projects) or of a PyPI package (for Python projects).
+    NAME must be either the name of a NuGet package (for C# projects), a PyPI package (for Python projects),
+    or a path to a Lean CLI library.
 
-    If --version is not given, the package is pinned to the latest compatible version.
+    If --version is not given, and the library is a NuGet or PyPI package the package, it is pinned to the latest
+    compatible version.
     For C# projects, this is the latest available version.
-    For Python projects, this is the latest version compatible with Python 3.6 (which is what the Docker images use).
+    For Python projects, this is the latest version compatible with Python 3.8 (which is what the Docker images use).
+    For Lean CLI library projects, this is ignored.
 
     Custom C# libraries are added to your project's .csproj file,
     which is then restored if dotnet is on your PATH and the --no-local flag has not been given.
 
     Custom Python libraries are added to your project's requirements.txt file and are installed in your local Python
     environment so you get local autocomplete for the library. The last step can be skipped with the --no-local flag.
 
     \b
     C# example usage:
     $ lean library add "My CSharp Project" Microsoft.ML
     $ lean library add "My CSharp Project" Microsoft.ML --version 1.5.5
+    $ lean library add "My CSharp Project" "Library/My CSharp Library"
 
     \b
     Python example usage:
     $ lean library add "My Python Project" tensorflow
     $ lean library add "My Python Project" tensorflow --version 2.5.0
+    $ lean library add "My Python Project" "Library/My Python Library"
     """
-    project_config = container.project_config_manager().get_project_config(project)
+    logger = container.logger
+    project_config = container.project_config_manager.get_project_config(project)
     project_language = project_config.get("algorithm-language", None)
 
     if project_language is None:
         raise MoreInfoError(f"{project} is not a Lean CLI project",
-                            "https://www.lean.io/docs/lean-cli/projects/project-management#02-Create-Projects")
+                            "https://www.lean.io/docs/v2/lean-cli/projects/project-management#02-Create-Projects")
 
-    if project_language == "CSharp":
-        _add_csharp(project, name, version, no_local)
+    library_manager = container.library_manager
+    library_dir = Path(name).expanduser().resolve()
+
+    if library_manager.is_lean_library(library_dir):
+        logger.info(f"Adding Lean CLI library {library_dir} to project {project}")
+        if project_language == "CSharp":
+            library_manager.add_lean_library_to_csharp_project(project, library_dir, no_local)
+        else:
+            library_manager.add_lean_library_to_python_project(project, library_dir)
     else:
-        _add_python(project, name, version, no_local)
+        logger.info(f"Adding package {name} to project {project}")
+        if project_language == "CSharp":
+            _add_nuget_package_to_csharp_project(project, name, version, no_local)
+        else:
+            _add_pypi_package_to_python_project(project, name, version, no_local)
```

### Comparing `lean-1.0.99/lean/commands/cloud/status.py` & `lean-1.155/lean/commands/cloud/status.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,33 +7,33 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import click
+from click import command, argument
 
 from lean.click import LeanCommand
 from lean.container import container
 from lean.models.api import QCLiveAlgorithmStatus
 from lean.models.brokerages.cloud import all_cloud_brokerages, PaperTradingBrokerage
 
 
-@click.command(cls=LeanCommand)
-@click.argument("project", type=str)
+@command(cls=LeanCommand)
+@argument("project", type=str)
 def status(project: str) -> None:
     """Show the live trading status of a project in the cloud.
 
     PROJECT must be the name or the id of the project to show the status for.
     """
-    logger = container.logger()
-    api_client = container.api_client()
+    logger = container.logger
+    api_client = container.api_client
 
-    cloud_project_manager = container.cloud_project_manager()
+    cloud_project_manager = container.cloud_project_manager
     cloud_project = cloud_project_manager.get_cloud_project(project, False)
 
     live_algorithm = next((d for d in api_client.live.get_all() if d.projectId == cloud_project.projectId), None)
 
     logger.info(f"Project id: {cloud_project.projectId}")
     logger.info(f"Project name: {cloud_project.name}")
     logger.info(f"Project url: {cloud_project.get_url()}")
```

### Comparing `lean-1.0.99/lean/commands/cloud/pull.py` & `lean-1.155/lean/commands/cloud/live/stop.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,40 +7,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Optional
-
-import click
 
+from click import command, argument
 from lean.click import LeanCommand
 from lean.container import container
 
 
-@click.command(cls=LeanCommand)
-@click.option("--project", type=str, help="Name or id of the project to pull (all cloud projects if not specified)")
-@click.option("--pull-bootcamp", is_flag=True, default=False, help="Pull Boot Camp projects (disabled by default)")
-def pull(project: Optional[str], pull_bootcamp: bool) -> None:
-    """Pull projects from QuantConnect to the local drive.
-
-    This command overrides the content of local files with the content of their respective counterparts in the cloud.
-
-    This command will not delete local files for which there is no counterpart in the cloud.
+@command(cls=LeanCommand)
+@argument("project", type=str)
+def stop(project: str) -> None:
     """
-    api_client = container.api_client()
-    all_projects = api_client.projects.get_all()
+    Stops live trading for a certain project without liquidating existing positions.
+    """
+    logger = container.logger
+    api_client = container.api_client
 
-    # Parse which projects need to be pulled
-    if project is not None:
-        projects_to_pull = [p for p in all_projects if str(p.projectId) == project or p.name == project]
-        if len(projects_to_pull) == 0:
-            raise RuntimeError("No project with the given name or id exists in the cloud")
+    cloud_project_manager = container.cloud_project_manager
+    cloud_project = cloud_project_manager.get_cloud_project(project, False)
+    logger.info(f"cloud.live.stop(): sending command.")
+    response = api_client.live.stop(cloud_project.projectId)
+    if response.success:
+        logger.info(f"cloud.live.stop(): command executed successfully.")
     else:
-        projects_to_pull = all_projects
-        if not pull_bootcamp:
-            projects_to_pull = [p for p in projects_to_pull if not p.name.startswith("Boot Camp/")]
+        raise Exception("cloud.live.stop(): Failed: to execute the command successfully.")
+
 
-    pull_manager = container.pull_manager()
-    pull_manager.pull_projects(projects_to_pull)
```

### Comparing `lean-1.0.99/lean/commands/cloud/live/liquidate.py` & `lean-1.155/lean/commands/cloud/live/liquidate.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-import click
+from click import command, argument
 from lean.click import LeanCommand
 from lean.container import container
 
 
-@click.command(cls=LeanCommand)
-@click.argument("project", type=str)
+@command(cls=LeanCommand)
+@argument("project", type=str)
 def liquidate(project: str) -> None:
     """
     Stops live trading and liquidates existing positions for a certain project.
     """
-    logger = container.logger()
-    api_client = container.api_client()
+    logger = container.logger
+    api_client = container.api_client
 
-    cloud_project_manager = container.cloud_project_manager()
+    cloud_project_manager = container.cloud_project_manager
     cloud_project = cloud_project_manager.get_cloud_project(project, False)
     logger.info(f"cloud.live.liquidate(): sending command.")
     response = api_client.live.liquidate_and_stop(cloud_project.projectId)
     if response.success:
         logger.info(f"cloud.live.liquidate(): command executed successfully.")
     else:
-        raise Exception("cloud.live.liquidate(): Failed: to execute the command successfully.")
+        raise Exception("cloud.live.liquidate(): Failed: to execute the command successfully.")
```

### Comparing `lean-1.0.99/lean/commands/cloud/live/deploy.py` & `lean-1.155/lean/commands/cloud/live/deploy.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,91 +7,113 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import webbrowser
-from typing import Dict, List, Tuple, Optional
-import click
+from typing import Any, Dict, List, Tuple, Optional
+from click import prompt, option, argument, Choice, confirm
 from lean.click import LeanCommand, ensure_options
 from lean.components.api.api_client import APIClient
 from lean.components.util.logger import Logger
 from lean.container import container
 from lean.models.api import (QCEmailNotificationMethod, QCNode, QCNotificationMethod, QCSMSNotificationMethod,
-                             QCWebhookNotificationMethod, QCProject)
+                             QCWebhookNotificationMethod, QCTelegramNotificationMethod, QCProject)
+from lean.models.json_module import LiveInitialStateInput
 from lean.models.logger import Option
 from lean.models.brokerages.cloud.cloud_brokerage import CloudBrokerage
-from lean.models.configuration import Configuration, InfoConfiguration, InternalInputUserInput, OrganzationIdConfiguration
-from lean.models.click_options import options_from_json
+from lean.models.configuration import InternalInputUserInput
+from lean.models.click_options import options_from_json, get_configs_for_options
 from lean.models.brokerages.cloud import all_cloud_brokerages
 from lean.commands.cloud.live.live import live
+from lean.components.util.live_utils import get_last_portfolio_cash_holdings, configure_initial_cash_balance, configure_initial_holdings,\
+                                            _configure_initial_cash_interactively, _configure_initial_holdings_interactively
 
 def _log_notification_methods(methods: List[QCNotificationMethod]) -> None:
     """Logs a list of notification methods."""
-    logger = container.logger()
+    logger = container.logger
 
     email_methods = [method for method in methods if isinstance(method, QCEmailNotificationMethod)]
     email_methods = "None" if len(email_methods) == 0 else ", ".join(method.address for method in email_methods)
 
     webhook_methods = [method for method in methods if isinstance(method, QCWebhookNotificationMethod)]
     webhook_methods = "None" if len(webhook_methods) == 0 else ", ".join(method.address for method in webhook_methods)
 
     sms_methods = [method for method in methods if isinstance(method, QCSMSNotificationMethod)]
     sms_methods = "None" if len(sms_methods) == 0 else ", ".join(method.phoneNumber for method in sms_methods)
 
+    telegram_methods = [method for method in methods if isinstance(method, QCTelegramNotificationMethod)]
+    telegram_methods = "None" if len(telegram_methods) == 0 else ", ".join(f"{{{method.id}, {method.token}}}" for method in telegram_methods)
+
     logger.info(f"Email notifications: {email_methods}")
     logger.info(f"Webhook notifications: {webhook_methods}")
     logger.info(f"SMS notifications: {sms_methods}")
+    logger.info(f"Telegram notifications: {telegram_methods}")
 
 
 def _prompt_notification_method() -> QCNotificationMethod:
     """Prompts the user to add a notification method.
 
     :return: the notification method configured by the user
     """
-    logger = container.logger()
+    logger = container.logger
     selected_method = logger.prompt_list("Select a notification method", [Option(id="email", label="Email"),
                                                                           Option(id="webhook", label="Webhook"),
-                                                                          Option(id="sms", label="SMS")])
+                                                                          Option(id="sms", label="SMS"),
+                                                                          Option(id="telegram", label="Telegram")])
 
     if selected_method == "email":
-        address = click.prompt("Email address")
-        subject = click.prompt("Subject")
+        address = prompt("Email address")
+        subject = prompt("Subject")
         return QCEmailNotificationMethod(address=address, subject=subject)
     elif selected_method == "webhook":
-        address = click.prompt("URL")
+        address = prompt("URL")
         headers = {}
 
         while True:
             headers_str = "None" if headers == {} else ", ".join(f"{key}={headers[key]}" for key in headers)
             logger.info(f"Headers: {headers_str}")
 
-            if not click.confirm("Do you want to add a header?", default=False):
+            if not confirm("Do you want to add a header?", default=False):
                 break
 
-            key = click.prompt("Header key")
-            value = click.prompt("Header value")
+            key = prompt("Header key")
+            value = prompt("Header value")
             headers[key] = value
 
         return QCWebhookNotificationMethod(address=address, headers=headers)
+    elif selected_method == "telegram":
+        chat_id = prompt("User Id/Group Id")
+
+        custom_bot = confirm("Is a custom bot being used?", default=False)
+        if custom_bot:
+            token = prompt("Token (optional)")
+        else:
+            token = None
+
+        return QCTelegramNotificationMethod(id=chat_id, token=token)
     else:
-        phone_number = click.prompt("Phone number")
+        phone_number = prompt("Phone number")
         return QCSMSNotificationMethod(phoneNumber=phone_number)
 
 
-def _configure_brokerage(logger: Logger) -> CloudBrokerage:
+def _configure_brokerage(logger: Logger, user_provided_options: Dict[str, Any], show_secrets: bool) -> CloudBrokerage:
     """Interactively configures the brokerage to use.
 
     :param logger: the logger to use
+    :param user_provided_options: the dictionary containing user provided options
+    :param show_secrets: whether to show secrets on input
     :return: the cloud brokerage the user configured
     """
     brokerage_options = [Option(id=b, label=b.get_name()) for b in all_cloud_brokerages]
-    return logger.prompt_list("Select a brokerage", brokerage_options).build(None,logger)
+    return logger.prompt_list("Select a brokerage", brokerage_options).build(None,
+                                                                             logger,
+                                                                             user_provided_options,
+                                                                             hide_input=not show_secrets)
 
 
 def _configure_live_node(logger: Logger, api_client: APIClient, cloud_project: QCProject) -> QCNode:
     """Interactively configures the live node to use.
 
     :param logger: the logger to use
     :param api_client: the API client to make API requests with
@@ -113,123 +135,128 @@
     """Interactively configures how and when notifications should be sent.
 
     :param logger: the logger to use
     :return: whether notifications must be enabled for order events and insights, and the notification methods
     """
     logger.info(
         "You can optionally request for your strategy to send notifications when it generates an order or emits an insight")
-    logger.info("You can use any combination of email notifications, webhook notifications and SMS notifications")
-    notify_order_events = click.confirm("Do you want to send notifications on order events?", default=False)
-    notify_insights = click.confirm("Do you want to send notifications on insights?", default=False)
+    logger.info("You can use any combination of email notifications, webhook notifications, SMS notifications, and telegram notifications")
+    notify_order_events = confirm("Do you want to send notifications on order events?", default=False)
+    notify_insights = confirm("Do you want to send notifications on insights?", default=False)
     notify_methods = []
 
     if notify_order_events or notify_insights:
         _log_notification_methods(notify_methods)
         notify_methods.append(_prompt_notification_method())
 
         while True:
             _log_notification_methods(notify_methods)
-            if not click.confirm("Do you want to add another notification method?", default=False):
+            if not confirm("Do you want to add another notification method?", default=False):
                 break
             notify_methods.append(_prompt_notification_method())
 
     return notify_order_events, notify_insights, notify_methods
 
 
 def _configure_auto_restart(logger: Logger) -> bool:
     """Interactively configures whether automatic algorithm restarting must be enabled.
 
     :param logger: the logger to use
     :return: whether automatic algorithm restarting must be enabled
     """
     logger.info("Automatic restarting uses best efforts to restart the algorithm if it fails due to a runtime error")
     logger.info("This can help improve its resilience to temporary errors such as a brokerage API disconnection")
-    return click.confirm("Do you want to enable automatic algorithm restarting?", default=True)
+    return confirm("Do you want to enable automatic algorithm restarting?", default=True)
 
-#TODO: same duplication present in commands\live.py
-def _get_configs_for_options() -> Dict[Configuration, str]: 
-    run_options: Dict[str, Configuration] = {}
-    for module in all_cloud_brokerages:
-        for config in module.get_all_input_configs([InternalInputUserInput, InfoConfiguration]):
-            if config._id in run_options:
-                raise ValueError(f'Options names should be unique. Duplicate key present: {config._id}')
-            run_options[config._id] = config
-    return list(run_options.values())
 
 @live.command(cls=LeanCommand, default_command=True, name="deploy")
-@click.argument("project", type=str)
-@click.option("--brokerage",
-              type=click.Choice([b.get_name() for b in all_cloud_brokerages], case_sensitive=False),
+@argument("project", type=str)
+@option("--brokerage",
+              type=Choice([b.get_name() for b in all_cloud_brokerages], case_sensitive=False),
               help="The brokerage to use")
-@options_from_json(_get_configs_for_options())
-@click.option("--node", type=str, help="The name or id of the live node to run on")
-@click.option("--auto-restart", type=bool, help="Whether automatic algorithm restarting must be enabled")
-@click.option("--notify-order-events", type=bool, help="Whether notifications must be sent for order events")
-@click.option("--notify-insights", type=bool, help="Whether notifications must be sent for emitted insights")
-@click.option("--notify-emails",
+@options_from_json(get_configs_for_options("live-cloud"))
+@option("--node", type=str, help="The name or id of the live node to run on")
+@option("--auto-restart", type=bool, help="Whether automatic algorithm restarting must be enabled")
+@option("--notify-order-events", type=bool, help="Whether notifications must be sent for order events")
+@option("--notify-insights", type=bool, help="Whether notifications must be sent for emitted insights")
+@option("--notify-emails",
               type=str,
               help="A comma-separated list of 'email:subject' pairs configuring email-notifications")
-@click.option("--notify-webhooks",
+@option("--notify-webhooks",
               type=str,
               help="A comma-separated list of 'url:HEADER_1=VALUE_1:HEADER_2=VALUE_2:etc' pairs configuring webhook-notifications")
-@click.option("--notify-sms", type=str, help="A comma-separated list of phone numbers configuring SMS-notifications")
-@click.option("--push",
+@option("--notify-sms", type=str, help="A comma-separated list of phone numbers configuring SMS-notifications")
+@option("--notify-telegram", type=str, help="A comma-separated list of 'user/group Id:token(optional)' pairs configuring telegram-notifications")
+@option("--live-cash-balance",
+              type=str,
+              default="",
+              help=f"A comma-separated list of currency:amount pairs of initial cash balance")
+@option("--live-holdings",
+              type=str,
+              default="",
+              help=f"A comma-separated list of symbol:symbolId:quantity:averagePrice of initial portfolio holdings")
+@option("--push",
               is_flag=True,
               default=False,
               help="Push local modifications to the cloud before starting live trading")
-@click.option("--open", "open_browser",
+@option("--open", "open_browser",
               is_flag=True,
               default=False,
               help="Automatically open the live results in the browser once the deployment starts")
+@option("--show-secrets", is_flag=True, show_default=True, default=False, help="Show secrets as they are input")
 def deploy(project: str,
-         brokerage: str,
-         node: str,
-         auto_restart: bool,
-         notify_order_events: Optional[bool],
-         notify_insights: Optional[bool],
-         notify_emails: Optional[str],
-         notify_webhooks: Optional[str],
-         notify_sms: Optional[str],
-         push: bool,
-         open_browser: bool,
-         **kwargs) -> None:
+           brokerage: str,
+           node: str,
+           auto_restart: bool,
+           notify_order_events: Optional[bool],
+           notify_insights: Optional[bool],
+           notify_emails: Optional[str],
+           notify_webhooks: Optional[str],
+           notify_sms: Optional[str],
+           notify_telegram: Optional[str],
+           live_cash_balance: Optional[str],
+           live_holdings: Optional[str],
+           push: bool,
+           open_browser: bool,
+           show_secrets: bool,
+           **kwargs) -> None:
     """Start live trading for a project in the cloud.
 
     PROJECT must be the name or the id of the project to start live trading for.
 
     By default an interactive wizard is shown letting you configure the deployment.
     If --brokerage is given the command runs in non-interactive mode.
     In this mode the CLI does not prompt for input or confirmation.
     In non-interactive mode the options specific to the given brokerage are required,
     as well as --node, --auto-restart, --notify-order-events and --notify-insights.
     """
-    logger = container.logger()
-    api_client = container.api_client()
+    logger = container.logger
+    api_client = container.api_client
 
-    cloud_project_manager = container.cloud_project_manager()
+    cloud_project_manager = container.cloud_project_manager
     cloud_project = cloud_project_manager.get_cloud_project(project, push)
 
-    cloud_runner = container.cloud_runner()
+    cloud_runner = container.cloud_runner
     finished_compile = cloud_runner.compile_project(cloud_project)
 
     if brokerage is not None:
         ensure_options(["brokerage", "node", "auto_restart", "notify_order_events", "notify_insights"])
 
         brokerage_instance = None
         [brokerage_instance] = [cloud_brokerage for cloud_brokerage in all_cloud_brokerages if cloud_brokerage.get_name() == brokerage]
         # update essential properties from brokerage to datafeed
         # needs to be updated before fetching required properties
-        essential_properties = [brokerage_instance._convert_lean_key_to_variable(prop) for prop in brokerage_instance.get_essential_properties()]
+        essential_properties = [brokerage_instance.convert_lean_key_to_variable(prop) for prop in brokerage_instance.get_essential_properties()]
         ensure_options(essential_properties)
-        essential_properties_value = {brokerage_instance._convert_variable_to_lean_key(prop) : kwargs[prop] for prop in essential_properties}
+        essential_properties_value = {brokerage_instance.convert_variable_to_lean_key(prop) : kwargs[prop] for prop in essential_properties}
         brokerage_instance.update_configs(essential_properties_value)
         # now required properties can be fetched as per data provider from esssential properties
-        required_properties = [brokerage_instance._convert_lean_key_to_variable(prop) for prop in brokerage_instance.get_required_properties([OrganzationIdConfiguration, InternalInputUserInput])]
+        required_properties = [brokerage_instance.convert_lean_key_to_variable(prop) for prop in brokerage_instance.get_required_properties([InternalInputUserInput])]
         ensure_options(required_properties)
-        required_properties_value = {brokerage_instance._convert_variable_to_lean_key(prop) : kwargs[prop] for prop in required_properties}
+        required_properties_value = {brokerage_instance.convert_variable_to_lean_key(prop) : kwargs[prop] for prop in required_properties}
         brokerage_instance.update_configs(required_properties_value)
 
         all_nodes = api_client.nodes.get_all(cloud_project.organizationId)
         live_node = next((n for n in all_nodes.live if n.id == node or n.name == node), None)
 
         if live_node is None:
             raise RuntimeError(f"You have no live node with name or id '{node}'")
@@ -249,19 +276,47 @@
                 address, *headers = config.split(":")
                 headers = {header.split("=")[0]: header.split("=")[1] for header in headers}
                 notify_methods.append(QCWebhookNotificationMethod(address=address, headers=headers))
 
         if notify_sms is not None:
             for phoneNumber in notify_sms.split(","):
                 notify_methods.append(QCSMSNotificationMethod(phoneNumber=phoneNumber))
+
+        if notify_telegram is not None:
+            for config in notify_telegram.split(","):
+                id_token_pair = config.split(":", 1)    # telegram token is like "01234567:Abc132xxx..."
+                if len(id_token_pair) == 2:
+                    chat_id, token = id_token_pair
+                    token = None if not token else token
+                    notify_methods.append(QCTelegramNotificationMethod(id=chat_id, token=token))
+                else:
+                    notify_methods.append(QCTelegramNotificationMethod(id=id_token_pair[0]))
+
+        cash_balance_option, holdings_option, last_cash, last_holdings = get_last_portfolio_cash_holdings(api_client, brokerage_instance, cloud_project.projectId, project)
+
+        if cash_balance_option != LiveInitialStateInput.NotSupported:
+            live_cash_balance = configure_initial_cash_balance(logger, cash_balance_option, live_cash_balance, last_cash)
+        elif live_cash_balance is not None and live_cash_balance != "":
+            raise RuntimeError(f"Custom cash balance setting is not available for {brokerage_instance.get_name()}")
+
+        if holdings_option != LiveInitialStateInput.NotSupported:
+            live_holdings = configure_initial_holdings(logger, holdings_option, live_holdings, last_holdings)
+        elif live_holdings is not None and live_holdings != "":
+            raise RuntimeError(f"Custom portfolio holdings setting is not available for {brokerage_instance.get_name()}")
+
     else:
-        brokerage_instance = _configure_brokerage(logger)
+        brokerage_instance = _configure_brokerage(logger, kwargs, show_secrets=show_secrets)
         live_node = _configure_live_node(logger, api_client, cloud_project)
         notify_order_events, notify_insights, notify_methods = _configure_notifications(logger)
         auto_restart = _configure_auto_restart(logger)
+        cash_balance_option, holdings_option, last_cash, last_holdings = get_last_portfolio_cash_holdings(api_client, brokerage_instance, cloud_project.projectId, project)
+        if cash_balance_option != LiveInitialStateInput.NotSupported:
+            live_cash_balance = _configure_initial_cash_interactively(logger, cash_balance_option, last_cash)
+        if holdings_option != LiveInitialStateInput.NotSupported:
+            live_holdings = _configure_initial_holdings_interactively(logger, holdings_option, last_holdings)
 
     brokerage_settings = brokerage_instance.get_settings()
     price_data_handler = brokerage_instance.get_price_data_handler()
 
     logger.info(f"Brokerage: {brokerage_instance.get_name()}")
     logger.info(f"Project id: {cloud_project.projectId}")
     logger.info(f"Environment: {brokerage_settings['environment'].title()}")
@@ -269,29 +324,36 @@
     logger.info(f"Server type: {live_node.sku}")
     logger.info(f"Data provider: {price_data_handler.replace('Handler', '')}")
     logger.info(f"LEAN version: {cloud_project.leanVersionId}")
     logger.info(f"Order event notifications: {'Yes' if notify_order_events else 'No'}")
     logger.info(f"Insight notifications: {'Yes' if notify_insights else 'No'}")
     if notify_order_events or notify_insights:
         _log_notification_methods(notify_methods)
+    if live_cash_balance:
+        logger.info(f"Initial live cash balance: {live_cash_balance}")
+    if live_holdings:
+        logger.info(f"Initial live portfolio holdings: {live_holdings}")
     logger.info(f"Automatic algorithm restarting: {'Yes' if auto_restart else 'No'}")
 
     if brokerage is None:
-        click.confirm(f"Are you sure you want to start live trading for project '{cloud_project.name}'?",
+        confirm(f"Are you sure you want to start live trading for project '{cloud_project.name}'?",
                       default=False,
                       abort=True)
 
     live_algorithm = api_client.live.start(cloud_project.projectId,
                                            finished_compile.compileId,
                                            live_node.id,
                                            brokerage_settings,
                                            price_data_handler,
                                            auto_restart,
                                            cloud_project.leanVersionId,
                                            notify_order_events,
                                            notify_insights,
-                                           notify_methods)
+                                           notify_methods,
+                                           live_cash_balance,
+                                           live_holdings)
 
     logger.info(f"Live url: {live_algorithm.get_url()}")
 
     if open_browser:
-        webbrowser.open(live_algorithm.get_url())
+        from webbrowser import open
+        open(live_algorithm.get_url())
```

### Comparing `lean-1.0.99/lean/commands/cloud/live/live.py` & `lean-1.155/lean/commands/cloud/live/live.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import click
+from click import group
 from lean.components.util.click_group_default_command import DefaultCommandGroup
 
-@click.group(cls=DefaultCommandGroup)
+@group(cls=DefaultCommandGroup)
 def live() -> None:
     """Interact with the QuantConnect cloud live deployments."""
     # This method is intentionally empty
     # It is used as the command group for all `lean cloud <command>` commands
     pass
```

### Comparing `lean-1.0.99/lean/commands/cloud/live/__init__.py` & `lean-1.155/lean/commands/cloud/live/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/commands/cloud/live/stop.py` & `lean-1.155/lean/commands/cloud/push.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,33 +7,41 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from pathlib import Path
+from typing import Optional
 
+from click import command, option
 
-import click
-from lean.click import LeanCommand
+from lean.click import LeanCommand, PathParameter
+from lean.constants import PROJECT_CONFIG_FILE_NAME
 from lean.container import container
 
 
-@click.command(cls=LeanCommand)
-@click.argument("project", type=str)
-def stop(project: str) -> None:
-    """
-    Stops live trading for a certain project without liquidating existing positions.
-    """
-    logger = container.logger()
-    api_client = container.api_client()
+@command(cls=LeanCommand)
+@option("--project",
+        type=PathParameter(exists=True, file_okay=False, dir_okay=True),
+        help="Path to the local project to push (all local projects if not specified)")
+def push(project: Optional[Path]) -> None:
+    """Push local projects to QuantConnect.
 
-    cloud_project_manager = container.cloud_project_manager()
-    cloud_project = cloud_project_manager.get_cloud_project(project, False)
-    logger.info(f"cloud.live.stop(): sending command.")
-    response = api_client.live.stop(cloud_project.projectId)
-    if response.success:
-        logger.info(f"cloud.live.stop(): command executed successfully.")
-    else:
-        raise Exception("cloud.live.stop(): Failed: to execute the command successfully.")
+    This command overrides the content of cloud files with the content of their respective local counterparts.
 
+    This command will delete cloud files which don't have a local counterpart.
+    """
+    push_manager = container.push_manager
+
+    # Parse which projects need to be pushed
+    if project is not None:
+        project_config_manager = container.project_config_manager
+        project_config = project_config_manager.get_project_config(project)
+        if not project_config.file.exists():
+            raise RuntimeError(f"'{project}' is not a Lean project")
 
+        push_manager.push_project(project)
+    else:
+        projects_to_push = [p.parent for p in Path.cwd().rglob(PROJECT_CONFIG_FILE_NAME)]
+        push_manager.push_projects(projects_to_push)
```

### Comparing `lean-1.0.99/lean/commands/cloud/optimize.py` & `lean-1.155/lean/commands/cloud/optimize.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import functools
-import operator
-from datetime import timedelta
-from math import ceil
 from typing import List, Optional, Tuple
 
-import click
+from click import command, option, Choice, argument, confirm
 
 from lean.click import LeanCommand, ensure_options
 from lean.components.config.optimizer_config_manager import NodeType, available_nodes
 from lean.container import container
 from lean.models.api import QCOptimizationBacktest, QCProject, QCCompileWithLogs, QCFullOrganization
 from lean.models.optimizer import OptimizationConstraint, OptimizationExtremum, OptimizationParameter, \
     OptimizationTarget
@@ -29,24 +25,27 @@
 
 def _calculate_backtest_count(parameters: List[OptimizationParameter]) -> int:
     """Calculates the number of backtests needed for the given optimization parameters.
 
     :param parameters: the parameters to optimize
     :return: the number of backtests a grid search on the parameters would require
     """
+    from operator import mul
+    from functools import reduce
     steps_per_parameter = [round((p.max - p.min) / p.step) + 1 for p in parameters]
-    return int(functools.reduce(operator.mul, steps_per_parameter, 1))
+    return int(reduce(mul, steps_per_parameter, 1))
 
 
 def _calculate_hours(backtest_time: int, backtest_count: int) -> float:
     """Calculates the total number of hours the optimization will take, given only one node is used.
 
     :param backtest_time: the number of seconds one backtest is expected to take
     :param backtest_count: the number of backtests that need to be ran
     """
+    from math import ceil
     deploy_time = 30
     backtest_cpu_factor = 1.5
     seconds = (deploy_time + backtest_time * backtest_cpu_factor) * backtest_count
     hours = ceil((seconds * 100) / 3600) / 100
     return max(0.1, hours)
 
 
@@ -55,14 +54,16 @@
 
     If the number of hours is less than 1 this returns "x minutes".
     If the number of hours is greater than or equal to 1 this returns "x hours".
 
     :param hours: the number of hours
     :return: the formatted number of hours
     """
+    from datetime import timedelta
+
     seconds = timedelta(hours=hours).total_seconds()
 
     if seconds < 60 * 60:
         amount = round(seconds / 60)
         unit = "minute"
     else:
         amount = round(seconds / (60 * 60))
@@ -94,15 +95,15 @@
 def _backtest_meets_constraints(backtest: QCOptimizationBacktest, constraints: List[OptimizationConstraint]) -> bool:
     """Returns whether the backtest meets all constraints.
 
     :param backtest: the backtest to check
     :param constraints: the constraints the backtest has to meet
     :return: True if the backtest meets all constraints, False if not
     """
-    optimizer_config_manager = container.optimizer_config_manager()
+    optimizer_config_manager = container.optimizer_config_manager
 
     for constraint in constraints:
         expression = str(constraint)
 
         for target, _ in optimizer_config_manager.available_targets:
             expression = expression.replace(target, str(_get_backtest_statistic(backtest, target)))
 
@@ -119,15 +120,16 @@
                       strategy: str,
                       target: OptimizationTarget,
                       parameters: List[OptimizationParameter],
                       constraints: List[OptimizationConstraint],
                       node: NodeType,
                       parallel_nodes: int) -> None:
     """Displays the estimated optimization time and cost."""
-    api_client = container.api_client()
+    from math import ceil
+    api_client = container.api_client
     estimate = api_client.optimizations.estimate(cloud_project.projectId,
                                                  finished_compile.compileId,
                                                  name,
                                                  strategy,
                                                  target,
                                                  parameters,
                                                  constraints,
@@ -136,46 +138,46 @@
 
     backtest_count = _calculate_backtest_count(parameters)
 
     hours = _calculate_hours(estimate.time, backtest_count)
     batch_time = ceil((hours * 100) / parallel_nodes) / 100
     batch_cost = max(0.01, ceil(node.price * hours * 100) / 100)
 
-    logger = container.logger()
+    logger = container.logger
     logger.info(f"Estimated number of backtests: {backtest_count:,}")
     logger.info(f"Estimated batch time: {_format_hours(batch_time)}")
     logger.info(f"Estimated batch cost: ${batch_cost:,.2f}")
     logger.info(
         f"Organization balance: {organization.credit.balance:,.0f} QCC (${organization.credit.balance / 100:,.2f})")
 
 
-@click.command(cls=LeanCommand)
-@click.argument("project", type=str)
-@click.option("--target",
+@command(cls=LeanCommand)
+@argument("project", type=str)
+@option("--target",
               type=str,
               help="The target statistic of the optimization")
-@click.option("--target-direction",
-              type=click.Choice(["min", "max"], case_sensitive=False),
+@option("--target-direction",
+              type=Choice(["min", "max"], case_sensitive=False),
               help="Whether the target must be minimized or maximized")
-@click.option("--parameter",
+@option("--parameter",
               type=(str, float, float, float),
               multiple=True,
               help="The 'parameter min max step' pairs configuring the parameters to optimize")
-@click.option("--constraint",
+@option("--constraint",
               type=str,
               multiple=True,
               help="The 'statistic operator value' pairs configuring the constraints of the optimization")
-@click.option("--node",
-              type=click.Choice([node.name for node in available_nodes], case_sensitive=False),
+@option("--node",
+              type=Choice([node.name for node in available_nodes], case_sensitive=False),
               help="The node type to run the optimization on")
-@click.option("--parallel-nodes",
+@option("--parallel-nodes",
               type=int,
               help="The number of nodes that may be run in parallel")
-@click.option("--name", type=str, help="The name of the optimization (a random one is generated if not specified)")
-@click.option("--push",
+@option("--name", type=str, help="The name of the optimization (a random one is generated if not specified)")
+@option("--push",
               is_flag=True,
               default=False,
               help="Push local modifications to the cloud before starting the optimization")
 def optimize(project: str,
              target: Optional[str],
              target_direction: Optional[str],
              parameter: List[Tuple[str, float, float, float]],
@@ -203,27 +205,27 @@
     - --constraint "<statistic> <operator> <value>"
     - --constraint "Sharpe Ratio >= 0.5" --constraint "Drawdown < 0.25"
 
     If the project that has to be optimized has been pulled to the local drive
     with `lean cloud pull` it is possible to use the --push option to push local
     modifications to the cloud before running the optimization.
     """
-    logger = container.logger()
-    api_client = container.api_client()
+    logger = container.logger
+    api_client = container.api_client
 
-    cloud_project_manager = container.cloud_project_manager()
+    cloud_project_manager = container.cloud_project_manager
     cloud_project = cloud_project_manager.get_cloud_project(project, push)
 
     if name is None:
-        name = container.name_generator().generate_name()
+        name = container.name_generator.generate_name()
 
-    cloud_runner = container.cloud_runner()
+    cloud_runner = container.cloud_runner
     finished_compile = cloud_runner.compile_project(cloud_project)
 
-    optimizer_config_manager = container.optimizer_config_manager()
+    optimizer_config_manager = container.optimizer_config_manager
     organization = api_client.organizations.get(cloud_project.organizationId)
 
     if target is not None:
         ensure_options(["target", "target_direction", "parameter", "node", "parallel_nodes"])
 
         optimization_strategy = "QuantConnect.Optimizer.Strategies.GridSearchOptimizationStrategy"
         optimization_target = OptimizationTarget(target=optimizer_config_manager.parse_target(target),
@@ -263,15 +265,15 @@
                               optimization_strategy,
                               optimization_target,
                               optimization_parameters,
                               optimization_constraints,
                               node,
                               parallel_nodes)
 
-            if click.confirm("Do you want to start the optimization on the selected node type?", default=True):
+            if confirm("Do you want to start the optimization on the selected node type?", default=True):
                 break
 
     optimization = cloud_runner.run_optimization(cloud_project,
                                                  finished_compile,
                                                  name,
                                                  optimization_strategy,
                                                  optimization_target,
```

### Comparing `lean-1.0.99/lean/commands/cloud/__init__.py` & `lean-1.155/lean/commands/cloud/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import click
+from click import group
 
 from lean.commands.cloud.backtest import backtest
 from lean.commands.cloud.live.live import live
 from lean.commands.cloud.optimize import optimize
 from lean.commands.cloud.pull import pull
 from lean.commands.cloud.push import push
 from lean.commands.cloud.status import status
 
 
-@click.group()
+@group()
 def cloud() -> None:
     """Interact with the QuantConnect cloud."""
     # This method is intentionally empty
     # It is used as the command group for all `lean cloud <command>` commands
     pass
```

### Comparing `lean-1.0.99/lean/commands/cloud/backtest.py` & `lean-1.155/lean/commands/cloud/backtest.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,52 +7,58 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import webbrowser
 from typing import Optional
-
-import click
-
+from click import command, argument, option
 from lean.click import LeanCommand
 from lean.container import container
 
-
-@click.command(cls=LeanCommand)
-@click.argument("project", type=str)
-@click.option("--name", type=str, help="The name of the backtest (a random one is generated if not specified)")
-@click.option("--push",
+@command(cls=LeanCommand)
+@argument("project", type=str)
+@option("--name", type=str, help="The name of the backtest (a random one is generated if not specified)")
+@option("--push",
               is_flag=True,
               default=False,
               help="Push local modifications to the cloud before running the backtest")
-@click.option("--open", "open_browser",
+@option("--open", "open_browser",
               is_flag=True,
               default=False,
               help="Automatically open the results in the browser when the backtest is finished")
 def backtest(project: str, name: Optional[str], push: bool, open_browser: bool) -> None:
     """Backtest a project in the cloud.
 
     PROJECT must be the name or id of the project to run a backtest for.
 
     If the project that has to be backtested has been pulled to the local drive
     with `lean cloud pull` it is possible to use the --push option to push local
     modifications to the cloud before running the backtest.
     """
-    logger = container.logger()
+    from pathlib import Path
+
+    logger = container.logger
 
-    cloud_project_manager = container.cloud_project_manager()
-    cloud_project = cloud_project_manager.get_cloud_project(project, push)
+    cloud_project_manager = container.cloud_project_manager
+    try:
+        cloud_project = cloud_project_manager.get_cloud_project(project, push)
+    except RuntimeError as e:
+        if cloud_project_manager._project_config_manager.try_get_project_config(Path.cwd() / project):
+            error_message = f'No project with the given name or id "{project}" found in your cloud projects.'
+            error_message += f" Please use `lean cloud backtest --push {project}` to backtest in cloud."
+        else:
+            error_message = f'No project with the given name or id "{project}" found in your cloud or local projects.'
+        raise RuntimeError(error_message)
 
     if name is None:
-        name = container.name_generator().generate_name()
+        name = container.name_generator.generate_name()
 
-    cloud_runner = container.cloud_runner()
+    cloud_runner = container.cloud_runner
     finished_backtest = cloud_runner.run_backtest(cloud_project, name)
 
     if finished_backtest.error is None and finished_backtest.stacktrace is None:
         logger.info(finished_backtest.get_statistics_table())
 
     logger.info(f"Backtest id: {finished_backtest.backtestId}")
     logger.info(f"Backtest name: {finished_backtest.name}")
@@ -67,8 +73,9 @@
 
         # Don't open the results in the browser if the error happened during initialization
         # In the browser the logs won't show these errors, you'll just get empty charts and empty logs
         if error.startswith("During the algorithm initialization, the following exception has occurred:"):
             open_browser = False
 
     if open_browser:
-        webbrowser.open(finished_backtest.get_url())
+        from webbrowser import open
+        open(finished_backtest.get_url())
```

### Comparing `lean-1.0.99/lean/commands/config/set.py` & `lean-1.155/lean/commands/config/set.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,28 +7,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import click
-
+from click import command, argument
 from lean.click import LeanCommand
 from lean.container import container
 
 
-@click.command(cls=LeanCommand)
-@click.argument("key", type=str)
-@click.argument("value", type=str)
+@command(cls=LeanCommand)
+@argument("key", type=str)
+@argument("value", type=str)
 def set(key: str, value: str) -> None:
     """Set a configurable option.
 
     Run `lean config list` to show all available options.
     """
-    cli_config_manager = container.cli_config_manager()
+    cli_config_manager = container.cli_config_manager
 
     option = cli_config_manager.get_option_by_key(key)
     option.set_value(value)
 
-    logger = container.logger()
+    logger = container.logger
     logger.info(f"Successfully updated the value of '{key}' to '{option.get_value()}'")
```

### Comparing `lean-1.0.99/lean/commands/config/__init__.py` & `lean-1.155/lean/commands/config/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import click
+from click import group
 
 from lean.commands.config.get import get
 from lean.commands.config.list import list
 from lean.commands.config.set import set
 from lean.commands.config.unset import unset
 
 
-@click.group()
+@group()
 def config() -> None:
     """Configure Lean CLI options."""
     # This method is intentionally empty
     # It is used as the command group for all `lean config <command>` commands
     pass
```

### Comparing `lean-1.0.99/lean/commands/config/list.py` & `lean-1.155/lean/commands/config/list.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,38 +7,38 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import click
-from rich import box
-from rich.table import Table
+from click import command
 
 from lean.click import LeanCommand
 from lean.container import container
 
 
-@click.command(cls=LeanCommand)
+@command(cls=LeanCommand)
 def list() -> None:
     """List the configurable options and their current values."""
+    from rich import box
+    from rich.table import Table
     table = Table(box=box.SQUARE)
     table.add_column("Key", overflow="fold")
     table.add_column("Value", overflow="fold")
     table.add_column("Location", overflow="fold")
     table.add_column("Description", overflow="fold")
 
-    for option in container.cli_config_manager().all_options:
+    for option in container.cli_config_manager.all_options:
         value = option.get_value(default="<not set>")
 
         # Mask values of sensitive options
         if value != "<not set>" and option.is_sensitive:
             value = "*" * 12 + value[-3:] if len(value) >= 5 else "*" * 15
 
         table.add_row(option.key,
                       value,
                       str(option.location),
                       option.description)
 
-    logger = container.logger()
+    logger = container.logger
     logger.info(table)
```

### Comparing `lean-1.0.99/lean/commands/config/unset.py` & `lean-1.155/lean/commands/config/unset.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import click
+from click import command, argument
 
 from lean.click import LeanCommand
 from lean.container import container
 
 
-@click.command(cls=LeanCommand)
-@click.argument("key", type=str)
+@command(cls=LeanCommand)
+@argument("key", type=str)
 def unset(key: str) -> None:
     """Unset a configurable option.
 
     Run `lean config list` to show all available options.
     """
-    cli_config_manager = container.cli_config_manager()
+    cli_config_manager = container.cli_config_manager
 
     option = cli_config_manager.get_option_by_key(key)
     option.unset()
 
-    logger = container.logger()
+    logger = container.logger
     logger.info(f"Successfully unset '{key}'")
```

### Comparing `lean-1.0.99/lean/commands/config/get.py` & `lean-1.155/lean/commands/config/get.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,38 +7,38 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import click
+from click import command, argument
 
 from lean.click import LeanCommand
 from lean.container import container
 from lean.models.errors import MoreInfoError
 
 
-@click.command(cls=LeanCommand)
-@click.argument("key", type=str)
+@command(cls=LeanCommand)
+@argument("key", type=str)
 def get(key: str) -> None:
     """Get the current value of a configurable option.
 
     Sensitive options like credentials cannot be retrieved this way for security reasons.
     Please open ~/.lean/credentials if you want to see your currently stored credentials.
 
     Run `lean config list` to show all available options.
     """
-    cli_config_manager = container.cli_config_manager()
+    cli_config_manager = container.cli_config_manager
 
     option = cli_config_manager.get_option_by_key(key)
     if option.is_sensitive:
         raise RuntimeError(
             "Sensitive options like credentials cannot be retrieved using `lean config get` for security reasons")
 
     value = option.get_value()
     if value is None:
         raise MoreInfoError(f"The option with key '{key}' doesn't have a value set",
-                            "https://www.lean.io/docs/lean-cli/api-reference/lean-config-set")
+                            "https://www.lean.io/docs/v2/lean-cli/api-reference/lean-config-set")
 
-    logger = container.logger()
+    logger = container.logger
     logger.info(value)
```

### Comparing `lean-1.0.99/lean/commands/optimize.py` & `lean-1.155/lean/commands/report.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,246 +7,253 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
-import re
-from datetime import datetime
 from pathlib import Path
-from typing import Optional, List, Tuple
+from typing import Any, Dict, Optional
 
-import click
-import json5
-from docker.types import Mount
+from click import command, option
 
-from lean.click import LeanCommand, PathParameter, ensure_options
-from lean.constants import DEFAULT_ENGINE_IMAGE
+from lean.click import LeanCommand, PathParameter
+from lean.constants import DEFAULT_ENGINE_IMAGE, PROJECT_CONFIG_FILE_NAME
 from lean.container import container
-from lean.models.api import QCParameter, QCBacktest
 from lean.models.errors import MoreInfoError
-from lean.models.optimizer import OptimizationTarget
+from lean.components.util.live_utils import get_latest_result_json_file
 
 
-@click.command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
-@click.argument("project", type=PathParameter(exists=True, file_okay=True, dir_okay=True))
-@click.option("--output",
-              type=PathParameter(exists=False, file_okay=False, dir_okay=True),
-              help="Directory to store results in (defaults to PROJECT/optimizations/TIMESTAMP)")
-@click.option("--detach", "-d",
+def _find_project_directory(backtest_file: Path) -> Optional[Path]:
+    """Returns the project directory, or None if backtest_file is not stored in a project directory.
+
+    :param backtest_file: the path to the JSON file containing the backtest results
+    :return: the path to the project directory, or None if backtest_file is stored outside a project directory
+    """
+    current_directory = backtest_file.parent
+
+    # Loop until we find the root directory
+    while current_directory != current_directory.parent:
+        if (current_directory / PROJECT_CONFIG_FILE_NAME).is_file():
+            return current_directory
+
+        current_directory = current_directory.parent
+
+    return None
+
+
+@command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
+@option("--backtest-results",
+              type=PathParameter(exists=True, file_okay=True, dir_okay=False),
+              help="Path to the JSON file containing the backtest results")
+@option("--live-results",
+              type=PathParameter(exists=True, file_okay=True, dir_okay=False),
+              help="Path to the JSON file containing the live trading results")
+@option("--report-destination",
+              type=PathParameter(exists=False, file_okay=True, dir_okay=False),
+              default=lambda: Path.cwd() / "report.html",
+              help="Path where the generated report is stored as HTML (defaults to ./report.html)")
+@option("--detach", "-d",
               is_flag=True,
               default=False,
-              help="Run the optimization in a detached Docker container and return immediately")
-@click.option("--optimizer-config",
-              type=PathParameter(exists=True, file_okay=True, dir_okay=False),
-              help=f"The optimizer configuration file that should be used")
-@click.option("--strategy",
-              type=click.Choice(["Grid Search", "Euler Search"], case_sensitive=False),
-              help="The optimization strategy to use")
-@click.option("--target",
+              help="Run the report creator in a detached Docker container and return immediately")
+@option("--strategy-name",
+              type=str,
+              help="Name of the strategy, will appear at the top-right corner of each page")
+@option("--strategy-version",
               type=str,
-              help="The target statistic of the optimization")
-@click.option("--target-direction",
-              type=click.Choice(["min", "max"], case_sensitive=False),
-              help="Whether the target must be minimized or maximized")
-@click.option("--parameter",
-              type=(str, float, float, float),
-              multiple=True,
-              help="The 'parameter min max step' pairs configuring the parameters to optimize")
-@click.option("--constraint",
+              help="Version number of the strategy, will appear next to the project name")
+@option("--strategy-description",
               type=str,
-              multiple=True,
-              help="The 'statistic operator value' pairs configuring the constraints of the optimization")
-@click.option("--release",
+              help="Description of the strategy, will appear under the 'Strategy Description' section")
+@option("--overwrite",
               is_flag=True,
               default=False,
-              help="Compile C# projects in release configuration instead of debug")
-@click.option("--image",
+              help="Overwrite --report-destination if it already contains a file")
+@option("--image",
               type=str,
               help=f"The LEAN engine image to use (defaults to {DEFAULT_ENGINE_IMAGE})")
-@click.option("--update",
+@option("--update",
               is_flag=True,
               default=False,
-              help="Pull the LEAN engine image before running the optimizer")
-def optimize(project: Path,
-             output: Optional[Path],
-             detach: bool,
-             optimizer_config: Optional[Path],
-             strategy: Optional[str],
-             target: Optional[str],
-             target_direction: Optional[str],
-             parameter: List[Tuple[str, float, float, float]],
-             constraint: List[str],
-             release: bool,
-             image: Optional[str],
-             update: bool) -> None:
-    """Optimize a project's parameters locally using Docker.
-
-    \b
-    If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
-    If PROJECT is a file, the algorithm in the specified file will be executed.
-
-    By default an interactive wizard is shown letting you configure the optimizer.
-    If --optimizer-config or --strategy is given the command runs in non-interactive mode.
-    In this mode the CLI does not prompt for input.
-
-    \b
-    The --optimizer-config option can be used to specify the configuration to run the optimizer with.
-    When using the option it should point to a file like this (the algorithm-* properties should be omitted):
-    https://github.com/QuantConnect/Lean/blob/master/Optimizer.Launcher/config.json
-
-    If --strategy is given the optimizer configuration is read from the given options.
-    In this case --strategy, --target, --target-direction and --parameter become required.
-
-    \b
-    In non-interactive mode the --parameter option can be provided multiple times to configure multiple parameters:
-    - --parameter <name> <min value> <max value> <step size>
-    - --parameter my-first-parameter 1 10 0.5 --parameter my-second-parameter 20 30 5
-
-    \b
-    In non-interactive mode the --constraint option can be provided multiple times to configure multiple constraints:
-    - --constraint "<statistic> <operator> <value>"
-    - --constraint "Sharpe Ratio >= 0.5" --constraint "Drawdown < 0.25"
+              help="Pull the LEAN engine image before running the report creator")
+@option("--pdf",
+              is_flag=True,
+              default=False,
+              help="Create a PDF version along with the HTML version of the report")
+def report(backtest_results: Optional[Path],
+           live_results: Optional[Path],
+           report_destination: Path,
+           detach: bool,
+           strategy_name: Optional[str],
+           strategy_version: Optional[str],
+           strategy_description: Optional[str],
+           overwrite: bool,
+           image: Optional[str],
+           update: bool,
+           pdf: bool) -> None:
+    """Generate a report of a backtest.
+
+    This runs the LEAN Report Creator in Docker to generate a polished, professional-grade report of a backtest.
+
+    If --backtest-results is not given, a report is generated for the most recent local backtest.
+
+    The name, description, and version are optional and will be blank if not given.
+
+    If the given backtest data source file is stored in a project directory (or one of its subdirectories, like the
+    default <project>/backtests/<timestamp>), the default name is the name of the project directory and the default
+    description is the description stored in the project's config.json file.
 
     By default the official LEAN engine image is used.
     You can override this using the --image option.
     Alternatively you can set the default engine image for all commands using `lean config set engine-image <image>`.
     """
-    project_manager = container.project_manager()
-    algorithm_file = project_manager.find_algorithm_file(project)
+    from json import dump
+    from docker.types import Mount
 
-    if output is None:
-        output = algorithm_file.parent / "optimizations" / datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
+    if report_destination.exists() and not overwrite:
+        raise RuntimeError(f"{report_destination} already exists, use --overwrite to overwrite it")
 
-    optimizer_config_manager = container.optimizer_config_manager()
-    config = None
+    environment = "backtests"
+    output_config_manager = container.output_config_manager
+    output_directory = output_config_manager.get_latest_output_directory(environment)
+
+    if output_directory is None:
+        raise ValueError(f"No output {environment} directories were found. "
+                         f"Make sure you run a backtest or live deployment first.")
+
+    if backtest_results is None:
+        backtest_results = get_latest_result_json_file(output_directory)
+        if not backtest_results:
+            raise MoreInfoError(
+            "Could not find a recent backtest result file, please use the --backtest-results option",
+            "https://www.lean.io/docs/v2/lean-cli/reports#02-Generate-Reports"
+            )
 
-    if optimizer_config is not None and strategy is not None:
-        raise RuntimeError("--optimizer-config and --strategy are mutually exclusive")
-
-    if optimizer_config is not None:
-        config = json5.loads(optimizer_config.read_text(encoding="utf-8"))
-
-        # Remove keys which are configured in the Lean config
-        for key in ["algorithm-type-name", "algorithm-language", "algorithm-location"]:
-            config.pop(key, None)
-    elif strategy is not None:
-        ensure_options(["strategy", "target", "target_direction", "parameter"])
-
-        optimization_strategy = f"QuantConnect.Optimizer.Strategies.{strategy.replace(' ', '')}OptimizationStrategy"
-        optimization_target = OptimizationTarget(target=optimizer_config_manager.parse_target(target),
-                                                 extremum=target_direction)
-        optimization_parameters = optimizer_config_manager.parse_parameters(parameter)
-        optimization_constraints = optimizer_config_manager.parse_constraints(constraint)
-    else:
-        project_config_manager = container.project_config_manager()
-        project_config = project_config_manager.get_project_config(algorithm_file.parent)
-        project_parameters = [QCParameter(key=k, value=v) for k, v in project_config.get("parameters", {}).items()]
-
-        if len(project_parameters) == 0:
-            raise MoreInfoError("The given project has no parameters to optimize",
-                                "https://www.lean.io/docs/lean-cli/optimization/parameters")
-
-        optimization_strategy = optimizer_config_manager.configure_strategy(cloud=False)
-        optimization_target = optimizer_config_manager.configure_target()
-        optimization_parameters = optimizer_config_manager.configure_parameters(project_parameters, cloud=False)
-        optimization_constraints = optimizer_config_manager.configure_constraints()
-
-    if config is None:
-        # noinspection PyUnboundLocalVariable
-        config = {
-            "optimization-strategy": optimization_strategy,
-            "optimization-strategy-settings": {
-                "$type": "QuantConnect.Optimizer.Strategies.StepBaseOptimizationStrategySettings, QuantConnect.Optimizer",
-                "default-segment-amount": 10
-            },
-            "optimization-criterion": {
-                "target": optimization_target.target,
-                "extremum": optimization_target.extremum.value
-            },
-            "parameters": [parameter.dict() for parameter in optimization_parameters],
-            "constraints": [constraint.dict(by_alias=True) for constraint in optimization_constraints]
-        }
-
-    config["optimizer-close-automatically"] = True
-    config["results-destination-folder"] = "/Results"
+    logger = container.logger
 
-    config_path = output / "optimizer-config.json"
-    config_path.parent.mkdir(parents=True, exist_ok=True)
-    with config_path.open("w+", encoding="utf-8") as file:
-        file.write(json.dumps(config, indent=4) + "\n")
+    if live_results is None:
+        logger.info(f"Generating a report from '{backtest_results}'")
+    else:
+        logger.info(f"Generating a report from '{backtest_results}' and '{live_results}'")
 
-    project_config_manager = container.project_config_manager()
-    cli_config_manager = container.cli_config_manager()
+    project_directory = _find_project_directory(backtest_results)
 
-    project_config = project_config_manager.get_project_config(algorithm_file.parent)
-    engine_image = cli_config_manager.get_engine_image(image or project_config.get("engine-image", None))
+    if project_directory is not None:
+        if strategy_name is None:
+            strategy_name = project_directory.name
+
+        if strategy_description is None:
+            project_config_manager = container.project_config_manager
+            project_config = project_config_manager.get_project_config(project_directory)
+            strategy_description = project_config.get("description", "")
+
+    # The configuration given to the report creator
+    # See https://github.com/QuantConnect/Lean/blob/master/Report/config.example.json
+    report_config = {
+        "data-folder": "/Lean/Data",
+        "strategy-name": strategy_name or "",
+        "strategy-version": strategy_version or "",
+        "strategy-description": strategy_description or "",
+        "live-data-source-file": "live-data-source-file.json" if live_results is not None else "",
+        "backtest-data-source-file": "backtest-data-source-file.json",
+        "report-destination": "/tmp/report.html",
+        "report-format": "pdf" if pdf else "",
+        "environment": "report",
+
+        "log-handler": "QuantConnect.Logging.CompositeLogHandler",
+        "messaging-handler": "QuantConnect.Messaging.Messaging",
+        "job-queue-handler": "QuantConnect.Queues.JobQueue",
+        "api-handler": "QuantConnect.Api.Api",
+        "map-file-provider": "QuantConnect.Data.Auxiliary.LocalDiskMapFileProvider",
+        "factor-file-provider": "QuantConnect.Data.Auxiliary.LocalDiskFactorFileProvider",
+        "data-provider": "QuantConnect.Lean.Engine.DataFeeds.DefaultDataProvider",
+        "alpha-handler": "QuantConnect.Lean.Engine.Alphas.DefaultAlphaHandler",
+        "data-channel-provider": "DataChannelProvider",
+
+        "environments": {
+            "report": {
+                "live-mode": False,
+
+                "setup-handler": "QuantConnect.Lean.Engine.Setup.ConsoleSetupHandler",
+                "result-handler": "QuantConnect.Lean.Engine.Results.BacktestingResultHandler",
+                "data-feed-handler": "QuantConnect.Lean.Engine.DataFeeds.FileSystemDataFeed",
+                "real-time-handler": "QuantConnect.Lean.Engine.RealTime.BacktestingRealTimeHandler",
+                "history-provider": "QuantConnect.Lean.Engine.HistoricalData.SubscriptionDataReaderHistoryProvider",
+                "transaction-handler": "QuantConnect.Lean.Engine.TransactionHandlers.BacktestingTransactionHandler"
+            }
+        }
+    }
 
-    lean_config_manager = container.lean_config_manager()
-    lean_config = lean_config_manager.get_complete_lean_config("backtesting", algorithm_file, None)
+    config_path = container.temp_manager.create_temporary_directory() / "config.json"
+    with config_path.open("w+", encoding="utf-8") as file:
+        dump(report_config, file)
 
-    if not output.exists():
-        output.mkdir(parents=True)
+    backtest_id = container.output_config_manager.get_backtest_id(output_directory)
 
-    output_config_manager = container.output_config_manager()
-    lean_config["algorithm-id"] = str(output_config_manager.get_optimization_id(output))
-    lean_config["messaging-handler"] = "QuantConnect.Messaging.Messaging"
+    lean_config_manager = container.lean_config_manager
+    data_dir = lean_config_manager.get_data_directory()
 
-    lean_runner = container.lean_runner()
-    run_options = lean_runner.get_basic_docker_config(lean_config, algorithm_file, output, None, release, detach)
+    report_destination.parent.mkdir(parents=True, exist_ok=True)
 
-    run_options["working_dir"] = "/Lean/Optimizer.Launcher/bin/Debug"
-    run_options["commands"].append("dotnet QuantConnect.Optimizer.Launcher.dll")
-    run_options["mounts"].append(
-        Mount(target="/Lean/Optimizer.Launcher/bin/Debug/config.json",
-              source=str(config_path),
-              type="bind",
-              read_only=True)
-    )
+    run_options: Dict[str, Any] = {
+        "detach": detach,
+        "name": f"lean_cli_report_{backtest_id}",
+        "working_dir": "/Lean/Report/bin/Debug",
+        "commands": ["dotnet QuantConnect.Report.dll", f'cp /tmp/report.html "/Output/{report_destination.name}"'],
+        "mounts": [
+            Mount(target="/Lean/Report/bin/Debug/config.json",
+                  source=str(config_path),
+                  type="bind",
+                  read_only=True),
+            Mount(target="/Lean/Report/bin/Debug/backtest-data-source-file.json",
+                  source=str(backtest_results),
+                  type="bind",
+                  read_only=True)
+        ],
+        "volumes": {
+            str(data_dir): {
+                "bind": "/Lean/Data",
+                "mode": "rw"
+            },
+            str(report_destination.parent): {
+                "bind": "/Output",
+                "mode": "rw"
+            }
+        }
+    }
 
-    container.update_manager().pull_docker_image_if_necessary(engine_image, update)
+    if pdf:
+        run_options["commands"].append(f'cp /tmp/report.pdf "/Output/{report_destination.name.replace(".html", ".pdf")}"')
+    if live_results is not None:
+        run_options["mounts"].append(Mount(target="/Lean/Report/bin/Debug/live-data-source-file.json",
+                                           source=str(live_results),
+                                           type="bind",
+                                           read_only=True))
+
+    cli_config_manager = container.cli_config_manager
+    engine_image_override = image
+
+    if engine_image_override is None and project_directory is not None:
+        project_config_manager = container.project_config_manager
+        project_config = project_config_manager.get_project_config(project_directory)
+        engine_image_override = project_config.get("engine-image", None)
 
-    project_manager.copy_code(algorithm_file.parent, output / "code")
+    engine_image = cli_config_manager.get_engine_image(engine_image_override)
 
-    success = container.docker_manager().run_image(engine_image, **run_options)
+    container.update_manager.pull_docker_image_if_necessary(engine_image, update)
 
-    logger = container.logger()
-    cli_root_dir = container.lean_config_manager().get_cli_root_directory()
-    relative_project_dir = project.relative_to(cli_root_dir)
-    relative_output_dir = output.relative_to(cli_root_dir)
+    success = container.docker_manager.run_image(engine_image, **run_options)
+    if not success:
+        raise RuntimeError(
+            "Something went wrong while running the LEAN Report Creator, see the logs above for more information")
 
     if detach:
-        temp_manager = container.temp_manager()
+        temp_manager = container.temp_manager
         temp_manager.delete_temporary_directories_when_done = False
 
-        logger.info(
-            f"Successfully started optimization for '{relative_project_dir}' in the '{run_options['name']}' container")
-        logger.info(f"The output will be stored in '{relative_output_dir}'")
+        logger.info(f"Successfully started the report creator in the '{run_options['name']}' container")
+        logger.info(f"The report will be generated to '{report_destination}'")
         logger.info("You can use Docker's own commands to manage the detached container")
-    elif success:
-        optimizer_logs = (output / "log.txt").read_text(encoding="utf-8")
-        groups = re.findall(r"ParameterSet: \(([^)]+)\) backtestId '([^']+)'", optimizer_logs)
-
-        if len(groups) > 0:
-            optimal_parameters, optimal_id = groups[0]
-
-            optimal_results = json.loads((output / optimal_id / f"{optimal_id}.json").read_text(encoding="utf-8"))
-            optimal_backtest = QCBacktest(backtestId=optimal_id,
-                                          projectId=1,
-                                          status="",
-                                          name=optimal_id,
-                                          created=datetime.now(),
-                                          completed=True,
-                                          progress=1.0,
-                                          runtimeStatistics=optimal_results["RuntimeStatistics"],
-                                          statistics=optimal_results["Statistics"])
-
-            logger.info(f"Optimal parameters: {optimal_parameters.replace(':', ': ').replace(',', ', ')}")
-            logger.info(f"Optimal backtest results:")
-            logger.info(optimal_backtest.get_statistics_table())
+        return
 
-        logger.info(f"Successfully optimized '{relative_project_dir}' and stored the output in '{relative_output_dir}'")
-    else:
-        raise RuntimeError(
-            f"Something went wrong while running the optimization, the output is stored in '{relative_output_dir}'")
+    logger.info(f"Successfully generated report to '{report_destination}'")
```

### Comparing `lean-1.0.99/lean/commands/logs.py` & `lean-1.155/lean/commands/logs.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,42 +10,42 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from pathlib import Path
 from typing import Optional, List
 
-import click
+from click import option, command
 
 from lean.click import LeanCommand, PathParameter
 from lean.constants import PROJECT_CONFIG_FILE_NAME
 from lean.container import container
 
 
 def _get_project_directories() -> List[Path]:
-    directories_to_check = [container.lean_config_manager().get_cli_root_directory()]
+    directories_to_check = [container.lean_config_manager.get_cli_root_directory()]
     project_directories = []
 
     while len(directories_to_check) > 0:
         directory = directories_to_check.pop(0)
 
         config_file = directory / PROJECT_CONFIG_FILE_NAME
         if config_file.is_file():
             project_directories.append(directory)
         else:
             directories_to_check.extend(d for d in directory.iterdir() if d.is_dir())
 
     return project_directories
 
 
-@click.command(cls=LeanCommand, requires_lean_config=True)
-@click.option("--backtest", is_flag=True, default=False, help="Display the most recent backtest logs (default)")
-@click.option("--live", is_flag=True, default=False, help="Display the most recent live logs")
-@click.option("--optimization", is_flag=True, default=False, help="Display the most recent optimization logs")
-@click.option("--project",
+@command(cls=LeanCommand, requires_lean_config=True)
+@option("--backtest", is_flag=True, default=False, help="Display the most recent backtest logs (default)")
+@option("--live", is_flag=True, default=False, help="Display the most recent live logs")
+@option("--optimization", is_flag=True, default=False, help="Display the most recent optimization logs")
+@option("--project",
               type=PathParameter(exists=True, file_okay=False, dir_okay=True),
               help="The project to get the most recent logs from")
 def logs(backtest: bool, live: bool, optimization: bool, project: Optional[Path]) -> None:
     """Display the most recent backtest/live/optimization logs."""
     if [backtest, live, optimization].count(True) > 1:
         raise RuntimeError("--backtest, --live and --optimization are mutually exclusive")
```

### Comparing `lean-1.0.99/lean/commands/research.py` & `lean-1.155/lean/commands/research.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,107 +7,130 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import webbrowser
 from pathlib import Path
-from typing import Optional
-import click
-from docker.errors import APIError
-from docker.types import Mount
+from typing import Optional, Tuple
+from click import command, argument, option, Choice
 from lean.click import LeanCommand, PathParameter
-from lean.constants import DEFAULT_RESEARCH_IMAGE
+from lean.constants import DEFAULT_RESEARCH_IMAGE, LEAN_ROOT_PATH
 from lean.container import container
 from lean.models.data_providers import QuantConnectDataProvider, all_data_providers
 from lean.components.util.name_extraction import convert_to_class_name
+from lean.components.util.json_modules_handler import get_and_build_module
+from lean.models.click_options import options_from_json, get_configs_for_options
 
 def _check_docker_output(chunk: str, port: int) -> None:
     """Checks the output of the Docker container and opens the browser if Jupyter Lab has started.
 
     :param chunk: the output chunk
     :param port: the port Jupyter Lab will be running on
     """
+    from webbrowser import open
     if "is running at:" in chunk:
-        webbrowser.open(f"http://localhost:{port}/")
+        open(f"http://localhost:{port}/")
 
 
-@click.command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
-@click.argument("project", type=PathParameter(exists=True, file_okay=False, dir_okay=True))
-@click.option("--port", type=int, default=8888, help="The port to run Jupyter Lab on (defaults to 8888)")
-@click.option("--data-provider",
-              type=click.Choice([dp.get_name() for dp in all_data_providers], case_sensitive=False),
+@command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
+@argument("project", type=PathParameter(exists=True, file_okay=False, dir_okay=True))
+@option("--port", type=int, default=8888, help="The port to run Jupyter Lab on (defaults to 8888)")
+@option("--data-provider",
+              type=Choice([dp.get_name() for dp in all_data_providers], case_sensitive=False),
+              default="Local",
               help="Update the Lean configuration file to retrieve data from the given provider")
-@click.option("--download-data",
+@options_from_json(get_configs_for_options("research"))
+@option("--download-data",
               is_flag=True,
               default=False,
               help=f"Update the Lean configuration file to download data from the QuantConnect API, alias for --data-provider {QuantConnectDataProvider.get_name()}")
-@click.option("--data-purchase-limit",
+@option("--data-purchase-limit",
               type=int,
               help="The maximum amount of QCC to spend on downloading data during the research session when using QuantConnect as data provider")
-@click.option("--detach", "-d",
+@option("--detach", "-d",
               is_flag=True,
               default=False,
               help="Run Jupyter Lab in a detached Docker container and return immediately")
-@click.option("--no-open",
+@option("--no-open",
               is_flag=True,
               default=False,
               help="Don't open the Jupyter Lab environment in the browser after starting it")
-@click.option("--image", type=str, help=f"The LEAN research image to use (defaults to {DEFAULT_RESEARCH_IMAGE})")
-@click.option("--update",
+@option("--image", type=str, help=f"The LEAN research image to use (defaults to {DEFAULT_RESEARCH_IMAGE})")
+@option("--update",
               is_flag=True,
               default=False,
               help="Pull the LEAN research image before starting the research environment")
+@option("--extra-config",
+              type=(str, str),
+              multiple=True,
+              hidden=True)
+@option("--no-update",
+              is_flag=True,
+              default=False,
+              help="Use the local LEAN research image instead of pulling the latest version")
 def research(project: Path,
              port: int,
              data_provider: Optional[str],
              download_data: bool,
              data_purchase_limit: Optional[int],
              detach: bool,
              no_open: bool,
              image: Optional[str],
-             update: bool) -> None:
+             update: bool,
+             extra_config: Optional[Tuple[str, str]],
+             no_update: bool,
+             **kwargs) -> None:
     """Run a Jupyter Lab environment locally using Docker.
 
     By default the official LEAN research image is used.
     You can override this using the --image option.
     Alternatively you can set the default research image using `lean config set research-image <image>`.
     """
-    project_manager = container.project_manager()
+    from docker.types import Mount
+    from docker.errors import APIError
+
+    logger = container.logger
+
+    project_manager = container.project_manager
     algorithm_file = project_manager.find_algorithm_file(project)
     algorithm_name = convert_to_class_name(project)
 
-    lean_config_manager = container.lean_config_manager()
+    lean_config_manager = container.lean_config_manager
     lean_config = lean_config_manager.get_complete_lean_config("backtesting", algorithm_file, None)
-    lean_config["composer-dll-directory"] = "/Lean/Launcher/bin/Debug"
+    lean_config["composer-dll-directory"] = LEAN_ROOT_PATH
     lean_config["research-object-store-name"] = algorithm_name
 
     if download_data:
         data_provider = QuantConnectDataProvider.get_name()
 
     if data_provider is not None:
-        data_provider = next(dp for dp in all_data_providers if dp.get_name() == data_provider)
-        data_provider.build(lean_config, container.logger()).configure(lean_config, "backtesting")
+        [data_provider_configurer] = [get_and_build_module(data_provider, all_data_providers, kwargs, logger)]
+        data_provider_configurer.configure(lean_config, "backtesting")
 
     lean_config_manager.configure_data_purchase_limit(lean_config, data_purchase_limit)
 
-    lean_runner = container.lean_runner()
-    temp_manager = container.temp_manager()
+    lean_runner = container.lean_runner
+    temp_manager = container.temp_manager
+
+    # Set extra config
+    for key, value in extra_config:
+        lean_config[key] = value
+        
     run_options = lean_runner.get_basic_docker_config(lean_config,
                                                       algorithm_file,
                                                       temp_manager.create_temporary_directory(),
                                                       None,
                                                       False,
                                                       detach)
 
     # Mount the config in the notebooks directory as well
     local_config_path = next(m["Source"] for m in run_options["mounts"] if m["Target"].endswith("config.json"))
-    run_options["mounts"].append(Mount(target="/Lean/Launcher/bin/Debug/Notebooks/config.json",
+    run_options["mounts"].append(Mount(target=f"{LEAN_ROOT_PATH}/Notebooks/config.json",
                                        source=str(local_config_path),
                                        type="bind",
                                        read_only=True))
 
     # Jupyter Lab runs on port 8888, we expose it to the local port specified by the user
     run_options["ports"]["8888"] = str(port)
 
@@ -116,59 +139,55 @@
         run_options["on_output"] = lambda chunk: _check_docker_output(chunk, port)
 
     # Make Ctrl+C stop Jupyter Lab immediately
     run_options["stop_signal"] = "SIGKILL"
 
     # Mount the project to the notebooks directory
     run_options["volumes"][str(project)] = {
-        "bind": "/Lean/Launcher/bin/Debug/Notebooks",
+        "bind": f"{LEAN_ROOT_PATH}/Notebooks",
         "mode": "rw"
     }
 
-    # Add references to all DLLs in QuantConnect.csx so custom C# libraries can be imported with using statements
-    run_options["commands"].append(" && ".join([
-        'find . -maxdepth 1 -iname "*.dll" | xargs -I _ echo \'#r "_"\' | cat - QuantConnect.csx > NewQuantConnect.csx',
-        "mv NewQuantConnect.csx QuantConnect.csx"
-    ]))
-
     # Allow notebooks to be embedded in iframes
     run_options["commands"].append("mkdir -p ~/.jupyter")
     run_options["commands"].append(
-        'echo "c.NotebookApp.disable_check_xsrf = True\nc.NotebookApp.tornado_settings = {\'headers\': {\'Content-Security-Policy\': \'frame-ancestors self *\'}}" > ~/.jupyter/jupyter_notebook_config.py')
+        'echo "c.ServerApp.disable_check_xsrf = True\nc.ServerApp.tornado_settings = {\'headers\': {\'Content-Security-Policy\': \'frame-ancestors self *\'}}" > ~/.jupyter/jupyter_server_config.py')
 
     # Hide headers in notebooks
     run_options["commands"].append("mkdir -p ~/.ipython/profile_default/static/custom")
     run_options["commands"].append(
         'echo "#header-container { display: none !important; }" > ~/.ipython/profile_default/static/custom/custom.css')
 
     # Run the script that starts Jupyter Lab when all set up has been done
     run_options["commands"].append("./start.sh")
 
-    project_config_manager = container.project_config_manager()
-    cli_config_manager = container.cli_config_manager()
+    project_config_manager = container.project_config_manager
+    cli_config_manager = container.cli_config_manager
 
     project_config = project_config_manager.get_project_config(algorithm_file.parent)
     research_image = cli_config_manager.get_research_image(image or project_config.get("research-image", None))
 
-    container.update_manager().pull_docker_image_if_necessary(research_image, update)
+    if str(research_image) != DEFAULT_RESEARCH_IMAGE:
+        logger.warn(f'A custom research image: "{research_image}" is being used!')
+
+    container.update_manager.pull_docker_image_if_necessary(research_image, update, no_update)
 
     try:
-        container.docker_manager().run_image(research_image, **run_options)
+        container.docker_manager.run_image(research_image, **run_options)
     except APIError as error:
         msg = error.explanation
         if isinstance(msg, str) and any(m in msg.lower() for m in [
             "port is already allocated",
             "ports are not available"
             "an attempt was made to access a socket in a way forbidden by its access permissions"
         ]):
             raise RuntimeError(f"Port {port} is already in use, please specify a different port using --port <number>")
         raise error
 
     if detach:
         temp_manager.delete_temporary_directories_when_done = False
 
-        logger = container.logger()
         relative_project_dir = algorithm_file.parent.relative_to(lean_config_manager.get_cli_root_directory())
 
         logger.info(
             f"Successfully started Jupyter Lab environment for '{relative_project_dir}' in the '{run_options['name']}' container")
         logger.info("You can use Docker's own commands to manage the detached container")
```

### Comparing `lean-1.0.99/lean/commands/report.py` & `lean-1.155/lean/click.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,241 +7,282 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
 from pathlib import Path
-from typing import Any, Dict, Optional
+from typing import Optional, List, Callable
 
-import click
-from docker.types import Mount
+from click import Command, Context, Parameter, ParamType, Option as ClickOption
+from click.decorators import FC, option
 
-from lean.click import LeanCommand, PathParameter
-from lean.constants import DEFAULT_ENGINE_IMAGE, PROJECT_CONFIG_FILE_NAME
+from lean.constants import DEFAULT_LEAN_CONFIG_FILE_NAME
 from lean.container import container
 from lean.models.errors import MoreInfoError
+from lean.models.logger import Option
 
 
-def _find_project_directory(backtest_file: Path) -> Optional[Path]:
-    """Returns the project directory, or None if backtest_file is not stored in a project directory.
+class VerboseOption(ClickOption):
+    def __init__(self, *args, **kwargs):
+        super().__init__(["--verbose"],
+                         help="Enable debug logging",
+                         is_flag=True,
+                         default=False,
+                         expose_value=False,
+                         is_eager=True,
+                         callback=self._parse_verbose_option)
+
+    @staticmethod
+    def _parse_verbose_option(ctx: Context, param: Parameter, value: Optional[bool]) -> None:
+        """Parses the --verbose option."""
+        if not value:
+            return
+
+        from platform import platform
+        from sys import version as sys_version
+        from lean import __version__ as lean_cli_version
+
+        logger = container.logger
+        logger.debug_logging_enabled = True
+
+        # show additional context information
+        python_version = sys_version.replace("\n", ". ")
+        logger.debug(f"Context information:\n"
+                     f"  Python version: {python_version}\n"
+                     f"  OS: {platform()}\n"
+                     f"  Lean CLI version: {lean_cli_version}")
+
+
+def verbose_option() -> Callable[[FC], FC]:
+    return option(cls=VerboseOption)
+
+
+class LeanCommand(Command):
+    """A click.Command wrapper with some Lean CLI customization."""
+
+    def __init__(self,
+                 requires_lean_config: bool = False,
+                 requires_docker: bool = False,
+                 allow_unknown_options: bool = False,
+                 *args,
+                 **kwargs):
+        """Creates a new LeanCommand instance.
+
+        :param requires_lean_config: True if this command requires a Lean config, False if not
+        :param requires_docker: True if this command uses Docker, False if not
+        :param allow_unknown_options: True if unknown options are allowed, False if not
+        :param args: the args that are passed on to the click.Command constructor
+        :param kwargs: the kwargs that are passed on to the click.Command constructor
+        """
+        self._requires_lean_config = requires_lean_config
+        self._requires_docker = requires_docker
+        self._allow_unknown_options = allow_unknown_options
+
+        super().__init__(*args, **kwargs)
+
+        # By default the width of help messages is min(terminal_width, max_content_width)
+        # max_content_width defaults to 80, which we increase to 120 to improve readability on wide terminals
+        self.context_settings["max_content_width"] = 120
+
+        # Don't fail if unknown options are passed in when they're allowed
+        self.context_settings["ignore_unknown_options"] = allow_unknown_options
+        self.context_settings["allow_extra_args"] = allow_unknown_options
+
+    def invoke(self, ctx: Context):
+        if self._requires_lean_config:
+            lean_config_manager = container.lean_config_manager
+            try:
+                # This method will raise an error if the directory cannot be found
+                lean_config_manager.get_cli_root_directory()
+            except Exception:
+                # Use one of the cached Lean config locations to avoid having to abort the command
+                lean_config_paths = lean_config_manager.get_known_lean_config_paths()
+                if len(lean_config_paths) > 0:
+                    lean_config_path = container.logger.prompt_list("Select the Lean configuration file to use", [
+                        Option(id=p, label=str(p)) for p in lean_config_paths
+                    ])
+                    lean_config_manager.set_default_lean_config_path(lean_config_path)
+                else:
+                    # Abort with a display-friendly error message if the command requires a Lean config and none found
+                    raise MoreInfoError(
+                        "This command requires a Lean configuration file, run `lean init` in an empty directory to create one, or specify the file to use with --lean-config",
+                        "https://www.lean.io/docs/v2/lean-cli/key-concepts/troubleshooting#02-Common-Errors"
+                    )
+
+        if self._requires_docker and container.platform_manager.is_system_linux():
+            from sys import modules, executable, argv
+            if "pytest" not in modules:
+                from shutil import which
+                from os import getuid, execlp
+                # The CLI uses temporary directories in /tmp because sometimes it may leave behind files owned by root
+                # These files cannot be deleted by the CLI itself, so we rely on the OS to empty /tmp on reboot
+                # The Snap version of Docker does not provide access to files outside $HOME, so we can't support it
+
+                docker_path = which("docker")
+                if docker_path is not None and docker_path.startswith("/snap"):
+                    raise MoreInfoError(
+                        "The Lean CLI does not work with the Snap version of Docker, please re-install Docker via the official installation instructions",
+                        "https://docs.docker.com/engine/install/")
+
+                # A usual Docker installation on Linux requires the user to use sudo to run Docker
+                # If we detect that this is the case and the CLI was started without sudo we elevate automatically
+                if getuid() != 0 and container.docker_manager.is_missing_permission():
+                    container.logger.info(
+                        "This command requires access to Docker, you may be asked to enter your password")
+
+                    args = ["sudo", "--preserve-env=HOME", executable, *argv]
+                    execlp(args[0], *args)
+
+        if self._allow_unknown_options:
+            from itertools import chain
+            # Unknown options are passed to ctx.args and need to be parsed manually
+            # We parse them to ctx.params so they're available like normal options
+            # Because of this all commands with allow_unknown_options=True must have a **kwargs argument
+            arguments = list(chain(*[arg.split("=") for arg in ctx.args]))
+
+            skip_next = False
+            for index in range(len(arguments) - 1):
+                if skip_next:
+                    skip_next = False
+                    continue
+
+                if arguments[index].startswith("--"):
+                    option = arguments[index].replace("--", "")
+                    value = arguments[index + 1]
+                    ctx.params[option] = value
+                    skip_next = True
+
+        update_manager = container.update_manager
+        update_manager.show_announcements()
+
+        result = super().invoke(ctx)
+
+        update_manager.warn_if_cli_outdated()
+
+        return result
+
+    def get_params(self, ctx: Context):
+        params = super().get_params(ctx)
+
+        # Add --lean-config option if the command requires a Lean config
+        if self._requires_lean_config:
+            params.insert(len(params) - 1, ClickOption(["--lean-config"],
+                                                        type=PathParameter(exists=True, file_okay=True, dir_okay=False),
+                                                        help=f"The Lean configuration file that should be used (defaults to the nearest {DEFAULT_LEAN_CONFIG_FILE_NAME})",
+                                                        expose_value=False,
+                                                        is_eager=True,
+                                                        callback=self._parse_config_option))
+
+        # Add --verbose option
+        params.insert(len(params) - 1, VerboseOption())
+
+        return params
+
+    def _parse_config_option(self, ctx: Context, param: Parameter, value: Optional[Path]) -> None:
+        """Parses the --config option."""
+        if value is not None:
+            lean_config_manager = container.lean_config_manager
+            lean_config_manager.set_default_lean_config_path(value)
+
+
+
+class PathParameter(ParamType):
+    """A limited version of click.Path which uses pathlib.Path."""
+
+    def __init__(self, exists: bool = False, file_okay: bool = True, dir_okay: bool = True):
+        """Creates a new PathParameter instance.
+
+        :param exists: True if the path needs to point to an existing object, False if not
+        :param file_okay: True if the path may point to a file, False if not
+        :param dir_okay: True if the path may point to a directory, False if not
+        """
+        self._exists = exists
+        self._file_okay = file_okay
+        self._dir_okay = dir_okay
+
+        if file_okay and not dir_okay:
+            self.name = "file"
+            self._path_type = "File"
+        elif dir_okay and not file_okay:
+            self.name = "directory"
+            self._path_type = "Directory"
+        else:
+            self.name = "path"
+            self._path_type = "Path"
+
+    def convert(self, value: str, param: Parameter, ctx: Context) -> Path:
+        path = Path(value).expanduser().resolve()
+
+        if not container.path_manager.is_cli_path_valid(path):
+            self.fail(f"{self._path_type} '{value}' is not a valid path.", param, ctx)
+
+        if self._exists and not path.exists():
+            self.fail(f"{self._path_type} '{value}' does not exist.", param, ctx)
+
+        if not self._file_okay and path.is_file():
+            self.fail(f"{self._path_type} '{value}' is a file.", param, ctx)
+
+        if not self._dir_okay and path.is_dir():
+            self.fail(f"{self._path_type} '{value}' is a directory.", param, ctx)
+
+        return path
+
+
+class DateParameter(ParamType):
+    """A click parameter which returns datetime.datetime objects and requires yyyyMMdd input."""
+
+    name = "date"
+
+    def get_metavar(self, param: Parameter) -> str:
+        return "[yyyyMMdd]"
+
+    def convert(self, value: str, param: Parameter, ctx: Context):
+        from datetime import datetime
+        for date_format in ["%Y%m%d", "%Y-%m-%d"]:
+            try:
+                return datetime.strptime(value, date_format)
+            except ValueError:
+                pass
+
+        self.fail(f"'{value}' does not match the yyyyMMdd format.", param, ctx)
 
-    :param backtest_file: the path to the JSON file containing the backtest results
-    :return: the path to the project directory, or None if backtest_file is stored outside a project directory
-    """
-    current_directory = backtest_file.parent
 
-    # Loop until we find the root directory
-    while current_directory != current_directory.parent:
-        if (current_directory / PROJECT_CONFIG_FILE_NAME).is_file():
-            return current_directory
-
-        current_directory = current_directory.parent
-
-    return None
-
-
-@click.command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
-@click.option("--backtest-results",
-              type=PathParameter(exists=True, file_okay=True, dir_okay=False),
-              help="Path to the JSON file containing the backtest results")
-@click.option("--live-results",
-              type=PathParameter(exists=True, file_okay=True, dir_okay=False),
-              help="Path to the JSON file containing the live trading results")
-@click.option("--report-destination",
-              type=PathParameter(exists=False, file_okay=True, dir_okay=False),
-              default=lambda: Path.cwd() / "report.html",
-              help="Path where the generated report is stored as HTML (defaults to ./report.html)")
-@click.option("--detach", "-d",
-              is_flag=True,
-              default=False,
-              help="Run the report creator in a detached Docker container and return immediately")
-@click.option("--strategy-name",
-              type=str,
-              help="Name of the strategy, will appear at the top-right corner of each page")
-@click.option("--strategy-version",
-              type=str,
-              help="Version number of the strategy, will appear next to the project name")
-@click.option("--strategy-description",
-              type=str,
-              help="Description of the strategy, will appear under the 'Strategy Description' section")
-@click.option("--overwrite",
-              is_flag=True,
-              default=False,
-              help="Overwrite --report-destination if it already contains a file")
-@click.option("--image",
-              type=str,
-              help=f"The LEAN engine image to use (defaults to {DEFAULT_ENGINE_IMAGE})")
-@click.option("--update",
-              is_flag=True,
-              default=False,
-              help="Pull the LEAN engine image before running the report creator")
-def report(backtest_results: Optional[Path],
-           live_results: Optional[Path],
-           report_destination: Path,
-           detach: bool,
-           strategy_name: Optional[str],
-           strategy_version: Optional[str],
-           strategy_description: Optional[str],
-           overwrite: bool,
-           image: Optional[str],
-           update: bool) -> None:
-    """Generate a report of a backtest.
-
-    This runs the LEAN Report Creator in Docker to generate a polished, professional-grade report of a backtest.
-
-    If --backtest-results is not given, a report is generated for the most recent local backtest.
-
-    The name, description, and version are optional and will be blank if not given.
-
-    If the given backtest data source file is stored in a project directory (or one of its subdirectories, like the
-    default <project>/backtests/<timestamp>), the default name is the name of the project directory and the default
-    description is the description stored in the project's config.json file.
-
-    By default the official LEAN engine image is used.
-    You can override this using the --image option.
-    Alternatively you can set the default engine image for all commands using `lean config set engine-image <image>`.
+def ensure_options(options: List[str]) -> None:
+    """Ensures certain options have values, raises an error if not.
+
+    :param options: the Python names of the options that must have values
     """
-    if report_destination.exists() and not overwrite:
-        raise RuntimeError(f"{report_destination} already exists, use --overwrite to overwrite it")
+    from click import get_current_context
+
+    ctx = get_current_context()
 
-    if backtest_results is None:
-        backtest_json_files = list(Path.cwd().rglob("backtests/*/*.json"))
-        result_json_files = [f for f in backtest_json_files if
-                             not f.name.endswith("-order-events.json") and not f.name.endswith("alpha-results.json")]
-
-        if len(result_json_files) == 0:
-            raise MoreInfoError(
-                "Could not find a recent backtest result file, please use the --backtest-results option",
-                "https://www.lean.io/docs/lean-cli/backtesting/report#02-Generate-a-Report"
-            )
-
-        backtest_results = sorted(result_json_files, key=lambda f: f.stat().st_mtime, reverse=True)[0]
-
-    logger = container.logger()
-
-    if live_results is None:
-        logger.info(f"Generating a report from '{backtest_results}'")
-    else:
-        logger.info(f"Generating a report from '{backtest_results}' and '{live_results}'")
-
-    project_directory = _find_project_directory(backtest_results)
-
-    if project_directory is not None:
-        if strategy_name is None:
-            strategy_name = project_directory.name
-
-        if strategy_description is None:
-            project_config_manager = container.project_config_manager()
-            project_config = project_config_manager.get_project_config(project_directory)
-            strategy_description = project_config.get("description", "")
-
-    # The configuration given to the report creator
-    # See https://github.com/QuantConnect/Lean/blob/master/Report/config.example.json
-    report_config = {
-        "data-folder": "/Lean/Data",
-        "strategy-name": strategy_name or "",
-        "strategy-version": strategy_version or "",
-        "strategy-description": strategy_description or "",
-        "live-data-source-file": "live-data-source-file.json" if live_results is not None else "",
-        "backtest-data-source-file": "backtest-data-source-file.json",
-        "report-destination": "/tmp/report.html",
-
-        "environment": "report",
-
-        "log-handler": "QuantConnect.Logging.CompositeLogHandler",
-        "messaging-handler": "QuantConnect.Messaging.Messaging",
-        "job-queue-handler": "QuantConnect.Queues.JobQueue",
-        "api-handler": "QuantConnect.Api.Api",
-        "map-file-provider": "QuantConnect.Data.Auxiliary.LocalDiskMapFileProvider",
-        "factor-file-provider": "QuantConnect.Data.Auxiliary.LocalDiskFactorFileProvider",
-        "data-provider": "QuantConnect.Lean.Engine.DataFeeds.DefaultDataProvider",
-        "alpha-handler": "QuantConnect.Lean.Engine.Alphas.DefaultAlphaHandler",
-        "data-channel-provider": "DataChannelProvider",
-
-        "environments": {
-            "report": {
-                "live-mode": False,
-
-                "setup-handler": "QuantConnect.Lean.Engine.Setup.ConsoleSetupHandler",
-                "result-handler": "QuantConnect.Lean.Engine.Results.BacktestingResultHandler",
-                "data-feed-handler": "QuantConnect.Lean.Engine.DataFeeds.FileSystemDataFeed",
-                "real-time-handler": "QuantConnect.Lean.Engine.RealTime.BacktestingRealTimeHandler",
-                "history-provider": "QuantConnect.Lean.Engine.HistoricalData.SubscriptionDataReaderHistoryProvider",
-                "transaction-handler": "QuantConnect.Lean.Engine.TransactionHandlers.BacktestingTransactionHandler"
-            }
-        }
-    }
-
-    config_path = container.temp_manager().create_temporary_directory() / "config.json"
-    with config_path.open("w+", encoding="utf-8") as file:
-        json.dump(report_config, file)
-
-    backtest_id = container.output_config_manager().get_backtest_id(backtest_results.parent)
-
-    lean_config_manager = container.lean_config_manager()
-    data_dir = lean_config_manager.get_data_directory()
-
-    report_destination.parent.mkdir(parents=True, exist_ok=True)
-
-    run_options: Dict[str, Any] = {
-        "detach": detach,
-        "name": f"lean_cli_report_{backtest_id}",
-        "working_dir": "/Lean/Report/bin/Debug",
-        "commands": ["dotnet QuantConnect.Report.dll", f'cp /tmp/report.html "/Output/{report_destination.name}"'],
-        "mounts": [
-            Mount(target="/Lean/Report/bin/Debug/config.json",
-                  source=str(config_path),
-                  type="bind",
-                  read_only=True),
-            Mount(target="/Lean/Report/bin/Debug/backtest-data-source-file.json",
-                  source=str(backtest_results),
-                  type="bind",
-                  read_only=True)
-        ],
-        "volumes": {
-            str(data_dir): {
-                "bind": "/Lean/Data",
-                "mode": "rw"
-            },
-            str(report_destination.parent): {
-                "bind": "/Output",
-                "mode": "rw"
-            }
-        }
-    }
-
-    if live_results is not None:
-        run_options["mounts"].append(Mount(target="/Lean/Report/bin/Debug/live-data-source-file.json",
-                                           source=str(live_results),
-                                           type="bind",
-                                           read_only=True))
-
-    cli_config_manager = container.cli_config_manager()
-    engine_image_override = image
-
-    if engine_image_override is None and project_directory is not None:
-        project_config_manager = container.project_config_manager()
-        project_config = project_config_manager.get_project_config(project_directory)
-        engine_image_override = project_config.get("engine-image", None)
-
-    engine_image = cli_config_manager.get_engine_image(engine_image_override)
-
-    container.update_manager().pull_docker_image_if_necessary(engine_image, update)
-
-    success = container.docker_manager().run_image(engine_image, **run_options)
-    if not success:
-        raise RuntimeError(
-            "Something went wrong while running the LEAN Report Creator, see the logs above for more information")
-
-    if detach:
-        temp_manager = container.temp_manager()
-        temp_manager.delete_temporary_directories_when_done = False
-
-        logger.info(f"Successfully started the report creator in the '{run_options['name']}' container")
-        logger.info(f"The report will be generated to '{report_destination}'")
-        logger.info("You can use Docker's own commands to manage the detached container")
+    missing_options = []
+    for key, value in ctx.params.items():
+        has_value = value is not None
+
+        if isinstance(value, tuple) and len(value) == 0:
+            has_value = False
+
+        if not has_value and key in options:
+            missing_options.append(key)
+
+    if len(missing_options) == 0:
         return
 
-    logger.info(f"Successfully generated report to '{report_destination}'")
+    missing_options = sorted(missing_options, key=lambda param: options.index(param))
+    help_records = []
+
+    for name in missing_options:
+        option = next(param for param in ctx.command.params if param.name == name)
+        help_records.append(option.get_help_record(ctx))
+
+    from click import HelpFormatter
+
+    help_formatter = HelpFormatter(max_width=120)
+    help_formatter.write_dl(help_records)
+
+    raise RuntimeError(f"""
+You are missing the following option{"s" if len(missing_options) > 1 else ""}:
+{''.join(help_formatter.buffer)}
+    """.strip())
```

### Comparing `lean-1.0.99/lean/commands/build.py` & `lean-1.155/lean/commands/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import re
 from pathlib import Path
 from typing import Optional
 
-import click
+from click import option, command, argument
 
 from lean.click import LeanCommand, PathParameter
 from lean.container import container
 from lean.models.docker import DockerImage
-
+from lean.constants import CUSTOM_FOUNDATION, CUSTOM_RESEARCH, CUSTOM_ENGINE
 
 def _normalize_newlines(text: str) -> str:
     """Normalizes the newlines in a string to use \n (instead of \r or \r\n).
 
     :param text: the text to normalize the newlines in
     :return: the text with the newlines normalized
     """
@@ -37,15 +36,15 @@
     :param dockerfile: the path to the local Dockerfile to check
     :return: whether the local Dockerfile is the same as the one used for the quantconnect/lean:foundation image
     """
     local_dockerfile = dockerfile.read_text(encoding="utf-8").strip()
 
     try:
         cloud_url = f"https://raw.githubusercontent.com/QuantConnect/Lean/master/{dockerfile.name}"
-        cloud_dockerfile = container.http_client().get(cloud_url)
+        cloud_dockerfile = container.http_client.get(cloud_url)
         cloud_dockerfile = cloud_dockerfile.text.strip()
     except:
         # We build a new image if for whatever reason we can't check the Dockerfile used for the official image
         return False
 
     return _normalize_newlines(local_dockerfile) == _normalize_newlines(cloud_dockerfile)
 
@@ -53,20 +52,20 @@
 def _compile_csharp(root: Path, csharp_dir: Path, docker_image: DockerImage) -> None:
     """Compiles C# code.
 
     :param root: the root directory in which the command is ran
     :param csharp_dir: the directory containing the C# code
     :param docker_image: the Docker image to compile in
     """
-    logger = container.logger()
+    logger = container.logger
     logger.info(f"Compiling the C# code in '{csharp_dir}'")
 
     build_path = Path("/LeanCLI") / csharp_dir.relative_to(root)
 
-    docker_manager = container.docker_manager()
+    docker_manager = container.docker_manager
     docker_manager.create_volume("lean_cli_nuget")
     success = docker_manager.run_image(docker_image,
                                        entrypoint=["dotnet", "build", str(build_path)],
                                        environment={
                                            "DOTNET_CLI_TELEMETRY_OPTOUT": "true",
                                            "DOTNET_NOLOGO": "true"
                                        },
@@ -89,94 +88,90 @@
     """Builds a Docker image.
 
     :param root: the path to build from
     :param dockerfile: the path to the Dockerfile to build
     :param base_image: the base image to use, or None if the default should be used
     :param target_image: the name of the new image
     """
-    logger = container.logger()
+    from re import MULTILINE, sub
+
+    logger = container.logger
     if base_image is not None:
         logger.info(f"Building '{target_image}' from '{dockerfile}' using '{base_image}' as base image")
     else:
         logger.info(f"Building '{target_image}' from '{dockerfile}'")
 
     if not dockerfile.is_file():
         raise RuntimeError(f"'{dockerfile}' does not exist")
 
     current_content = dockerfile.read_text(encoding="utf-8")
 
     if base_image is not None:
-        new_content = re.sub(r"^FROM.*$", f"FROM {base_image}", current_content, flags=re.MULTILINE)
+        new_content = sub(r"^FROM.*$", f"FROM {base_image}", current_content, flags=MULTILINE)
         dockerfile.write_text(new_content, encoding="utf-8")
 
     try:
-        docker_manager = container.docker_manager()
+        docker_manager = container.docker_manager
         docker_manager.build_image(root, dockerfile, target_image)
     finally:
         if base_image is not None:
             dockerfile.write_text(current_content, encoding="utf-8")
 
 
-@click.command(cls=LeanCommand, requires_docker=True)
-@click.argument("root", type=PathParameter(exists=True, file_okay=False, dir_okay=True), default=lambda: Path.cwd())
-@click.option("--tag", type=str, default="latest", help="The tag to apply to custom images (defaults to latest)")
+@command(cls=LeanCommand, requires_docker=True)
+@argument("root", type=PathParameter(exists=True, file_okay=False, dir_okay=True), default=lambda: Path.cwd())
+@option("--tag", type=str, default="latest", help="The tag to apply to custom images (defaults to latest)")
 def build(root: Path, tag: str) -> None:
-    """Build Docker images of your own version of LEAN and the Alpha Streams SDK.
+    """Build Docker images of your own version of LEAN.
 
     \b
-    ROOT must point to a directory containing the LEAN repository and the Alpha Streams SDK repository:
-    https://github.com/QuantConnect/Lean & https://github.com/QuantConnect/AlphaStreams
+    ROOT must point to a directory containing the LEAN repository:
+    https://github.com/QuantConnect/Lean
 
     When ROOT is not given, the current directory is used as root directory.
 
     \b
     This command performs the following actions:
     1. The lean-cli/foundation:latest image is built from Lean/DockerfileLeanFoundation(ARM).
     2. LEAN is compiled in a Docker container using the lean-cli/foundation:latest image.
-    3. The Alpha Streams SDK is compiled in a Docker container using the lean-cli/foundation:latest image.
-    4. The lean-cli/engine:latest image is built from Lean/Dockerfile using lean-cli/foundation:latest as base image.
-    5. The lean-cli/research:latest image is built from Lean/DockerfileJupyter using lean-cli/engine:latest as base image.
-    6. The default engine image is set to lean-cli/engine:latest.
-    7. The default research image is set to lean-cli/research:latest.
+    3. The lean-cli/engine:latest image is built from Lean/Dockerfile using lean-cli/foundation:latest as base image.
+    4. The lean-cli/research:latest image is built from Lean/DockerfileJupyter using lean-cli/engine:latest as base image.
+    5. The default engine image is set to lean-cli/engine:latest.
+    6. The default research image is set to lean-cli/research:latest.
 
     When the foundation Dockerfile is the same as the official foundation Dockerfile,
     quantconnect/lean:foundation is used instead of building a custom foundation image.
     """
     lean_dir = root / "Lean"
     if not lean_dir.is_dir():
         raise RuntimeError(f"Please clone https://github.com/QuantConnect/Lean to '{lean_dir}'")
 
-    alpha_streams_dir = root / "AlphaStreams"
-    if not lean_dir.is_dir():
-        raise RuntimeError(f"Please clone https://github.com/QuantConnect/AlphaStreams to '{alpha_streams_dir}'")
-
     (root / "DataLibraries").mkdir(exist_ok=True)
 
-    if container.platform_manager().is_host_arm():
+    if container.platform_manager.is_host_arm():
         foundation_dockerfile = lean_dir / "DockerfileLeanFoundationARM"
     else:
         foundation_dockerfile = lean_dir / "DockerfileLeanFoundation"
 
     if _is_foundation_dockerfile_same_as_cloud(foundation_dockerfile):
         foundation_image = DockerImage(name="quantconnect/lean", tag="foundation")
-        container.docker_manager().pull_image(foundation_image)
+        container.docker_manager.pull_image(foundation_image)
     else:
-        foundation_image = DockerImage(name="lean-cli/foundation", tag=tag)
+        foundation_image = DockerImage(name=CUSTOM_FOUNDATION, tag=tag)
         _build_image(root, foundation_dockerfile, None, foundation_image)
 
     _compile_csharp(root, lean_dir, foundation_image)
-    _compile_csharp(root, alpha_streams_dir, foundation_image)
 
-    custom_engine_image = DockerImage(name="lean-cli/engine", tag=tag)
+    custom_engine_image = DockerImage(name=CUSTOM_ENGINE, tag=tag)
     _build_image(root, lean_dir / "Dockerfile", foundation_image, custom_engine_image)
 
-    custom_research_image = DockerImage(name="lean-cli/research", tag=tag)
+    custom_research_image = DockerImage(name=CUSTOM_RESEARCH, tag=tag)
     _build_image(root, lean_dir / "DockerfileJupyter", custom_engine_image, custom_research_image)
 
-    logger = container.logger()
-    cli_config_manager = container.cli_config_manager()
+    logger = container.logger
+    cli_config_manager = container.cli_config_manager
 
     logger.info(f"Setting default engine image to '{custom_engine_image}'")
     cli_config_manager.engine_image.set_value(str(custom_engine_image))
 
     logger.info(f"Setting default research image to '{custom_research_image}'")
     cli_config_manager.research_image.set_value(str(custom_research_image))
```

### Comparing `lean-1.0.99/lean/commands/backtest.py` & `lean-1.155/lean/commands/backtest.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,65 +7,68 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
-import os
-from datetime import datetime
+
 from pathlib import Path
-from typing import Optional
-import click
+from typing import List, Optional, Tuple
+from click import command, option, argument, Choice
 
 from lean.click import LeanCommand, PathParameter
-from lean.constants import DEFAULT_ENGINE_IMAGE
-from lean.container import container
+from lean.constants import DEFAULT_ENGINE_IMAGE, LEAN_ROOT_PATH
+from lean.container import container, Logger
 from lean.models.api import QCMinimalOrganization
 from lean.models.utils import DebuggingMethod
 from lean.models.logger import Option
 from lean.models.data_providers import QuantConnectDataProvider, all_data_providers
-
+from lean.components.util.json_modules_handler import build_and_configure_modules, get_and_build_module
+from lean.models.click_options import options_from_json, get_configs_for_options
 
 # The _migrate_* methods automatically update launch configurations for a given debugging method.
 #
 # Occasionally we make changes which require updated launch configurations.
 # Projects which are created after these update have the correct configuration already,
 # but projects created before that need changes.
 #
 # These methods checks if the project has outdated configurations, and if so, update them to keep it working.
 
-def _migrate_python_pycharm(project_dir: Path) -> None:
+def _migrate_python_pycharm(logger: Logger, project_dir: Path) -> None:
+    from os import path
+    from click import Abort
+
     workspace_xml_path = project_dir / ".idea" / "workspace.xml"
     if not workspace_xml_path.is_file():
         return
 
-    xml_manager = container.xml_manager()
+    xml_manager = container.xml_manager
     current_content = xml_manager.parse(workspace_xml_path.read_text(encoding="utf-8"))
 
     config = current_content.find('.//configuration[@name="Debug with Lean CLI"]')
     if config is None:
         return
 
     path_mappings = config.find('.//PathMappingSettings/option[@name="pathMappings"]/list')
     if path_mappings is None:
         return
 
     made_changes = False
     has_library_mapping = False
 
-    library_dir = container.lean_config_manager().get_cli_root_directory() / "Library"
+    library_dir = container.lean_config_manager.get_cli_root_directory() / "Library"
+
     if library_dir.is_dir():
-        library_dir = f"$PROJECT_DIR$/{os.path.relpath(library_dir, project_dir)}".replace("\\", "/")
+        library_dir = f"$PROJECT_DIR$/{path.relpath(library_dir, project_dir)}".replace("\\", "/")
     else:
         library_dir = None
 
     for mapping in path_mappings.findall(".//mapping"):
-        if mapping.get("local-root") == "$PROJECT_DIR$" and mapping.get("remote-root") == "/Lean/Launcher/bin/Debug":
+        if mapping.get("local-root") == "$PROJECT_DIR$" and mapping.get("remote-root") == LEAN_ROOT_PATH:
             mapping.set("remote-root", "/LeanCLI")
             made_changes = True
 
         if library_dir is not None \
             and mapping.get("local-root") == library_dir \
             and mapping.get("remote-root") == "/Library":
             has_library_mapping = True
@@ -76,63 +79,66 @@
         library_mapping.set("remote-root", "/Library")
         path_mappings.append(library_mapping)
         made_changes = True
 
     if made_changes:
         workspace_xml_path.write_text(xml_manager.to_string(current_content), encoding="utf-8")
 
-        logger = container.logger()
+        logger = container.logger
         logger.warn("Your run configuration has been updated to work with the latest version of LEAN")
         logger.warn("Please restart the debugger in PyCharm and run this command again")
 
-        raise click.Abort()
+        raise Abort()
 
 
 def _migrate_python_vscode(project_dir: Path) -> None:
+    from json import dumps, loads
     launch_json_path = project_dir / ".vscode" / "launch.json"
     if not launch_json_path.is_file():
         return
 
-    current_content = json.loads(launch_json_path.read_text(encoding="utf-8"))
+    current_content = loads(launch_json_path.read_text(encoding="utf-8"))
     if "configurations" not in current_content or not isinstance(current_content["configurations"], list):
         return
 
     config = next((c for c in current_content["configurations"] if c["name"] == "Debug with Lean CLI"), None)
     if config is None:
         return
 
     made_changes = False
     has_library_mapping = False
 
-    library_dir = container.lean_config_manager().get_cli_root_directory() / "Library"
+    library_dir = container.lean_config_manager.get_cli_root_directory() / "Library"
     if not library_dir.is_dir():
         library_dir = None
 
     for mapping in config["pathMappings"]:
-        if mapping["localRoot"] == "${workspaceFolder}" and mapping["remoteRoot"] == "/Lean/Launcher/bin/Debug":
+        if mapping["localRoot"] == "${workspaceFolder}" and mapping["remoteRoot"] == LEAN_ROOT_PATH:
             mapping["remoteRoot"] = "/LeanCLI"
             made_changes = True
 
         if library_dir is not None and mapping["localRoot"] == str(library_dir) and mapping["remoteRoot"] == "/Library":
             has_library_mapping = True
 
     if library_dir is not None and not has_library_mapping:
         config["pathMappings"].append({
             "localRoot": str(library_dir),
             "remoteRoot": "/Library"
         })
         made_changes = True
 
     if made_changes:
-        launch_json_path.write_text(json.dumps(current_content, indent=4), encoding="utf-8")
+        launch_json_path.write_text(dumps(current_content, indent=4), encoding="utf-8")
 
 
-def _migrate_csharp_rider(project_dir: Path) -> None:
+def _migrate_csharp_rider(logger: Logger, project_dir: Path) -> None:
+    from click import Abort
+
     made_changes = False
-    xml_manager = container.xml_manager()
+    xml_manager = container.xml_manager
 
     for dir_name in [f".idea.{project_dir.stem}", f".idea.{project_dir.stem}.dir"]:
         workspace_xml_path = project_dir / ".idea" / dir_name / ".idea" / "workspace.xml"
         if not workspace_xml_path.is_file():
             continue
 
         current_content = xml_manager.parse(workspace_xml_path.read_text(encoding="utf-8"))
@@ -147,31 +153,31 @@
 
         run_manager.remove(config)
 
         workspace_xml_path.write_text(xml_manager.to_string(current_content), encoding="utf-8")
         made_changes = True
 
     if made_changes:
-        container.project_manager().generate_rider_config()
+        container.project_manager.generate_rider_config()
 
-        logger = container.logger()
         logger.warn("Your run configuration has been updated to work with the .NET 5 version of LEAN")
         logger.warn("Please restart Rider and start debugging again")
         logger.warn(
-            "See https://www.lean.io/docs/lean-cli/backtesting/debugging#05-C-and-Rider for the updated instructions")
+            "See https://www.lean.io/docs/v2/lean-cli/backtesting/debugging#05-C-and-Rider for the updated instructions")
 
-        raise click.Abort()
+        raise Abort()
 
 
 def _migrate_csharp_vscode(project_dir: Path) -> None:
+    from json import dumps, loads
     launch_json_path = project_dir / ".vscode" / "launch.json"
     if not launch_json_path.is_file():
         return
 
-    current_content = json.loads(launch_json_path.read_text(encoding="utf-8"))
+    current_content = loads(launch_json_path.read_text(encoding="utf-8"))
     if "configurations" not in current_content or not isinstance(current_content["configurations"], list):
         return
 
     config = next((c for c in current_content["configurations"] if c["name"] == "Debug with Lean CLI"), None)
     if config is None:
         return
 
@@ -192,23 +198,23 @@
         "quoteArgs": False
     }
 
     config["logging"] = {
         "moduleLoad": False
     }
 
-    launch_json_path.write_text(json.dumps(current_content, indent=4), encoding="utf-8")
+    launch_json_path.write_text(dumps(current_content, indent=4), encoding="utf-8")
 
 
 def _migrate_csharp_csproj(project_dir: Path) -> None:
     csproj_path = next((f for f in project_dir.rglob("*.csproj")), None)
     if csproj_path is None:
         return
 
-    xml_manager = container.xml_manager()
+    xml_manager = container.xml_manager
 
     current_content = xml_manager.parse(csproj_path.read_text(encoding="utf-8"))
     if current_content.find(".//PropertyGroup/DefaultItemExcludes") is not None:
         return
 
     property_group = current_content.find(".//PropertyGroup")
     if property_group is None:
@@ -223,141 +229,183 @@
 
 
 def _select_organization() -> QCMinimalOrganization:
     """Asks the user for the organization that should be charged when downloading data.
 
     :return: the selected organization
     """
-    api_client = container.api_client()
+    api_client = container.api_client
 
     organizations = api_client.organizations.get_all()
     options = [Option(id=organization, label=organization.name) for organization in organizations]
 
-    logger = container.logger()
+    logger = container.logger
     return logger.prompt_list("Select the organization to purchase and download data with", options)
 
 
-@click.command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
-@click.argument("project", type=PathParameter(exists=True, file_okay=True, dir_okay=True))
-@click.option("--output",
+@command(cls=LeanCommand, requires_lean_config=True, requires_docker=True)
+@argument("project", type=PathParameter(exists=True, file_okay=True, dir_okay=True))
+@option("--output",
               type=PathParameter(exists=False, file_okay=False, dir_okay=True),
               help="Directory to store results in (defaults to PROJECT/backtests/TIMESTAMP)")
-@click.option("--detach", "-d",
+@option("--detach", "-d",
               is_flag=True,
               default=False,
               help="Run the backtest in a detached Docker container and return immediately")
-@click.option("--debug",
-              type=click.Choice(["pycharm", "ptvsd", "vsdbg", "rider"], case_sensitive=False),
+@option("--debug",
+              type=Choice(["pycharm", "ptvsd", "vsdbg", "rider", "local-platform"], case_sensitive=False),
               help="Enable a certain debugging method (see --help for more information)")
-@click.option("--data-provider",
-              type=click.Choice([dp.get_name() for dp in all_data_providers], case_sensitive=False),
+@option("--data-provider",
+              type=Choice([dp.get_name() for dp in all_data_providers], case_sensitive=False),
+              default="Local",
               help="Update the Lean configuration file to retrieve data from the given provider")
-@click.option("--download-data",
+@options_from_json(get_configs_for_options("backtest"))
+@option("--download-data",
               is_flag=True,
               default=False,
               help="Update the Lean configuration file to download data from the QuantConnect API, alias for --data-provider QuantConnect")
-@click.option("--data-purchase-limit",
+@option("--data-purchase-limit",
               type=int,
               help="The maximum amount of QCC to spend on downloading data during the backtest when using QuantConnect as data provider")
-@click.option("--release",
+@option("--release",
               is_flag=True,
               default=False,
               help="Compile C# projects in release configuration instead of debug")
-@click.option("--image",
+@option("--image",
               type=str,
               help=f"The LEAN engine image to use (defaults to {DEFAULT_ENGINE_IMAGE})")
-@click.option("--update",
+@option("--python-venv",
+              type=str,
+              help=f"The path of the python virtual environment to be used")
+@option("--update",
               is_flag=True,
               default=False,
               help="Pull the LEAN engine image before running the backtest")
-@click.option("--backtest-name",
+@option("--backtest-name",
               type=str,
               help="Backtest name")
+@option("--addon-module",
+              type=str,
+              multiple=True,
+              hidden=True)
+@option("--extra-config",
+              type=(str, str),
+              multiple=True,
+              hidden=True)
+@option("--no-update",
+              is_flag=True,
+              default=False,
+              help="Use the local LEAN engine image instead of pulling the latest version")
 def backtest(project: Path,
              output: Optional[Path],
              detach: bool,
              debug: Optional[str],
              data_provider: Optional[str],
              download_data: bool,
              data_purchase_limit: Optional[int],
              release: bool,
              image: Optional[str],
+             python_venv: Optional[str],
              update: bool,
-             backtest_name: str) -> None:
+             backtest_name: str,
+             addon_module: Optional[List[str]],
+             extra_config: Optional[Tuple[str, str]],
+             no_update: bool,
+             **kwargs) -> None:
     """Backtest a project locally using Docker.
 
     \b
     If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
     If PROJECT is a file, the algorithm in the specified file will be executed.
 
     \b
     Go to the following url to learn how to debug backtests locally using the Lean CLI:
-    https://www.lean.io/docs/lean-cli/backtesting/debugging
+    https://www.lean.io/docs/v2/lean-cli/backtesting/debugging
 
     By default the official LEAN engine image is used.
     You can override this using the --image option.
     Alternatively you can set the default engine image for all commands using `lean config set engine-image <image>`.
     """
-    project_manager = container.project_manager()
+    from datetime import datetime
+    logger = container.logger
+    project_manager = container.project_manager
     algorithm_file = project_manager.find_algorithm_file(Path(project))
-    lean_config_manager = container.lean_config_manager()
-
+    lean_config_manager = container.lean_config_manager
     if output is None:
         output = algorithm_file.parent / "backtests" / datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
 
     debugging_method = None
     if debug == "pycharm":
         debugging_method = DebuggingMethod.PyCharm
-        _migrate_python_pycharm(algorithm_file.parent)
+        _migrate_python_pycharm(logger, algorithm_file.parent)
     elif debug == "ptvsd":
         debugging_method = DebuggingMethod.PTVSD
         _migrate_python_vscode(algorithm_file.parent)
     elif debug == "vsdbg":
         debugging_method = DebuggingMethod.VSDBG
         _migrate_csharp_vscode(algorithm_file.parent)
     elif debug == "rider":
         debugging_method = DebuggingMethod.Rider
-        _migrate_csharp_rider(algorithm_file.parent)
+        _migrate_csharp_rider(logger, algorithm_file.parent)
+    elif debug == "local-platform":
+        debugging_method = DebuggingMethod.LocalPlatform
 
-    if debugging_method is not None and detach:
+    if detach and debugging_method != None and debugging_method != DebuggingMethod.LocalPlatform:
         raise RuntimeError("Running a debugging session in a detached container is not supported")
 
     if algorithm_file.name.endswith(".cs"):
         _migrate_csharp_csproj(algorithm_file.parent)
 
     lean_config = lean_config_manager.get_complete_lean_config("backtesting", algorithm_file, debugging_method)
 
     if download_data:
         data_provider = QuantConnectDataProvider.get_name()
 
     if data_provider is not None:
-        data_provider = next(dp for dp in all_data_providers if dp.get_name() == data_provider)
-        data_provider.build(lean_config, container.logger()).configure(lean_config, "backtesting")
+        [data_provider_configurer] = [get_and_build_module(data_provider, all_data_providers, kwargs, logger)]
+        data_provider_configurer.configure(lean_config, "backtesting")
 
     lean_config_manager.configure_data_purchase_limit(lean_config, data_purchase_limit)
 
-    cli_config_manager = container.cli_config_manager()
-    project_config_manager = container.project_config_manager()
+    cli_config_manager = container.cli_config_manager
+    project_config_manager = container.project_config_manager
 
     project_config = project_config_manager.get_project_config(algorithm_file.parent)
     engine_image = cli_config_manager.get_engine_image(image or project_config.get("engine-image", None))
 
-    container.update_manager().pull_docker_image_if_necessary(engine_image, update)
+    if str(engine_image) != DEFAULT_ENGINE_IMAGE:
+        logger.warn(f'A custom engine image: "{engine_image}" is being used!')
+
+    container.update_manager.pull_docker_image_if_necessary(engine_image, update, no_update)
 
     if not output.exists():
         output.mkdir(parents=True)
 
-    output_config_manager = container.output_config_manager()
-    lean_config["algorithm-id"] = str(output_config_manager.get_backtest_id(output))
-
     # Set backtest name
     if backtest_name is not None and backtest_name != "":
         lean_config["backtest-name"] = backtest_name
-    
-    lean_runner = container.lean_runner()
+
+    # Set extra config
+    given_algorithm_id = None
+    for key, value in extra_config:
+        if key == "algorithm-id":
+            given_algorithm_id = int(value)
+        else:
+            lean_config[key] = value
+
+    output_config_manager = container.output_config_manager
+    lean_config["algorithm-id"] = str(output_config_manager.get_backtest_id(output, given_algorithm_id))
+
+    if python_venv is not None and python_venv != "":
+        lean_config["python-venv"] = f'{"/" if python_venv[0] != "/" else ""}{python_venv}'
+
+    # Configure addon modules
+    build_and_configure_modules(addon_module, container.organization_manager.try_get_working_organization_id(), lean_config, logger, "backtesting")
+
+    lean_runner = container.lean_runner
     lean_runner.run_lean(lean_config,
                          "backtesting",
                          algorithm_file,
                          output,
                          engine_image,
                          debugging_method,
                          release,
```

### Comparing `lean-1.0.99/lean/commands/login.py` & `lean-1.155/lean/commands/login.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,48 +9,50 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Optional
 
-import click
+from click import command, option, prompt
 
 from lean.click import LeanCommand
 from lean.container import container
 from lean.models.errors import MoreInfoError
+from lean.components.api.api_client import APIClient
 
 
-@click.command(cls=LeanCommand)
-@click.option("--user-id", "-u", type=str, help="QuantConnect user id")
-@click.option("--api-token", "-t", type=str, help="QuantConnect API token")
-def login(user_id: Optional[str], api_token: Optional[str]) -> None:
+@command(cls=LeanCommand)
+@option("--user-id", "-u", type=str, help="QuantConnect user id")
+@option("--api-token", "-t", type=str, help="QuantConnect API token")
+@option("--show-secrets", is_flag=True, show_default=True, default=False, help="Show secrets as they are input")
+def login(user_id: Optional[str], api_token: Optional[str], show_secrets: bool) -> None:
     """Log in with a QuantConnect account.
 
     If user id or API token is not provided an interactive prompt will show.
 
     Credentials are stored in ~/.lean/credentials and are removed upon running `lean logout`.
     """
-    logger = container.logger()
-    credentials_storage = container.credentials_storage()
+    logger = container.logger
+    credentials_storage = container.credentials_storage
 
     if user_id is None or api_token is None:
         logger.info("Your user id and API token are needed to make authenticated requests to the QuantConnect API")
         logger.info("You can request these credentials on https://www.quantconnect.com/account")
         logger.info(f"Both will be saved in {credentials_storage.file}")
 
     if user_id is None:
-        user_id = click.prompt("User id")
+        user_id = prompt("User id")
 
     if api_token is None:
-        api_token = logger.prompt_password("API token")
+        api_token = logger.prompt_password("API token", hide_input=not show_secrets)
 
-    api_client = container.api_client(user_id=user_id, api_token=api_token)
-    if not api_client.is_authenticated():
-        raise MoreInfoError("Credentials are invalid",
-                            "https://www.lean.io/docs/lean-cli/initialization/authenticating-accounts#02-Log-In")
+    container.api_client.set_user_token(user_id=user_id, api_token=api_token)
+    if not container.api_client.is_authenticated():
+        raise MoreInfoError("Credentials are invalid. Please ensure your computer clock is correct, or try using another terminal, or enter API token manually instead of copy-pasting.",
+                            "https://www.lean.io/docs/v2/lean-cli")
 
-    cli_config_manager = container.cli_config_manager()
+    cli_config_manager = container.cli_config_manager
     cli_config_manager.user_id.set_value(user_id)
     cli_config_manager.api_token.set_value(api_token)
 
     logger.info("Successfully logged in")
```

### Comparing `lean-1.0.99/lean/models/pydantic.py` & `lean-1.155/lean/models/pydantic.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/models/data_providers/data_provider.py` & `lean-1.155/lean/models/data_providers/data_provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any, Dict
 from lean.models.lean_config_configurer import LeanConfigConfigurer
-from lean.models.configuration import Configuration
-
 
 class DataProvider(LeanConfigConfigurer):
     """A JsonModule implementation for the Json data provider module."""
 
     def __init__(self, json_data_provider_data: Dict[str, Any]) -> None:
         super().__init__(json_data_provider_data)
```

### Comparing `lean-1.0.99/lean/models/data_providers/__init__.py` & `lean-1.155/lean/models/data_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/models/logger.py` & `lean-1.155/lean/models/logger.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/models/brokerages/cloud/cloud_brokerage.py` & `lean-1.155/lean/models/brokerages/cloud/cloud_brokerage.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,16 +46,23 @@
                     value = config._value
                 else:
                     for option in config._value_options:
                         if option._condition.check(self.get_config_value_from_name(option._condition._dependent_config_id)):
                             value = option._value
                             break
                     if not value:
+                        options_to_log = set([(opt._condition._dependent_config_id,
+                                               self.get_config_value_from_name(opt._condition._dependent_config_id))
+                                              for opt in config._value_options])
                         raise ValueError(
-                            f'No condtion matched among present options for {config._cloud_id}')
+                            f'No condition matched among present options for "{config._cloud_id}". '
+                            f'Please review ' +
+                            ', '.join([f'"{x[0]}"' for x in options_to_log]) +
+                            f' given value{"s" if len(options_to_log) > 1 else ""} ' +
+                            ', '.join([f'"{x[1]}"' for x in options_to_log]))
             else:
                 value = config._value
             settings[config._cloud_id] = value
         return settings
 
     def get_settings(self) -> Dict[str, str]:
         """Returns all settings for this brokerage.
```

### Comparing `lean-1.0.99/lean/models/brokerages/cloud/__init__.py` & `lean-1.155/lean/models/brokerages/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/models/brokerages/local/__init__.py` & `lean-1.155/lean/models/brokerages/local/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
+from os import environ
 from typing import Dict, Type, List
 from lean.container import container
 from lean.models.brokerages.local.local_brokerage import LocalBrokerage
 from lean.models.brokerages.local.data_feed import DataFeed
 from lean.models import json_modules
 
 all_local_brokerages: List[LocalBrokerage] = []
@@ -26,13 +26,13 @@
 for json_module in json_modules:
     if "local-brokerage" in json_module["type"]:
         all_local_brokerages.append(LocalBrokerage(json_module))
     if "data-queue-handler" in json_module["type"]:
         all_local_data_feeds.append(DataFeed(json_module))
 
 # Remove IQFeed DataFeed for other than windows machines
-if not [container.platform_manager().is_host_windows() or os.environ.get("__README__", "false") == "true"]:
+if not [container.platform_manager.is_host_windows() or environ.get("__README__", "false") == "true"]:
     all_local_data_feeds = [
         data_feed for data_feed in all_local_data_feeds if data_feed._id != "IQFeed"]
 
 for local_brokerage in all_local_brokerages:
     local_brokerage_data_feeds[local_brokerage] = all_local_data_feeds
```

### Comparing `lean-1.0.99/lean/models/brokerages/local/local_brokerage.py` & `lean-1.155/lean/models/brokerages/local/data_feed.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any, Dict
 from lean.models.lean_config_configurer import LeanConfigConfigurer
-from lean.models.configuration import Configuration
 
 
-class LocalBrokerage(LeanConfigConfigurer):
-    """A JsonModule implementation for the Json brokerage module."""
+class DataFeed(LeanConfigConfigurer):
+    """A JsonModule implementation for the Json data feed module."""
 
-    def __init__(self, json_brokerage_data: Dict[str, Any]) -> None:
-        super().__init__(json_brokerage_data)
+    def __init__(self, json_datafeed_data: Dict[str, Any]) -> None:
+        super().__init__(json_datafeed_data)
 
     def get_live_name(self, environment_name: str) -> str:
         live_name = self._id
         environment_obj = self.get_configurations_env_values_from_name(
             environment_name)
         if environment_obj:
             [live_name] = [x["value"]
-                           for x in environment_obj if x["name"] == "live-mode-brokerage"]
+                           for x in environment_obj if x["name"] == "data-queue-handler"]
         return live_name
```

### Comparing `lean-1.0.99/lean/models/brokerages/__init__.py` & `lean-1.155/lean/components/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/models/options.py` & `lean-1.155/lean/models/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,24 +64,27 @@
     """
 
     def __init__(self,
                  key: str,
                  description: str,
                  allowed_values: List[str],
                  is_sensitive: bool,
-                 storage: Storage) -> None:
+                 storage: Storage,
+                 default_value: str = None) -> None:
         """Creates a new ChoiceOption instance.
 
         :param key: the name of the key of the option in the given file, should use hyphens for separation
         :param description: a display-friendly description of the option
         :param allowed_values: the values which can be set
         :param is_sensitive: whether the contents of this option may be logged without masking it
         :param storage: the Storage instance to store this option in
+        :param default_value: the default value to use for the choices
         """
         self.allowed_values = allowed_values
+        self.default_value = default_value
 
         if description.endswith("."):
             description = description[:-1]
         description = description + f" (allowed values: {', '.join(allowed_values)})."
 
         super().__init__(key, description, is_sensitive, storage)
```

### Comparing `lean-1.0.99/lean/models/configuration.py` & `lean-1.155/lean/models/configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,23 +8,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from pathlib import Path
-import re
 from typing import Any, Dict, List
-import click
-import abc
+from click import prompt, Choice
+from abc import ABC, abstractmethod
 from lean.components.util.logger import Logger
 from lean.click import PathParameter
 
 
-class BaseCondition(abc.ABC):
+class BaseCondition(ABC):
     """Base condition class extended to all types of conditions"""
 
     def __init__(self, condition_object: Dict[str, str]):
         self._type: str = condition_object["type"]
         self._pattern: str = str(condition_object["pattern"])
         self._dependent_config_id: str = condition_object["dependent-config-id"]
 
@@ -39,15 +38,15 @@
             return RegexCondition(condition_object)
         elif condition_object["type"] == "exact-match":
             return ExactMatchCondition(condition_object)
         else:
             raise ValueError(
                 f'Undefined condition type {condition_object["type"]}')
 
-    @abc.abstractmethod
+    @abstractmethod
     def check(self, target_value: str) -> bool:
         """validates the condition against the provided values
 
         :param target_value: value to validate the condition against
         :return: True if the condition is valid otherwise False
         """
         raise NotImplementedError()
@@ -70,39 +69,40 @@
 
     def check(self, target_value: str) -> bool:
         """validates the condition against the provided values
 
         :param target_value: value to validate the condition against
         :return: True if the condition is valid otherwise False
         """
-        return len(re.findall(self._pattern, target_value, re.I)) > 0
+        from re import findall, I
+        return len(findall(self._pattern, target_value, I)) > 0
 
 
 class ConditionalValueOption():
     """This class is used when mutliple values needs to be evaluated based on conditions."""
 
     def __init__(self, option_object: Dict[str, Any]):
         self._value: str = option_object["value"]
         self._condition: BaseCondition = BaseCondition.factory(
             option_object["condition"])
 
 
-class Configuration(abc.ABC):
+class Configuration(ABC):
     """Base configuration class extended to all types of configurations"""
 
     def __init__(self, config_json_object):
         self._id: str = config_json_object["id"]
         self._config_type: str = config_json_object["type"]
         self._value: str = config_json_object["value"]
+        self._is_cloud_property: bool = "cloud-id" in config_json_object
         self._is_required_from_user = False
+        self._save_persistently_in_lean = False
         self._is_type_configurations_env: bool = type(
             self) is ConfigurationsEnvConfiguration
         self._is_type_trading_env: bool = type(self) is TradingEnvConfiguration
-        self.is_type_organization_id: bool = type(
-            self) is OrganzationIdConfiguration
         self._log_message: str = ""
         if "log-message" in config_json_object.keys():
             self._log_message = config_json_object["log-message"]
         if "filters" in config_json_object.keys():
             self._filter = Filter(config_json_object["filters"])
         else:
             self._filter = Filter([])
@@ -115,18 +115,18 @@
         :return: An instance of Configuration.
         """
 
         if config_json_object["type"] in ["info", "configurations-env"]:
             return InfoConfiguration.factory(config_json_object)
         elif config_json_object["type"] in ["input", "internal-input"]:
             return UserInputConfiguration.factory(config_json_object)
-        elif config_json_object["type"] in ["filter-env", "trading-env"]:
+        elif config_json_object["type"] == "filter-env":
             return BrokerageEnvConfiguration.factory(config_json_object)
-        elif config_json_object["type"] == "organization-id":
-            return OrganzationIdConfiguration(config_json_object)
+        elif config_json_object["type"] == "trading-env":
+            return TradingEnvConfiguration.factory(config_json_object)
         else:
             raise ValueError(
                 f'Undefined input method type {config_json_object["type"]}')
 
 
 class Filter():
     """This class handles the conditional filters added to configurations.
@@ -169,45 +169,49 @@
 
     def __init__(self, config_json_object):
         super().__init__(config_json_object)
         self._env_and_values = {
             env_obj["name"]: env_obj["value"] for env_obj in self._value}
 
 
-class UserInputConfiguration(Configuration, abc.ABC):
-    """Base class extended to all confiugration class than store values in Lean config.
+class UserInputConfiguration(Configuration, ABC):
+    """Base class extended to all configuration class that requires input from user.
 
     Values are expected from the user via prompts.
     Values of this configuration is persistently saved in the Lean configuration,
     until specified explicitly.
     """
 
     def __init__(self, config_json_object):
         super().__init__(config_json_object)
         self._is_required_from_user = True
+        self._save_persistently_in_lean = True
         self._input_method = self._prompt_info = self._help = ""
         self._input_default = self._cloud_id = None
         if "input-method" in config_json_object.keys():
             self._input_method = config_json_object["input-method"]
         if "prompt-info" in config_json_object.keys():
             self._prompt_info = config_json_object["prompt-info"]
         if "help" in config_json_object.keys():
             self._help = config_json_object["help"]
         if "input-default" in config_json_object.keys():
             self._input_default = config_json_object["input-default"]
         if "cloud-id" in config_json_object.keys():
             self._cloud_id = config_json_object["cloud-id"]
+        if "save-persistently-in-lean" in config_json_object.keys():
+            self._save_persistently_in_lean = config_json_object["save-persistently-in-lean"]
 
-    @abc.abstractmethod
-    def AskUserForInput(self, default_value: Any, logger: Logger):
+    @abstractmethod
+    def ask_user_for_input(self, default_value, logger: Logger, hide_input: bool = False):
         """Prompts user to provide input while validating the type of input
         against the expected type
 
         :param default_value: The default to prompt to the user.
         :param logger: The instance of logger class.
+        :param hide_input: Whether to hide the input
         :return: The value provided by the user.
         """
         return NotImplemented()
 
     def factory(config_json_object) -> 'UserInputConfiguration':
         """Creates an instance of the child classes.
 
@@ -239,24 +243,24 @@
         value_options: List[ConditionalValueOption] = []
         if "value-options" in config_json_object.keys():
             value_options = [ConditionalValueOption(
                 value_option) for value_option in config_json_object["value-options"]]
             self._is_conditional = True
         self._value_options = value_options
 
-    def AskUserForInput(self, default_value, logger: Logger):
+    def ask_user_for_input(self, default_value, logger: Logger, hide_input: bool = False):
         """Prompts user to provide input while validating the type of input
         against the expected type
 
         :param default_value: The default to prompt to the user.
         :param logger: The instance of logger class.
+        :param hide_input: Whether to hide the input (not used for this type of input, which is never hidden).
         :return: The value provided by the user.
         """
-        raise ValueError(
-            f'user input not allowed with {self.__class__.__name__}')
+        raise ValueError(f'user input not allowed with {self.__class__.__name__}')
 
 
 class PromptUserInput(UserInputConfiguration):
     map_to_types = {
         "string": str,
         "boolean": bool,
         "integer": int
@@ -264,179 +268,188 @@
 
     def __init__(self, config_json_object):
         super().__init__(config_json_object)
         self._input_type: str = "string"
         if "input-type" in config_json_object.keys():
             self._input_type = config_json_object["input-type"]
 
-    def AskUserForInput(self, default_value, logger: Logger):
+    def ask_user_for_input(self, default_value, logger: Logger, hide_input: bool = False):
         """Prompts user to provide input while validating the type of input
         against the expected type
 
         :param default_value: The default to prompt to the user.
         :param logger: The instance of logger class.
+        :param hide_input: Whether to hide the input (not used for this type of input, which is never hidden).
         :return: The value provided by the user.
         """
-        return click.prompt(self._prompt_info, default_value, type=self.get_input_type())
+        return prompt(self._prompt_info, default_value, type=self.get_input_type())
 
     def get_input_type(self):
         return self.map_to_types.get(self._input_type, self._input_type)
 
 
 class ChoiceUserInput(UserInputConfiguration):
     def __init__(self, config_json_object):
         super().__init__(config_json_object)
         self._choices: List[str] = []
         if "input-choices" in config_json_object.keys():
             self._choices = config_json_object["input-choices"]
 
-    def AskUserForInput(self, default_value, logger: Logger):
+    def ask_user_for_input(self, default_value, logger: Logger, hide_input: bool = False):
         """Prompts user to provide input while validating the type of input
         against the expected type
 
         :param default_value: The default to prompt to the user.
         :param logger: The instance of logger class.
+        :param hide_input: Whether to hide the input (not used for this type of input, which is never hidden).
         :return: The value provided by the user.
         """
-        return click.prompt(
+        return prompt(
             self._prompt_info,
             default_value,
-            type=click.Choice(self._choices, case_sensitive=False)
+            type=Choice(self._choices, case_sensitive=False)
         )
 
 
 class PathParameterUserInput(UserInputConfiguration):
     def __init__(self, config_json_object):
         super().__init__(config_json_object)
 
-    def AskUserForInput(self, default_value, logger: Logger):
+    def ask_user_for_input(self, default_value, logger: Logger, hide_input: bool = False):
         """Prompts user to provide input while validating the type of input
         against the expected type
 
         :param default_value: The default to prompt to the user.
         :param logger: The instance of logger class.
+        :param hide_input: Whether to hide the input (not used for this type of input, which is never hidden).
         :return: The value provided by the user.
         """
 
         default_binary = None
         if default_value is not None:
             default_binary = Path(default_value)
         elif self._input_default is not None and Path(self._input_default).is_file():
             default_binary = Path(self._input_default)
         else:
             default_binary = ""
-        value = click.prompt(self._prompt_info,
+        value = prompt(self._prompt_info,
                              default=default_binary,
                              type=PathParameter(
                                  exists=False, file_okay=True, dir_okay=False)
                              )
         return value
 
 
 class ConfirmUserInput(UserInputConfiguration):
     def __init__(self, config_json_object):
         super().__init__(config_json_object)
 
-    def AskUserForInput(self, default_value, logger: Logger):
+    def ask_user_for_input(self, default_value, logger: Logger, hide_input: bool = False):
         """Prompts user to provide input while validating the type of input
         against the expected type
 
         :param default_value: The default to prompt to the user.
         :param logger: The instance of logger class.
+        :param hide_input: Whether to hide the input (not used for this type of input, which is never hidden).
         :return: The value provided by the user.
         """
-        return click.prompt(self._prompt_info, default_value, type=bool)
+        return prompt(self._prompt_info, default_value, type=bool)
 
 
 class PromptPasswordUserInput(UserInputConfiguration):
     def __init__(self, config_json_object):
         super().__init__(config_json_object)
 
-    def AskUserForInput(self, default_value, logger: Logger):
+    def ask_user_for_input(self, default_value, logger: Logger, hide_input: bool = True):
         """Prompts user to provide input while validating the type of input
         against the expected type
 
         :param default_value: The default to prompt to the user.
         :param logger: The instance of logger class.
+        :param hide_input: Whether to hide the input
         :return: The value provided by the user.
         """
-        return logger.prompt_password(self._prompt_info, default_value)
-
-
-class OrganzationIdConfiguration(PromptUserInput):
-    """This class is used for job-organzation-id configurations"""
-
-    def __init__(self, config_json_object):
-        super().__init__(config_json_object)
+        return logger.prompt_password(self._prompt_info, default_value, hide_input=hide_input)
 
 
 class BrokerageEnvConfiguration(PromptUserInput, ChoiceUserInput, ConfirmUserInput):
     """This class is base class extended by all classes that needs to add value to user filters"""
 
     def __init__(self, config_json_object):
         super().__init__(config_json_object)
 
     def factory(config_json_object) -> 'BrokerageEnvConfiguration':
         """Creates an instance of the child classes.
 
         :param config_json_object: the json object dict with configuration info
-        :return: An instance of BrokerageEnvConfiguration.
+        :return: An instance of BrokerageEnvConfiguration
         """
-        if config_json_object["type"] == "trading-env":
-            return TradingEnvConfiguration(config_json_object)
-        elif config_json_object["type"] == "filter-env":
+        if config_json_object["type"] == "filter-env":
             return FilterEnvConfiguration(config_json_object)
         else:
             raise ValueError(
                 f'Undefined input method type {config_json_object["type"]}')
 
-    def AskUserForInput(self, default_value, logger: Logger):
+    def ask_user_for_input(self, default_value, logger: Logger, hide_input: bool = False):
         """Prompts user to provide input while validating the type of input
         against the expected type
 
         :param default_value: The default to prompt to the user.
         :param logger: The instance of logger class.
+        :param hide_input: Whether to hide the input (not used for this type of input, which is never hidden).
         :return: The value provided by the user.
         """
         if self._input_method == "confirm":
-            return ConfirmUserInput.AskUserForInput(self, default_value, logger)
+            return ConfirmUserInput.ask_user_for_input(self, default_value, logger)
         elif self._input_method == "choice":
-            return ChoiceUserInput.AskUserForInput(self, default_value, logger)
+            return ChoiceUserInput.ask_user_for_input(self, default_value, logger)
         elif self._input_method == "prompt":
-            return PromptUserInput.AskUserForInput(self, default_value, logger)
+            return PromptUserInput.ask_user_for_input(self, default_value, logger)
         else:
-            raise ValueError(
-                f"Undefined input method type {self._input_method}")
+            raise ValueError(f"Undefined input method type {self._input_method}")
 
 
-class TradingEnvConfiguration(BrokerageEnvConfiguration):
+class TradingEnvConfiguration(PromptUserInput, ChoiceUserInput, ConfirmUserInput):
     """This class adds trading-mode/envirionment based user filters.
-    
-    Normalizes the value of envrionment values(live/paper) for cloud live. 
+
+    Normalizes the value of envrionment values(live/paper) for cloud live.
     """
 
     def __init__(self, config_json_object):
         super().__init__(config_json_object)
 
-    def AskUserForInput(self, default_value, logger: Logger):
+    def factory(config_json_object) -> 'TradingEnvConfiguration':
+        """Creates an instance of the child classes.
+
+        :param config_json_object: the json object dict with configuration info
+        :return: An instance of TradingEnvConfiguration.
+        """
+        if config_json_object["type"] == "trading-env":
+            return TradingEnvConfiguration(config_json_object)
+        else:
+            raise ValueError(
+                f'Undefined input method type {config_json_object["type"]}')
+
+    def ask_user_for_input(self, default_value, logger: Logger, hide_input: bool = False):
         """Prompts user to provide input while validating the type of input
         against the expected type
 
         :param default_value: The default to prompt to the user.
         :param logger: The instance of logger class.
+        :param hide_input: Whether to hide the input (not used for this type of input, which is never hidden).
         :return: The value provided by the user.
         """
         # NOTE: trading envrionment config should not use old boolean value as default
         if type(default_value) == bool:
             default_value = "paper" if default_value else "live"
         if self._input_method == "confirm":
             raise ValueError(
                 f'input method -- {self._input_method} is not allowed with {self.__class__.__name__}')
         else:
-            return BrokerageEnvConfiguration.AskUserForInput(self, default_value, logger)
+            return BrokerageEnvConfiguration.ask_user_for_input(self, default_value, logger)
 
 
 class FilterEnvConfiguration(BrokerageEnvConfiguration):
     """This class adds extra filters to user filters."""
 
     def __init__(self, config_json_object):
         super().__init__(config_json_object)
```

### Comparing `lean-1.0.99/lean/models/__init__.py` & `lean-1.155/lean/models/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,37 +7,48 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
-import json
-import requests
+from os import path
+from json import load
 from pathlib import Path
+from time import time
 
 json_modules = {}
-file_name = "modules-1.3.json"
-dirname = os.path.dirname(__file__)
-file_path = os.path.join(dirname, f'../{file_name}')
+file_name = "modules-1.11.json"
+directory = Path(__file__).parent
+file_path = directory.parent / file_name
 
-# check if new file is avaiable online
+# check if new file is available online
 url = f"https://cdn.quantconnect.com/cli/{file_name}"
+error = None
 try:
-    res = requests.get(url)
-    if res.ok:
-        new_content = res.json()
-        with open(file_path, 'w', encoding='utf-8') as f:
-            json.dump(new_content, f, ensure_ascii=False, indent=4)
+    # fetch if file not available or fetched before 1 day
+    if not path.exists(file_path) or (time() - path.getmtime(file_path) > 86400):
+        from requests import get
+        res = get(url, timeout=5)
+        if res.ok:
+            new_content = res.json()
+            from json import dump
+            # create parents if not exists
+            file_path.parent.mkdir(parents=True, exist_ok=True)
+            with open(file_path, 'w', encoding='utf-8') as f:
+                dump(new_content, f, ensure_ascii=False, indent=4)
+        else:
+            res.raise_for_status()
 except Exception as e:
-    # No need to do anything if file isn't avaiable
+    # No need to do anything if file isn't available
+    error = str(e)
     pass
 
 # check if file exists
 if not Path(file_path).is_file():
+    error_message = f": {error}" if error is not None else ""
     raise FileNotFoundError(
-        f"Modules json not found in the given path {file_path}")
+        f"Modules json not found in the given path {file_path}{error_message}")
 
 with open(file_path) as f:
-    data = json.load(f)
+    data = load(f)
     json_modules = data['modules']
```

### Comparing `lean-1.0.99/lean/models/api.py` & `lean-1.155/lean/models/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,25 +7,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import re
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import validator
-from rich import box
-from rich.table import Table
-from rich.text import Text
 
-from lean.constants import EQUITY_SECURITY_MASTER_PRODUCT_ID, BULK_EQUITY_SECURITY_MASTER_PRODUCT_ID
+from lean.constants import EQUITY_SECURITY_MASTER_PRODUCT_ID
 from lean.models.pydantic import WrappedBaseModel
 
 
 # The models in this module are all parts of responses from the QuantConnect API
 # The keys of properties are not changed, so they don't obey the rest of the project's naming conventions
 
 
@@ -44,69 +40,73 @@
     value: str
     min: Optional[float]
     max: Optional[float]
     step: Optional[float]
     type: Optional[str]
 
 
-class QCLiveResults(WrappedBaseModel):
-    eStatus: str
-    sDeployID: Optional[str] = None
-    sServerType: Optional[str] = None
-    dtLaunched: Optional[datetime] = None
-    dtStopped: Optional[datetime] = None
-    sBrokerage: Optional[str] = None
-    sSecurityTypes: Optional[str] = None
-    dUnrealized: Optional[float] = None
-    dfees: Optional[float] = None
-    dnetprofit: Optional[float] = None
-    dEquity: Optional[float] = None
-    dHoldings: Optional[float] = None
-    dCapital: Optional[float] = None
-    dVolume: Optional[float] = None
-    iTrades: Optional[int] = None
-    sErrorMessage: Optional[str] = None
-
-
 class QCLanguage(str, Enum):
     CSharp = "C#"
     FSharp = "F#"
     VisualBasic = "VB"
     Java = "Ja"
     Python = "Py"
 
 
+class QCProjectLibrary(WrappedBaseModel):
+    projectId: int
+    libraryName: str
+    ownerName: str
+    access: bool
+
+    def __hash__(self):
+        return hash(self.projectId)
+
+    def __eq__(self, other: Any):
+        if not isinstance(other, type(self)):
+            return NotImplemented
+        return self.projectId == other.projectId
+
+
 class QCProject(WrappedBaseModel):
     projectId: int
     organizationId: str
     name: str
     description: str
     modified: datetime
     created: datetime
     language: QCLanguage
     collaborators: List[QCCollaborator]
     leanVersionId: int
     leanPinnedToMaster: bool
+    leanEnvironment: int
     parameters: List[QCParameter]
-    liveResults: QCLiveResults
-    libraries: List[int]
+    libraries: List[QCProjectLibrary]
 
     @validator("parameters", pre=True)
     def process_parameters_dict(cls, value: Any) -> Any:
         if isinstance(value, dict):
             return list(value.values())
         return value
 
     def get_url(self) -> str:
         """Returns the url of the project page in the cloud.
 
         :return: a url which when visited opens an Algorithm Lab tab containing the project
         """
         return f"https://www.quantconnect.com/project/{self.projectId}"
 
+    def __hash__(self):
+        return hash(self.projectId)
+
+    def __eq__(self, other: Any):
+        if not isinstance(other, type(self)):
+            return NotImplemented
+        return self.projectId == other.projectId
+
 
 class QCCreatedProject(WrappedBaseModel):
     projectId: int
     name: str
     modified: datetime
     created: datetime
 
@@ -186,19 +186,23 @@
     def get_url(self) -> str:
         """Returns the url of the backtests results page in the cloud.
 
         :return: a url which when visited opens an Algorithm Lab tab containing the backtest's results
         """
         return f"https://www.quantconnect.com/project/{self.projectId}/{self.backtestId}"
 
-    def get_statistics_table(self) -> Table:
+    def get_statistics_table(self):
         """Converts the statistics into a pretty table.
 
         :return: a table containing all statistics
         """
+        from rich import box
+        from rich.table import Table
+        from rich.text import Text
+
         stats = []
 
         for key, value in self.runtimeStatistics.items():
             stats.append(key)
 
             if "-" in value:
                 stats.append(Text.from_markup(f"[red]{value}[/red]"))
@@ -316,15 +320,20 @@
     headers: Dict[str, str]
 
 
 class QCSMSNotificationMethod(WrappedBaseModel):
     phoneNumber: str
 
 
-QCNotificationMethod = Union[QCEmailNotificationMethod, QCWebhookNotificationMethod, QCSMSNotificationMethod]
+class QCTelegramNotificationMethod(WrappedBaseModel):
+    id: str
+    token: Optional[str] = None
+
+
+QCNotificationMethod = Union[QCEmailNotificationMethod, QCWebhookNotificationMethod, QCSMSNotificationMethod, QCTelegramNotificationMethod]
 
 
 class QCCard(WrappedBaseModel):
     brand: str
     expiration: str
     last4: str
 
@@ -401,15 +410,15 @@
         # For now, simple checks for an equity "Security Master" subscription
         # Issue created here: https://github.com/QuantConnect/lean-cli/issues/73
 
         data_products_product = next((x for x in self.products if x.name == "Data"), None)
         if data_products_product is None:
             return False
 
-        return any(x.productId in {EQUITY_SECURITY_MASTER_PRODUCT_ID, BULK_EQUITY_SECURITY_MASTER_PRODUCT_ID} for x in data_products_product.items)
+        return any(x.productId in {EQUITY_SECURITY_MASTER_PRODUCT_ID} for x in data_products_product.items)
 
 
 class QCMinimalOrganization(WrappedBaseModel):
     id: str
     name: str
     type: str
     ownerName: str
@@ -499,16 +508,17 @@
     regex: Any
 
     # Price in QCC
     price: Optional[float]
 
     @validator("regex", pre=True)
     def parse_regex(cls, value: Any) -> Any:
+        from re import compile
         if isinstance(value, str):
-            return re.compile(value[value.index("/") + 1:value.rindex("/")])
+            return compile(value[value.index("/") + 1:value.rindex("/")])
         return value
 
 
 class QCDataInformation(WrappedBaseModel):
     datasources: Dict[str, Any]
     prices: List[QCDataVendor]
     agreement: str
@@ -546,7 +556,15 @@
     content: str
     image: str
     link: str
     year_deleted: Optional[Any]
     week_deleted: Optional[Any]
     created: datetime
     date: datetime
+
+
+class QCLeanEnvironment(WrappedBaseModel):
+    id: int
+    name: str
+    path: Optional[str]
+    description: str
+    public: bool
```

### Comparing `lean-1.0.99/lean/models/docker.py` & `lean-1.155/lean/models/docker.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/models/modules.py` & `lean-1.155/lean/models/modules.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,19 +7,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import re
 
 from lean.models.pydantic import WrappedBaseModel
 
-
 class NuGetPackage(WrappedBaseModel):
     name: str
     version: str
 
     def get_file_name(self) -> str:
         """Returns the file name of the package.
 
@@ -30,11 +28,12 @@
     @classmethod
     def parse(cls, file_name: str) -> 'NuGetPackage':
         """Parses a file name into a NuGetPackage instance.
 
         :param file_name: the file name of the NuGet package
         :return: the NuGetPackage instance containing the name and version of the package with the given file name
         """
-        name = re.search(r"([^\d]+)\.\d", file_name).group(1)
+        from re import search
+        name = search(r"([^\d]+)\.\d", file_name).group(1)
         version = file_name.replace(f"{name}.", "").replace(".nupkg", "")
 
         return NuGetPackage(name=name, version=version)
```

### Comparing `lean-1.0.99/lean/models/data.py` & `lean-1.155/lean/models/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import abc
-import multiprocessing
-import re
+from abc import ABC
 from datetime import datetime
 from enum import Enum
 from typing import List, Any, Optional, Dict, Set, Tuple, Pattern
 
-import click
-from dateutil.rrule import rrule, DAILY
-from joblib import Parallel, delayed
+from click import prompt
 from pydantic import validator
 
 from lean.click import DateParameter
 from lean.container import container
 from lean.models.api import QCDataVendor
 from lean.models.logger import Option
 from lean.models.pydantic import WrappedBaseModel
@@ -32,15 +28,15 @@
 
 class OptionResult(WrappedBaseModel):
     """The OptionResult class represents an option's result with an internal value and a display-friendly label."""
     value: Any
     label: str
 
 
-class DatasetCondition(WrappedBaseModel, abc.ABC):
+class DatasetCondition(WrappedBaseModel, ABC):
     def check(self, option_results: Dict[str, OptionResult]) -> bool:
         """Evaluates the condition against a set of options.
 
         If there is not enough information because of missing options the condition evaluates to True.
 
         :param option_results: the option id -> option result dictionary to evaluate against
         :return: False if the condition definitely
@@ -55,37 +51,40 @@
     def check(self, option_results: Dict[str, OptionResult]) -> bool:
         if self.option not in option_results:
             return True
         # TODO: bug? ^ returns true even if option hasn't been resolved
 
         return option_results[self.option].value in self.values
 
+
 class DatasetOrCondition(DatasetCondition):
     options: List[DatasetCondition]
 
     def check(self, option_results: Dict[str, OptionResult]) -> bool:
         # Check each option, if any return true then its true
         for option in self.options:
             if option.check(option_results):
                 return True
-        
+
         return False
 
+
 class DatasetAndCondition(DatasetCondition):
     options: List[DatasetCondition]
 
     def check(self, option_results: Dict[str, OptionResult]) -> bool:
         # Check each option, if any return false, then its false
         for option in self.options:
             if not option.check(option_results):
                 return False
 
         return True
 
-class DatasetOption(WrappedBaseModel, abc.ABC):
+
+class DatasetOption(WrappedBaseModel, ABC):
     id: str
     label: str
     description: str
     condition: Optional[DatasetCondition] = None
 
     @validator("condition", pre=True)
     def parse_condition(cls, value: Optional[Any]) -> Any:
@@ -147,19 +146,19 @@
 
 
 class DatasetTextOption(DatasetOption):
     transform: DatasetTextOptionTransform
     multiple: bool = False
 
     def configure_interactive(self) -> OptionResult:
-        prompt = self.label
+        prompt_to_show = self.label
         if self.multiple:
-            prompt += " (comma-separated)"
+            prompt_to_show += " (comma-separated)"
 
-        user_input = click.prompt(prompt)
+        user_input = prompt(prompt_to_show)
         return self.configure_non_interactive(user_input)
 
     def configure_non_interactive(self, user_input: str) -> OptionResult:
         if len(user_input.strip()) == 0:
             raise ValueError("Value cannot be a blank string")
 
         if self.multiple:
@@ -179,23 +178,23 @@
             return "value"
 
 
 class DatasetSelectOption(DatasetOption):
     choices: Dict[str, str]
 
     def configure_interactive(self) -> OptionResult:
-        logger = container.logger()
+        logger = container.logger
 
         keys = list(self.choices.keys())
 
         if len(keys) <= 5:
             key = logger.prompt_list(self.label, [Option(id=key, label=key) for key in keys])
         else:
             while True:
-                user_input = click.prompt(f"{self.label} (example: {min(keys, key=len)})")
+                user_input = prompt(f"{self.label} (example: {min(keys, key=len)})")
 
                 key = next((key for key in keys if key.lower() == user_input.lower()), None)
                 if key is not None:
                     break
 
                 logger.info(f"Error: '{user_input}' is not a valid option")
 
@@ -221,19 +220,20 @@
         keys = list(self.choices.keys())
 
         if len(keys) <= 5:
             return "|".join(keys)
         else:
             return f"value (example: {min(keys, key=len)})"
 
+
 class DatasetDateOption(DatasetOption):
     start_end: bool = False
 
     def configure_interactive(self) -> OptionResult:
-        date = click.prompt(f"{self.label} (yyyyMMdd)", type=DateParameter())
+        date = prompt(f"{self.label} (yyyyMMdd)", type=DateParameter())
         return OptionResult(value=date, label=date.strftime("%Y-%m-%d"))
 
     def configure_non_interactive(self, user_input: str) -> OptionResult:
         for date_format in ["%Y%m%d", "%Y-%m-%d"]:
             try:
                 date = datetime.strptime(user_input, date_format)
                 return OptionResult(value=date, label=date.strftime("%Y-%m-%d"))
@@ -333,15 +333,15 @@
 
 
 class DataFile(WrappedBaseModel):
     file: str
     vendor: QCDataVendor
 
 
-class DataFileGroup(WrappedBaseModel, abc.ABC):
+class DataFileGroup(WrappedBaseModel, ABC):
     prefix: str
 
     def get_valid_files(self, files_with_prefix: Optional[List[str]]) -> Set[str]:
         raise NotImplementedError()
 
 
 class DataFileAllGroup(DataFileGroup):
@@ -371,14 +371,17 @@
     option_results: Dict[str, OptionResult]
 
     def get_data_files(self) -> List[str]:
         """Returns all data files for the given product configuration.
 
         :return: the list of files that need to be downloaded for this product
         """
+        from multiprocessing import cpu_count
+        from joblib import Parallel, delayed
+
         groups = []
         variables = {option_id: result.value for option_id, result in self.option_results.items()}
 
         multiple_option = next((o for o in self.dataset.options if isinstance(o, DatasetTextOption) and o.multiple),
                                None)
         if multiple_option is not None and multiple_option.id in self.option_results:
             result = self.option_results[multiple_option.id]
@@ -390,25 +393,28 @@
                 }))
         else:
             groups.extend(self._get_data_file_groups(variables))
 
         prefixes = set(group.prefix for group in groups)
         prefixes_to_files = {}
 
-        parallel = Parallel(n_jobs=max(1, multiprocessing.cpu_count() - 1), backend="threading")
+        parallel = Parallel(n_jobs=max(1, cpu_count() - 1), backend="threading")
         for prefix, files_with_prefix in parallel(delayed(self._list_files)(prefix) for prefix in prefixes):
             prefixes_to_files[prefix] = files_with_prefix
 
         data_files = set()
         for group in groups:
             data_files.update(group.get_valid_files(prefixes_to_files[group.prefix]))
 
         return sorted(list(data_files))
 
     def _get_data_file_groups(self, variables: Dict[str, Any]) -> List[DataFileGroup]:
+        from dateutil.rrule import rrule, DAILY
+        from re import split, compile
+
         groups = []
 
         for path in self.dataset.paths:
             if path.condition is None or path.condition.check(self.option_results):
                 path_to_use = path
                 break
         else:
@@ -435,27 +441,27 @@
             prefix = self._get_common_prefix(list(possible_files))
 
             groups.append(DataFileAllGroup(prefix=prefix, possible_files=possible_files))
 
         for regex_template in path_to_use.templates.latest:
             rendered_regex = self._render_template(regex_template, variables)
 
-            prefix = re.split(r"[\\[\]()]", rendered_regex)[0]
-            compiled_regex = re.compile(rendered_regex)
+            prefix = split(r"[\\[\]()]", rendered_regex)[0]
+            compiled_regex = compile(rendered_regex)
 
             groups.append(DataFileLatestGroup(prefix=prefix, regex=compiled_regex))
 
         return groups
 
     def _list_files(self, prefix: str) -> Tuple[str, Optional[List[str]]]:
         if len(prefix.split("/")) < 3:
             # Cannot get cloud directory listing less than 3 levels deep
             return prefix, None
         else:
-            return prefix, container.api_client().data.list_files(prefix)
+            return prefix, container.api_client.data.list_files(prefix)
 
     def _get_common_prefix(self, values: List[str]) -> str:
         """Finds the common prefix in a list of strings.
 
         :param values: the strings to find the common prefix of
         :return: the common prefix of the given strings
         """
```

### Comparing `lean-1.0.99/lean/models/optimizer.py` & `lean-1.155/lean/models/optimizer.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/models/errors.py` & `lean-1.155/lean/models/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,21 +9,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Optional
 
-import requests
-
 
 class RequestFailedError(Exception):
     """A RequestFailedError indicates that an HTTP request has failed."""
 
-    def __init__(self, response: requests.Response, message: Optional[str] = None) -> None:
+    def __init__(self, response, message: Optional[str] = None) -> None:
         """Creates a new RequestFailedError instance.
 
         :param response: the data of the failed response
         :param message: a display-friendly error message, defaults to a message based on the response
         """
         if message is None:
             request = response.request
@@ -50,8 +48,8 @@
 
 class AuthenticationError(MoreInfoError):
     """An error indicating that a request has failed because the used credentials were invalid."""
 
     def __init__(self) -> None:
         """Creates a new AuthenticationError instance."""
         super().__init__("Invalid credentials, please log in using `lean login`",
-                         "https://www.lean.io/docs/lean-cli/initialization/authenticating-accounts#02-Log-In")
+                         "https://www.lean.io/docs/v2/lean-cli/initialization/authenticating-accounts#02-Log-In")
```

### Comparing `lean-1.0.99/lean/models/json_module.py` & `lean-1.155/lean/models/json_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,51 +7,53 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from enum import Enum
 from typing import Any, Dict, List, Type
 from lean.components.util.logger import Logger
-from lean.container import container
-from lean.models.logger import Option
 from lean.models.configuration import BrokerageEnvConfiguration, Configuration, InternalInputUserInput
-import copy
-import abc
+from copy import copy
+from abc import ABC
 
 
-class JsonModule(abc.ABC):
+class JsonModule(ABC):
     """The JsonModule class is the base class extended for all json modules."""
 
     def __init__(self, json_module_data: Dict[str, Any]) -> None:
         self._type: List[str] = json_module_data["type"]
         self._product_id: int = json_module_data["product-id"]
         self._id: str = json_module_data["id"]
         self._display_name: str = json_module_data["display-id"]
         self._installs: bool = json_module_data["installs"]
         self._lean_configs: List[Configuration] = []
         for config in json_module_data["configurations"]:
             self._lean_configs.append(Configuration.factory(config))
         self._lean_configs = self.sort_configs()
         self._is_module_installed: bool = False
-        self._is_installed_and_build: bool = False
+        self._initial_cash_balance: LiveInitialStateInput = LiveInitialStateInput(json_module_data["live-cash-balance-state"]) \
+            if "live-cash-balance-state" in json_module_data \
+            else None
+        self._initial_holdings: LiveInitialStateInput = LiveInitialStateInput(json_module_data["live-holdings-state"]) \
+            if "live-holdings-state" in json_module_data \
+            else False
+        self._minimum_seat = json_module_data["minimum-seat"] if "minimum-seat" in json_module_data else None
 
     def sort_configs(self) -> List[Configuration]:
         sorted_configs = []
         brokerage_configs = []
-        organization_config = []
         for config in self._lean_configs:
             if isinstance(config, BrokerageEnvConfiguration):
                 brokerage_configs.append(config)
-            elif config.is_type_organization_id:
-                organization_config.append(config)
             else:
                 sorted_configs.append(config)
-        return organization_config + brokerage_configs + sorted_configs
+        return brokerage_configs + sorted_configs
 
     def get_name(self) -> str:
         """Returns the user-friendly name which users can identify this object by.
 
         :return: the user-friendly name to display to users
         """
         return self._display_name
@@ -85,100 +87,107 @@
                         config._is_type_configurations_env and self.check_if_config_passes_filters(
                             config)
                         ] or [None]
         if env_config is not None and target_env in env_config._env_and_values.keys():
             env_config_values = env_config._env_and_values[target_env]
         return env_config_values
 
-    def get_organzation_id(self) -> str:
-        [organization_id] = [
-            config._value for config in self._lean_configs if config.is_type_organization_id]
-        return organization_id
+    def get_config_from_type(self, config_type: Configuration) -> str:
+        return [copy(config) for config in self._lean_configs if type(config) is config_type]
 
     def update_value_for_given_config(self, target_name: str, value: Any) -> None:
         [idx] = [i for i in range(len(self._lean_configs))
                  if self._lean_configs[i]._id == target_name]
         self._lean_configs[idx]._value = value
 
     def get_config_value_from_name(self, target_name: str) -> str:
         [idx] = [i for i in range(len(self._lean_configs))
                  if self._lean_configs[i]._id == target_name]
         return self._lean_configs[idx]._value
 
-    def get_non_user_required_properties(self) -> List[Configuration]:
+    def get_non_user_required_properties(self) -> List[str]:
         return [config._id for config in self._lean_configs if not config._is_required_from_user and not
                 config._is_type_configurations_env and self.check_if_config_passes_filters(config)]
 
     def get_required_properties(self, filters: List[Type[Configuration]] = []) -> List[str]:
         return [config._id for config in self.get_required_configs(filters)]
 
     def get_required_configs(self, filters: List[Type[Configuration]] = []) -> List[Configuration]:
-        required_configs = [copy.copy(config) for config in self._lean_configs if config._is_required_from_user
+        required_configs = [copy(config) for config in self._lean_configs if config._is_required_from_user
                             and type(config) not in filters
                             and self.check_if_config_passes_filters(config)]
         return required_configs
 
+    def get_persistent_save_properties(self, filters: List[Type[Configuration]] = []) -> List[str]:
+        return [config._id for config in self.get_required_configs(filters) if config._save_persistently_in_lean]
+
     def get_essential_properties(self) -> List[str]:
         return [config._id for config in self.get_essential_configs()]
 
     def get_essential_configs(self) -> List[Configuration]:
-        return [copy.copy(config) for config in self._lean_configs if isinstance(config, BrokerageEnvConfiguration)]
+        return [copy(config) for config in self._lean_configs if isinstance(config, BrokerageEnvConfiguration)]
 
     def get_all_input_configs(self, filters: List[Type[Configuration]] = []) -> List[Configuration]:
-        return [copy.copy(config) for config in self._lean_configs if config._is_required_from_user
+        return [copy(config) for config in self._lean_configs if config._is_required_from_user
                 if type(config) not in filters
                 and self.check_if_config_passes_module_filter(config)]
 
-    def _convert_lean_key_to_variable(self, lean_key: str) -> str:
+    def convert_lean_key_to_variable(self, lean_key: str) -> str:
         """Replaces hyphens with underscore to follow python naming convention.
 
         :param lean_key: string that uses hyphnes as separator. Used in lean config
         """
         return lean_key.replace('-', '_')
 
-    def _convert_variable_to_lean_key(self, variable_key: str) -> str:
+    def convert_variable_to_lean_key(self, variable_key: str) -> str:
         """Replaces underscore with hyphens to follow lean config naming convention.
 
         :param variable_key: string that uses underscore as separator as per python convention.
         """
         return variable_key.replace('_', '-')
 
-    def build(self, lean_config: Dict[str, Any], logger: Logger) -> 'JsonModule':
+    def build(self,
+              lean_config: Dict[str, Any],
+              logger: Logger,
+              properties: Dict[str, Any] = {},
+              hide_input: bool = False) -> 'JsonModule':
         """Builds a new instance of this class, prompting the user for input when necessary.
 
         :param lean_config: the Lean configuration dict to read defaults from
         :param logger: the logger to use
+        :param properties: the properties that passed as options
+        :param hide_input: whether to hide secrets inputs
         :return: a LeanConfigConfigurer instance containing all the details needed to configure the Lean config
         """
-        if self._is_installed_and_build:
-            return self
         logger.info(f'Configure credentials for {self._display_name}')
         for configuration in self._lean_configs:
             if not self.check_if_config_passes_filters(configuration):
                 continue
             if not configuration._is_required_from_user:
                 continue
             if type(configuration) is InternalInputUserInput:
                 continue
+            if self.__class__.__name__ == 'CloudBrokerage' and not configuration._is_cloud_property:
+                continue
             if configuration._log_message is not None:
                 logger.info(configuration._log_message.strip())
-            if configuration.is_type_organization_id:
-                api_client = container.api_client()
-                organizations = api_client.organizations.get_all()
-                options = [Option(id=organization.id, label=organization.name)
-                           for organization in organizations]
-                organization_id = logger.prompt_list(
-                    "Select the organization with the {} module subscription".format(
-                        self.get_name()),
-                    options
-                )
-                user_choice = organization_id
+
+            property_name = self.convert_lean_key_to_variable(configuration._id)
+            # Only ask for user input if the config wasn't given as an option
+            if property_name in properties and properties[property_name]:
+                user_choice = properties[property_name]
             else:
                 default_value = None
                 # TODO: use type(class) equality instead of class name (str)
                 if self.__class__.__name__ != 'CloudBrokerage':
                     default_value = self._get_default(lean_config, configuration._id)
-                user_choice = configuration.AskUserForInput(default_value, logger)
-            self.update_value_for_given_config(
-                configuration._id, user_choice)
+                user_choice = configuration.ask_user_for_input(default_value, logger, hide_input=hide_input)
+
+            self.update_value_for_given_config(configuration._id, user_choice)
 
         return self
+
+
+class LiveInitialStateInput(str, Enum):
+    Required = "required"
+    Optional = "optional"
+    NotSupported = "not-supported"
```

### Comparing `lean-1.0.99/lean/models/market_hours_database.py` & `lean-1.155/lean/models/market_hours_database.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/models/utils.py` & `lean-1.155/lean/models/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,30 +8,41 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from enum import Enum
+from pathlib import Path
+
 from lean.models.pydantic import WrappedBaseModel
 
 class DebuggingMethod(Enum):
     """The debugging methods supported by the CLI."""
     PyCharm = 1
     PTVSD = 2
     VSDBG = 3
     Rider = 4
+    LocalPlatform  = 5
 
     def get_internal_name(self) -> str:
         """Returns the LEAN debugging method that should be used for the current enum member.
 
         :return: a valid LEAN debugging method that should be used for the current enum member
         """
         return {
             DebuggingMethod.PyCharm: "PyCharm",
-            DebuggingMethod.PTVSD: "PTVSD"
+            DebuggingMethod.PTVSD: "PTVSD",
+            DebuggingMethod.LocalPlatform: "DebugPy" # QC -> DebugPy, If its Python it uses DebugPy, if its C# LEAN safely ignores DebugPy
         }.get(self, "LocalCmdline")
 
+
 class CSharpLibrary(WrappedBaseModel):
     """The information of a PackageReference tag in a .csproj file."""
     name: str
-    version: str
+    version: str
+
+
+class LeanLibraryReference(WrappedBaseModel):
+    """The information of a library reference in a project's config.json file"""
+    name: str
+    path: Path
```

### Comparing `lean-1.0.99/lean/main.py` & `lean-1.155/lean/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,22 +7,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import ctypes
-import os
-import platform
-import site
-import sys
-import time
-from pathlib import Path
-
+from platform import system
 
 # Docker's pywin32 dependency on Windows is a common source of issues
 # In a lot of cases you'd have to manually run pywin32's post-install script as admin after pip installing the library
 # This is a hassle, so the CLI attempts to automate this step when it's necessary
 # Additionally, we can also fix the issues for some users by updating os.environ["PATH"]
 # If this works we use this fix instead as it removes the need to request admin permissions
 # This code must run before the Docker package is imported anywhere in the code
@@ -37,107 +30,112 @@
         return False
 
 
 def _ensure_win32_available() -> None:
     if _is_win32_available():
         return
 
-    possible_paths = sys.path + [sys.prefix] + site.getsitepackages() + [site.getusersitepackages()]
+    from site import getsitepackages, getusersitepackages
+    from sys import executable, path, exit, prefix
+    from os import environ
+    from pathlib import Path
+
+    possible_paths = path + [prefix] + getsitepackages() + [getusersitepackages()]
     possible_paths = [Path(p) for p in possible_paths]
     possible_directories = set(p for p in possible_paths if p.is_dir())
 
     for directory in possible_directories:
         target_directory = directory / "pywin32_system32"
         if not target_directory.is_dir():
             continue
 
-        os.environ["PATH"] += ";" + str(target_directory)
+        environ["PATH"] += ";" + str(target_directory)
 
         if _is_win32_available():
             return
 
     for directory in possible_directories:
         target_file = directory / "Scripts" / "pywin32_postinstall.py"
         if not target_file.is_file():
             continue
 
+        from ctypes import windll
         print(f"Running pywin32's post-install script at {target_file}")
-        ctypes.windll.shell32.ShellExecuteW(None, "runas", sys.executable, f'"{target_file}" -install', None, 1)
+        windll.shell32.ShellExecuteW(None, "runas", executable, f'"{target_file}" -install', None, 1)
 
         # ShellExecuteW returns immediately after the UAC dialog, we wait a second to give the script some time to run
-        time.sleep(1)
+        from time import sleep
+        sleep(1)
 
         if _is_win32_available():
             return
 
-    if any("AppData\\Local\\Packages\\PythonSoftwareFoundation.Python" in p for p in sys.path):
+    if any("AppData\\Local\\Packages\\PythonSoftwareFoundation.Python" in p for p in path):
         print("It looks like you're using the Python distribution from the Microsoft Store")
         print("This distribution is not supported by the CLI, we recommend using the Anaconda distribution instead")
         print(
-            "See https://www.lean.io/docs/lean-cli/installation/installing-pip#02-Install-on-Windows for more information")
-        sys.exit(1)
+            "See https://www.lean.io/docs/v2/lean-cli/installation/installing-pip#02-Install-on-Windows for more information")
+        exit(1)
 
     print("pywin32 has not been installed completely, which may lead to errors")
     print("You can fix this issue by running pywin32's post-install script")
     print(f"Run the following command in an elevated terminal from your Python environment's Scripts directory:")
     print("python pywin32_postinstall.py -install")
 
-
-if platform.system() == "Windows":
+if system() == "Windows":
     _ensure_win32_available()
 
-import traceback
-from io import StringIO
-
-import click
-import requests
-from pydantic import ValidationError
-
 from lean.commands import lean
 from lean.container import container
-from lean.models.errors import MoreInfoError
 
 
 def main() -> None:
     """This function is the entrypoint when running a Lean command in a terminal."""
     try:
         lean.main(standalone_mode=False)
 
-        temp_manager = container.temp_manager()
+        temp_manager = container.temp_manager
         if temp_manager.delete_temporary_directories_when_done:
             temp_manager.delete_temporary_directories()
     except Exception as exception:
-        logger = container.logger()
-        logger.debug(traceback.format_exc().strip())
+        from traceback import format_exc, print_exc
+        from click import UsageError, Abort
+        from requests import exceptions
+        from io import StringIO
+        from pydantic import ValidationError
+        from lean.models.errors import MoreInfoError
+
+        logger = container.logger
+        logger.debug(format_exc().strip())
 
         if isinstance(exception, ValidationError) and hasattr(exception, "input_value"):
             logger.debug("Value that failed validation:")
             logger.debug(exception.input_value)
             logger.error(f"Error: {exception}")
         elif isinstance(exception, MoreInfoError):
             logger.error(f"Error: {exception}")
             logger.error(f"Visit {exception.link} for more information")
-        elif isinstance(exception, click.UsageError):
+        elif isinstance(exception, UsageError):
             io = StringIO()
             exception.show(file=io)
 
             exception_str = io.getvalue().strip()
             exception_str = exception_str.replace("Try 'lean", "\nTry 'lean")
             exception_str = exception_str.replace("for help.",
-                                                  "for help or go to the following url for a list of common errors:\nhttps://www.lean.io/docs/lean-cli/key-concepts/troubleshooting#02-Common-Errors")
+                                                  "for help or go to the following url for a list of common errors:\nhttps://www.lean.io/docs/v2/lean-cli/key-concepts/troubleshooting#02-Common-Errors")
 
-            container.update_manager().warn_if_cli_outdated(force=True)
+            container.update_manager.warn_if_cli_outdated(force=True)
 
             logger.info(exception_str)
-        elif isinstance(exception, click.Abort):
+        elif isinstance(exception, Abort):
             logger.info("Aborted!")
-        elif isinstance(exception, requests.exceptions.ConnectionError):
+        elif isinstance(exception, exceptions.ConnectionError):
             logger.error(f"Error: {exception}")
             logger.error("It looks like you don't have an internet connection, please check your system settings")
         else:
             logger.error(f"Error: {exception}")
 
-        temp_manager = container.temp_manager()
+        temp_manager = container.temp_manager
         if temp_manager.delete_temporary_directories_when_done:
             temp_manager.delete_temporary_directories()
 
-        sys.exit(1)
+        exit(1)
```

### Comparing `lean-1.0.99/lean/__init__.py` & `lean-1.155/lean/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # The version is always set to "dev" in the Git repository. When a new release is ready,
 # a maintainer will push a new Git tag which will trigger GitHub Actions to publish a new
 # package to PyPI with the version of the tag.
-__version__ = "1.0.99"
+__version__ = "1.0155"
```

### Comparing `lean-1.0.99/lean/ssh/key` & `lean-1.155/lean/ssh/key`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/components/api/market_client.py` & `lean-1.155/lean/components/api/market_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/components/api/service_client.py` & `lean-1.155/lean/components/api/service_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/components/api/backtest_client.py` & `lean-1.155/lean/components/api/backtest_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,19 +57,20 @@
         """Creates a new backtest.
 
         :param project_id: the id of the project to create a backtest for
         :param compile_id: the id of a compilation of the given project
         :param name: the name of the new backtest
         :return: the created backtest
         """
+        from lean import __version__
         data = self._api.post("backtests/create", {
             "projectId": project_id,
             "compileId": compile_id,
             "backtestName": name,
-            "requestSource": f"CLI {lean.__version__}"
+            "requestSource": f"CLI {__version__}"
         })
 
         return QCBacktest(**data["backtest"])
 
     def get_report(self, project_id: int, backtest_id: str) -> QCBacktestReport:
         """Returns the report of a backtest.
```

### Comparing `lean-1.0.99/lean/components/api/api_client.py` & `lean-1.155/lean/components/api/api_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,28 +7,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import traceback
-from hashlib import sha256
-from time import time
 from typing import Any, Dict
-from urllib.parse import urljoin
 
-import requests
-
-import lean
 from lean.components.api.account_client import AccountClient
 from lean.components.api.backtest_client import BacktestClient
 from lean.components.api.compile_client import CompileClient
 from lean.components.api.data_client import DataClient
 from lean.components.api.file_client import FileClient
+from lean.components.api.lean_client import LeanClient
 from lean.components.api.live_client import LiveClient
 from lean.components.api.market_client import MarketClient
 from lean.components.api.module_client import ModuleClient
 from lean.components.api.node_client import NodeClient
 from lean.components.api.optimization_client import OptimizationClient
 from lean.components.api.organization_client import OrganizationClient
 from lean.components.api.project_client import ProjectClient
@@ -49,16 +43,15 @@
         :param logger: the logger to use to print debug messages to
         :param http_client: the HTTP client to make HTTP requests with
         :param user_id: the QuantConnect user id to use when sending authenticated requests
         :param api_token: the QuantConnect API token to use when sending authenticated requests
         """
         self._logger = logger
         self._http_client = http_client
-        self._user_id = user_id
-        self._api_token = api_token
+        self.set_user_token(user_id, api_token)
 
         # Create the clients containing the methods to send requests to the various API endpoints
         self.accounts = AccountClient(self)
         self.backtests = BacktestClient(self)
         self.compiles = CompileClient(self)
         self.data = DataClient(self, http_client)
         self.files = FileClient(self)
@@ -67,14 +60,19 @@
         self.modules = ModuleClient(self)
         self.nodes = NodeClient(self)
         self.optimizations = OptimizationClient(self)
         self.organizations = OrganizationClient(self)
         self.projects = ProjectClient(self)
         self.services = ServiceClient(self)
         self.users = UserClient(self)
+        self.lean = LeanClient(self)
+
+    def set_user_token(self, user_id: str, api_token: str):
+        self._user_id = user_id
+        self._api_token = api_token
 
     def get(self, endpoint: str, parameters: Dict[str, Any] = {}) -> Any:
         """Makes an authenticated GET request to the given endpoint with the given parameters.
 
         Raises an error if the request fails or if the current credentials are invalid.
 
         :param endpoint: the API endpoint to send the request to
@@ -101,60 +99,69 @@
 
         :return: True if the current credentials are valid, False if not
         """
         try:
             self.get("authenticate")
             return True
         except (RequestFailedError, AuthenticationError):
-            self._logger.debug(traceback.format_exc().strip())
+            from traceback import format_exc
+            self._logger.debug(format_exc().strip())
             return False
 
     def _request(self, method: str, endpoint: str, options: Dict[str, Any] = {}, retry_http_5xx: bool = True) -> Any:
         """Makes an authenticated request to the given endpoint.
 
         :param method: the HTTP method to use for the request
         :param endpoint: the API endpoint to send the request to
         :param options: additional options to pass on to requests.request()
         :param retry_http_5xx: True if the request should be retried on an HTTP 5xx response, False if not
         :return: the parsed response of the request
         """
+        from hashlib import sha256
+        from urllib.parse import urljoin
+        from lean import __version__
+        from time import time
+
         full_url = urljoin(API_BASE_URL, endpoint)
 
         # Create the hash which is used to authenticate the user to the API
         timestamp = str(int(time()))
         password = sha256(f"{self._api_token}:{timestamp}".encode("utf-8")).hexdigest()
 
         headers = {
             "Timestamp": timestamp
         }
 
-        version = lean.__version__
-        if lean.__version__ == 'dev':
+        version = __version__
+        if __version__ == 'dev':
             version = 99999999
         headers["User-Agent"] = f"Lean CLI {version}"
 
         response = self._http_client.request(method,
                                              full_url,
                                              headers=headers,
                                              auth=(self._user_id, password),
                                              raise_for_status=False,
                                              **options)
 
+        if self._logger.debug_logging_enabled:
+            self._logger.debug(f"Request response: {response.text}")
+
         if 500 <= response.status_code < 600 and retry_http_5xx:
             return self._request(method, endpoint, options, False)
 
         if response.status_code == 500:
             raise AuthenticationError()
 
         if response.status_code < 200 or response.status_code >= 300:
             raise RequestFailedError(response)
 
         return self._parse_response(response)
 
-    def _parse_response(self, response: requests.Response) -> Any:
+    def _parse_response(self, response) -> Any:
         """Parses the data in a response.
 
         Raises an error if the data in the response indicates something went wrong.
 
         :param response: the response of the request
         :return: the data in the response
         """
@@ -164,15 +171,17 @@
             return data
 
         self._http_client.log_unsuccessful_response(response)
 
         if "errors" in data and len(data["errors"]) > 0:
             if data["errors"][0].startswith("Hash doesn't match."):
                 raise AuthenticationError()
-
+            if data["errors"][0].startswith('UserID not valid'):
+                data["errors"].append('Please login to your account with "lean login". '
+                                      'https://www.quantconnect.com/docs/v2/lean-cli/api-reference/lean-login')
             raise RequestFailedError(response, "\n".join(data["errors"]))
 
         if "messages" in data and len(data["messages"]) > 0:
             raise RequestFailedError(response, "\n".join(data["messages"]))
 
         if "Message" in data:
             raise RequestFailedError(response, data["Message"])
```

### Comparing `lean-1.0.99/lean/components/api/file_client.py` & `lean-1.155/lean/components/api/file_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/components/api/module_client.py` & `lean-1.155/lean/components/api/module_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/components/api/project_client.py` & `lean-1.155/lean/components/api/project_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,93 +10,133 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List, Optional
 
 from lean.components.api.api_client import *
-from lean.models.api import QCCreatedProject, QCLanguage, QCProject
+from lean.models.api import QCLanguage, QCProject
 
 
 class ProjectClient:
     """The ProjectClient class contains methods to interact with projects/* API endpoints."""
 
     def __init__(self, api_client: 'APIClient') -> None:
         """Creates a new ProjectClient instance.
 
         :param api_client: the APIClient instance to use when making requests
         """
         self._api = api_client
 
-    def get(self, project_id: int) -> QCProject:
+    def get(self, project_id: int, organization_id: Optional[str]) -> QCProject:
         """Returns the details of a project.
 
         :param project_id: the id of the project to retrieve the details of
+        :param organization_id: the id of the organization where the project is located
         :return: the details of the specified project
         """
-        data = self._api.get("projects/read", {
-            "projectId": project_id
-        })
+        payload = {"projectId": project_id}
+        if organization_id is not None:
+            payload["organizationId"] = organization_id
+
+        data = self._api.get("projects/read", payload)
 
         return self._process_project(QCProject(**data["projects"][0]))
 
-    def get_all(self) -> List[QCProject]:
+    def get_all(self, organization_id: Optional[str]) -> List[QCProject]:
         """Returns all the projects the user has access to.
 
         :return: a list containing all the projects the user has access to
+        :param organization_id: the id of the organization where the projects are located
         """
-        data = self._api.get("projects/read")
+        payload = {}
+        if organization_id is not None:
+            payload["organizationId"] = organization_id
+
+        data = self._api.get("projects/read", payload)
+
         return [self._process_project(QCProject(**project)) for project in data["projects"]]
 
-    def create(self, name: str, language: QCLanguage) -> QCCreatedProject:
+    def create(self, name: str, language: QCLanguage, organization_id: Optional[str]) -> QCProject:
         """Creates a new project.
 
         :param name: the name of the project to create
         :param language: the language of the project to create
+        :param organization_id: the id of the organization to create the project in
         :return: the created project
         """
-        data = self._api.post("projects/create", {
+        parameters = {
             "name": name,
             "language": language.value
-        })
+        }
+        if organization_id is not None:
+            parameters["organizationId"] = organization_id
+        data = self._api.post("projects/create", parameters)
 
-        return self._process_project(QCCreatedProject(**data["projects"][0]))
+        return self._process_project(QCProject(**data["projects"][0]))
 
     def update(self,
                project_id: int,
                name: Optional[str] = None,
                description: Optional[str] = None,
-               parameters: Optional[Dict[str, str]] = None) -> None:
+               parameters: Optional[Dict[str, str]] = None,
+               lean_engine: Optional[int] = None,
+               python_venv: Optional[int] = None,
+               files: Optional[List[Dict[str, str]]] = None,
+               libraries: Optional[List[int]] = None) -> None:
         """Updates an existing project.
 
         :param project_id: the id of the project to update
         :param name: the new name to assign to the project, or None if the name shouldn't be changed
         :param description: the new description to assign to the project, or None if the description shouldn't be changed
         :param parameters: the new parameters of the project, or None if the parameters shouldn't be changed
+        :param lean_engine: the lean engine id for the project, or None if the lean engine shouldn't be changed
+        :param python_venv: the python venv id for the project, or None if the python venv shouldn't be changed
+        :param files: the list of files for the project
+        :param libraries: the list of libraries referenced by the project
         """
         request_parameters = {
             "projectId": project_id
         }
 
         if name is not None:
             request_parameters["name"] = name
 
         if description is not None:
             request_parameters["description"] = description
 
         if parameters is not None:
             if len(parameters) > 0:
-                index = 0
-                for key, value in parameters.items():
+                for index, (key, value) in enumerate(parameters.items()):
                     request_parameters[f"parameters[{index}][key]"] = key
                     request_parameters[f"parameters[{index}][value]"] = value
-                    index += 1
             else:
                 request_parameters["parameters"] = ""
 
+        if lean_engine is not None:
+            request_parameters["versionId"] = lean_engine
+
+        if python_venv is not None:
+            request_parameters["leanEnvironment"] = python_venv
+
+        if files is not None:
+            if len(files) > 0:
+                for index, file in enumerate(files):
+                    request_parameters[f"files[{index}][name]"] = file["name"]
+                    request_parameters[f"files[{index}][content]"] = file["content"]
+            else:
+                request_parameters["files"] = []
+
+        if libraries is not None:
+            if len(libraries) > 0:
+                for index, library in enumerate(libraries):
+                    request_parameters[f"libraries[{index}]"] = library
+            else:
+                request_parameters["libraries"] = []
+
         self._api.post("projects/update", request_parameters, data_as_json=False)
 
     def delete(self, project_id: int) -> None:
         """Deletes an existing project.
 
         :param project_id: the id of the project to delete
         """
```

### Comparing `lean-1.0.99/lean/components/api/user_client.py` & `lean-1.155/lean/components/api/user_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/components/api/account_client.py` & `lean-1.155/lean/components/api/account_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/components/api/__init__.py` & `lean-1.155/lean/components/config/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/components/api/organization_client.py` & `lean-1.155/lean/components/api/organization_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/components/api/node_client.py` & `lean-1.155/lean/components/api/node_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/components/api/data_client.py` & `lean-1.155/lean/components/api/data_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
-from shutil import move
-from tempfile import NamedTemporaryFile
 from lean.components.api.api_client import *
 from lean.models.api import QCDataInformation
 from typing import List, Callable
 
 
 class DataClient:
     """The DataClient class contains methods to interact with data/* API endpoints."""
@@ -38,14 +35,18 @@
         """Downloads the content of a downloadable data file.
 
         :param relative_file_path: the relative path of the data file
         :param organization_id: the id of the organization that should be billed
         :param local_filename: the final local path where the data file will be stored
         :param progress_callback: the download progress callback
         """
+        from tempfile import NamedTemporaryFile
+        from shutil import move
+        from os import path, makedirs
+
         data = self._api.post("data/read", {
             "format": "link",
             "filePath": relative_file_path,
             "organizationId": organization_id
         })
 
         # we stream the data into a temporary file and later move it to it's final location
@@ -68,16 +69,16 @@
                     if total_size != 0:
                         # progressive progress update if we can
                         progress_callback((current_size / total_size) - previous)
             if total_size == 0:
                 # if total size not available update progress at the end
                 progress_callback(1)
 
-            directory = os.path.dirname(local_filename)
-            os.makedirs(directory, exist_ok=True)
+            directory = path.dirname(local_filename)
+            makedirs(directory, exist_ok=True)
             move(temp_file_name, local_filename)
 
     def download_public_file(self, data_endpoint: str) -> bytes:
         """Downloads the content of a downloadable public file.
 
         :param data_endpoint: the url of the public file
         :return: the content of the file
```

### Comparing `lean-1.0.99/lean/components/api/optimization_client.py` & `lean-1.155/lean/components/api/optimization_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/components/api/compile_client.py` & `lean-1.155/lean/components/api/compile_client.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/components/api/live_client.py` & `lean-1.155/lean/components/api/live_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from datetime import datetime
-from math import floor
 from typing import List, Optional
 
 from lean.components.api.api_client import *
 from lean.models.api import QCFullLiveAlgorithm, QCLiveAlgorithmStatus, QCMinimalLiveAlgorithm, QCNotificationMethod, QCRestResponse
 
 
 class LiveClient:
@@ -37,14 +36,15 @@
         """Retrieves all live algorithms.
 
         :param status: the status to filter by or None if no status filter should be applied
         :param start: the earliest launch time the returned algorithms should have
         :param end: the latest launch time the returned algorithms should have
         :return: a list of live algorithms which match the given filters
         """
+        from math import floor
         parameters = {
             "start": floor(start.timestamp()),
             "end": floor(end.timestamp())
         }
 
         if status is not None:
             parameters["status"] = status.value
@@ -52,36 +52,45 @@
         data = self._api.get("live/read", parameters)
         return [QCFullLiveAlgorithm(**algorithm) for algorithm in data["live"]]
 
     def start(self,
               project_id: int,
               compile_id: str,
               node_id: str,
-              brokerage_settings: Dict[str, str],
+              brokerage_settings: Dict[str, Any],
               price_data_handler: str,
               automatic_redeploy: bool,
               version_id: int,
               notify_order_events: bool,
               notify_insights: bool,
-              notify_methods: List[QCNotificationMethod]) -> QCMinimalLiveAlgorithm:
+              notify_methods: List[QCNotificationMethod],
+              live_cash_balance: Optional[List[Dict[str, float]]] = None,
+              live_holdings: Optional[List[Dict[str, float]]] = None) -> QCMinimalLiveAlgorithm:
         """Starts live trading for a project.
 
         :param project_id: the id of the project to start live trading for
         :param compile_id: the id of the compile to use for live trading
         :param node_id: the id of the node to start live trading on
         :param brokerage_settings: the brokerage settings to use
         :param price_data_handler: the data feed to use
         :param automatic_redeploy: whether automatic redeploys are enabled
         :param version_id: the id of the LEAN version to use
         :param notify_order_events: whether notifications should be sent on order events
         :param notify_insights: whether notifications should be sent on insights
         :param notify_methods: the places to send notifications to
+        :param live_cash_balance: the list of initial cash balance
+        :param live_holdings: the list of initial portfolio holdings
         :return: the created live algorithm
         """
 
+        if live_cash_balance:
+            brokerage_settings["cash"] = live_cash_balance
+        if live_holdings:
+            brokerage_settings["holdings"] = live_holdings
+
         parameters = {
             "projectId": project_id,
             "compileId": compile_id,
             "nodeId": node_id,
             "brokerage": brokerage_settings,
             "dataHandler": price_data_handler,
             "automaticRedeploy": automatic_redeploy,
@@ -93,15 +102,15 @@
             if notify_order_events:
                 events.append("orderEvent")
             if notify_insights:
                 events.append("insight")
 
             parameters["notification"] = {
                 "events": events,
-                "targets": [method.dict() for method in notify_methods]
+                "targets": [{x: y for x, y in method.dict().items() if y} for method in notify_methods]
             }
 
         data = self._api.post("live/create", parameters)
         return QCMinimalLiveAlgorithm(**data)
 
     def stop(self, project_id: int) -> QCRestResponse:
         """Stops live trading for a certain project without liquidated existing positions.
@@ -117,8 +126,8 @@
         """Stops live trading and liquidates existing positions for a certain project.
 
         :param project_id: the id of the project to stop live trading and liquidate existing positions for
         """
         data = self._api.post("live/update/liquidate", {
             "projectId": project_id
         })
-        return QCRestResponse(**data)
+        return QCRestResponse(**data)
```

### Comparing `lean-1.0.99/lean/components/cloud/pull_manager.py` & `lean-1.155/lean/components/cloud/push_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,186 +7,234 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import traceback
 from pathlib import Path
-from typing import List
+from typing import List, Dict
 
 from lean.components.api.api_client import APIClient
 from lean.components.config.project_config_manager import ProjectConfigManager
 from lean.components.util.logger import Logger
-from lean.components.util.platform_manager import PlatformManager
+from lean.components.util.organization_manager import OrganizationManager
 from lean.components.util.project_manager import ProjectManager
-from lean.models.api import QCProject
+from lean.models.api import QCLanguage, QCProject
+from lean.models.utils import LeanLibraryReference
 
-
-class PullManager:
-    """The PullManager class is responsible for synchronizing cloud projects to the local drive."""
+class PushManager:
+    """The PushManager class is responsible for synchronizing local projects to the cloud."""
 
     def __init__(self,
                  logger: Logger,
                  api_client: APIClient,
                  project_manager: ProjectManager,
                  project_config_manager: ProjectConfigManager,
-                 platform_manager: PlatformManager) -> None:
-        """Creates a new PullManager instance.
+                 organization_manager: OrganizationManager) -> None:
+        """Creates a new PushManager instance.
 
         :param logger: the logger to use when printing messages
         :param api_client: the APIClient instance to use when communicating with the cloud
-        :param project_manager: the ProjectManager instance to use when creating new projects
+        :param project_manager: the ProjectManager to use when looking for certain projects
         :param project_config_manager: the ProjectConfigManager instance to use
-        :param platform_manager: the PlatformManager used when checking which operating system is in use
         """
         self._logger = logger
         self._api_client = api_client
         self._project_manager = project_manager
         self._project_config_manager = project_config_manager
-        self._platform_manager = platform_manager
-        self._last_file = None
+        self._organization_manager = organization_manager
+        self._cloud_projects = []
+
+    def push_project(self, project: Path) -> None:
+        """Pushes the given project from the local drive to the cloud.
+
+        It will also push every library referenced by the project and add or remove references.
+
+        :param project: path to the directory containing the local project that needs to be pushed
+        """
+        libraries = self._project_manager.get_project_libraries(project)
+        self.push_projects(libraries + [project])
+
+    def push_projects(self, projects_to_push: List[Path]) -> None:
+        """Pushes the given projects from the local drive to the cloud.
 
-    def pull_projects(self, projects_to_pull: List[QCProject]) -> None:
-        """Pulls the given projects from the cloud to the local drive.
+        It will also push every library referenced by each project and add or remove references.
 
-        :param projects_to_pull: the cloud projects that need to be pulled
+        :param projects_to_push: a list of directories containing the local projects that need to be pushed
         """
-        projects_to_pull = sorted(projects_to_pull, key=lambda p: p.name)
+        if len(projects_to_push) == 0:
+            return
 
-        for index, project in enumerate(projects_to_pull, start=1):
+        organization_id = self._organization_manager.try_get_working_organization_id()
+
+        for index, path in enumerate(projects_to_push, start=1):
+            relative_path = path.relative_to(Path.cwd())
             try:
-                self._logger.info(f"[{index}/{len(projects_to_pull)}] Pulling '{project.name}'")
-                self._pull_project(project)
+                self._logger.info(f"[{index}/{len(projects_to_push)}] Pushing '{relative_path}'")
+                self._push_project(path, organization_id)
             except Exception as ex:
-                self._logger.debug(traceback.format_exc().strip())
-                if self._last_file is not None:
-                    self._logger.warn(
-                        f"Cannot pull '{project.name}' (id {project.projectId}, failed on {self._last_file}): {ex}")
-                else:
-                    self._logger.warn(f"Cannot pull '{project.name}' (id {project.projectId}): {ex}")
+                from traceback import format_exc
+                self._logger.debug(format_exc().strip())
+                self._logger.warn(f"Cannot push '{relative_path}': {ex}")
 
-    def _pull_project(self, project: QCProject) -> None:
-        """Pulls a single project from the cloud to the local drive.
+    def _get_local_libraries_cloud_ids(self, project_dir: Path) -> List[int]:
+        project_config = self._project_config_manager.get_project_config(project_dir)
 
-        Raises an error with a descriptive message if the project cannot be pulled.
+        libraries_in_config = project_config.get("libraries", [])
+        library_paths = [LeanLibraryReference(**library).path.expanduser().resolve() for library in libraries_in_config]
 
-        :param project: the cloud project to pull
-        """
-        local_project_path = self.get_local_project_path(project)
+        local_libraries_cloud_ids = [int(self._project_config_manager.get_project_config(path).get("cloud-id", None))
+                                     for path in library_paths]
 
-        # Pull the cloud files to the local drive
-        self._pull_files(project, local_project_path)
+        return local_libraries_cloud_ids
 
-        # Update the local project config with the latest details
-        project_config = self._project_config_manager.get_project_config(local_project_path)
-        project_config.set("cloud-id", project.projectId)
-        project_config.set("algorithm-language", project.language.name)
-        project_config.set("parameters", {parameter.key: parameter.value for parameter in project.parameters})
-        project_config.set("description", project.description)
+    def _push_project(self, project_path: Path, organization_id: str, suggested_rename_path: Path = None) -> None:
+        """Pushes a single local project to the cloud.
 
-    def _pull_files(self, project: QCProject, local_project_path: Path) -> None:
-        """Pull the files of a single project.
+        Raises an error with a descriptive message if the project cannot be pushed.
 
-        :param project: the cloud project of which the files need to be pulled
-        :param local_project_path: the path to the local project directory
+        :param project_path: the local project to push
+        :param organization_id: the id of the organization to push the project to
+        :param suggested_rename_path: the path to move the project to.
         """
-        if not local_project_path.exists():
-            self._project_manager.create_new_project(local_project_path, project.language)
+        
+        project_name = project_path.relative_to(Path.cwd()).as_posix()
 
-        for cloud_file in self._api_client.files.get_all(project.projectId):
-            self._last_file = cloud_file.name
+        potential_new_name = project_name
+        if suggested_rename_path and suggested_rename_path != project_path:
+            potential_new_name = suggested_rename_path.relative_to(Path.cwd()).as_posix()
+            
 
-            if cloud_file.isLibrary:
-                continue
+        project_config = self._project_config_manager.get_project_config(project_path)
+        cloud_id = project_config.get("cloud-id")
 
-            local_file_path = local_project_path / cloud_file.name
+        # check if project name is valid or if rename is required
+        if cloud_id is not None:
+            expected_correct_project_path = self._project_manager.get_local_project_path(potential_new_name, cloud_id)
+        else:
+            local_id = self._project_config_manager.get_local_id(project_path)
+            expected_correct_project_path = self._project_manager.get_local_project_path(potential_new_name, None, local_id)
+        if expected_correct_project_path != project_path:
+            # rename project
+            valid_project_name = expected_correct_project_path.relative_to(Path.cwd()).as_posix()
+            self._logger.info(f"Renaming '{project_name}' to '{valid_project_name}'")
+            self._project_manager.rename_project_and_contents(project_path, expected_correct_project_path)
+            project_path = expected_correct_project_path
+            project_name = valid_project_name
+            project_config = self._project_config_manager.get_project_config(project_path)
+
+        # Find the cloud project to push the files to
+        if cloud_id is not None:
+            # Project has cloud id which matches cloud project, update cloud project
+            cloud_project = self._get_cloud_project(cloud_id, organization_id)
+        else:
+            # Project has invalid cloud id or no cloud id at all, create new cloud project
+            cloud_project = self._api_client.projects.create(project_name,
+                                                             QCLanguage[project_config.get("algorithm-language")],
+                                                             organization_id)
+            project_config.set("cloud-id", cloud_project.projectId)
+            project_config.set("organization-id", cloud_project.organizationId)
+
+            if cloud_project.name != project_name:
+                # cloud project name was changed. Repeat steps to validate the new name locally.
+                self._logger.info(f"Received new name '{cloud_project.name}' for project '{project_name}' from QuantConnect.com")
+                self._push_project(project_path, organization_id, Path.cwd() / cloud_project.name)
+                return
+
+            self._cloud_projects.append(cloud_project)
+            organization_message_part = f" in organization '{organization_id}'" if organization_id is not None else ""
+            self._logger.info(f"Successfully created cloud project '{cloud_project.name}'{organization_message_part}")
+
+        # Finalize pushing by updating locally modified metadata, files and libraries
+        self._push_metadata(project_path, cloud_project)
+
+    def _get_files(self, project: Path) -> List[Dict[str, str]]:
+        """Pushes the files of a local project to the cloud.
+
+        :param project: the local project to push the files of
+        """
+        paths = self._project_manager.get_source_files(project)
+        files = []
+
+        for path in paths:
+            relative_path = path.relative_to(project).as_posix()
+            if "bin/" in relative_path and "obj/" in relative_path and ".ipynb_checkpoints/" in relative_path:
+                continue
 
-            # Skip if the local file already exists with the correct content
-            if local_file_path.exists():
-                if local_file_path.read_text(encoding="utf-8").strip() == cloud_file.content.strip():
-                    self._project_manager.update_last_modified_time(local_file_path, cloud_file.modified)
-                    continue
+            files.append({
+                'name': relative_path,
+                'content': path.read_text(encoding="utf-8")
+            })
 
-            local_file_path.parent.mkdir(parents=True, exist_ok=True)
-            with local_file_path.open("w+", encoding="utf-8") as local_file:
-                if cloud_file.content != "" and not cloud_file.content.endswith("\n"):
-                    local_file.write(cloud_file.content + "\n")
-                else:
-                    local_file.write(cloud_file.content)
+        return files
 
-            self._project_manager.update_last_modified_time(local_file_path, cloud_file.modified)
-            self._logger.info(f"Successfully pulled '{project.name}/{cloud_file.name}'")
+    def _push_metadata(self, project: Path, cloud_project: QCProject) -> None:
+        """Pushes local project description and parameters to the cloud.
 
-        self._last_file = None
-        self._project_manager.update_last_modified_time(local_project_path, project.modified)
+        Does nothing if the cloud is already up-to-date.
 
-    def get_local_project_path(self, project: QCProject) -> Path:
-        """Returns the local path where a certain cloud project should be stored.
+        :param project: the local project to push the parameters of
+        :param cloud_project: the cloud project to push the parameters to
+        """
+        project_config = self._project_config_manager.get_project_config(project)
 
-        If two cloud projects are named "Project", they are pulled to ./Project and ./Project 2.
+        local_description = project_config.get("description", "")
+        cloud_description = cloud_project.description
 
-        :param project: the cloud project to get the project path of
-        :return: the path to the local project directory
-        """
-        local_path = self._format_local_path(project.name)
+        local_parameters = project_config.get("parameters", {})
+        cloud_parameters = {parameter.key: parameter.value for parameter in cloud_project.parameters}
 
-        current_index = 1
-        while True:
-            path_suffix = "" if current_index == 1 else f" {current_index}"
-            current_path = Path.cwd() / (local_path + path_suffix)
+        # Use latest (-1) by default
+        local_lean_version = int(project_config.get("lean-engine", "-1"))
+        cloud_lean_version = cloud_project.leanVersionId
 
-            if not current_path.exists():
-                return current_path
+        local_lean_venv = project_config.get("python-venv", None)
+        cloud_lean_venv = cloud_project.leanEnvironment
 
-            current_project_config = self._project_config_manager.get_project_config(current_path)
-            if current_project_config.get("cloud-id") == project.projectId:
-                return current_path
+        update_args = {}
 
-            current_index += 1
+        expected_correct_project_name = project.relative_to(Path.cwd()).as_posix()
 
-    def _format_local_path(self, cloud_path: str) -> str:
-        """Converts the given cloud path into a local path which is valid for the current operating system.
+        # update project name in cloud in case it was incorrect and renamed locally otherwise update the same name
+        update_args["name"] = expected_correct_project_name
+        if cloud_project.name != expected_correct_project_name:
+            self._logger.info(f"Renaming project in cloud from '{cloud_project.name}' to '{expected_correct_project_name}'")
 
-        :param cloud_path: the path of the project in the cloud
-        :return: the converted cloud_path so that it is valid locally
-        """
-        # Remove forbidden characters and OS-specific path separator that are not path separators on QuantConnect
-        if self._platform_manager.is_host_windows():
-            # Windows, \":*?"<>| are forbidden
-            # Windows, \ is a path separator, but \ is not a path separator on QuantConnect
-            forbidden_characters = ["\\", ":", "*", "?", '"', "<", ">", "|"]
-        elif self._platform_manager.is_host_macos():
-            # macOS, : is a path separator, but : is not a path separator on QuantConnect
-            forbidden_characters = [":"]
-        else:
-            # Linux, no forbidden characters
-            forbidden_characters = []
+        if local_description != cloud_description:
+            update_args["description"] = local_description
 
-        for forbidden_character in forbidden_characters:
-            cloud_path = cloud_path.replace(forbidden_character, " ")
+        if local_parameters != cloud_parameters:
+            update_args["parameters"] = local_parameters
 
-        # On Windows we need to ensure each path component is valid
-        if self._platform_manager.is_host_windows():
-            new_components = []
+        if (local_lean_version != cloud_lean_version and
+           (local_lean_version != -1 or not cloud_project.leanPinnedToMaster)):
+            update_args["lean_engine"] = local_lean_version
 
-            for component in cloud_path.split("/"):
-                # Some names are reserved
-                for reserved_name in ["CON", "PRN", "AUX", "NUL",
-                                      "COM1", "COM2", "COM3", "COM4", "COM5", "COM6", "COM7", "COM8", "COM9",
-                                      "LPT1", "LPT2", "LPT3", "LPT4", "LPT5", "LPT6", "LPT7", "LPT8", "LPT9"]:
-                    # If the component is a reserved name, we add an underscore to it so it can be used
-                    if component.upper() == reserved_name:
-                        component += "_"
+        # Initially, python-venv is not defined in the config and the default one will be used.
+        # After it is changed, in order to use the default one again, it must not be removed from the config,
+        # but it should be set to the default env id explicitly instead.
+        if local_lean_venv is not None and local_lean_venv != cloud_lean_venv:
+            update_args["python_venv"] = local_lean_venv
 
-                # Components cannot start or end with a space
-                component = component.strip(" ")
+        update_args["files"] = self._get_files(project)
+        update_args["libraries"] = self._get_local_libraries_cloud_ids(project)
 
-                # Components cannot end with a period
-                component = component.rstrip(".")
+        if update_args != {}:
+            self._api_client.projects.update(cloud_project.projectId, **update_args)
 
-                new_components.append(component)
+            updated_keys = list(update_args)
+            if len(updated_keys) == 1:
+                updated_keys_str = updated_keys[0]
+            elif len(updated_keys) == 2:
+                updated_keys_str = " and ".join(updated_keys)
+            else:
+                updated_keys_str = ", ".join(updated_keys[:-1]) + f", and {updated_keys[-1]}"
+            self._logger.info(f"Successfully updated {updated_keys_str} for '{cloud_project.name}'")
 
-            cloud_path = "/".join(new_components)
+    def _get_cloud_project(self, project_id: int, organization_id: str) -> QCProject:
+        project = next(iter(p for p in self._cloud_projects if p.projectId == project_id), None)
+        if project is None:
+            project = self._api_client.projects.get(project_id, organization_id)
+            self._cloud_projects.append(project)
 
-        return cloud_path
+        return project
```

### Comparing `lean-1.0.99/lean/components/cloud/cloud_runner.py` & `lean-1.155/lean/components/cloud/cloud_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List
 
-import click
+from click import confirm
 
 from lean.components.api.api_client import APIClient
 from lean.components.util.logger import Logger
 from lean.components.util.task_manager import TaskManager
 from lean.models.api import QCBacktest, QCCompileState, QCCompileWithLogs, QCOptimization, QCProject
 from lean.models.errors import RequestFailedError
 from lean.models.optimizer import OptimizationConstraint, OptimizationParameter, OptimizationTarget
@@ -53,15 +53,15 @@
         try:
             return self._task_manager.poll(
                 make_request=lambda: self._api_client.backtests.get(project.projectId, created_backtest.backtestId),
                 is_done=lambda data: data.is_complete(),
                 get_progress=lambda data: data.progress
             )
         except KeyboardInterrupt as e:
-            if click.confirm("Do you want to cancel and delete the running backtest?", True):
+            if confirm("Do you want to cancel and delete the running backtest?", True):
                 self._api_client.backtests.delete(project.projectId, created_backtest.backtestId)
                 self._logger.info(f"Successfully cancelled and deleted backtest '{name}'")
             raise e
 
     def run_optimization(self,
                          project: QCProject,
                          finished_compile: QCCompileWithLogs,
@@ -101,15 +101,15 @@
         try:
             return self._task_manager.poll(
                 make_request=lambda: self._api_client.optimizations.get(created_optimization.optimizationId),
                 is_done=lambda data: data.status != "active" and data.status != "running",
                 get_progress=lambda data: data.get_progress()
             )
         except KeyboardInterrupt as e:
-            if click.confirm("Do you want to cancel and delete the running optimization?", True):
+            if confirm("Do you want to cancel and delete the running optimization?", True):
                 try:
                     self._api_client.optimizations.abort(created_optimization.optimizationId)
                 except RequestFailedError:
                     # The optimization finished between the user pressed Ctrl+C and confirmed the deletion
                     pass
                 finally:
                     self._api_client.optimizations.delete(created_optimization.optimizationId)
```

### Comparing `lean-1.0.99/lean/components/cloud/cloud_project_manager.py` & `lean-1.155/lean/components/cloud/cloud_project_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,81 +13,88 @@
 
 from pathlib import Path
 
 from lean.components.api.api_client import APIClient
 from lean.components.cloud.pull_manager import PullManager
 from lean.components.cloud.push_manager import PushManager
 from lean.components.config.project_config_manager import ProjectConfigManager
+from lean.components.util.organization_manager import OrganizationManager
 from lean.components.util.path_manager import PathManager
+from lean.components.util.project_manager import ProjectManager
 from lean.models.api import QCProject
 
 
 class CloudProjectManager:
     """The CloudProjectManager class is responsible for finding the correct cloud project in cloud commands."""
 
     def __init__(self,
                  api_client: APIClient,
                  project_config_manager: ProjectConfigManager,
                  pull_manager: PullManager,
                  push_manager: PushManager,
-                 path_manager: PathManager) -> None:
+                 path_manager: PathManager,
+                 project_manager: ProjectManager,
+                 organization_manager: OrganizationManager) -> None:
         """Creates a new PullManager instance.
 
         :param api_client: the APIClient instance to use when communicating with the cloud
         :param project_config_manager: the ProjectConfigManager instance to use
         :param pull_manager: the PullManager instance to use
         :param push_manager: the PushManager instance to use
         :param path_manager: the PathManager instance to use when validating paths
+        :param organization_manager: the OrganizationManager instance to use to get the working organization id
         """
         self._api_client = api_client
         self._project_config_manager = project_config_manager
         self._pull_manager = pull_manager
         self._push_manager = push_manager
         self._path_manager = path_manager
+        self._project_manager = project_manager
+        self._organization_manager = organization_manager
 
     def get_cloud_project(self, input: str, push: bool) -> QCProject:
         """Retrieves the cloud project to use given a certain input and whether the local project needs to be pushed.
 
         Many cloud commands look like "lean cloud <command> <name or id> --push".
         This method handles parsing the "<name or id> --push" part.
         This method returns the cloud project we think the user wants to use with the given command.
 
         :param input: the input the user gave, either a local project name, a cloud project name or a cloud id
         :param push: True if the local counterpart of the cloud project needs to be pushed
         :return: the cloud project to use
         """
+        organization_id = self._organization_manager.try_get_working_organization_id()
+
         # If the given input is a valid project directory, we try to use that project
         local_path = Path.cwd() / input
-        if self._path_manager.is_path_valid(local_path) \
-                and local_path.is_dir() \
-                and self._project_config_manager.get_project_config(local_path).file.exists():
+        if self._project_config_manager.try_get_project_config(local_path):
             if push:
                 self._push_manager.push_projects([local_path])
 
                 cloud_id = self._project_config_manager.get_project_config(local_path).get("cloud-id")
                 if cloud_id is None:
                     raise RuntimeError("Something went wrong while pushing the project to the cloud")
 
-                return self._api_client.projects.get(cloud_id)
+                return self._api_client.projects.get(cloud_id, organization_id)
             else:
                 cloud_id = self._project_config_manager.get_project_config(local_path).get("cloud-id")
                 if cloud_id is not None:
-                    return self._api_client.projects.get(cloud_id)
+                    return self._api_client.projects.get(cloud_id, organization_id)
 
         # If the given input is not a valid project directory, we look for a cloud project with a matching name or id
         # If there are multiple, we use the first one
-        for cloud_project in self._api_client.projects.get_all():
+        for cloud_project in self._api_client.projects.get_all(organization_id):
             if str(cloud_project.projectId) != input and cloud_project.name != input:
                 continue
 
             # If the user wants to push and the input doesn't match a local project name, we attempt to push again
             # This may happen if the input is an id instead of a name
             # If the local directory exists, we push it and return the updated cloud project
             if push:
-                local_path = self._pull_manager.get_local_project_path(cloud_project)
+                local_path = self._project_manager.get_local_project_path(cloud_project.name, cloud_project.projectId)
                 if local_path.exists():
                     self._push_manager.push_projects([local_path])
-                    return self._api_client.projects.get(cloud_project.projectId)
+                    return self._api_client.projects.get(cloud_project.projectId, organization_id)
 
             return cloud_project
 
         raise RuntimeError("No project with the given name or id could be found")
```

### Comparing `lean-1.0.99/lean/components/cloud/data_downloader.py` & `lean-1.155/lean/components/cloud/data_downloader.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,22 +7,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import multiprocessing
-import tarfile
 from pathlib import Path
-from datetime import *
+from datetime import datetime, timedelta
 from typing import Any, List, Callable
 
-from joblib import delayed, Parallel
-
 from lean.components.api.api_client import APIClient
 from lean.components.config.lean_config_manager import LeanConfigManager
 from lean.components.util.logger import Logger
 from lean.models.errors import MoreInfoError, RequestFailedError
 
 
 def _store_local_file(file_content: bytes, file_path: Path):
@@ -75,19 +71,21 @@
     def download_files(self, data_files: List[Any], overwrite: bool, organization_id: str) -> None:
         """Downloads files from QuantConnect Datasets to the local data directory.
 
         :param data_files: the list of data files to download
         :param overwrite: whether existing files may be overwritten
         :param organization_id: the id of the organization that should be billed
         """
+        from joblib import delayed, Parallel
+        from multiprocessing import cpu_count
         progress = self._logger.progress(suffix="{task.percentage:0.0f}% ({task.completed:,.0f}/{task.total:,.0f})")
         progress_task = progress.add_task("", total=len(data_files))
 
         try:
-            parallel = Parallel(n_jobs=max(1, multiprocessing.cpu_count() - 1), backend="threading")
+            parallel = Parallel(n_jobs=max(1, cpu_count() - 1), backend="threading")
 
             data_dir = self._lean_config_manager.get_data_directory()
             parallel(delayed(self._download_file)(data_file.file, overwrite, data_dir, organization_id,
                                                   lambda advance: progress.update(progress_task, advance=advance))
                      for data_file in data_files)
 
             # update our config after we download all files, and not in parallel!
@@ -104,18 +102,26 @@
 
             progress.stop()
         except KeyboardInterrupt as e:
             progress.stop()
             raise e
 
     def _process_bulk(self, file: Path, destination: Path):
-        tar = tarfile.open(file)
+        from tarfile import open
+        tar = open(file)
         tar.errorlevel = 0
         tar.extractall(destination)
         tar.close()
+        from os import remove
+        remove(file)
+
+    def remove_suffix(self,input_string, suffix):
+        if suffix and input_string.endswith(suffix):
+            return input_string[:-len(suffix)]
+        return input_string
 
     def _download_file(self,
                        relative_file: str,
                        overwrite: bool,
                        data_directory: Path,
                        organization_id: str,
                        progress_callback: Callable[[float], None]) -> None:
@@ -126,27 +132,38 @@
 
         :param relative_file: the relative path to the file in the data directory
         :param overwrite: whether existing files may be overwritten
         :param data_directory: the path to the local data directory
         :param organization_id: the id of the organization that should be billed
         :param callback: the lambda that is called just before the method returns
         """
-        local_path = data_directory / relative_file
 
-        if local_path.exists() and not overwrite:
+        local_path = canary_path = data_directory / relative_file
+
+        is_bulk = "setup/" in relative_file and relative_file.endswith(".tar")
+        if is_bulk:
+            # for bulk, we will download to a temporary folder and delete it at the end
+            import tempfile
+            local_path = tempfile.gettempdir() + "/" + relative_file
+            canary_path = Path(self.remove_suffix(str(data_directory / relative_file), ".tar") + ".log")
+
+        if canary_path.exists() and not overwrite:
             self._logger.warn("\n".join([
-                f"{local_path} already exists, use --overwrite to overwrite it",
+                f"{relative_file} already exists, use --overwrite to overwrite it",
                 "You have not been charged for this file"
             ]))
             progress_callback(1)
             return
 
         try:
             self._api_client.data.download_file(relative_file, organization_id, local_path, progress_callback)
         except RequestFailedError as error:
-            self._logger.warn(f"{local_path}: {error}\nYou have not been charged for this file")
+            self._logger.warn(f"{relative_file}: {error}\nYou have not been charged for this file")
             progress_callback(1)
             return
 
         # Special case: bulk files need unpacked
-        if "setup/" in relative_file and relative_file.endswith(".tar"):
+        if is_bulk:
+            canary_path.parent.mkdir(parents=True, exist_ok=True)
+            with open(canary_path, 'a') as log_file:
+                log_file.write(f'Downloaded: {relative_file}\n')
             self._process_bulk(local_path, data_directory)
```

### Comparing `lean-1.0.99/lean/components/cloud/__init__.py` & `lean-1.155/lean/components/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/components/cloud/module_manager.py` & `lean-1.155/lean/components/cloud/module_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -98,26 +98,27 @@
         """
         package_file = Path(MODULES_DIRECTORY) / package.get_file_name()
 
         if package_file.is_file():
             if product_id not in self._installed_packages:
                 self._installed_packages[product_id] = []
             self._installed_packages[product_id].append(package)
+            self._logger.debug(f"ModuleManager._download_file(): {package_file} already exists locally")
             return
 
         self._logger.info(f"Downloading '{package_file.name}'")
 
         package_file.parent.mkdir(parents=True, exist_ok=True)
-
         link = self._api_client.modules.get_link(product_id, organization_id, package_file.name)
         try:
             with self._http_client.get(link, stream=True) as response:
                 with package_file.open("wb+") as file:
                     for chunk in response.iter_content(chunk_size=8192):
                         file.write(chunk)
         except Exception as exception:
             package_file.unlink(missing_ok=True)
             raise exception
 
         if product_id not in self._installed_packages:
             self._installed_packages[product_id] = []
         self._installed_packages[product_id].append(package)
+        self._logger.debug(f"ModuleManager._download_file(): adding {package.name} to _installed_packages")
```

### Comparing `lean-1.0.99/lean/components/docker/lean_runner.py` & `lean-1.155/lean/components/docker/lean_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,34 +7,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
-import re
-import uuid
-from datetime import datetime
 from pathlib import Path
 from typing import Any, Dict, Optional, List
-
-from docker.types import Mount
-from pkg_resources import Requirement
-
 from lean.components.cloud.module_manager import ModuleManager
 from lean.components.config.lean_config_manager import LeanConfigManager
 from lean.components.config.output_config_manager import OutputConfigManager
 from lean.components.config.project_config_manager import ProjectConfigManager
 from lean.components.docker.docker_manager import DockerManager
 from lean.components.util.logger import Logger
 from lean.components.util.project_manager import ProjectManager
 from lean.components.util.temp_manager import TempManager
 from lean.components.util.xml_manager import XMLManager
-from lean.constants import MODULES_DIRECTORY, TERMINAL_LINK_PRODUCT_ID
+from lean.constants import MODULES_DIRECTORY, TERMINAL_LINK_PRODUCT_ID, LEAN_ROOT_PATH, DEFAULT_DATA_DIRECTORY_NAME
+from lean.constants import DOCKER_PYTHON_SITE_PACKAGES_PATH
 from lean.models.docker import DockerImage
 from lean.models.utils import DebuggingMethod
 
 class LeanRunner:
     """The LeanRunner class contains the code that runs the LEAN engine locally."""
 
     def __init__(self,
@@ -124,31 +117,41 @@
 
             self._docker_manager.create_volume("lean_cli_rider")
             run_options["volumes"]["lean_cli_rider"] = {
                 "bind": "/root/.local/share/JetBrains",
                 "mode": "rw"
             }
 
+        # Setup debugging with QC Extension
+        if debugging_method == DebuggingMethod.LocalPlatform:
+            run_options["ports"]["5678"] = "0" # Using port 0 will assign a random port every time
+
         run_options["commands"].append("exec dotnet QuantConnect.Lean.Launcher.dll")
 
         # Copy the project's code to the output directory
         self._project_manager.copy_code(algorithm_file.parent, output_dir / "code")
 
         # Run the engine and log the result
         # Run as a subprocess to capture the output before logging it
 
         # Format error messages for cleaner output logs
         run_options["format_output"] = self.format_error_before_logging
-        
+
         success = self._docker_manager.run_image(image, **run_options)
 
         cli_root_dir = self._lean_config_manager.get_cli_root_directory()
         relative_project_dir = project_dir.relative_to(cli_root_dir)
         relative_output_dir = output_dir.relative_to(cli_root_dir)
 
+        if debugging_method == DebuggingMethod.LocalPlatform:
+            # set the container port mapped with host in config for later retrieval
+            port = self._docker_manager.get_container_port(run_options["name"], "5678/tcp")
+            output_config = self._output_config_manager.get_output_config(output_dir)
+            output_config.set("debugport", port)
+
         if detach:
             self._temp_manager.delete_temporary_directories_when_done = False
 
             self._logger.info(
                 f"Successfully started '{relative_project_dir}' in the '{environment}' environment in the '{run_options['name']}' container")
             self._logger.info(f"The output will be stored in '{relative_output_dir}'")
             self._logger.info("You can use Docker's own commands to manage the detached container")
@@ -174,21 +177,25 @@
         :param algorithm_file: the path to the file containing the algorithm
         :param output_dir: the directory to save output data to
         :param debugging_method: the debugging method if debugging needs to be enabled, None if not
         :param release: whether C# projects should be compiled in release configuration instead of debug
         :param detach: whether LEAN should run in a detached container
         :return: the Docker configuration containing basic configuration to run Lean
         """
+        from docker.types import Mount
+        from uuid import uuid4
+        from json import dumps
+
         project_dir = algorithm_file.parent
         project_config = self._project_config_manager.get_project_config(project_dir)
         docker_project_config = project_config.get("docker", {})
 
         # Install the required modules when they're needed
         if lean_config.get("data-provider", None) == "QuantConnect.Lean.Engine.DataFeeds.DownloaderDataProvider" \
-            and lean_config.get("data-downloader", None) == "BloombergDataDownloader":
+            and lean_config.get("data-downloader", None) == "TerminalLinkDataDownloader":
             self._module_manager.install_module(TERMINAL_LINK_PRODUCT_ID, lean_config["job-organization-id"])
 
         # Force the use of the LocalDisk map/factor providers if no recent zip present and not using ApiDataProvider
         data_dir = self._lean_config_manager.get_data_directory()
         if lean_config.get("data-provider", None) != "QuantConnect.Lean.Engine.DataFeeds.ApiDataProvider":
             self._force_disk_provider_if_necessary(lean_config,
                                                    "map-file-provider",
@@ -223,14 +230,17 @@
             "environment": docker_project_config.get("environment", {}),
             "stop_signal": "SIGINT" if debugging_method is None else "SIGKILL",
             "mounts": [],
             "volumes": {},
             "ports": docker_project_config.get("ports", {})
         }
 
+        # mount the project and library directories
+        self.mount_project_and_library_directories(project_dir, run_options)
+
         # Mount the data directory
         run_options["volumes"][str(data_dir)] = {
             "bind": "/Lean/Data",
             "mode": "rw"
         }
 
         # Mount the output directory
@@ -243,43 +253,49 @@
         run_options["volumes"][str(storage_dir)] = {
             "bind": "/Storage",
             "mode": "rw"
         }
 
         # Mount all local files referenced in the Lean config
         cli_root_dir = self._lean_config_manager.get_cli_root_directory()
-        for key in ["transaction-log", "bloomberg-symbol-map-file"]:
+        files_to_mount = [
+            ("transaction-log", cli_root_dir),
+            ("terminal-link-symbol-map-file", cli_root_dir / DEFAULT_DATA_DIRECTORY_NAME / "symbol-properties")
+        ]
+        for key, base_path in files_to_mount:
             if key not in lean_config or lean_config[key] == "":
                 continue
 
-            local_path = cli_root_dir / lean_config[key]
+            lean_config_entry = Path(lean_config[key])
+            local_path = lean_config_entry if lean_config_entry.is_absolute() else base_path / lean_config_entry
             if not local_path.exists():
                 local_path.parent.mkdir(parents=True, exist_ok=True)
                 local_path.touch()
 
             run_options["mounts"].append(Mount(target=f"/Files/{key}",
                                                source=str(local_path),
                                                type="bind",
                                                read_only=False))
 
             lean_config[key] = f"/Files/{key}"
 
         # Update all hosts that need to point to the host's localhost to host.docker.internal so they resolve properly
-        for key in ["bloomberg-server-host"]:
+        for key in ["terminal-link-server-host"]:
             if key not in lean_config:
                 continue
 
             if lean_config[key] == "localhost" or lean_config[key] == "127.0.0.1":
                 lean_config[key] = "host.docker.internal"
 
         set_up_common_csharp_options_called = False
 
         # Set up modules
         installed_packages = self._module_manager.get_installed_packages()
         if len(installed_packages) > 0:
+            self._logger.debug(f"LeanRunner.run_lean(): installed packages {len(installed_packages)}")
             self.set_up_common_csharp_options(run_options)
             set_up_common_csharp_options_called = True
 
             # Mount the modules directory
             run_options["volumes"][MODULES_DIRECTORY] = {
                 "bind": "/Modules",
                 "mode": "ro"
@@ -292,14 +308,15 @@
             run_options["commands"].append("mkdir /ModulesProject")
             run_options["commands"].append("dotnet new sln -o /ModulesProject")
             run_options["commands"].append("dotnet new classlib -o /ModulesProject -f net6.0 --no-restore")
             run_options["commands"].append("rm /ModulesProject/Class1.cs")
 
             # Add all modules to the project, automatically resolving all dependencies
             for package in installed_packages:
+                self._logger.debug(f"LeanRunner.run_lean(): Adding module {package} to the project")
                 run_options["commands"].append(f"rm -rf /root/.nuget/packages/{package.name.lower()}")
                 run_options["commands"].append(
                     f"dotnet add /ModulesProject package {package.name} --version {package.version}")
 
             # Copy all module files to /Lean/Launcher/bin/Debug, but don't overwrite anything that already exists
             run_options["commands"].append(
                 "python /copy_csharp_dependencies.py /Compile/obj/ModulesProject/project.assets.json")
@@ -307,72 +324,68 @@
         # Set up language-specific run options
         self.setup_language_specific_run_options(run_options, project_dir, algorithm_file,
                                             set_up_common_csharp_options_called, release)
 
         # Save the final Lean config to a temporary file so we can mount it into the container
         config_path = self._temp_manager.create_temporary_directory() / "config.json"
         with config_path.open("w+", encoding="utf-8") as file:
-            file.write(json.dumps(lean_config, indent=4))
+            file.write(dumps(lean_config, indent=4))
 
         # Mount the Lean config
-        run_options["mounts"].append(Mount(target="/Lean/Launcher/bin/Debug/config.json",
+        run_options["mounts"].append(Mount(target=f"{LEAN_ROOT_PATH}/config.json",
                                            source=str(config_path),
                                            type="bind",
                                            read_only=True))
 
         # Assign the container a name and store it in the output directory's configuration
-        run_options["name"] = f"lean_cli_{str(uuid.uuid4()).replace('-', '')}"
+        if "container-name" in lean_config:
+            run_options["name"] = lean_config["container-name"]
+        else:
+            run_options["name"] = f"lean_cli_{str(uuid4()).replace('-', '')}"
+
+        # set the hostname
+        if "hostname" in lean_config:
+            run_options["hostname"] = lean_config["hostname"]
+
         output_config = self._output_config_manager.get_output_config(output_dir)
         output_config.set("container", run_options["name"])
         if "backtest-name" in lean_config:
             output_config.set("backtest-name", lean_config["backtest-name"])
-
         if "environment" in lean_config and "environments" in lean_config:
             environment = lean_config["environments"][lean_config["environment"]]
             if "live-mode-brokerage" in environment:
                 output_config.set("brokerage", environment["live-mode-brokerage"].split(".")[-1])
 
         return run_options
 
     def set_up_python_options(self, project_dir: Path, run_options: Dict[str, Any]) -> None:
         """Sets up Docker run options specific to Python projects.
 
         :param project_dir: the path to the project directory
         :param run_options: the dictionary to append run options to
         """
 
+        from docker.types import Mount
         # Compile python files
         source_files = self._project_manager.get_source_files(project_dir)
         source_files = [file.relative_to(
             project_dir).as_posix() for file in source_files]
         source_files = [f'"/LeanCLI/{file}"' for file in source_files]
 
+        # Only need to compile files in backtest/live (where the files were mounted in "/LeanCLI") but not research
         run_options["commands"].append(
-            f"python -m compileall {' '.join(source_files)}")
-            
-        # Mount the project directory
-        run_options["volumes"][str(project_dir)] = {
-            "bind": "/LeanCLI",
-            "mode": "rw"
-        }
-
-        # Check if the user has library projects
-        library_dir = self._lean_config_manager.get_cli_root_directory() / "Library"
-        if library_dir.is_dir():
-            # Mount the library projects
-            run_options["volumes"][str(library_dir)] = {
-                "bind": "/Library",
-                "mode": "rw"
-            }
-
-            # Ensure library projects are used when resolving Python imports
-            run_options["commands"].append("mkdir -p $(python -m site --user-site)")
-            run_options["commands"].append("echo /Library > $(python -m site --user-site)/lean-cli.pth")
+            f"""if [ -d '/LeanCLI' ];
+            then
+                python -m compileall {' '.join(source_files)};
+            else
+                echo '/LeanCLI is not mounted, skipping compilation...';
+            fi""")
 
         # Combine the requirements from all library projects and the current project
+        library_dir = self._lean_config_manager.get_cli_root_directory() / "Library"
         requirements_files = list(library_dir.rglob("requirements.txt")) + [project_dir / "requirements.txt"]
         requirements_files = [file for file in requirements_files if file.is_file()]
         requirements = self._concat_python_requirements(requirements_files)
 
         # Check if we have any dependencies to install, so we don't mount volumes needlessly
         if requirements == "":
             return
@@ -394,40 +407,41 @@
             "bind": "/root/.cache/pip",
             "mode": "rw"
         }
 
         # Mount a volume to the user packages directory so we don't install packages every time
         site_packages_volume = self._docker_manager.create_site_packages_volume(requirements_txt)
         run_options["volumes"][site_packages_volume] = {
-            "bind": "/root/.local/lib/python3.6/site-packages",
+            "bind": f"{DOCKER_PYTHON_SITE_PACKAGES_PATH}",
             "mode": "rw"
         }
 
         # Update PATH in the Docker container to prevent pip install warnings about its executables not being on PATH
         run_options["commands"].append('export PATH="$PATH:/root/.local/bin"')
 
         # Install custom libraries to the cached user packages directory
         # We only need to do this if it hasn't already been done before for this site packages volume
         # To keep track of this we create a special file in the site packages directory after installation
         # If this file already exists we can skip pip install completely
-        marker_file = "/root/.local/lib/python3.6/site-packages/pip-install-done"
+        marker_file = f"{DOCKER_PYTHON_SITE_PACKAGES_PATH}/pip-install-done"
         run_options["commands"].extend([
             f"! test -f {marker_file} && pip install --user --progress-bar off -r /requirements.txt",
             f"touch {marker_file}"
         ])
 
     def _concat_python_requirements(self, requirements_files: List[Path]) -> str:
         """Combines the requirements from multiple requirements.txt files.
 
         Ensures there are no duplicate requirements and that all output lines are valid.
         Requirements are sorted alphabetically to ensure consistent output.
 
         :param requirements_files: the paths to the requirements.txt files
         :return: the normalized requirements from all given requirements.txt files
         """
+        from pkg_resources import Requirement
         requirements = []
         for file in requirements_files:
             for line in file.read_text(encoding="utf-8").splitlines():
                 try:
                     requirements.append(Requirement.parse(line))
                 except ValueError:
                     pass
@@ -441,20 +455,14 @@
 
         :param project_dir: the path to the project directory
         :param run_options: the dictionary to append run options to
         :param release: whether C# projects should be compiled in release configuration instead of debug
         """
         compile_root = self._get_csharp_compile_root(project_dir)
 
-        # Mount the compile root
-        run_options["volumes"][str(compile_root)] = {
-            "bind": "/LeanCLI",
-            "mode": "ro"
-        }
-
         # Ensure all .csproj files refer to the version of LEAN in the Docker container
         csproj_temp_dir = self._temp_manager.create_temporary_directory()
         for path in compile_root.rglob("*.csproj"):
             self._ensure_csproj_uses_correct_lean(compile_root, path, csproj_temp_dir, run_options)
 
         # Set up the MSBuild properties
         msbuild_properties = {
@@ -475,45 +483,47 @@
 
         # Find the .csproj file to compile
         project_file = next(project_dir.glob("*.csproj"))
 
         # Inherit NoWarn from the user's .csproj
         csproj = self._xml_manager.parse(project_file.read_text(encoding="utf-8"))
         existing_no_warn = csproj.find(".//NoWarn")
+        from re import split
         if existing_no_warn is not None:
-            codes = [c for c in re.split(r"[^a-zA-Z0-9]", existing_no_warn.text) if c != ""]
+            codes = [c for c in split(r"[^a-zA-Z0-9]", existing_no_warn.text) if c != ""]
             msbuild_properties["NoWarn"] += codes
 
         # Turn the NoWarn property into a string
         # %3B is the encoded version of ";", because a raw ";" is seen as a separator between properties
         msbuild_properties["NoWarn"] = "%3B".join(msbuild_properties["NoWarn"])
 
         # Build the project before running LEAN
         relative_project_file = str(project_file.relative_to(compile_root)).replace("\\", "/")
         msbuild_properties = ";".join(f"{key}={value}" for key, value in msbuild_properties.items())
         run_options["commands"].append(f'dotnet build "/LeanCLI/{relative_project_file}" "-p:{msbuild_properties}"')
 
         # Copy over the algorithm DLL
         # Copy over the project reference DLLs'
         # Copy over all output DLLs that don't already exist in /Lean/Launcher/bin/Debug
-        run_options["commands"].append("cp -R -n /Compile/bin/. /Lean/Launcher/bin/Debug/")
+        run_options["commands"].append(f"cp -R -n /Compile/bin/. {LEAN_ROOT_PATH}/")
 
         # Copy over all library DLLs that don't already exist in /Lean/Launcher/bin/Debug
         # CopyLocalLockFileAssemblies does not copy the OS-specific DLLs to the output directory
         # We therefore use a custom Python script that does take the OS into account when deciding what to copy
         run_options["commands"].append(
             f'python /copy_csharp_dependencies.py "/Compile/obj/{project_file.stem}/project.assets.json"')
 
     def set_up_common_csharp_options(self, run_options: Dict[str, Any]) -> None:
         """Sets up common Docker run options that is needed for all C# work.
 
         This method is only called if the user has installed modules and/or if the project to run is written in C#.
 
         :param run_options: the dictionary to append run options to
         """
+        from docker.types import Mount
         # Mount a volume to NuGet's cache directory so we only download packages once
         self._docker_manager.create_volume("lean_cli_nuget")
         run_options["volumes"]["lean_cli_nuget"] = {
             "bind": "/root/.nuget/packages",
             "mode": "rw"
         }
 
@@ -635,28 +645,29 @@
         this causes compiling to fail with readable error messages instead of ugly messages at runtime.
 
         :param compile_root: the path that is mounted in the Docker container
         :param csproj_path: the path to the .csproj file
         :param temp_dir: the temporary directory in which temporary .csproj files should be placed
         :param run_options: the dictionary to append run options to
         """
+        from docker.types import Mount
         csproj = self._xml_manager.parse(csproj_path.read_text(encoding="utf-8"))
         include_added = False
 
         for package_reference in csproj.iter("PackageReference"):
             if not package_reference.get("Include", "").lower().startswith("quantconnect."):
                 continue
 
             if include_added:
                 package_reference.getparent().remove(package_reference)
 
             package_reference.clear()
 
             package_reference.tag = "Reference"
-            package_reference.set("Include", "/Lean/Launcher/bin/Debug/*.dll")
+            package_reference.set("Include", f"{LEAN_ROOT_PATH}/*.dll")
             package_reference.append(self._xml_manager.parse("<Private>False</Private>"))
 
             include_added = True
 
         if not include_added:
             return
 
@@ -680,23 +691,26 @@
 
         :param lean_config: the Lean config to update
         :param config_key: the key of the configuration property
         :param zip_provider: the fully classified name of the zip provider for this property
         :param disk_provider: the fully classified name of the disk provider for this property
         :param zip_dir: the directory where the zip provider looks for zip files
         """
+        from re import sub
+        from datetime import datetime
+
         if lean_config.get(config_key, None) != zip_provider:
             return
 
         if not zip_dir.exists():
             lean_config[config_key] = disk_provider
             return
 
         zip_names = sorted([f.name for f in zip_dir.iterdir() if f.name.endswith(".zip")], reverse=True)
-        zip_names = [re.sub(r"[^\d]", "", name) for name in zip_names]
+        zip_names = [sub(r"[^\d]", "", name) for name in zip_names]
 
         if len(zip_names) == 0 or (datetime.now() - datetime.strptime(zip_names[0], "%Y%m%d")).days > 7:
             lean_config[config_key] = disk_provider
 
     def setup_language_specific_run_options(self, run_options, project_dir, algorithm_file,
                                             set_up_common_csharp_options_called, release) -> None:
         # Set up language-specific run options
@@ -705,21 +719,38 @@
         else:
             if not set_up_common_csharp_options_called:
                 self.set_up_common_csharp_options(run_options)
             self.set_up_csharp_options(project_dir, run_options, release)
 
     def format_error_before_logging(self, chunk: str):
         from lean.components.util import compiler
+        from json import loads
         errors = []
 
         # As we don't have algorithm type information. We can check errors for both
         # Python
         jsonString = compiler.get_errors("python", chunk)
-        jsonData = json.loads(jsonString)
+        jsonData = loads(jsonString)
         errors.extend(jsonData["aErrors"])
         # CSharp
         jsonString = compiler.get_errors("csharp", chunk)
-        jsonData = json.loads(jsonString)
+        jsonData = loads(jsonString)
         errors.extend(jsonData["aErrors"])
 
         for error in errors:
-            self._logger.info(error)
+            self._logger.info(error)
+
+    def mount_project_and_library_directories(self, project_dir: Path, run_options: Dict[str, Any]) -> None:
+        # Mount the project directory
+        run_options["volumes"][str(project_dir)] = {
+            "bind": "/LeanCLI",
+            "mode": "rw"
+        }
+
+        # Check if the user has library projects and mount the Library directory
+        library_dir = self._lean_config_manager.get_cli_root_directory() / "Library"
+        if library_dir.is_dir():
+            # Mount the library projects
+            run_options["volumes"][str(library_dir)] = {
+                "bind": "/Library",
+                "mode": "rw"
+            }
```

### Comparing `lean-1.0.99/lean/components/docker/__init__.py` & `lean-1.155/lean/components/util/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/components/docker/docker_manager.py` & `lean-1.155/lean/components/docker/docker_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,42 +7,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import hashlib
-import json
-import os
-import platform
-import shutil
-import signal
-import subprocess
-import sys
-import threading
-import time
-import types
 from pathlib import Path
 from typing import Optional, Set, Any, Dict
-from subprocess import Popen, PIPE
-import docker
-from dateutil.parser import isoparse
-from docker.errors import APIError
-from docker.models.containers import Container
-from docker.types import Mount
 
 from lean.components.util.logger import Logger
 from lean.components.util.platform_manager import PlatformManager
 from lean.components.util.temp_manager import TempManager
 from lean.constants import SITE_PACKAGES_VOLUME_LIMIT, \
-    DOCKER_NETWORK
+    DOCKER_NETWORK, CUSTOM_FOUNDATION, CUSTOM_RESEARCH, CUSTOM_ENGINE
+
 from lean.models.docker import DockerImage
 from lean.models.errors import MoreInfoError
-
+from lean.components.util.custom_json_encoder import DecimalEncoder
 
 class DockerManager:
     """The DockerManager contains methods to manage and run Docker images."""
 
     def __init__(self, logger: Logger, temp_manager: TempManager, platform_manager: PlatformManager) -> None:
         """Creates a new DockerManager instance.
 
@@ -55,26 +39,33 @@
         self._platform_manager = platform_manager
 
     def pull_image(self, image: DockerImage) -> None:
         """Pulls a Docker image.
 
         :param image: the image to pull
         """
+        from shutil import which
+        from subprocess import run
+
+        if image.name == CUSTOM_RESEARCH or image.name == CUSTOM_ENGINE or image.name == CUSTOM_FOUNDATION:
+            self._logger.info(f"Skip pulling local image {image}...")
+            return
+
         self._logger.info(f"Pulling {image}...")
 
         # We cannot really use docker_client.images.pull() here as it doesn't let us log the progress
         # Downloading multiple gigabytes without showing progress does not provide good developer experience
         # Since the pull command is the same on Windows, macOS and Linux we can safely use a system call
-        if shutil.which("docker") is not None:
-            process = subprocess.run(["docker", "image", "pull", str(image)])
+        if which("docker") is not None:
+            process = run(["docker", "image", "pull", str(image), "--platform=linux/amd64"])
             if process.returncode != 0:
                 raise RuntimeError(
                     f"Something went wrong while pulling {image}, see the logs above for more information")
         else:
-            self._get_docker_client().images.pull(image.name, image.tag)
+            self._get_docker_client().images.pull(image.name, image.tag, platform="linux/amd64")
 
     def run_image(self, image: DockerImage, **kwargs) -> bool:
         """Runs a Docker image. If the image is not available locally it will be pulled first.
 
         See https://docker-py.readthedocs.io/en/stable/containers.html for all the supported kwargs.
 
         If kwargs contains an "on_output" property, it is removed before passing it on to docker.containers.run
@@ -90,14 +81,22 @@
         If kwargs sets "detach" to True, the method returns as soon as the container starts.
         If this is not the case, the method is blocking and runs until the container exits.
 
         :param image: the image to run
         :param kwargs: the kwargs to forward to docker.containers.run
         :return: True if the command in the container exited successfully, False if not
         """
+        from signal import signal, SIGINT, Signals
+        from platform import node
+        from sys import stdout, exit
+        from threading import Thread
+        from types import FrameType
+        from docker.errors import APIError
+        from docker.types import Mount
+
         if not self.image_installed(image):
             self.pull_image(image)
 
         on_output = kwargs.pop("on_output", lambda chunk: None)
         format_output = kwargs.pop("format_output", lambda chunk: None)
         commands = kwargs.pop("commands", None)
 
@@ -127,18 +126,18 @@
 
         if "volumes" in kwargs:
             for key in list(kwargs["volumes"].keys()):
                 new_key = self._format_source_path(key)
                 kwargs["volumes"][new_key] = kwargs["volumes"].pop(key)
 
         detach = kwargs.pop("detach", False)
-        is_tty = sys.stdout.isatty()
+        is_tty = stdout.isatty()
 
         kwargs["detach"] = True
-        kwargs["hostname"] = platform.node()
+        kwargs["hostname"] = kwargs["hostname"] if "hostname" in kwargs else node()
         kwargs["tty"] = is_tty and not detach
         kwargs["stdin_open"] = is_tty and not detach
         kwargs["stop_signal"] = kwargs.get("stop_signal", "SIGKILL")
 
         if detach and "remove" not in kwargs:
             kwargs["remove"] = True
 
@@ -181,32 +180,32 @@
                 else:
                     container.stop(timeout=60)
                 container.remove()
             except APIError:
                 pass
             finally:
                 self._temp_manager.delete_temporary_directories()
-                sys.exit(1)
+                exit(1)
 
         # Kill the container on Ctrl+C
-        def signal_handler(sig: signal.Signals, frame: types.FrameType) -> None:
+        def signal_handler(sig: Signals, frame: FrameType) -> None:
             nonlocal force_kill_next
             if not is_tty or force_kill_next or kwargs["stop_signal"] == "SIGKILL":
                 force_kill_current = True
             else:
                 self._logger.info("Waiting 1 minute for LEAN to exit gracefully, press Ctrl+C again to force stop")
                 force_kill_next = True
                 force_kill_current = False
 
             # If we run this code on the current thread, a second Ctrl+C won't be detected on Windows
-            kill_thread = threading.Thread(target=kill_container, args=[force_kill_current])
+            kill_thread = Thread(target=kill_container, args=[force_kill_current])
             kill_thread.daemon = True
             kill_thread.start()
 
-        signal.signal(signal.SIGINT, signal_handler)
+        signal(SIGINT, signal_handler)
 
         # container.logs() is blocking, we run it on a separate thread so the SIGINT handler works properly
         # If we run this code on the current thread, SIGINT won't be triggered on Windows when Ctrl+C is triggered
         def print_logs() -> None:
             chunk_buffer = bytes()
             is_first_time = True
             log_dump = ""
@@ -256,28 +255,28 @@
                 pass
 
         def print_and_format_logs():
             log_dump = print_logs()
             if format_output is not None:
                 format_output(log_dump)
 
-        logs_thread = threading.Thread(target=print_and_format_logs)
+        logs_thread = Thread(target=print_and_format_logs)
         logs_thread.daemon = True
         logs_thread.start()
 
         while logs_thread.is_alive():
             logs_thread.join(0.1)
 
         if killed:
             try:
                 container.remove()
             except APIError:
                 pass
             finally:
-                sys.exit(1)
+                exit(1)
 
         container.wait()
 
         container.reload()
         success = container.attrs["State"]["ExitCode"] == 0
 
         container.remove()
@@ -286,18 +285,19 @@
     def build_image(self, root: Path, dockerfile: Path, target: DockerImage) -> None:
         """Builds a Docker image.
 
         :param root: the path build from
         :param dockerfile: the path to the Dockerfile to build
         :param target: the target name and tag
         """
+        from subprocess import run
         # We cannot really use docker_client.images.build() here as it doesn't let us log the progress
         # Building images without showing progress does not provide good developer experience
         # Since the build command is the same on Windows, macOS and Linux we can safely use a system call
-        process = subprocess.run(["docker", "build", "-t", str(target), "-f", str(dockerfile), "."], cwd=root)
+        process = run(["docker", "build", "-t", str(target), "-f", str(dockerfile), "."], cwd=root)
 
         if process.returncode != 0:
             raise RuntimeError(
                 f"Something went wrong while building '{dockerfile}', see the logs above for more information")
 
     def image_installed(self, image: DockerImage) -> bool:
         """Returns whether a certain image is installed.
@@ -354,15 +354,18 @@
 
         This method automatically returns the best volume for the given requirements.
         It also rotates out older volumes as needed to ensure we don't use too much disk space.
 
         :param requirements_file: the path to the requirements file that will be pip installed in the container
         :return: the name of the Docker volume to use
         """
-        requirements_hash = hashlib.md5(requirements_file.read_text(encoding="utf-8").encode("utf-8")).hexdigest()
+        from hashlib import md5
+        from dateutil.parser import isoparse
+
+        requirements_hash = md5(requirements_file.read_text(encoding="utf-8").encode("utf-8")).hexdigest()
         volume_name = f"lean_cli_python_{requirements_hash}"
 
         docker_client = self._get_docker_client()
         existing_volumes = [v for v in docker_client.volumes.list() if v.name.startswith("lean_cli_python_")]
 
         if any(v.name == volume_name for v in existing_volumes):
             return volume_name
@@ -378,15 +381,15 @@
         """Returns the names of all running containers.
 
         :return: a set containing the names of all running Docker containers
         """
         containers = self._get_docker_client().containers.list()
         return {c.name.lstrip("/") for c in containers if c.status == "running"}
 
-    def get_container_by_name(self, container_name: str) -> Optional[Container]:
+    def get_container_by_name(self, container_name: str):
         """Finds a container with a given name.
 
         :param container_name: the name of the container to find
         :return: the container with the given name, or None if it does not exist
         """
         for container in self._get_docker_client().containers.list(all=True):
             if container.name.lstrip("/") == container_name:
@@ -396,123 +399,133 @@
 
     def show_logs(self, container_name: str, follow: bool = False) -> None:
         """Shows the logs of a Docker container in the terminal.
 
         :param container_name: the name of the container to show the logs of
         :param follow: whether the logs should be streamed in real-time if the container is running (defaults to False)
         """
+        from subprocess import run
         if self.get_container_by_name(container_name) is None:
             return
 
         # We cannot use the Docker Python SDK to get live logs consistently
         # Since the logs command is the same on Windows, macOS and Linux we can safely use a system call
         command = ["docker", "logs"]
         if follow:
             command.append("-f")
         command.append(container_name)
 
-        subprocess.run(command)
+        run(command)
 
     def is_missing_permission(self) -> bool:
         """Returns whether we cannot connect to the Docker client because of a permissions issue.
 
         A permissions issue usually indicates that the client can only be used with root privileges.
 
         :return: True if we cannot connect to the Docker client because of a permissions issue, False if that's not
         """
         try:
-            docker.from_env()
+            from docker import from_env
+            from_env()
         except Exception as exception:
             return "Permission denied" in str(exception)
         return False
 
-    def write_to_file(self, docker_container_name: str, docker_file: Path, data: Dict[str, Any]) -> None:        
+    def write_to_file(self, docker_container_name: str, docker_file: Path, data: Dict[str, Any]) -> None:
         """Write data to the file in docker.
 
         Args:
             docker_container_name: The name of the container to write to
             docker_file: The Dockerfile to write to.
             data: The data to write to the Dockerfile.
         """
+        from subprocess import run, CalledProcessError
+        from json import dumps
+
         docker_container = self.get_container_by_name(docker_container_name)
         if docker_container is None:
             raise ValueError(f"Container {docker_container_name} does not exist")
         if docker_container.status != "running":
             raise ValueError(f"Container {docker_container_name} is not running")
-            
-        data = json.dumps(data)
+
+        data = dumps(data, cls=DecimalEncoder)
         data = data.replace('"','\\"')
         command = f'docker exec {docker_container_name} bash -c "echo \'{data}\' > {docker_file.as_posix()}"'
         try:
-            subprocess.run(command, shell=True, check=True)
-        except subprocess.CalledProcessError as exception:
+            run(command, shell=True, check=True)
+        except CalledProcessError as exception:
             raise ValueError(f"Failed to write to {docker_file.name}: {exception.output.decode('utf-8')}")
         except Exception as e:
             raise ValueError(f"Failed to write to {docker_file.name}: {e}")
-    
+
     def read_from_file(self, docker_container_name: str, docker_file: Path, interval=1, timeout=30) -> Dict[str,Any]:
         """Read data from file in docker.
 
         Args:
             docker_container_name: The name of the container to write to
             docker_file: The Dockerfile to write to.
             interval: The interval to sleep before checking again.
             timeout: The timeout to wait for the file.
         """
+        from json import loads
+        from subprocess import Popen, PIPE, CalledProcessError
+        from time import sleep, time
+
         command = f'docker exec {docker_container_name} bash -c "cat {docker_file.as_posix()}"'
-        start = time.time()
+        start = time()
         success = False
         error_message = None
         container_running = True
-        while time.time() - start < timeout:
+        while time() - start < timeout:
             try:
                 docker_container = self.get_container_by_name(docker_container_name)
                 if docker_container is None:
                     error_message = f"Container {docker_container_name} does not exist"
                     container_running = False
                     break
                 p = Popen(command, shell=True, stdin=PIPE, stdout=PIPE, stderr=PIPE)
                 output = p.stdout.read().decode('utf-8')
                 if output is not None and output != "":
                     success = True
                     break
-            except subprocess.CalledProcessError as exception:
+            except CalledProcessError as exception:
                 error_message = f"Failed to read result from docker file {docker_file.name}: {exception.output.decode('utf-8')} {p.stderr.read().decode('utf-8')}"
-                time.sleep(interval)
+                sleep(interval)
             except Exception as e:
                 error_message = f"Failed to read result from docker file {docker_file.name}: {e} {p.stderr.read().decode('utf-8')}"
-                time.sleep(interval)
+                sleep(interval)
 
         if success:
-            result = json.loads(output)
+            result = loads(output)
             success = result["Success"]
             if not success:
                 error_message = "Rejected by Lean. Possible arguments error. Please check your logs and try again."
         if not success and not error_message:
             error_message = f"Failed to read result from docker file {docker_file.name} within {timeout} seconds"
-        
+
         return {
             "error": error_message,
             "success": success,
             "container-running": container_running
         }
 
 
-    def _get_docker_client(self) -> docker.DockerClient:
+    def _get_docker_client(self):
         """Creates a DockerClient instance.
 
         Raises an error if Docker is not running.
 
         :return: a DockerClient instance which responds to requests
         """
         error = MoreInfoError("Please make sure Docker is installed and running",
-                              "https://www.lean.io/docs/lean-cli/key-concepts/troubleshooting#02-Common-Errors")
+                              "https://www.lean.io/docs/v2/lean-cli/key-concepts/troubleshooting#02-Common-Errors")
 
         try:
-            docker_client = docker.from_env()
+            from docker import from_env
+            docker_client = from_env()
         except Exception:
             raise error
 
         try:
             if not docker_client.ping():
                 raise error
         except Exception:
@@ -526,25 +539,49 @@
         This method does two things:
         1. If Docker Toolbox is in use, it converts paths like C:/Path to /c/Path.
         2. If Docker is running in Docker, it converts paths to the corresponding paths on the host system.
 
         :param path: the original path
         :return: the original path formatted in such a way that Docker can understand it
         """
+        from os import environ
+        from json import loads
+
         # Docker Toolbox modifications
         is_windows = self._platform_manager.is_system_windows()
-        is_docker_toolbox = "machine/machines" in os.environ.get("DOCKER_CERT_PATH", "").replace("\\", "/")
+        is_docker_toolbox = "machine/machines" in environ.get("DOCKER_CERT_PATH", "").replace("\\", "/")
         if is_windows and is_docker_toolbox:
             # Backward slashes to forward slashes
             path = path.replace('\\', '/')
 
             # C:/Path to /c/Path
             path = f"/{path[0].lower()}/{path[3:]}"
 
         # Docker in Docker modifications
-        path_mappings = json.loads(os.environ.get("DOCKER_PATH_MAPPINGS", "{}"))
+        path_mappings = loads(environ.get("DOCKER_PATH_MAPPINGS", "{}"))
         for container_path, host_path in path_mappings.items():
             if path.startswith(container_path):
                 path = host_path + path[len(container_path):]
                 break
 
         return path
+    
+    def get_container_port(self, container_name: str, internal_port: str) -> Optional[int]:
+        """
+        Returns a containers external port for a mapped internal port
+        :param container_name: Name of the container
+        :param internal_port: The internal port of container. If protocol not included
+        we assume /tcp. ex. 5678/tcp 
+        :return: The external port that is linked to it, or None if it does not exist
+        """
+
+        # In case a port is supplied without a protocol assume tcp
+        if not internal_port.__contains__("/tcp") and not internal_port.__contains__("/udp"):
+            internal_port = str(internal_port) + "/tcp"
+
+        container = self.get_container_by_name(container_name)
+
+        # Grab the host port assigned
+        if container is not None and internal_port in container.ports:
+            return container.ports[internal_port][0]["HostPort"]
+
+        return None
```

### Comparing `lean-1.0.99/lean/components/config/cli_config_manager.py` & `lean-1.155/lean/components/config/cli_config_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,16 @@
                                 True,
                                 credentials_storage)
 
         self.default_language = ChoiceOption("default-language",
                                              "The default language used when creating new projects.",
                                              ["python", "csharp"],
                                              False,
-                                             general_storage)
+                                             general_storage,
+                                             "python")
 
         self.engine_image = Option("engine-image",
                                    f"The Docker image used when running the LEAN engine ({DEFAULT_ENGINE_IMAGE} if not set).",
                                    False,
                                    general_storage)
 
         self.research_image = Option("research-image",
@@ -71,15 +72,15 @@
         :param key: the key to look for
         :return: the option having a key equal to the given key
         """
         option = next((x for x in self.all_options if x.key == key), None)
 
         if option is None:
             raise MoreInfoError(f"There doesn't exist an option with key '{key}'",
-                                "https://www.lean.io/docs/lean-cli/api-reference/lean-config-set#02-Description")
+                                "https://www.lean.io/docs/v2/lean-cli/api-reference/lean-config-set#02-Description")
 
         return option
 
     def get_engine_image(self, override: Optional[str] = None) -> DockerImage:
         """Returns the LEAN engine image to use.
 
         :param override: the image name to use, overriding any defaults or previously configured options
```

### Comparing `lean-1.0.99/lean/components/config/lean_config_manager.py` & `lean-1.155/lean/components/config/lean_config_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,24 +7,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import re
 from pathlib import Path
 from typing import Any, Dict, Optional, List
 
-import json5
 
 from lean.components.cloud.module_manager import ModuleManager
 from lean.components.config.cli_config_manager import CLIConfigManager
 from lean.components.config.project_config_manager import ProjectConfigManager
-from lean.components.config.storage import Storage
+from lean.components.config.storage import Storage, safe_save
 from lean.components.util.logger import Logger
 from lean.constants import DEFAULT_LEAN_CONFIG_FILE_NAME
 from lean.models.errors import MoreInfoError
 from lean.models.utils import DebuggingMethod
 
 
 class LeanConfigManager:
@@ -70,21 +68,22 @@
 
         # Recurse upwards in the directory tree until we find a Lean config file
         current_dir = Path.cwd()
         while True:
             target_file = current_dir / DEFAULT_LEAN_CONFIG_FILE_NAME
             if target_file.exists():
                 self._lean_config_path = target_file
+
                 self.store_known_lean_config_path(self._lean_config_path)
                 return self._lean_config_path
 
             # If the parent directory is the same as the current directory we can't go up any more
             if current_dir.parent == current_dir:
                 raise MoreInfoError(f"'{DEFAULT_LEAN_CONFIG_FILE_NAME}' not found",
-                                    "https://www.lean.io/docs/lean-cli/initialization/configuration#03-Lean-Configuration")
+                                    "https://www.lean.io/docs/v2/lean-cli/initialization/configuration#03-Lean-Configuration")
 
             current_dir = current_dir.parent
 
     def set_default_lean_config_path(self, path: Path) -> None:
         """Overrides the default search for the path to the Lean config file.
 
         :param path: the path to the Lean config file to return in future calls to get_lean_config_path()
@@ -106,14 +105,23 @@
         return lean_config_paths
 
     def store_known_lean_config_path(self, path: Path) -> None:
         """Caches a path as being a known Lean configuration file path.
 
         :param path: the path to the Lean configuration file
         """
+        try:
+            lean_config = self.get_lean_config()
+            if lean_config.get("organization-id") is None:
+                return
+        except Exception as e:
+            # If we can't get the Lean config then it must be from the lean init.
+            # Therefore, we can trust it's valid
+            self._logger.debug(f"LeanConfigManager.store_known_lean_config_path(): Failed to get Lean config: {e}")
+            pass
         lean_config_paths = set(self._cache_storage.get("known-lean-config-paths", []))
         lean_config_paths.add(str(path))
         self._cache_storage.set("known-lean-config-paths", list(lean_config_paths))
 
     def get_cli_root_directory(self) -> Path:
         """Returns the path to the directory containing the Lean config file.
 
@@ -133,29 +141,32 @@
         """Sets a properties in the Lean config file.
 
         If a property does not exist yet it is added automatically.
         Comments in the Lean config file are preserved.
 
         :param updates: the key -> new value updates to apply to the current config
         """
+        from json5 import dumps
+        from re import sub
+
         config = self.get_lean_config()
 
         config_path = self.get_lean_config_path()
         config_text = config_path.read_text(encoding="utf-8")
 
         for key, value in reversed(list(updates.items())):
-            json_value = json5.dumps(value)
+            json_value = dumps(value)
 
             # We can only use regex to set the property because converting the config back to JSON drops all comments
             if key in config:
-                config_text = re.sub(fr'"{key}":\s*("?[^",]*"?)', f'"{key}": {json_value}', config_text)
+                config_text = sub(fr'"{key}":\s*("?[^",]*"?)', f'"{key}": {json_value}', config_text)
             else:
                 config_text = config_text.replace("{", f'{{\n  "{key}": {json_value},', 1)
 
-        config_path.write_text(config_text, encoding="utf-8")
+        safe_save(path=config_path, data=config_text)
 
     def clean_lean_config(self, config: str) -> str:
         """Removes the properties from a Lean config file which can be set in get_complete_lean_config().
 
         This removes all the properties which the CLI can configure automatically based on the command that is ran.
 
         For example, given the following config:
@@ -174,25 +185,27 @@
         }
 
         Because "environment" can be set automatically based on the command that is ran.
 
         :param config: the configuration to remove the auto-configurable keys from
         :return: the same config as passed in with the config argument, but without the auto-configurable keys
         """
+        from re import split
+
         # The keys that we can set automatically based on the command that is ran
         keys_to_remove = ["environment",
                           "composer-dll-directory",
                           "debugging", "debugging-method",
                           "job-user-id", "api-access-token",
                           "algorithm-type-name", "algorithm-language", "algorithm-location",
                           "parameters", "intrinio-username", "intrinio-password", "ema-fast", "ema-slow"]
 
         # This function is implemented by doing string manipulation because the config contains comments
         # If we were to parse it as JSON, we would have to remove the comments, which we don't want to do
-        sections = re.split(r"\n\s*\n", config)
+        sections = split(r"\n\s*\n", config)
         for key in keys_to_remove:
             sections = [section for section in sections if f"\"{key}\": " not in section]
         config = "\n\n".join(sections)
 
         # For some keys we should only remove the key itself, instead of their entire section
         lines = config.split("\n")
         for key in ["ib-host", "ib-port", "ib-tws-dir", "ib-version"]:
@@ -250,22 +263,33 @@
                 config[key] = value
 
         if algorithm_file.name.endswith(".py"):
             config["algorithm-type-name"] = algorithm_file.name.split(".")[0]
             config["algorithm-language"] = "Python"
             config["algorithm-location"] = f"/LeanCLI/{algorithm_file.name}"
         else:
+            from re import findall
             algorithm_text = algorithm_file.read_text(encoding="utf-8")
-            config["algorithm-type-name"] = re.findall(r"class\s*([^\s:]+)\s*:\s*QCAlgorithm", algorithm_text)[0]
+            config["algorithm-type-name"] = findall(r"class\s*([^\s:]+)\s*:\s*QCAlgorithm", algorithm_text)[0]
             config["algorithm-language"] = "CSharp"
             config["algorithm-location"] = f"{algorithm_file.parent.name}.dll"
 
         project_config = self._project_config_manager.get_project_config(algorithm_file.parent)
         config["parameters"] = project_config.get("parameters", {})
 
+        # Add libraries paths to python project
+        project_language = project_config.get("algorithm-language", None)
+        if project_language == "Python":
+            library_references = project_config.get("libraries", [])
+            python_paths = config.get("python-additional-paths", [])
+            python_paths.extend([(Path("/") / library["path"]).as_posix() for library in library_references])
+            if len(python_paths) > 0:
+                python_paths.append("/Library")
+            config["python-additional-paths"] = python_paths
+
         # No real limit for the object store by default
         if "storage-limit-mb" not in config:
             config["storage-limit-mb"] = "9999999"
         if "storage-file-count" not in config:
             config["storage-file-count"] = "9999999"
 
         return config
@@ -289,8 +313,43 @@
         lean_config["data-purchase-limit"] = data_purchase_limit
 
     def get_lean_config(self) -> Dict[str, Any]:
         """Reads the Lean config into a dict.
 
         :return: a dict containing the contents of the Lean config file
         """
-        return json5.loads(self.get_lean_config_path().read_text(encoding="utf-8"))
+        path = self.get_lean_config_path()
+        content = path.read_text(encoding="utf-8")
+        return self.parse_json(content)
+
+    def parse_json(self, content) -> Dict[str, Any]:
+        try:
+            from json import loads
+            from re import sub
+
+            # remove multi line or single line comments without double quotes
+            config = sub(r'/\*.*?\*/|//[^\r\n"]*[\r\n]', '', content)
+
+            # let's handle single line comments with double quotes in them
+            new_config = ''
+            for line in config.split('\n'):
+                double_quotes_count = 0
+                previous_element = ''
+                for current_element in line:
+                    if current_element == '/' and double_quotes_count % 2 == 0:
+                        if previous_element == '/':
+                            break
+                    else:
+                        # count not escaped double quotes
+                        if current_element == '"' and previous_element != '\\':
+                            double_quotes_count = double_quotes_count + 1
+                        new_config += current_element
+                    previous_element = current_element
+            result = loads(new_config)
+            return result
+
+        except Exception as e:
+            self._logger.error(str(e))
+
+            # just in case slower fallback
+            from json5 import loads
+            return loads(content)
```

### Comparing `lean-1.0.99/lean/components/config/storage.py` & `lean-1.155/lean/components/config/storage.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,31 +7,72 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
 from pathlib import Path
 from typing import Any
 
 
+def safe_save(data: str, path: str, _retry: int = 0):
+    from uuid import uuid4
+    from shutil import move
+    from os import unlink, path as os_path
+    from time import time, sleep
+
+    lock_file = Path(str(path) + '.lock').resolve()
+    try:
+        with open(lock_file, 'x') as _:
+            # we create a tmp file we will use to write to. This was we avoid concurrency issues corrupting the file
+            tmp_file = Path(str(path) + '.' + str(uuid4())).resolve()
+            with open(tmp_file, "w+", encoding="utf-8") as targetFile:
+                targetFile.write(data)
+
+            # atomic move when on the same filesystem which is this case, they are side by side
+            move(tmp_file, path)
+        unlink(lock_file)
+    except FileExistsError:
+        try:
+            # lock is taken, delete if old, else wait and retry
+            if time() - os_path.getmtime(lock_file) >= 2:
+                unlink(lock_file)
+            else:
+                sleep(0.250)
+        except:
+            # some else might have deleted it
+            pass
+        if _retry < 10:
+            safe_save(data, path, ++_retry)
+
+
 class Storage:
     """A Storage instance manages the data in a single JSON file."""
 
     def __init__(self, file: str) -> None:
         """Creates a new Storage instance.
 
         :param file: the path to the file this Storage instance should manage
         """
+        from json import loads
+
         self.file = Path(file)
 
         if self.file.exists():
-            self._data = json.loads(self.file.read_text(encoding="utf-8"))
+            try:
+                content = self.file.read_text(encoding="utf-8")
+                if content:
+                    self._data = loads(content)
+                else:
+                    self._data = {}
+            except:
+                # Could happen rarely due to concurrency or unexpected failures, so if it does let's recover
+                self.file.unlink()
+                self._data = {}
         else:
             self._data = {}
 
     def get(self, key: str, default: Any = None) -> Any:
         """Returns the value assigned to the given key.
 
         Returns a default value when nothing is assigned to the given key.
@@ -74,16 +115,17 @@
 
     def clear(self) -> None:
         """Clears the Storage instance and deletes the underlying file."""
         self._data.clear()
         self._save()
 
     def _save(self) -> None:
+        from json import dumps
+
         """Saves the data to the underlying file, deleting the file if there is no data."""
         if len(self._data) > 0:
             self.file.parent.mkdir(parents=True, exist_ok=True)
 
-            with self.file.open("w+", encoding="utf-8") as file:
-                file.write(json.dumps(self._data, indent=4) + "\n")
+            safe_save(data=dumps(self._data, indent=4) + "\n", path=self.file.resolve())
         else:
             if self.file.exists():
                 self.file.unlink()
```

### Comparing `lean-1.0.99/lean/components/config/output_config_manager.py` & `lean-1.155/lean/components/config/output_config_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import random
 from pathlib import Path
 from typing import List, Optional
 
 from lean.components.config.lean_config_manager import LeanConfigManager
 from lean.components.config.storage import Storage
 
 
@@ -33,21 +32,22 @@
         """Returns a Storage instance to get/set the configuration of the contents of an output directory.
 
         :param output_directory: the path to the project to retrieve the configuration of
         :return: the Storage instance containing the configuration of the given backtest/optimization/live trading
         """
         return Storage(str(output_directory / "config"))
 
-    def get_backtest_id(self, backtest_directory: Path) -> int:
+    def get_backtest_id(self, backtest_directory: Path, backtest_id: int = None) -> int:
         """Returns the id of a backtest.
 
         :param backtest_directory: the path to the backtest to retrieve the id of
+        :param backtest_id: the id that needs to be set in the config file
         :return: the id of the given backtest
         """
-        return self._get_id(backtest_directory, 1)
+        return self._get_id(backtest_directory, 1, backtest_id)
 
     def get_backtest_name(self, backtest_directory: Path) -> str:
         """Returns the name of a backtest.
 
         :param backtest_directory: the path to the backtest to retrieve the id of
         :return: the name of the given backtest
         """
@@ -76,55 +76,94 @@
 
         :param backtest_id: the id of the backtest to get the directory of
         :param root_directory: the directory to search from, defaults to the `lean init` directory
         :return: the output directory of the backtest with the given id
         """
         return self._get_by_id("Backtest", backtest_id, ["backtests/*", "optimizations/*/*"], root_directory)
 
-    def get_optimization_id(self, optimization_directory: Path) -> int:
+    def get_optimization_id(self, optimization_directory: Path, optimization_id: int = None) -> int:
         """Returns the id of an optimization.
 
         :param optimization_directory: the path to the optimization to retrieve the id of
+        :param optimization_id: the id that needs to be set in the config file
         :return: the id of the given optimization
         """
-        return self._get_id(optimization_directory, 2)
+        return self._get_id(optimization_directory, 2, optimization_id)
 
     def get_optimization_by_id(self, optimization_id: int, root_directory: Optional[Path] = None) -> Path:
         """Finds the directory of an optimization by its id.
 
         :param optimization_id: the id of the optimization to get the directory of
         :param root_directory: the directory to search from, defaults to the `lean init` directory
         :return: the output directory of the optimization with the given id
         """
         return self._get_by_id("Optimization", optimization_id, ["optimizations/*"], root_directory)
 
-    def get_live_deployment_id(self, live_deployment_directory: Path) -> int:
+    def get_live_deployment_id(self, live_deployment_directory: Path, live_deployment_id: int = None) -> int:
         """Returns the id of a live deployment.
 
         :param live_deployment_directory: the path to the live deployment to retrieve the id of
+        :param live_deployment_id: the id that needs to be set in the config file
         :return: the id of the given optimization
         """
-        return self._get_id(live_deployment_directory, 3)
+        return self._get_id(live_deployment_directory, 3, live_deployment_id)
 
     def get_live_deployment_by_id(self, live_deployment_id: int, root_directory: Optional[Path] = None) -> Path:
         """Finds the directory of a live deployment by its id.
 
         :param live_deployment_id: the id of the live deployment to get the directory of
         :param root_directory: the directory to search from, defaults to the `lean init` directory
         :return: the output directory of the live deployment with the given id
         """
         return self._get_by_id("Live deployment", live_deployment_id, ["live/*"], root_directory)
 
-    def _get_id(self, output_directory: Path, prefix: int) -> int:
+    def get_latest_output_directory(self, environment: str) -> Optional[Path]:
+        """Finds the latest output directory for the given environment (live or backtests)
+
+        :param environment: The environment to find the latest output directory for (live or backtests)
+        :return: The path to the latest output directory for the given environment
+        :raises RuntimeError: If no output directory is found for the given environment
+        """
+        output_json_files = sorted(Path.cwd().rglob(f"{environment}/*/*.json"),
+                                   key=lambda d: d.stat().st_mtime,
+                                   reverse=True)
+
+        if len(output_json_files) == 0:
+            return None
+
+        return output_json_files[0].parent
+
+    def get_output_id(self, output_directory: Path) -> Optional[int]:
+        """Returns the id of an output, regardless of whether it is a backtest or a live deployment.
+
+        It will return None if the output directory does not contain any output with an existing id.
+
+        :param output_directory: the path to the output to retrieve the id of
+        :return: the id of the given output
+        """
+        output_id = self._get_id(output_directory, 9)
+
+        if str(output_id)[0] == '9':
+            # no existing id was found
+            return None
+
+        return output_id
+
+    def _get_id(self, output_directory: Path, prefix: int, id: int = None) -> int:
         config = self.get_output_config(output_directory)
 
+        if id is not None:
+            config.set("id", id)
+            return id
+
         if config.has("id"):
             return config.get("id")
 
-        new_id = int(str(prefix) + str(random.randint(100_000_000, 999_999_999)))
+        from random import randint
+        new_id = int(str(prefix) + str(randint(100_000_000, 999_999_999)))
         config.set("id", new_id)
 
         return new_id
 
     def _get_by_id(self, label: str, object_id: int, patterns: List[str], root_directory: Optional[Path]) -> Path:
         if root_directory is None:
             root_directory = self._lean_config_manager.get_cli_root_directory()
```

### Comparing `lean-1.0.99/lean/components/config/optimizer_config_manager.py` & `lean-1.155/lean/components/config/optimizer_config_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,19 +7,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import itertools
-import re
 from typing import List, Tuple
 
-import click
+from click import prompt, confirm, FLOAT, FloatRange, IntRange
 
 from lean.components.util.logger import Logger
 from lean.models.api import QCParameter
 from lean.models.logger import Option
 from lean.models.optimizer import (OptimizationConstraint, OptimizationConstraintOperator, OptimizationExtremum,
                                    OptimizationParameter, OptimizationTarget)
 from lean.models.pydantic import WrappedBaseModel
@@ -98,16 +96,17 @@
         return self._logger.prompt_list("Select the optimization strategy to use", options)
 
     def configure_target(self) -> OptimizationTarget:
         """Asks the user for the optimization target.
 
         :return: the chosen optimization target
         """
+        from itertools import product
         # Create a list of options containing a "<target> (min)" and "<target> (max)" option for every target
-        options = list(itertools.product(self.available_targets,
+        options = list(product(self.available_targets,
                                          [OptimizationExtremum.Minimum, OptimizationExtremum.Maximum]))
         options = [Option(id=OptimizationTarget(target=option[0][0], extremum=option[1]),
                           label=f"{option[0][1]} ({option[1]})") for option in options]
 
         return self._logger.prompt_list("Select an optimization target", options)
 
     def configure_parameters(self, project_parameters: List[QCParameter], cloud: bool) -> List[OptimizationParameter]:
@@ -120,20 +119,20 @@
         results: List[OptimizationParameter] = []
 
         for parameter in project_parameters:
             if cloud and len(results) == 2:
                 self._logger.warn(f"You can optimize up to 2 parameters in the cloud, skipping '{parameter.key}'")
                 continue
 
-            if not click.confirm(f"Should the '{parameter.key}' parameter be optimized?", default=True):
+            if not confirm(f"Should the '{parameter.key}' parameter be optimized?", default=True):
                 continue
 
-            minimum = click.prompt(f"Minimum value for '{parameter.key}'", type=click.FLOAT)
-            maximum = click.prompt(f"Maximum value for '{parameter.key}'", type=click.FloatRange(min=minimum))
-            step_size = click.prompt(f"Step size for '{parameter.key}'", type=click.FloatRange(min=0.0), default=1.0)
+            minimum = prompt(f"Minimum value for '{parameter.key}'", type=FLOAT)
+            maximum = prompt(f"Maximum value for '{parameter.key}'", type=FloatRange(min=minimum))
+            step_size = prompt(f"Step size for '{parameter.key}'", type=FloatRange(min=0.0), default=1.0)
 
             results.append(OptimizationParameter(name=parameter.key, min=minimum, max=maximum, step=step_size))
 
         return results
 
     def configure_constraints(self) -> List[OptimizationConstraint]:
         """Asks the user for the optimization constraints.
@@ -147,63 +146,64 @@
         results: List[OptimizationConstraint] = []
 
         while True:
             results_str = ", ".join([str(result) for result in results])
             results_str = results_str or "None"
             self._logger.info(f"Current constraints: {results_str}")
 
-            if not click.confirm("Do you want to add a constraint?", default=False):
+            if not confirm("Do you want to add a constraint?", default=False):
                 return results
 
             target_options = [Option(id=target[0], label=target[1]) for target in self.available_targets]
             target = self._logger.prompt_list("Select a constraint target", target_options)
 
             operator = self._logger.prompt_list("Select a constraint operator (<value> will be asked after this)", [
                 Option(id=OptimizationConstraintOperator.Less, label="Less than <value>"),
                 Option(id=OptimizationConstraintOperator.LessOrEqual, label="Less than or equal to <value>"),
                 Option(id=OptimizationConstraintOperator.Greater, label="Greater than <value>"),
                 Option(id=OptimizationConstraintOperator.GreaterOrEqual, label="Greater than or equal to <value>"),
                 Option(id=OptimizationConstraintOperator.Equals, label="Equal to <value>"),
                 Option(id=OptimizationConstraintOperator.NotEqual, label="Not equal to <value>")
             ])
 
-            value = click.prompt("Set the <value> for the selected operator", type=click.FLOAT)
+            value = prompt("Set the <value> for the selected operator", type=FLOAT)
 
             results.append(OptimizationConstraint(**{"target": target, "operator": operator, "target-value": value}))
 
     def configure_node(self) -> Tuple[NodeType, int]:
         """Asks the user for the node type and number of parallel nodes to run on.
 
         :return: the type of the node and the amount of parallel nodes to run
         """
         node_options = [
             Option(id=node, label=f"{node.name} ({node.cores} cores, {node.ram} GB RAM) @ ${node.price:.2f} per hour")
             for node in available_nodes
         ]
 
         node = self._logger.prompt_list("Select the optimization node type", node_options)
-        parallel_nodes = click.prompt(f"How many nodes should run in parallel ({node.min_nodes}-{node.max_nodes})",
-                                      type=click.IntRange(min=node.min_nodes, max=node.max_nodes),
+        parallel_nodes = prompt(f"How many nodes should run in parallel ({node.min_nodes}-{node.max_nodes})",
+                                      type=IntRange(min=node.min_nodes, max=node.max_nodes),
                                       default=node.default_nodes)
 
         return node, parallel_nodes
 
     def parse_target(self, target: str) -> str:
         """Parses a target given by the user.
 
         Converts a target like "Sharpe Ratio" into "TotalPerformance.PortfolioStatistics.SharpeRatio".
 
         :param target: the target given by the user
         :return: the target in a way it can be passed to the optimizer
         """
         if "." in target:
             return target
+        from re import sub
 
         # Turn "SharpeRatio" into "Sharpe Ratio" so the title() call doesn't lowercase the R
-        target = re.sub(r"([A-Z])", r" \1", target)
+        target = sub(r"([A-Z])", r" \1", target)
 
         return f"TotalPerformance.PortfolioStatistics.{target.title().replace(' ', '')}"
 
     def parse_parameters(self, parameters: List[Tuple[str, float, float, float]]) -> List[OptimizationParameter]:
         """Parses a list of parameters given by the user into a list of parameter objects.
 
         :param parameters: the parameters given by the user
```

### Comparing `lean-1.0.99/lean/components/config/__init__.py` & `lean-1.155/lean/models/brokerages/__init__.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/components/config/project_config_manager.py` & `lean-1.155/lean/components/config/project_config_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import random
 from pathlib import Path
 from typing import List
 
 from lean.components.config.storage import Storage
 from lean.components.util.xml_manager import XMLManager
 from lean.constants import PROJECT_CONFIG_FILE_NAME
 from lean.models.utils import CSharpLibrary
@@ -27,14 +26,25 @@
     def __init__(self, xml_manager: XMLManager) -> None:
         """Creates a new ProjectConfigManager instance.
 
         :param xml_manager: the XMLManager instance to use when parsing XML files
         """
         self._xml_manager = xml_manager
 
+    def try_get_project_config(self, project_directory: Path) -> Storage:
+        """Returns a Storage instance to get/set the configuration for a project.
+
+        :param project_directory: the path to the project to retrieve the configuration of
+        :return: the Storage instance containing the project-specific configuration of the given project
+        """
+        if self.get_project_config(project_directory).file.exists():
+            return Storage(str(project_directory / PROJECT_CONFIG_FILE_NAME))
+        else:
+            return False
+
     def get_project_config(self, project_directory: Path) -> Storage:
         """Returns a Storage instance to get/set the configuration for a project.
 
         :param project_directory: the path to the project to retrieve the configuration of
         :return: the Storage instance containing the project-specific configuration of the given project
         """
         return Storage(str(project_directory / PROJECT_CONFIG_FILE_NAME))
@@ -48,15 +58,16 @@
         :return: the local id of the given project
         """
         project_config = self.get_project_config(project_directory)
 
         if project_config.has("local-id"):
             return project_config.get("local-id")
 
-        project_id = random.randint(100_000_000, 999_999_999)
+        from random import randint
+        project_id = randint(100_000_000, 999_999_999)
         project_config.set("local-id", project_id)
 
         return project_id
 
     def get_latest_live_directory(self, project_directory: Path) -> Path:
         """Returns the path of the latest live directory.
 
@@ -67,18 +78,18 @@
         if not live_root_dir.is_dir():
             raise ValueError(f"live directory {live_root_dir} is not a directory")
 
         for live_dir in sorted(list(live_root_dir.iterdir()), reverse=True):
             if not (live_dir / "log.txt").is_file():
                 continue
             return live_dir
-        
+
         raise ValueError("live directory with log.txt not found")
 
-        
+
     def get_csharp_libraries(self, project_directory: Path) -> List[CSharpLibrary]:
         """Returns the custom C# libraries in a project.
 
         :param project_directory: the path to the project to retrieve the C# libraries of
         :return: a list containing the information of all PackageReferences in the project's .csproj file, if any
         """
         csproj_file = next((p for p in project_directory.iterdir() if p.name.endswith(".csproj")), None)
```

### Comparing `lean-1.0.99/lean/components/__init__.py` & `lean-1.155/lean/models/addon_modules/addon_module.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,7 +6,15 @@
 # You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+from lean.models.lean_config_configurer import LeanConfigConfigurer
+
+class AddonModule(LeanConfigConfigurer):
+    """A JsonModule implementation for add on modules."""
+
+
+
```

### Comparing `lean-1.0.99/lean/components/util/click_group_default_command.py` & `lean-1.155/lean/components/util/click_group_default_command.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import click
+from click import Group
 
-class DefaultCommandGroup(click.Group):
+class DefaultCommandGroup(Group):
     """allow a default command for a group"""
 
     def command(self, *args, **kwargs):
         default_command = kwargs.pop('default_command', False)
         if default_command and not args:
             kwargs['name'] = kwargs.get('name', '<>')
         decorator = super(
@@ -34,12 +34,12 @@
         return decorator
 
     def resolve_command(self, ctx, args):
         try:
             # test if the command parses
             return super(
                 DefaultCommandGroup, self).resolve_command(ctx, args)
-        except click.UsageError:
+        except Exception as e:
             # command did not parse, assume it is the default command
             args.insert(0, self.default_command)
             return super(
-                DefaultCommandGroup, self).resolve_command(ctx, args)
+                DefaultCommandGroup, self).resolve_command(ctx, args)
```

### Comparing `lean-1.0.99/lean/components/util/http_client.py` & `lean-1.155/lean/components/util/http_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,107 +7,103 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
-
-import requests
 
 from lean.components.util.logger import Logger
 
 
 class HTTPClient:
     """The HTTPClient class is a lightweight wrapper around the requests library with additional logging."""
 
     def __init__(self, logger: Logger) -> None:
         """Creates a new HTTPClient instance.
 
         :param logger: the logger to log debug messages with
         """
         self._logger = logger
 
-    def get(self, url: str, **kwargs) -> requests.Response:
+    def get(self, url: str, **kwargs):
         """A wrapper around requests.get().
 
         An error is raised if the response is unsuccessful unless kwargs["raise_for_status"] == False.
 
         :param url: the request url
         :param kwargs: any kwargs to pass on to requests.get()
         :return: the response of the request
         """
-        self._log_request("GET", url, **kwargs)
-
-        raise_for_status = kwargs.pop("raise_for_status", True)
-        response = requests.get(url, **kwargs)
-
-        self._check_response(response, raise_for_status)
-        return response
+        return self.request("GET", url, **kwargs)
 
-    def post(self, url: str, **kwargs) -> requests.Response:
+    def post(self, url: str, **kwargs):
         """A wrapper around requests.post().
 
         An error is raised if the response is unsuccessful unless kwargs["raise_for_status"] == False.
 
         :param url: the request url
         :param kwargs: any kwargs to pass on to requests.post()
         :return: the response of the request
         """
-        self._log_request("POST", url, **kwargs)
+        return self.request("POST", url, **kwargs)
 
-        raise_for_status = kwargs.pop("raise_for_status", True)
-        response = requests.post(url, **kwargs)
-
-        self._check_response(response, raise_for_status)
-        return response
-
-    def request(self, method: str, url: str, **kwargs) -> requests.Response:
+    def request(self, method: str, url: str, **kwargs):
         """A wrapper around requests.request().
 
         An error is raised if the response is unsuccessful unless kwargs["raise_for_status"] == False.
 
         :param method: the request method
         :param url: the request url
         :param kwargs: any kwargs to pass on to requests.request()
         :return: the response of the request
         """
+        from requests import request, exceptions
+
         self._log_request(method, url, **kwargs)
 
         raise_for_status = kwargs.pop("raise_for_status", True)
-        response = requests.request(method, url, **kwargs)
+        try:
+            response = request(method, url, **kwargs)
+        except exceptions.SSLError as e:
+            raise Exception(f"""
+Detected SSL error, this might be due to custom certificates in your environment or system trust store.
+A known limitation of the python requests implementation.
+Please consider installing library https://pypi.org/project/python-certifi-win32/.
+Related issue https://github.com/psf/requests/issues/2966
+    """.strip())
 
         self._check_response(response, raise_for_status)
         return response
 
-    def log_unsuccessful_response(self, response: requests.Response) -> None:
+    def log_unsuccessful_response(self, response) -> None:
         """Logs an unsuccessful response's status code and body.
 
         :param response: the response to log
         """
         body = f"body:\n{response.text}" if response.text != "" else "empty body"
         self._logger.debug(f"Request was not successful, status code {response.status_code}, {body}")
 
     def _log_request(self, method: str, url: str, **kwargs) -> None:
         """Logs a request.
 
         :param method: the request method
         :param url: the request url
         :param kwargs: any kwargs passed to a request.* method
         """
+        from json import dumps
         message = f"--> {method.upper()} {url}"
 
         data = next((kwargs.get(key) for key in ["json", "data", "params"] if key in kwargs), None)
         if data is not None and data != {}:
-            message += f" with data:\n{json.dumps(data, indent=4)}"
+            message += f" with data:\n{dumps(data, indent=4)}"
 
         self._logger.debug(message)
 
-    def _check_response(self, response: requests.Response, raise_for_status: bool) -> None:
+    def _check_response(self, response, raise_for_status: bool) -> None:
         """Checks a response, logging a debug message if it wasn't successful.
 
         :param response: the response to check
         :param raise_for_status: True if an error needs to be raised if the request wasn't successful, False if not
         """
         if response.status_code < 200 or response.status_code >= 300:
             self.log_unsuccessful_response(response)
```

### Comparing `lean-1.0.99/lean/components/util/click_custom_parameters.py` & `lean-1.155/lean/components/util/click_custom_parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import click
+from click import ParamType
 from decimal import Decimal, DecimalException
 
-class DecimalParamType(click.ParamType):
+class DecimalParamType(ParamType):
     name = "decimal"
 
     def convert(self, value, param, ctx):
         try:
             return Decimal(value)
         except DecimalException:
             self.fail(f"{value!r} is not a valid decimal", param, ctx)
 
-DECIMAL = DecimalParamType()
+DECIMAL = DecimalParamType()
```

### Comparing `lean-1.0.99/lean/components/util/logger.py` & `lean-1.155/lean/components/util/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,32 +7,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
-import platform
-import sys
 from typing import Any, List, Optional
 
-import click
-import maskpass
-from rich.console import Console
-from rich.progress import BarColumn, Progress, TextColumn
+from click import prompt
 
 from lean.models.logger import Option
 
 
 class Logger:
     """The Logger class handles all output printing."""
 
     def __init__(self) -> None:
         """Creates a new Logger instance."""
+        from rich.console import Console
         self._console = Console(markup=False, highlight=False, emoji=False, width=None)
         self.debug_logging_enabled = False
 
     def debug(self, message: Any) -> None:
         """Logs a debug message if debug logging is enabled.
 
         :param message: the message to log
@@ -57,21 +52,22 @@
     def error(self, message: Any) -> None:
         """Logs an error message.
 
         :param message: the message to log
         """
         self._console.print(message, style="red")
 
-    def progress(self, prefix: str = "", suffix: str = "{task.percentage:0.0f}%") -> Progress:
+    def progress(self, prefix: str = "", suffix: str = "{task.percentage:0.0f}%"):
         """Creates a Progress instance.
 
         :param prefix: the text to show before the bar (defaults to a blank string)
         :param suffix: the text to show after the bar (defaults to the task's percentage)
         :return: a Progress instance which can be used to display progress bars
         """
+        from rich.progress import BarColumn, Progress, TextColumn
         progress = Progress(TextColumn(prefix), BarColumn(), TextColumn(suffix), console=self._console)
         progress.start()
         return progress
 
     def prompt_list(self, text: str, options: List[Option], default: Optional[str] = None, multiple: bool = False) -> Any:
         """Asks the user to select an option from a list of possible options.
 
@@ -100,45 +96,50 @@
 
         self.info(f"{text}:")
         for i, option in enumerate(options):
             self.info(f"{i + 1}) {option.label}")
 
         while True:
             if not multiple:
-                user_input = click.prompt("Enter an option", type=str, default=default, show_default=True)
+                user_input = prompt("Enter an option", type=str, default=default, show_default=True)
                 user_selected_value = validate_option(user_input)
                 if user_selected_value is not None:
                     return user_selected_value
             else:
                 user_selected_values = []
-                user_inputs = click.prompt("To enter multiple options, separate them with comma.", type=str, default=default, show_default=True)
+                user_inputs = prompt("To enter multiple options, separate them with comma.", type=str, default=default, show_default=True)
                 user_inputs = str(user_inputs).strip(",").split(",")
                 expected_outputs = len(user_inputs)
                 for user_input in user_inputs:
                     user_selected_value = validate_option(user_input)
                     if user_selected_value is not None:
                         user_selected_values.append(user_selected_value)
                 if len(user_selected_values) == expected_outputs:
                     return user_selected_values
 
-    def prompt_password(self, text: str, default: Optional[str] = None) -> str:
+    def prompt_password(self, text: str, default: Optional[str] = None, hide_input: bool = True) -> str:
         """Asks the user for a string value while masking the given input.
 
         :param text: the text to display before prompting
         :param default: the default value if no input is given
+        :param hide_input: whether to hide the input
         :return: the given input
         """
+        from platform import uname
+        from sys import stdin
+        from maskpass import askpass
+
         if default is not None:
             text = f"{text} [{'*' * len(default)}]"
 
         # Masking does not work properly in WSL2 and when the input is not coming from a keyboard
-        if "microsoft" in platform.uname().release.lower() or not sys.stdin.isatty():
-            return click.prompt(text, default=default, show_default=False)
+        if "microsoft" in uname().release.lower() or not stdin.isatty() or not hide_input:
+            return prompt(text, default=default, show_default=False, hide_input=hide_input)
 
         while True:
-            user_input = maskpass.askpass(f"{text}: ")
+            user_input = askpass(f"{text}: ")
 
             if len(user_input) == 0 and default is not None:
                 return default
 
             if len(user_input) > 0:
                 return user_input
```

### Comparing `lean-1.0.99/lean/components/util/compiler.py` & `lean-1.155/lean/components/util/compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,37 +7,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
+from json import dumps
 from typing import Dict, Any
 from lean.container import container
-import sys
-import io
-from contextlib import redirect_stdout
-import re
-
-docker_manager = container.docker_manager()
-project_manager = container.project_manager()
-lean_runner = container.lean_runner()
-temp_manager = container.temp_manager()
-project_config_manager = container.project_config_manager()
-cli_config_manager = container.cli_config_manager()
-logger = container.logger()
+from pathlib import Path
+
+docker_manager = container.docker_manager
+project_manager = container.project_manager
+lean_runner = container.lean_runner
+temp_manager = container.temp_manager
+project_config_manager = container.project_config_manager
+cli_config_manager = container.cli_config_manager
+logger = container.logger
 
 
 def get_success() -> Dict[str, Any]:
     """Compiles success message.
 
     :return: success object as json dump.
     """
-    return json.dumps({
+    return dumps({
         "eType": "BuildSuccess",
     })
 
 
 def get_errors(algorithm_type: str, message: str, color_coding_required: bool = True,
                                         warning_required: bool = True) -> Dict[str, Any]:
     """Compiles error message based on given input
@@ -48,87 +45,94 @@
     """
     errors = []
     if algorithm_type == "csharp":
         errors.extend(_parse_csharp_errors(message, color_coding_required, warning_required))
     elif algorithm_type == "python":
         errors.extend(_parse_python_errors(message, color_coding_required))
 
-    return json.dumps({
+    return dumps({
         "eType": "BuildError",
         "aErrors": errors,
     })
 
 
 def redirect_stdout_of_subprocess(method_name_to_run, *args, **kwargs) -> tuple:
     """ It captures the stdout of the method given to run.
 
     :param method_name_to_run: name of the method to run
     :return: result of the method and the stdout of the process
     """
-    f = io.StringIO()
+    from io import StringIO
+    from contextlib import redirect_stdout
+    f = StringIO()
     with redirect_stdout(f):
         result = method_name_to_run(*args, **kwargs)
     stdout = f.getvalue()
     return (result, stdout)
 
 
 def compile() -> None:
     """This is a utility function that is used by the vscode plugin project.
     """
 
     # We need to print the stdout of the docker run command from here,
-    # so that it can be picked up by the subprocess that is being 
+    # so that it can be picked up by the subprocess that is being
     # called by the vscode plugin.
     compile_result, stdout = redirect_stdout_of_subprocess(_compile)
     if compile_result["result"]:
         processed_output = get_success()
     else:
         processed_output = get_errors(compile_result["algorithmType"], stdout, False, False)
     logger.info(processed_output)
 
 
 def _compile() -> Dict[str, Any]:
     """
     This function compile c# and python project files.
     """
+    from sys import argv
+
     message = {
         "result": False,
         "algorithmType": "",
     }
 
-    project_id = int(sys.argv[-1])
-    project_dir = project_manager.get_project_by_id(project_id)
+    project_dir = Path(argv[-1])
+    if not project_dir.exists():
+        raise(f"Project directory {project_dir} does not exist")
+
     algorithm_file = project_manager.find_algorithm_file(project_dir)
     message["algorithmType"] = "python" if algorithm_file.name.endswith(".py") else "csharp"
 
     # The dict containing all options passed to `docker run`
     # See all available options at https://docker-py.readthedocs.io/en/stable/containers.html
     run_options: Dict[str, Any] = {
         "commands": [],
         "environment": {},
         "mounts": [],
         "volumes": {}
     }
-
+    lean_runner.mount_project_and_library_directories(project_dir, run_options)
     lean_runner.setup_language_specific_run_options(run_options, project_dir, algorithm_file, False, False)
 
     project_config = project_config_manager.get_project_config(project_dir)
     engine_image = cli_config_manager.get_engine_image(
         project_config.get("engine-image", None))
 
     message["result"] = docker_manager.run_image(engine_image, **run_options)
     temp_manager.delete_temporary_directories_when_done = False
     return message
 
 def _parse_csharp_errors(csharp_output: str, color_coding_required: bool, warning_required: bool) -> list:
+    from re import findall
     errors = []
 
     try:
         relevant_output = csharp_output[csharp_output.index("Build FAILED."):]
-        for match in re.findall(r"(.*)\((\d+),(\d+)\): (error|warning) ([a-zA-Z0-9]+): ([^[]+) ", relevant_output):
+        for match in findall(r"(.*)\((\d+),(\d+)\): (error|warning) ([a-zA-Z0-9]+): ([^[]+) ", relevant_output):
             if color_coding_required:
                 if match[3] == "error":
                     errors.append(f'{bcolors.FAIL}{match[3]} File: {match[0].split("/")[-1]} Line {match[1]} Column {match[2]} - {match[5]}{bcolors.ENDC}\n')
                 elif warning_required:
                     errors.append(f'{bcolors.WARNING}{match[3]}: {match[0].split("/")[-1]} Line {match[1]} Column {match[2]} - {match[5]}{bcolors.ENDC}\n')
             else:
                 if match[3] == "warning" and not warning_required:
@@ -136,37 +140,38 @@
                 errors.append(f'{match[3]}: {match[0].split("/")[-1]} Line {match[1]} Column {match[2]} - {match[5]}\n')
     except Exception:
         pass
 
     return errors
 
 def _parse_python_errors(python_output: str, color_coding_required: bool) -> list:
+    from re import findall
     errors = []
 
     try:
-        for match in re.findall(r'\*\*\*   File "/LeanCLI/([^"]+)", line (\d+)\n.*\n(.*)\^.*\n(.*)', python_output):
+        for match in findall(r'\*\*\*   File "/LeanCLI/([^"]+)", line (\d+)\n.*\n(.*)\^.*\n(.*)', python_output):
             if color_coding_required:
                 errors.append(f"{bcolors.FAIL}Build Error File: {match[0]} Line {match[1]} Column {match[2]} - {match[3]}{bcolors.ENDC}\n")
             else:
                 errors.append(f"Build Error File: {match[0]} Line {match[1]} Column {match[2]} - {match[3]}\n")
 
         for match in re.findall(r"\*\*\* Sorry: ([^(]+) \(([^,]+), line (\d+)\)", python_output):
             if color_coding_required:
                 errors.append(f"{bcolors.FAIL}Build Error File: {match[1]} Line {match[2]} Column 0 - {match[0]}{bcolors.ENDC}\n")
             else:
                 errors.append(f"Build Error File: {match[1]} Line {match[2]} Column 0 - {match[0]}\n")
     except Exception:
         pass
-    
+
     return errors
 
 
 class bcolors:
     HEADER = '\033[95m'
     OKBLUE = '\033[94m'
     OKCYAN = '\033[96m'
     OKGREEN = '\033[92m'
     WARNING = '\033[33m'
     FAIL = '\033[31m'
     ENDC = '\033[0m'
     BOLD = '\033[1m'
-    UNDERLINE = '\033[4m'
+    UNDERLINE = '\033[4m'
```

### Comparing `lean-1.0.99/lean/components/util/platform_manager.py` & `lean-1.155/lean/components/util/platform_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
-import platform
 
 
 class PlatformManager:
     """The PlatformManager class makes it easy to detect which platform the user is using."""
 
     def __init__(self) -> None:
         """Creates a new PlatformManager instance."""
-        self._system = platform.system()
-        self._machine = platform.machine()
-        self._host_system = os.environ.get("QC_DOCKER_HOST_SYSTEM", None)
-        self._host_machine = os.environ.get("QC_DOCKER_HOST_MACHINE", None)
+        from os import environ
+        from platform import system, machine
+        self._system = system()
+        self._machine = machine()
+        self._host_system = environ.get("QC_DOCKER_HOST_SYSTEM", None)
+        self._host_machine = environ.get("QC_DOCKER_HOST_MACHINE", None)
 
     def is_system_windows(self) -> bool:
         """Returns whether the current system is running Windows.
 
         If this method is called inside Docker, it returns whether the Docker container is running Windows.
 
         :return: whether the current system is running Windows
```

### Comparing `lean-1.0.99/lean/components/util/task_manager.py` & `lean-1.155/lean/components/util/task_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import time
 from typing import Callable, List, Optional, TypeVar
 
 from lean.components.util.logger import Logger
 from lean.models.pydantic import WrappedBaseModel
 
 T = TypeVar("T")
 
@@ -92,15 +91,16 @@
                     progress.update(progress_task, completed=get_progress(data) * 100)
 
                 if is_done(data):
                     if progress is not None:
                         progress.stop()
                     return data
 
-                time.sleep(intervals[current_interval_index].interval_seconds)
+                from time import sleep
+                sleep(intervals[current_interval_index].interval_seconds)
 
                 poll_counter += 1
                 if poll_counter == intervals[current_interval_index].interval_uses:
                     current_interval_index += 1
                     poll_counter = 0
         except KeyboardInterrupt as e:
             if progress is not None:
```

### Comparing `lean-1.0.99/lean/components/util/xml_manager.py` & `lean-1.155/lean/components/util/xml_manager.py`

 * *Files identical despite different names*

### Comparing `lean-1.0.99/lean/components/util/update_manager.py` & `lean-1.155/lean/components/util/update_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,26 +7,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import hashlib
-import os
-from datetime import datetime, timedelta, timezone
-from distutils.version import StrictVersion
-
-import requests
-from docker.errors import APIError
-from rich import box
-from rich.panel import Panel
-from rich.table import Table
-
-import lean
 from lean.components.config.storage import Storage
 from lean.components.docker.docker_manager import DockerManager
 from lean.components.util.http_client import HTTPClient
 from lean.components.util.logger import Logger
 from lean.constants import (UPDATE_CHECK_INTERVAL_ANNOUNCEMENTS, UPDATE_CHECK_INTERVAL_CLI,
                             UPDATE_CHECK_INTERVAL_DOCKER_IMAGE)
 from lean.models.docker import DockerImage
@@ -55,47 +43,58 @@
     def warn_if_cli_outdated(self, force: bool = False) -> None:
         """Warns the user if the CLI is outdated.
 
         An update check is performed once every UPDATE_CHECK_INTERVAL_CLI hours, unless force is set to True.
 
         :param force: whether the update check interval should be bypassed (defaults to False)
         """
-        current_version = lean.__version__
+        from lean import __version__
+        current_version = __version__
 
         # A development version is never considered outdated
         if current_version == "dev":
             return
 
         if not force and not self._should_check_for_updates("cli", UPDATE_CHECK_INTERVAL_CLI):
             return
 
+        from requests import exceptions
         try:
             response = self._http_client.get("https://pypi.org/pypi/lean/json", raise_for_status=False)
-        except requests.exceptions.ConnectionError:
+        except exceptions.ConnectionError:
             # The user may be offline, do nothing
             return
 
         if not response.ok:
             return
 
         latest_version = response.json()["info"]["version"]
+        from distutils.version import StrictVersion
 
         if StrictVersion(latest_version) > StrictVersion(current_version):
             self._logger.warn(f"A new release of the Lean CLI is available ({current_version} -> {latest_version})")
             self._logger.warn("Run `pip install --upgrade lean` to update to the latest version")
 
-    def pull_docker_image_if_necessary(self, image: DockerImage, force: bool) -> None:
+    def pull_docker_image_if_necessary(self, image: DockerImage, force: bool, no_update = False) -> None:
         """Pulls a Docker image if necessary.
 
         Docker images are pulled when they are not installed yet,
         and once every UPDATE_CHECK_INTERVAL_DOCKER_IMAGE hours (the interval is per image).
 
         :param image: the image to pull
         :param force: skip the interval check to force a pull
+        :param no_update: do not pull the image
         """
+
+        if no_update:
+            if not force:
+                return
+            self._logger.warn("Both --no-update and --update were specified, ignoring --no-update")
+
+        from docker.errors import APIError
         if not force and self._docker_manager.image_installed(image):
             if not self._should_check_for_updates(str(image), UPDATE_CHECK_INTERVAL_DOCKER_IMAGE):
                 return
 
             local_digest = self._docker_manager.get_local_digest(image)
 
             # If the local digest does not exist the image was built locally so there is nothing to pull
@@ -115,32 +114,38 @@
         self._docker_manager.pull_image(image)
 
     def show_announcements(self) -> None:
         """Shows the announcements if they have been updated.
 
         We check for new announcements once every UPDATE_CHECK_INTERVAL_ANNOUNCEMENTS hours.
         """
+        from requests import exceptions
+        from hashlib import md5
+        from rich import box
+        from rich.panel import Panel
+        from rich.table import Table
+
         if not self._should_check_for_updates("announcements", UPDATE_CHECK_INTERVAL_ANNOUNCEMENTS):
             return
 
         try:
             response = self._http_client.get(
                 "https://raw.githubusercontent.com/QuantConnect/lean-cli/master/announcements.json",
                 raise_for_status=False
             )
-        except requests.exceptions.ConnectionError:
+        except exceptions.ConnectionError:
             # The user may be offline, do nothing
             return
 
         if not response.ok:
             return
 
         hash_cache_key = "last-announcements-hash"
 
-        remote_hash = hashlib.md5(response.content).hexdigest()
+        remote_hash = md5(response.content).hexdigest()
         local_hash = self._cache_storage.get(hash_cache_key, None)
 
         if local_hash == remote_hash:
             return
 
         self._cache_storage.set(hash_cache_key, remote_hash)
 
@@ -162,14 +167,16 @@
 
         When this method returns True, for the next <interval_hours> hours it returns False for <key>.
 
         :param key: the key which is used to identify the current update check
         :param interval_hours: the amount of hours between update checks for the given key
         :return: True if an update check should be performed, False if not
         """
+        from datetime import datetime, timedelta, timezone
+
         storage_key = f"last-update-check-{key}"
         should_check = False
 
         if not self._cache_storage.has(storage_key):
             # Perform an update check if we haven't ran one yet
             should_check = True
         else:
```

### Comparing `lean-1.0.99/lean/components/util/temp_manager.py` & `lean-1.155/lean/components/util/temp_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,36 +7,35 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import shutil
-import tempfile
 from pathlib import Path
 
-
 class TempManager:
     """The TempManager class provides access to temporary directories."""
 
     def __init__(self) -> None:
         """Creates a new TempManager instance."""
         self._temporary_directories = []
         self.delete_temporary_directories_when_done = True
 
     def create_temporary_directory(self) -> Path:
         """Returns the path to an empty temporary directory.
 
         :return: a path to an empty temporary directory
         """
-        path = Path(tempfile.mkdtemp(prefix="lean-cli-"))
+        from tempfile import mkdtemp
+        path = Path(mkdtemp(prefix="lean-cli-"))
         self._temporary_directories.append(path)
         return path
 
     def delete_temporary_directories(self) -> None:
         """Deletes temporary directories that were created while the CLI ran.
 
         Only the files that the user can delete are deleted, any permission errors are ignored.
         """
+        from shutil import rmtree
         for path in self._temporary_directories:
-            shutil.rmtree(path, ignore_errors=True)
+            rmtree(path, ignore_errors=True)
```

### Comparing `lean-1.0.99/lean/components/util/name_extraction.py` & `lean-1.155/lean/components/util/name_extraction.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import re
 from pathlib import Path
 
 def _capitalize(word: str) -> str:
     """Capitalizes the given word.
 
     :param word: the word to capitalize
     :return: the word with the first letter capitalized (any other uppercase characters are preserved)
@@ -27,8 +26,9 @@
 
 def convert_to_class_name(file_path: Path):
     """Converts the project name into a valid class name by removing all non-alphanumeric characters
 
     :param file_path: Path to the root project
     :return: returns a valid class name
     """
-    return re.sub(f"[^a-zA-Z0-9]", "", "".join(map(_capitalize, file_path.name.split(" "))))
+    from re import sub
+    return sub(f"[^a-zA-Z0-9]", "", "".join(map(_capitalize, file_path.name.split(" "))))
```

### Comparing `lean-1.0.99/lean/components/util/name_generator.py` & `lean-1.155/lean/components/util/name_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from random import choice
-
 
 class NameGenerator:
     """The NameGenerator generates random names."""
 
     def __init__(self) -> None:
         """Creates a new NameGenerator instance."""
         self._verbs = ["Determined", "Pensive", "Adaptable", "Calculating", "Logical", "Energetic", "Creative",
@@ -42,8 +40,9 @@
                          "Donkey", "Manatee", "Shark", "Bear", "kitten", "Fly", "Ant", "Sardine"]
 
     def generate_name(self) -> str:
         """Returns a random name.
 
         :return: a random name containing multiple words
         """
+        from random import choice
         return f"{choice(self._verbs)} {choice(self._colors)} {choice(self._animals)}"
```

### Comparing `lean-1.0.99/lean/components/util/market_hours_database.py` & `lean-1.155/lean/components/util/market_hours_database.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
-import re
 from typing import Dict, Optional, Any
 
 from lean.components.config.lean_config_manager import LeanConfigManager
 from lean.models.api import QCSecurityType
 from lean.models.market_hours_database import MarketHoursDatabaseEntry
 
 
@@ -52,19 +50,21 @@
         raise ValueError(f"Could not find entry in market hours database, checked following keys: {keys_to_check}")
 
     def _get_all_entries(self) -> Dict[str, MarketHoursDatabaseEntry]:
         """Reads the market hours database and returns all unparsed entries by name.
 
         :return: a dict containing all unparsed market hours database entries by name
         """
+        from re import sub, DOTALL
+        from json import loads
         if self._entries is not None:
             return self._entries
 
         data_dir = self._lean_config_manager.get_data_directory()
         market_hours_database_path = data_dir / "market-hours" / "market-hours-database.json"
 
         market_hours_database = market_hours_database_path.read_text(encoding="utf-8")
-        market_hours_database = re.sub(r"(/\*.*\*/)", "", market_hours_database, flags=re.DOTALL)
-        market_hours_database = json.loads(market_hours_database)
+        market_hours_database = sub(r"(/\*.*\*/)", "", market_hours_database, flags=DOTALL)
+        market_hours_database = loads(market_hours_database)
 
         self._entries = market_hours_database["entries"]
         return self._entries
```

### Comparing `lean-1.0.99/lean/constants.py` & `lean-1.155/lean/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,19 +7,36 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
+from os import environ
 from pathlib import Path
 
 # Due to the way the filesystem is mocked in unit tests, values should not be Path instances.
 
+# Custom images names
+CUSTOM_FOUNDATION = "lean-cli/foundation"
+CUSTOM_ENGINE = "lean-cli/engine"
+CUSTOM_RESEARCH = "lean-cli/research"
+
+# The python version of docker image
+LEAN_PYTHON_VERSION = "3.8"
+
+# The strict python version of docker image
+LEAN_STRICT_PYTHON_VERSION =  f"{LEAN_PYTHON_VERSION}.13"
+
+# The path to the root python directory in docker image
+DOCKER_PYTHON_SITE_PACKAGES_PATH = f"/root/.local/lib/python{LEAN_PYTHON_VERSION}/site-packages"
+
+# The file in which general CLI configuration is stored
+LEAN_ROOT_PATH = "/Lean/Launcher/bin/Debug"
+
 # The file in which general CLI configuration is stored
 GENERAL_CONFIG_PATH = str(Path("~/.lean/config").expanduser())
 
 # The file in which credentials are stored
 CREDENTIALS_CONFIG_PATH = str(Path("~/.lean/credentials").expanduser())
 
 # The file in which we store when we last checked for updates
@@ -53,15 +70,15 @@
 # This caches the installation and makes subsequent backtests much faster
 # Because the site packages are not versioned, we cannot reuse the volume between algorithms with different requirements
 # This constant defines how many site packages volumes get created before old ones are removed
 SITE_PACKAGES_VOLUME_LIMIT = 10
 
 # The base url of the QuantConnect API
 # This url should end with a forward slash
-_qc_api = os.environ.get("QC_API", "")
+_qc_api = environ.get("QC_API", "")
 if _qc_api == "local":
     API_BASE_URL = "http://localhost:5612/api/v2/"
 elif _qc_api == "beta":
     API_BASE_URL = "https://beta.quantconnect.com/api/v2/"
 else:
     API_BASE_URL = "https://www.quantconnect.com/api/v2/"
 
@@ -73,39 +90,12 @@
 
 # The interval in hours at which the CLI checks for new announcements
 UPDATE_CHECK_INTERVAL_ANNOUNCEMENTS = 24
 
 # The product id of the Equity Security Master subscription
 EQUITY_SECURITY_MASTER_PRODUCT_ID = 37
 
-# The product id of the Equity Bulk Security Master subscription
-BULK_EQUITY_SECURITY_MASTER_PRODUCT_ID = 180
-
 # The product id of the Terminal Link module
 TERMINAL_LINK_PRODUCT_ID = 44
 
-# The product id of the Trading Technologies module
-TRADING_TECHNOLOGIES_PRODUCT_ID = 64
-
-# The product id of the Atreyu module
-ATREYU_PRODUCT_ID = 65
-
-# The product id of the Kraken module
-KRAKEN_PRODUCT_ID = 130
-
-# The product id of the FTX module
-FTX_PRODUCT_ID = 138
-
-# The product id of the ZERODHA module
-ZERODHA_PRODUCT_ID = 174
-
-# The product id of the Binance module
-BINANCE_PRODUCT_ID = 176
-
-# The product id of the SAMCO module
-SAMCO_PRODUCT_ID = 173
-
-# The product id of the Interactive Brokers module
-INTERACTIVE_BROKERS_PRODUCT_ID = 181
-
 # The name of the Docker network which all Lean CLI containers are ran on
 DOCKER_NETWORK = "lean_cli"
```

### Comparing `lean-1.0.99/setup.py` & `lean-1.155/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,27 +42,24 @@
         return f">={latest_version}"
     except:
         return ""
 
 
 # Production dependencies
 install_requires = [
-    "click~=8.0.4",
-    "requests~=2.27.1",
-    "json5~=0.9.8",
-    "docker~=5.0.3",
-    "rich~=9.10.0",
-    "dependency-injector~=4.39.1",
-    "pydantic~=1.8.2",
-    "python-dateutil~=2.8.2",
-    "lxml~=4.9.0",
-    "maskpass==0.3.6",
-    "joblib~=1.1.0",
-    "python-certifi-win32~=1.6",
-    "pyshortcuts~=1.8.2",
+    "click>=8.0.4",
+    "requests>=2.27.1",
+    "json5>=0.9.8",
+    "docker>=6.0.0",
+    "rich>=9.10.0",
+    "pydantic>=1.8.2",
+    "python-dateutil>=2.8.2",
+    "lxml>=4.9.0",
+    "maskpass>=0.3.6",
+    "joblib>=1.1.0",
     "wrapt~=1.14.1",
     "setuptools",
     f"quantconnect-stubs{get_stubs_version_range()}"
 ]
 
 setup(
     name="lean",
@@ -77,24 +74,24 @@
     package_data={
         "lean": ["ssh/*"]
     },
     entry_points={
         "console_scripts": ["lean=lean.main:main"]
     },
     install_requires=install_requires,
-    python_requires=">= 3.6",
+    python_requires=">= 3.7",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Financial and Insurance Industry",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9"
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10"
     ],
     project_urls={
-        "Documentation": "https://www.lean.io/docs/lean-cli/key-concepts/getting-started",
+        "Documentation": "https://www.lean.io/docs/v2/lean-cli/key-concepts/getting-started",
         "Source": "https://github.com/QuantConnect/lean-cli"
     },
 )
```

### Comparing `lean-1.0.99/README.md` & `lean-1.155/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 
 [![Build Status](https://github.com/QuantConnect/lean-cli/workflows/Build/badge.svg)](https://github.com/QuantConnect/lean-cli/actions?query=workflow%3ABuild)
 [![PyPI Version](https://img.shields.io/pypi/v/lean)](https://pypi.org/project/lean/)
 [![Project Status](https://img.shields.io/pypi/status/lean)](https://pypi.org/project/lean/)
 
 The Lean CLI is a cross-platform CLI aimed at making it easier to develop with the LEAN engine locally and in the cloud.
 
-Visit the [documentation website](https://www.lean.io/docs/lean-cli/key-concepts/getting-started) for comprehensive and up-to-date documentation.
+Visit the [documentation website](https://www.lean.io/docs/v2/lean-cli/key-concepts/getting-started) for comprehensive and up-to-date documentation.
 
 ## Highlights
 
-- [Project scaffolding](https://www.lean.io/docs/lean-cli/projects/project-management)
-- [Local autocomplete](https://www.lean.io/docs/lean-cli/projects/autocomplete)
-- [Local data downloading](https://www.lean.io/docs/lean-cli/datasets/downloading-quantconnect-data)
-- [Local backtesting](https://www.lean.io/docs/lean-cli/backtesting/deployment#02-Run-Local-Backtests)
-- [Local debugging](https://www.lean.io/docs/lean-cli/backtesting/debugging)
-- [Local research environment](https://www.lean.io/docs/lean-cli/research)
-- [Local optimization](https://www.lean.io/docs/lean-cli/optimization/deployment#02-Run-Local-Optimizations)
-- [Local live trading](https://www.lean.io/docs/lean-cli/live-trading/quantconnect-paper-trading#02-Deploy-Local-Algorithms)
-- [Local backtest report creation](https://www.lean.io/docs/lean-cli/backtesting/report#02-Generate-a-Report)
-- [Cloud synchronization](https://www.lean.io/docs/lean-cli/projects/cloud-synchronization)
-- [Cloud backtesting](https://www.lean.io/docs/lean-cli/backtesting/deployment#03-Run-Cloud-Backtests)
-- [Cloud optimization](https://www.lean.io/docs/lean-cli/optimization/deployment#03-Run-Cloud-Optimizations)
-- [Cloud live trading](https://www.lean.io/docs/lean-cli/live-trading/quantconnect-paper-trading#03-Deploy-Cloud-Algorithms)
+- [Project scaffolding](https://www.lean.io/docs/v2/lean-cli/projects/project-management)
+- [Local autocomplete](https://www.lean.io/docs/v2/lean-cli/projects/autocomplete)
+- [Local data downloading](https://www.lean.io/docs/v2/lean-cli/datasets/downloading-quantconnect-data)
+- [Local backtesting](https://www.lean.io/docs/v2/lean-cli/backtesting/deployment#02-Run-Local-Backtests)
+- [Local debugging](https://www.lean.io/docs/v2/lean-cli/backtesting/debugging)
+- [Local research environment](https://www.lean.io/docs/v2/lean-cli/research)
+- [Local optimization](https://www.lean.io/docs/v2/lean-cli/optimization/deployment#02-Run-Local-Optimizations)
+- [Local live trading](https://www.lean.io/docs/v2/lean-cli/live-trading/quantconnect-paper-trading#02-Deploy-Local-Algorithms)
+- [Local backtest report creation](https://www.lean.io/docs/v2/lean-cli/backtesting/report#02-Generate-a-Report)
+- [Cloud synchronization](https://www.lean.io/docs/v2/lean-cli/projects/cloud-synchronization)
+- [Cloud backtesting](https://www.lean.io/docs/v2/lean-cli/backtesting/deployment#03-Run-Cloud-Backtests)
+- [Cloud optimization](https://www.lean.io/docs/v2/lean-cli/optimization/deployment#03-Run-Cloud-Optimizations)
+- [Cloud live trading](https://www.lean.io/docs/v2/lean-cli/live-trading/quantconnect-paper-trading#03-Deploy-Cloud-Algorithms)
 
 ## Installation
 
 The CLI can be installed and updated by running `pip install --upgrade lean`.
 
 Note that many commands in the CLI require Docker to run. See [Get Docker](https://docs.docker.com/get-docker/) for instructions on how to install Docker for your operating system.
 
@@ -61,15 +61,15 @@
 2. Run `lean create-project "Project Name"` to create a new project with some basic code to get you started.
 3. Work on your strategy in `./Project Name`.
 4. Run `lean research "Project Name"` to start a Jupyter Lab session to perform research in.
 5. Run `lean backtest "Project Name"` to run a backtest whenever there's something to test. This runs your strategy in a Docker container containing the same packages as the ones used on QuantConnect.com, but with your own data.
 
 ## Commands
 
-*Note: the readme only contains the `--help` text of all commands. Visit the [documentation website](https://www.lean.io/docs/lean-cli/key-concepts/getting-started) for more comprehensive documentation.*
+*Note: the readme only contains the `--help` text of all commands. Visit the [documentation website](https://www.lean.io/docs/v2/lean-cli/key-concepts/getting-started) for more comprehensive documentation.*
 
 <!-- commands start -->
 - [`lean backtest`](#lean-backtest)
 - [`lean build`](#lean-build)
 - [`lean cloud backtest`](#lean-cloud-backtest)
 - [`lean cloud live`](#lean-cloud-live)
 - [`lean cloud live deploy`](#lean-cloud-live-deploy)
@@ -82,14 +82,15 @@
 - [`lean config get`](#lean-config-get)
 - [`lean config list`](#lean-config-list)
 - [`lean config set`](#lean-config-set)
 - [`lean config unset`](#lean-config-unset)
 - [`lean create-project`](#lean-create-project)
 - [`lean data download`](#lean-data-download)
 - [`lean data generate`](#lean-data-generate)
+- [`lean delete-project`](#lean-delete-project)
 - [`lean init`](#lean-init)
 - [`lean library add`](#lean-library-add)
 - [`lean library remove`](#lean-library-remove)
 - [`lean live`](#lean-live)
 - [`lean live add-security`](#lean-live-add-security)
 - [`lean live cancel-order`](#lean-live-cancel-order)
 - [`lean live deploy`](#lean-live-deploy)
@@ -97,14 +98,16 @@
 - [`lean live stop`](#lean-live-stop)
 - [`lean live submit-order`](#lean-live-submit-order)
 - [`lean live update-order`](#lean-live-update-order)
 - [`lean login`](#lean-login)
 - [`lean logout`](#lean-logout)
 - [`lean logs`](#lean-logs)
 - [`lean optimize`](#lean-optimize)
+- [`lean project-create`](#lean-project-create)
+- [`lean project-delete`](#lean-project-delete)
 - [`lean report`](#lean-report)
 - [`lean research`](#lean-research)
 - [`lean whoami`](#lean-whoami)
 
 ### `lean backtest`
 
 Backtest a project locally using Docker.
@@ -114,63 +117,72 @@
 
   Backtest a project locally using Docker.
 
   If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
   If PROJECT is a file, the algorithm in the specified file will be executed.
 
   Go to the following url to learn how to debug backtests locally using the Lean CLI:
-  https://www.lean.io/docs/lean-cli/backtesting/debugging
+  https://www.lean.io/docs/v2/lean-cli/backtesting/debugging
 
   By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
   can set the default engine image for all commands using `lean config set engine-image <image>`.
 
 Options:
   --output DIRECTORY              Directory to store results in (defaults to PROJECT/backtests/TIMESTAMP)
   -d, --detach                    Run the backtest in a detached Docker container and return immediately
-  --debug [pycharm|ptvsd|vsdbg|rider]
+  --debug [pycharm|ptvsd|vsdbg|rider|local-platform]
                                   Enable a certain debugging method (see --help for more information)
-  --data-provider [Terminal Link|QuantConnect|Local]
+  --data-provider [QuantConnect|Local|Terminal Link]
                                   Update the Lean configuration file to retrieve data from the given provider
+  --terminal-link-environment [Production|Beta]
+                                  The environment to run in
+  --terminal-link-server-host TEXT
+                                  The host of the TerminalLink server
+  --terminal-link-server-port INTEGER
+                                  The port of the TerminalLink server
+  --terminal-link-openfigi-api-key TEXT
+                                  The Open FIGI API key to use for mapping options
   --download-data                 Update the Lean configuration file to download data from the QuantConnect API, alias
                                   for --data-provider QuantConnect
   --data-purchase-limit INTEGER   The maximum amount of QCC to spend on downloading data during the backtest when using
                                   QuantConnect as data provider
   --release                       Compile C# projects in release configuration instead of debug
   --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
+  --python-venv TEXT              The path of the python virtual environment to be used
   --update                        Pull the LEAN engine image before running the backtest
   --backtest-name TEXT            Backtest name
+  --no-update                     Use the local LEAN engine image instead of pulling the latest version
   --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
   --verbose                       Enable debug logging
   --help                          Show this message and exit.
 ```
 
 _See code: [lean/commands/backtest.py](lean/commands/backtest.py)_
 
 ### `lean build`
 
-Build Docker images of your own version of LEAN and the Alpha Streams SDK.
+Build Docker images of your own version of LEAN.
 
 ```
 Usage: lean build [OPTIONS] [ROOT]
 
-  Build Docker images of your own version of LEAN and the Alpha Streams SDK.
+  Build Docker images of your own version of LEAN.
 
-  ROOT must point to a directory containing the LEAN repository and the Alpha Streams SDK repository:
-  https://github.com/QuantConnect/Lean & https://github.com/QuantConnect/AlphaStreams
+  ROOT must point to a directory containing the LEAN repository:
+  https://github.com/QuantConnect/Lean
 
   When ROOT is not given, the current directory is used as root directory.
 
   This command performs the following actions:
   1. The lean-cli/foundation:latest image is built from Lean/DockerfileLeanFoundation(ARM).
   2. LEAN is compiled in a Docker container using the lean-cli/foundation:latest image.
-  3. The Alpha Streams SDK is compiled in a Docker container using the lean-cli/foundation:latest image.
-  4. The lean-cli/engine:latest image is built from Lean/Dockerfile using lean-cli/foundation:latest as base image.
-  5. The lean-cli/research:latest image is built from Lean/DockerfileJupyter using lean-cli/engine:latest as base image.
-  6. The default engine image is set to lean-cli/engine:latest.
-  7. The default research image is set to lean-cli/research:latest.
+  3. The lean-cli/engine:latest image is built from Lean/Dockerfile using lean-cli/foundation:latest as base image.
+  4. The lean-cli/research:latest image is built from Lean/DockerfileJupyter using lean-cli/engine:latest as base image.
+  5. The default engine image is set to lean-cli/engine:latest.
+  6. The default research image is set to lean-cli/research:latest.
 
   When the foundation Dockerfile is the same as the official foundation Dockerfile, quantconnect/lean:foundation is used
   instead of building a custom foundation image.
 
 Options:
   --tag TEXT  The tag to apply to custom images (defaults to latest)
   --verbose   Enable debug logging
@@ -217,16 +229,14 @@
 
 Commands:
   deploy     Start live trading for a project in the cloud.
   liquidate  Stops live trading and liquidates existing positions for a certain project.
   stop       Stops live trading for a certain project without liquidating existing positions.
 ```
 
-_See code: [lean/commands/cloud/live.py](lean/commands/cloud/live.py)_
-
 ### `lean cloud live deploy`
 
 Start live trading for a project in the cloud.
 
 ```
 Usage: lean cloud live deploy [OPTIONS] PROJECT
 
@@ -236,44 +246,48 @@
 
   By default an interactive wizard is shown letting you configure the deployment. If --brokerage is given the command
   runs in non-interactive mode. In this mode the CLI does not prompt for input or confirmation. In non-interactive mode
   the options specific to the given brokerage are required, as well as --node, --auto-restart, --notify-order-events and
   --notify-insights.
 
 Options:
-  --brokerage [Paper Trading|Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Kraken|FTX]
+  --brokerage [Paper Trading|Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Trading Technologies|Kraken|TDAmeritrade]
                                   The brokerage to use
   --ib-user-name TEXT             Your Interactive Brokers username
   --ib-account TEXT               Your Interactive Brokers account id
   --ib-password TEXT              Your Interactive Brokers password
+  --ib-weekly-restart-utc-time TEXT
+                                  Weekly restart UTC time (hh:mm:ss). Each week on Sunday your algorithm is restarted at
+                                  this time, and will require 2FA verification. This is required by Interactive Brokers.
+                                  Use this option explicitly to override the default value.
   --ib-data-feed BOOLEAN          Whether the Interactive Brokers price data feed must be used instead of the
                                   QuantConnect price data feed
   --tradier-account-id TEXT       Your Tradier account id
   --tradier-access-token TEXT     Your Tradier access token
   --tradier-environment [live|paper]
                                   Whether the developer sandbox should be used
-  --oanda-environment [Practice|Trade]
-                                  The environment to run in, Practice for fxTrade Practice, Trade for fxTrade
   --oanda-account-id TEXT         Your OANDA account id
   --oanda-access-token TEXT       Your OANDA API token
+  --oanda-environment [Practice|Trade]
+                                  The environment to run in, Practice for fxTrade Practice, Trade for fxTrade
   --bitfinex-api-key TEXT         Your Bitfinex API key
   --bitfinex-api-secret TEXT      Your Bitfinex API secret
-  --gdax-use-sandbox [live|paper]
-                                  Whether the sandbox should be used
   --gdax-api-key TEXT             Your Coinbase Pro API key
   --gdax-api-secret TEXT          Your Coinbase Pro API secret
   --gdax-passphrase TEXT          Your Coinbase Pro API passphrase
+  --gdax-use-sandbox [live|paper]
+                                  Whether the sandbox should be used
   --binance-exchange-name [Binance|BinanceUS]
                                   Binance exchange name [Binance, BinanceUS]
-  --binance-use-testnet [live|paper]
-                                  Whether the testnet should be used
   --binance-api-key TEXT          Your Binance API key
   --binanceus-api-key TEXT        Your Binance API key
   --binance-api-secret TEXT       Your Binance API secret
   --binanceus-api-secret TEXT     Your Binance API secret
+  --binance-use-testnet [live|paper]
+                                  Whether the testnet should be used
   --zerodha-api-key TEXT          Your Kite Connect API key
   --zerodha-access-token TEXT     Your Kite Connect access token
   --zerodha-product-type [mis|cnc|nrml]
                                   MIS if you are targeting intraday products, CNC if you are targeting delivery
                                   products, NRML if you are targeting carry forward products
   --zerodha-trading-segment [equity|commodity]
                                   EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
@@ -285,38 +299,47 @@
   --samco-year-of-birth TEXT      Your year of birth (YYYY) registered with Samco
   --samco-product-type [mis|cnc|nrml]
                                   MIS if you are targeting intraday products, CNC if you are targeting delivery
                                   products, NRML if you are targeting carry forward products
   --samco-trading-segment [equity|commodity]
                                   EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                   commodities on MCX
+  --tt-user-name TEXT             Your Trading Technologies username
+  --tt-session-password TEXT      Your Trading Technologies session password
+  --tt-account-name TEXT          Your Trading Technologies account name
+  --tt-rest-app-key TEXT          Your Trading Technologies REST app key
+  --tt-rest-app-secret TEXT       Your Trading Technologies REST app secret
+  --tt-rest-environment TEXT      The REST environment to run in
+  --tt-order-routing-sender-comp-id TEXT
+                                  The order routing sender comp id to use
   --kraken-api-key TEXT           Your Kraken API key
   --kraken-api-secret TEXT        Your Kraken API secret
   --kraken-verification-tier [Starter|Intermediate|Pro]
                                   Your Kraken Verification Tier
-  --ftx-exchange-name [FTX|FTXUS]
-                                  FTX exchange name [FTX, FTXUS]
-  --ftx-api-key TEXT              Your FTX API key
-  --ftxus-api-key TEXT            Your FTX API key
-  --ftx-api-secret TEXT           Your FTX API secret
-  --ftxus-api-secret TEXT         Your FTX API secret
-  --ftx-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6|VIP1|VIP2|VIP3|MM1|MM2|MM3]
-                                  Your FTX Account Tier
-  --ftxus-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6|Tier7|Tier8|Tier9|VIP1|VIP2|MM1|MM2|MM3]
-                                  Your FTX Account Tier
+  --tdameritrade-api-key TEXT     Your TDAmeritrade API key
+  --tdameritrade-access-token TEXT
+                                  Your TDAmeritrade OAuth Access Token
+  --tdameritrade-account-number TEXT
+                                  Your TDAmeritrade account number
   --node TEXT                     The name or id of the live node to run on
   --auto-restart BOOLEAN          Whether automatic algorithm restarting must be enabled
   --notify-order-events BOOLEAN   Whether notifications must be sent for order events
   --notify-insights BOOLEAN       Whether notifications must be sent for emitted insights
   --notify-emails TEXT            A comma-separated list of 'email:subject' pairs configuring email-notifications
   --notify-webhooks TEXT          A comma-separated list of 'url:HEADER_1=VALUE_1:HEADER_2=VALUE_2:etc' pairs
                                   configuring webhook-notifications
   --notify-sms TEXT               A comma-separated list of phone numbers configuring SMS-notifications
+  --notify-telegram TEXT          A comma-separated list of 'user/group Id:token(optional)' pairs configuring telegram-
+                                  notifications
+  --live-cash-balance TEXT        A comma-separated list of currency:amount pairs of initial cash balance
+  --live-holdings TEXT            A comma-separated list of symbol:symbolId:quantity:averagePrice of initial portfolio
+                                  holdings
   --push                          Push local modifications to the cloud before starting live trading
   --open                          Automatically open the live results in the browser once the deployment starts
+  --show-secrets                  Show secrets as they are input
   --verbose                       Enable debug logging
   --help                          Show this message and exit.
 ```
 
 _See code: [lean/commands/cloud/live/deploy.py](lean/commands/cloud/live/deploy.py)_
 
 ### `lean cloud live liquidate`
@@ -422,15 +445,15 @@
 ```
 Usage: lean cloud push [OPTIONS]
 
   Push local projects to QuantConnect.
 
   This command overrides the content of cloud files with the content of their respective local counterparts.
 
-  This command will not delete cloud files which don't have a local counterpart.
+  This command will delete cloud files which don't have a local counterpart.
 
 Options:
   --project DIRECTORY  Path to the local project to push (all local projects if not specified)
   --verbose            Enable debug logging
   --help               Show this message and exit.
 ```
 
@@ -525,15 +548,15 @@
   --help     Show this message and exit.
 ```
 
 _See code: [lean/commands/config/unset.py](lean/commands/config/unset.py)_
 
 ### `lean create-project`
 
-Create a new project containing starter code.
+Alias for 'project-create'
 
 ```
 Usage: lean create-project [OPTIONS] NAME
 
   Create a new project containing starter code.
 
   If NAME is a path containing subdirectories those will be created automatically.
@@ -558,26 +581,25 @@
   Purchase and download data from QuantConnect Datasets.
 
   An interactive wizard will show to walk you through the process of selecting data, accepting the CLI API Access and
   Data Agreement and payment. After this wizard the selected data will be downloaded automatically.
 
   If --dataset is given the command runs in non-interactive mode. In this mode the CLI does not prompt for input or
   confirmation but only halts when the agreement must be accepted. In non-interactive mode all options specific to the
-  selected dataset as well as --organization are required.
+  selected dataset are required.
 
   See the following url for the data that can be purchased and downloaded with this command:
   https://www.quantconnect.com/datasets
 
 Options:
-  --dataset TEXT       The name of the dataset to download non-interactively
-  --organization TEXT  The name or id of the organization to purchase and download data with
-  --overwrite          Overwrite existing local data
-  --lean-config FILE   The Lean configuration file that should be used (defaults to the nearest lean.json)
-  --verbose            Enable debug logging
-  --help               Show this message and exit.
+  --dataset TEXT      The name of the dataset to download non-interactively
+  --overwrite         Overwrite existing local data
+  --lean-config FILE  The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose           Enable debug logging
+  --help              Show this message and exit.
 ```
 
 _See code: [lean/commands/data/download.py](lean/commands/data/download.py)_
 
 ### `lean data generate`
 
 Generate random market data.
@@ -612,14 +634,15 @@
   By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
   can set the default engine image for all commands using `lean config set engine-image <image>`.
 
 Options:
   --start [yyyyMMdd]              Start date for the data to generate in yyyyMMdd format  [required]
   --end [yyyyMMdd]                End date for the data to generate in yyyyMMdd format (defaults to today)
   --symbol-count INTEGER RANGE    The number of symbols to generate data for  [x>=0; required]
+  --tickers TEXT                  Comma separated list of tickers to use for generated data
   --security-type [Equity|Forex|Cfd|Future|Crypto|Option]
                                   The security type to generate data for (defaults to Equity)
   --resolution [Tick|Second|Minute|Hour|Daily]
                                   The resolution of the generated data (defaults to Minute)
   --data-density [Dense|Sparse|VerySparse]
                                   The density of the generated data (defaults to Dense)
   --include-coarse BOOLEAN        Whether coarse universe data should be generated for Equity data (defaults to True)
@@ -629,26 +652,46 @@
   --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
   --verbose                       Enable debug logging
   --help                          Show this message and exit.
 ```
 
 _See code: [lean/commands/data/generate.py](lean/commands/data/generate.py)_
 
+### `lean delete-project`
+
+Alias for 'project-delete'
+
+```
+Usage: lean delete-project [OPTIONS] PROJECT
+
+  Delete a project locally and in the cloud if it exists.
+
+  The project is selected by name or cloud id.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/delete_project.py](lean/commands/delete_project.py)_
+
 ### `lean init`
 
 Scaffold a Lean configuration file and data directory.
 
 ```
 Usage: lean init [OPTIONS]
 
   Scaffold a Lean configuration file and data directory.
 
 Options:
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
+  --organization TEXT             The name or id of the organization the Lean CLI will be scaffolded for
+  -l, --language [python|csharp]  The default language to use for new projects
+  --verbose                       Enable debug logging
+  --help                          Show this message and exit.
 ```
 
 _See code: [lean/commands/init.py](lean/commands/init.py)_
 
 ### `lean library add`
 
 Add a custom library to a project.
@@ -656,33 +699,37 @@
 ```
 Usage: lean library add [OPTIONS] PROJECT NAME
 
   Add a custom library to a project.
 
   PROJECT must be the path to the project.
 
-  NAME must be the name of a NuGet package (for C# projects) or of a PyPI package (for Python projects).
+  NAME must be either the name of a NuGet package (for C# projects), a PyPI package (for Python projects), or a path to
+  a Lean CLI library.
 
-  If --version is not given, the package is pinned to the latest compatible version. For C# projects, this is the latest
-  available version. For Python projects, this is the latest version compatible with Python 3.6 (which is what the
-  Docker images use).
+  If --version is not given, and the library is a NuGet or PyPI package the package, it is pinned to the latest
+  compatible version. For C# projects, this is the latest available version. For Python projects, this is the latest
+  version compatible with Python 3.8 (which is what the Docker images use). For Lean CLI library projects, this is
+  ignored.
 
   Custom C# libraries are added to your project's .csproj file, which is then restored if dotnet is on your PATH and the
   --no-local flag has not been given.
 
   Custom Python libraries are added to your project's requirements.txt file and are installed in your local Python
   environment so you get local autocomplete for the library. The last step can be skipped with the --no-local flag.
 
   C# example usage:
   $ lean library add "My CSharp Project" Microsoft.ML
   $ lean library add "My CSharp Project" Microsoft.ML --version 1.5.5
+  $ lean library add "My CSharp Project" "Library/My CSharp Library"
 
   Python example usage:
   $ lean library add "My Python Project" tensorflow
   $ lean library add "My Python Project" tensorflow --version 2.5.0
+  $ lean library add "My Python Project" "Library/My Python Library"
 
 Options:
   --version TEXT  The version of the library to add (defaults to latest compatible version)
   --no-local      Skip making changes to your local environment
   --verbose       Enable debug logging
   --help          Show this message and exit.
 ```
@@ -696,15 +743,16 @@
 ```
 Usage: lean library remove [OPTIONS] PROJECT NAME
 
   Remove a custom library from a project.
 
   PROJECT must be the path to the project directory.
 
-  NAME must be the name of the NuGet package (for C# projects) or of the PyPI package (for Python projects) to remove.
+  NAME must be either the name of the NuGet package (for C# projects), the PyPI package (for Python projects), or the
+  path to the Lean CLI library to remove.
 
   Custom C# libraries are removed from the project's .csproj file, which is then restored if dotnet is on your PATH and
   the --no-local flag has not been given.
 
   Custom Python libraries are removed from the project's requirements.txt file.
 
   C# example usage:
@@ -739,16 +787,14 @@
   deploy        Start live trading a project locally using Docker.
   liquidate     Liquidate the given symbol from the latest deployment of the given project.
   stop          Stop an already running local live trading project.
   submit-order  Represents a command to submit an order to the algorithm.
   update-order  Represents a command to update a specific order by id.
 ```
 
-_See code: [lean/commands/live.py](lean/commands/live.py)_
-
 ### `lean live add-security`
 
 Represents a command to add a security to the algorithm.
 
 ```
 Usage: lean live add-security [OPTIONS] PROJECT
 
@@ -814,104 +860,89 @@
   By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
   can set the default engine image for all commands using `lean config set engine-image <image>`.
 
 Options:
   --environment TEXT              The environment to use
   --output DIRECTORY              Directory to store results in (defaults to PROJECT/live/TIMESTAMP)
   -d, --detach                    Run the live deployment in a detached Docker container and return immediately
-  --brokerage [Paper Trading|Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Terminal Link|Atreyu|Trading Technologies|Kraken|FTX]
+  --brokerage [Paper Trading|Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Terminal Link|Atreyu|Trading Technologies|Kraken|TDAmeritrade]
                                   The brokerage to use
-  --data-feed [Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Terminal Link|Trading Technologies|Kraken|FTX|IQFeed|Polygon Data Feed|Custom data only]
+  --data-feed [Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Terminal Link|Kraken|TDAmeritrade|IQFeed|Polygon Data Feed|Custom data only]
                                   The data feed to use
-  --data-provider [Terminal Link|QuantConnect|Local]
+  --data-provider [QuantConnect|Local]
                                   Update the Lean configuration file to retrieve data from the given provider
-  --ib-organization TEXT          The name or id of the organization with the Interactive Brokers module subscription
   --ib-user-name TEXT             Your Interactive Brokers username
   --ib-account TEXT               Your Interactive Brokers account id
   --ib-password TEXT              Your Interactive Brokers password
-  --ib-enable-delayed-streaming-data BOOLEAN
-                                  Whether delayed data may be used when your algorithm subscribes to a security you
-                                  don't have a market data subscription for
-  --tradier-organization TEXT     The name or id of the organization with the Tradier module subscription
+  --ib-weekly-restart-utc-time TEXT
+                                  Weekly restart UTC time (hh:mm:ss). Each week on Sunday your algorithm is restarted at
+                                  this time, and will require 2FA verification. This is required by Interactive Brokers.
+                                  Use this option explicitly to override the default value.
   --tradier-account-id TEXT       Your Tradier account id
   --tradier-access-token TEXT     Your Tradier access token
   --tradier-environment [live|paper]
                                   Whether the developer sandbox should be used
-  --oanda-organization TEXT       The name or id of the organization with the Oanda module subscription
-  --oanda-environment [Practice|Trade]
-                                  The environment to run in, Practice for fxTrade Practice, Trade for fxTrade
   --oanda-account-id TEXT         Your OANDA account id
   --oanda-access-token TEXT       Your OANDA API token
-  --bitfinex-organization TEXT    The name or id of the organization with the Bitfinex module subscription
+  --oanda-environment [Practice|Trade]
+                                  The environment to run in, Practice for fxTrade Practice, Trade for fxTrade
   --bitfinex-api-key TEXT         Your Bitfinex API key
   --bitfinex-api-secret TEXT      Your Bitfinex API secret
-  --gdax-organization TEXT        The name or id of the organization with the Coinbase Pro module subscription
-  --gdax-use-sandbox [live|paper]
-                                  Whether the sandbox should be used
   --gdax-api-key TEXT             Your Coinbase Pro API key
   --gdax-api-secret TEXT          Your Coinbase Pro API secret
   --gdax-passphrase TEXT          Your Coinbase Pro API passphrase
-  --binance-organization TEXT     The name or id of the organization with the Binance module subscription
+  --gdax-use-sandbox [live|paper]
+                                  Whether the sandbox should be used
   --binance-exchange-name [Binance|BinanceUS]
                                   Binance exchange name [Binance, BinanceUS]
-  --binance-use-testnet [live|paper]
-                                  Whether the testnet should be used
   --binance-api-key TEXT          Your Binance API key
   --binanceus-api-key TEXT        Your Binance API key
   --binance-api-secret TEXT       Your Binance API secret
   --binanceus-api-secret TEXT     Your Binance API secret
-  --zerodha-organization TEXT     The name or id of the organization with the zerodha module subscription
+  --binance-use-testnet [live|paper]
+                                  Whether the testnet should be used
   --zerodha-api-key TEXT          Your Kite Connect API key
   --zerodha-access-token TEXT     Your Kite Connect access token
   --zerodha-product-type [mis|cnc|nrml]
                                   MIS if you are targeting intraday products, CNC if you are targeting delivery
                                   products, NRML if you are targeting carry forward products
   --zerodha-trading-segment [equity|commodity]
                                   EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                   commodities on MCX
   --zerodha-history-subscription [true|false]
                                   Whether you have a history API subscription for Zerodha
-  --samco-organization TEXT       The name or id of the organization with the samco module subscription
   --samco-client-id TEXT          Your Samco account Client ID
   --samco-client-password TEXT    Your Samco account password
   --samco-year-of-birth TEXT      Your year of birth (YYYY) registered with Samco
   --samco-product-type [mis|cnc|nrml]
                                   MIS if you are targeting intraday products, CNC if you are targeting delivery
                                   products, NRML if you are targeting carry forward products
   --samco-trading-segment [equity|commodity]
                                   EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
                                   commodities on MCX
-  --terminal-link-organization TEXT
-                                  The name or id of the organization with the Terminal Link module subscription
-  --bloomberg-environment [Production|Beta]
+  --terminal-link-environment [Production|Beta]
                                   The environment to run in
-  --bloomberg-server-host TEXT    The host of the Bloomberg server
-  --bloomberg-server-port INTEGER
-                                  The port of the Bloomberg server
-  --bloomberg-symbol-map-file FILE
-                                  The path to the Bloomberg symbol map file
-  --bloomberg-emsx-broker TEXT    The EMSX broker to use
-  --bloomberg-emsx-user-time-zone TEXT
-                                  The EMSX user timezone to use
-  --bloomberg-emsx-account TEXT   The EMSX account to use
-  --bloomberg-emsx-strategy TEXT  The EMSX strategy to use
-  --bloomberg-emsx-notes TEXT     The EMSX notes to use
-  --bloomberg-emsx-handling TEXT  The EMSX handling to use
-  --bloomberg-allow-modification BOOLEAN
-                                  Whether modification is allowed
-  --atreyu-organization TEXT      The name or id of the organization with the Atreyu module subscription
+  --terminal-link-server-host TEXT
+                                  The host of the TerminalLink server
+  --terminal-link-server-port INTEGER
+                                  The port of the TerminalLink server
+  --terminal-link-emsx-broker TEXT
+                                  The EMSX broker to use
+  --terminal-link-emsx-account TEXT
+                                  The EMSX account to use
+  --terminal-link-openfigi-api-key TEXT
+                                  The Open FIGI API key to use for mapping options
   --atreyu-host TEXT              The host of the Atreyu server
   --atreyu-req-port INTEGER       The Atreyu request port
   --atreyu-sub-port INTEGER       The Atreyu subscribe port
   --atreyu-username TEXT          Your Atreyu username
   --atreyu-password TEXT          Your Atreyu password
   --atreyu-client-id TEXT         Your Atreyu client id
   --atreyu-broker-mpid TEXT       The broker MPID to use
   --atreyu-locate-rqd TEXT        The locate rqd to use
-  --tt-organization TEXT          The name or id of the organization with the Trading Technologies module subscription
   --tt-user-name TEXT             Your Trading Technologies username
   --tt-session-password TEXT      Your Trading Technologies session password
   --tt-account-name TEXT          Your Trading Technologies account name
   --tt-rest-app-key TEXT          Your Trading Technologies REST app key
   --tt-rest-app-secret TEXT       Your Trading Technologies REST app secret
   --tt-rest-environment TEXT      The REST environment to run in
   --tt-market-data-sender-comp-id TEXT
@@ -923,41 +954,41 @@
   --tt-order-routing-sender-comp-id TEXT
                                   The order routing sender comp id to use
   --tt-order-routing-target-comp-id TEXT
                                   The order routing target comp id to use
   --tt-order-routing-host TEXT    The host of the order routing server
   --tt-order-routing-port TEXT    The port of the order routing server
   --tt-log-fix-messages BOOLEAN   Whether FIX messages should be logged
-  --kraken-organization TEXT      The name or id of the organization with the kraken module subscription
   --kraken-api-key TEXT           Your Kraken API key
   --kraken-api-secret TEXT        Your Kraken API secret
   --kraken-verification-tier [Starter|Intermediate|Pro]
                                   Your Kraken Verification Tier
-  --ftx-organization TEXT         The name or id of the organization with the FTX module subscription
-  --ftx-exchange-name [FTX|FTXUS]
-                                  FTX exchange name [FTX, FTXUS]
-  --ftx-api-key TEXT              Your FTX API key
-  --ftxus-api-key TEXT            Your FTX API key
-  --ftx-api-secret TEXT           Your FTX API secret
-  --ftxus-api-secret TEXT         Your FTX API secret
-  --ftx-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6|VIP1|VIP2|VIP3|MM1|MM2|MM3]
-                                  Your FTX Account Tier
-  --ftxus-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6|Tier7|Tier8|Tier9|VIP1|VIP2|MM1|MM2|MM3]
-                                  Your FTX Account Tier
-  --iqfeed-iqconnect FILE         The path to the IQConnect binary
+  --tdameritrade-api-key TEXT     Your TDAmeritrade API key
+  --tdameritrade-access-token TEXT
+                                  Your TDAmeritrade OAuth Access Token
+  --tdameritrade-account-number TEXT
+                                  Your TDAmeritrade account number
+  --ib-enable-delayed-streaming-data BOOLEAN
+                                  Whether delayed data may be used when your algorithm subscribes to a security you
+                                  don't have a market data subscription for
+  --iqfeed-iqconnect TEXT         The path to the IQConnect binary
   --iqfeed-username TEXT          Your IQFeed username
   --iqfeed-password TEXT          Your IQFeed password
   --iqfeed-productName TEXT       The product name of your IQFeed developer account
   --iqfeed-version TEXT           The product version of your IQFeed developer account
   --polygon-api-key TEXT          Your Polygon data feed API Key
-  --quantconnect-organization TEXT
-                                  The name or id of the organization with the QuantConnect datafeed module subscription
   --release                       Compile C# projects in release configuration instead of debug
   --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
+  --python-venv TEXT              The path of the python virtual environment to be used
+  --live-cash-balance TEXT        A comma-separated list of currency:amount pairs of initial cash balance
+  --live-holdings TEXT            A comma-separated list of symbol:symbolId:quantity:averagePrice of initial portfolio
+                                  holdings
   --update                        Pull the LEAN engine image before starting live trading
+  --show-secrets                  Show secrets as they are input
+  --no-update                     Use the local LEAN engine image instead of pulling the latest version
   --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
   --verbose                       Enable debug logging
   --help                          Show this message and exit.
 ```
 
 _See code: [lean/commands/live/deploy.py](lean/commands/live/deploy.py)_
 
@@ -1057,14 +1088,15 @@
   If user id or API token is not provided an interactive prompt will show.
 
   Credentials are stored in ~/.lean/credentials and are removed upon running `lean logout`.
 
 Options:
   -u, --user-id TEXT    QuantConnect user id
   -t, --api-token TEXT  QuantConnect API token
+  --show-secrets        Show secrets as they are input
   --verbose             Enable debug logging
   --help                Show this message and exit.
 ```
 
 _See code: [lean/commands/login.py](lean/commands/login.py)_
 
 ### `lean logout`
@@ -1130,14 +1162,17 @@
   - --parameter <name> <min value> <max value> <step size>
   - --parameter my-first-parameter 1 10 0.5 --parameter my-second-parameter 20 30 5
 
   In non-interactive mode the --constraint option can be provided multiple times to configure multiple constraints:
   - --constraint "<statistic> <operator> <value>"
   - --constraint "Sharpe Ratio >= 0.5" --constraint "Drawdown < 0.25"
 
+  If --estimate is given, the optimization will not be executed.
+  The runtime estimate for the optimization will be calculated and outputted.
+
   By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
   can set the default engine image for all commands using `lean config set engine-image <image>`.
 
 Options:
   --output DIRECTORY              Directory to store results in (defaults to PROJECT/optimizations/TIMESTAMP)
   -d, --detach                    Run the optimization in a detached Docker container and return immediately
   --optimizer-config FILE         The optimizer configuration file that should be used
@@ -1147,21 +1182,64 @@
   --target-direction [min|max]    Whether the target must be minimized or maximized
   --parameter <TEXT FLOAT FLOAT FLOAT>...
                                   The 'parameter min max step' pairs configuring the parameters to optimize
   --constraint TEXT               The 'statistic operator value' pairs configuring the constraints of the optimization
   --release                       Compile C# projects in release configuration instead of debug
   --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
   --update                        Pull the LEAN engine image before running the optimizer
+  --estimate                      Estimate optimization runtime without running it
+  --max-concurrent-backtests INTEGER RANGE
+                                  Maximum number of concurrent backtests to run  [x>=1]
+  --no-update                     Use the local LEAN engine image instead of pulling the latest version
   --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
   --verbose                       Enable debug logging
   --help                          Show this message and exit.
 ```
 
 _See code: [lean/commands/optimize.py](lean/commands/optimize.py)_
 
+### `lean project-create`
+
+Create a new project containing starter code.
+
+```
+Usage: lean project-create [OPTIONS] NAME
+
+  Create a new project containing starter code.
+
+  If NAME is a path containing subdirectories those will be created automatically.
+
+  The default language can be set using `lean config set default-language python/csharp`.
+
+Options:
+  -l, --language [python|csharp]  The language of the project to create
+  --verbose                       Enable debug logging
+  --help                          Show this message and exit.
+```
+
+_See code: [lean/commands/project_create.py](lean/commands/project_create.py)_
+
+### `lean project-delete`
+
+Delete a project locally and in the cloud if it exists.
+
+```
+Usage: lean project-delete [OPTIONS] PROJECT
+
+  Delete a project locally and in the cloud if it exists.
+
+  The project is selected by name or cloud id.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/project_delete.py](lean/commands/project_delete.py)_
+
 ### `lean report`
 
 Generate a report of a backtest.
 
 ```
 Usage: lean report [OPTIONS]
 
@@ -1187,14 +1265,15 @@
   -d, --detach                 Run the report creator in a detached Docker container and return immediately
   --strategy-name TEXT         Name of the strategy, will appear at the top-right corner of each page
   --strategy-version TEXT      Version number of the strategy, will appear next to the project name
   --strategy-description TEXT  Description of the strategy, will appear under the 'Strategy Description' section
   --overwrite                  Overwrite --report-destination if it already contains a file
   --image TEXT                 The LEAN engine image to use (defaults to quantconnect/lean:latest)
   --update                     Pull the LEAN engine image before running the report creator
+  --pdf                        Create a PDF version along with the HTML version of the report
   --lean-config FILE           The Lean configuration file that should be used (defaults to the nearest lean.json)
   --verbose                    Enable debug logging
   --help                       Show this message and exit.
 ```
 
 _See code: [lean/commands/report.py](lean/commands/report.py)_
 
@@ -1208,16 +1287,24 @@
   Run a Jupyter Lab environment locally using Docker.
 
   By default the official LEAN research image is used. You can override this using the --image option. Alternatively you
   can set the default research image using `lean config set research-image <image>`.
 
 Options:
   --port INTEGER                  The port to run Jupyter Lab on (defaults to 8888)
-  --data-provider [Terminal Link|QuantConnect|Local]
+  --data-provider [QuantConnect|Local|Terminal Link]
                                   Update the Lean configuration file to retrieve data from the given provider
+  --terminal-link-environment [Production|Beta]
+                                  The environment to run in
+  --terminal-link-server-host TEXT
+                                  The host of the TerminalLink server
+  --terminal-link-server-port INTEGER
+                                  The port of the TerminalLink server
+  --terminal-link-openfigi-api-key TEXT
+                                  The Open FIGI API key to use for mapping options
   --download-data                 Update the Lean configuration file to download data from the QuantConnect API, alias
                                   for --data-provider QuantConnect
   --data-purchase-limit INTEGER   The maximum amount of QCC to spend on downloading data during the research session
                                   when using QuantConnect as data provider
   -d, --detach                    Run Jupyter Lab in a detached Docker container and return immediately
   --no-open                       Don't open the Jupyter Lab environment in the browser after starting it
   --image TEXT                    The LEAN research image to use (defaults to quantconnect/research:latest)
@@ -1244,15 +1331,15 @@
 ```
 
 _See code: [lean/commands/whoami.py](lean/commands/whoami.py)_
 <!-- commands end -->
 
 ## Development
 
-To work on the Lean CLI, clone the repository, enter an environment containing Python 3.6+ and run `pip install -r requirements.txt`. This command will install the required dependencies and installs the CLI in editable mode. This means you'll be able to edit the code and immediately see the results the next time you run `lean`.
+To work on the Lean CLI, clone the repository, enter an environment containing Python 3.7+ and run `pip install -r requirements.txt`. This command will install the required dependencies and installs the CLI in editable mode. This means you'll be able to edit the code and immediately see the results the next time you run `lean`.
 
 If you need to add dependencies, first update `setup.py` (if it is a production dependency) or `requirements.txt` (if it is a development dependency) and then re-run `pip install -r requirements.txt`.
 
 The automated tests can be ran by running `pytest`. The filesystem and HTTP requests are mocked when running tests to make sure they run in an isolated environment.
 
 Can build the lean CLI by running `python setup.py sdist bdist_wheel` from the root of the project and to install it `pip install --force-reinstall dist/lean-dev-py3-none-any.whl`. To update the commands reference part of the readme run `python scripts/readme.py` from the root of the project, after installing the new version.
```

