# Comparing `tmp/okdata-cli-2.0.0.tar.gz` & `tmp/okdata-cli-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okdata-cli-2.0.0.tar", last modified: Mon Apr 24 11:07:40 2023, max compression
+gzip compressed data, was "okdata-cli-2.0.1.tar", last modified: Wed May 24 07:16:08 2023, max compression
```

## Comparing `okdata-cli-2.0.0.tar` & `okdata-cli-2.0.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-04-24 11:07:40.861759 okdata-cli-2.0.0/
--rw-r--r--   0 simen     (1000) simen     (1000)     1077 2020-04-30 07:54:22.000000 okdata-cli-2.0.0/LICENSE
--rw-r--r--   0 simen     (1000) simen     (1000)     1045 2023-04-24 11:07:40.861759 okdata-cli-2.0.0/PKG-INFO
--rw-r--r--   0 simen     (1000) simen     (1000)      320 2023-04-21 08:20:57.000000 okdata-cli-2.0.0/README.md
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-04-24 11:07:40.857759 okdata-cli-2.0.0/okdata/
--rw-r--r--   0 simen     (1000) simen     (1000)       56 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/__init__.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-04-24 11:07:40.857759 okdata-cli-2.0.0/okdata/cli/
--rw-r--r--   0 simen     (1000) simen     (1000)       27 2023-04-21 09:45:40.000000 okdata-cli-2.0.0/okdata/cli/__init__.py
--rw-r--r--   0 simen     (1000) simen     (1000)     2534 2023-04-21 10:35:45.000000 okdata-cli-2.0.0/okdata/cli/__main__.py
--rw-r--r--   0 simen     (1000) simen     (1000)     4400 2023-04-24 11:06:10.000000 okdata-cli-2.0.0/okdata/cli/command.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-04-24 11:07:40.857759 okdata-cli-2.0.0/okdata/cli/commands/
--rw-r--r--   0 simen     (1000) simen     (1000)        0 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/commands/__init__.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-04-24 11:07:40.857759 okdata-cli-2.0.0/okdata/cli/commands/datasets/
--rw-r--r--   0 simen     (1000) simen     (1000)       69 2023-03-21 06:17:16.000000 okdata-cli-2.0.0/okdata/cli/commands/datasets/__init__.py
--rw-r--r--   0 simen     (1000) simen     (1000)    14604 2023-04-24 08:36:09.000000 okdata-cli-2.0.0/okdata/cli/commands/datasets/datasets.py
--rw-r--r--   0 simen     (1000) simen     (1000)     5669 2023-03-21 06:17:16.000000 okdata-cli-2.0.0/okdata/cli/commands/datasets/questions.py
--rw-r--r--   0 simen     (1000) simen     (1000)     4461 2023-03-21 06:17:16.000000 okdata-cli-2.0.0/okdata/cli/commands/datasets/validators.py
--rw-r--r--   0 simen     (1000) simen     (1000)     3699 2023-03-21 06:17:16.000000 okdata-cli-2.0.0/okdata/cli/commands/datasets/wizards.py
--rw-r--r--   0 simen     (1000) simen     (1000)     4568 2022-04-27 09:26:47.000000 okdata-cli-2.0.0/okdata/cli/commands/permissions.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-04-24 11:07:40.857759 okdata-cli-2.0.0/okdata/cli/commands/pubreg/
--rw-r--r--   0 simen     (1000) simen     (1000)       89 2021-09-24 07:58:38.000000 okdata-cli-2.0.0/okdata/cli/commands/pubreg/__init__.py
--rw-r--r--   0 simen     (1000) simen     (1000)     2392 2023-03-21 06:10:29.000000 okdata-cli-2.0.0/okdata/cli/commands/pubreg/client.py
--rw-r--r--   0 simen     (1000) simen     (1000)    11255 2023-04-24 08:36:09.000000 okdata-cli-2.0.0/okdata/cli/commands/pubreg/pubreg.py
--rw-r--r--   0 simen     (1000) simen     (1000)     5459 2023-03-13 08:50:41.000000 okdata-cli-2.0.0/okdata/cli/commands/pubreg/questions.py
--rw-r--r--   0 simen     (1000) simen     (1000)     3121 2023-03-13 08:50:41.000000 okdata-cli-2.0.0/okdata/cli/commands/pubreg/wizards.py
--rw-r--r--   0 simen     (1000) simen     (1000)     3067 2022-04-27 09:26:47.000000 okdata-cli-2.0.0/okdata/cli/commands/status.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-04-24 11:07:40.857759 okdata-cli-2.0.0/okdata/cli/commands/teams/
--rw-r--r--   0 simen     (1000) simen     (1000)     2997 2023-02-17 13:22:37.000000 okdata-cli-2.0.0/okdata/cli/commands/teams/questions.py
--rw-r--r--   0 simen     (1000) simen     (1000)     5633 2023-04-24 08:36:09.000000 okdata-cli-2.0.0/okdata/cli/commands/teams/teams.py
--rw-r--r--   0 simen     (1000) simen     (1000)      456 2022-12-09 07:24:37.000000 okdata-cli-2.0.0/okdata/cli/commands/teams/util.py
--rw-r--r--   0 simen     (1000) simen     (1000)     1223 2022-12-09 07:24:37.000000 okdata-cli-2.0.0/okdata/cli/commands/teams/wizards.py
--rw-r--r--   0 simen     (1000) simen     (1000)      341 2023-02-17 13:22:37.000000 okdata-cli-2.0.0/okdata/cli/commands/wizard.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-04-24 11:07:40.857759 okdata-cli-2.0.0/okdata/cli/data/
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-04-24 11:07:40.861759 okdata-cli-2.0.0/okdata/cli/data/output-format/
--rw-r--r--   0 simen     (1000) simen     (1000)      180 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/datasets_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      266 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/datasets_copy_file_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      206 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/datasets_copy_file_config_2.json
--rw-r--r--   0 simen     (1000) simen     (1000)      359 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/datasets_dataset_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      345 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/datasets_dataset_version_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      328 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/datasets_dataset_version_edition_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      119 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/datasets_dataset_version_edition_distributions_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      209 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/datasets_dataset_versions_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      146 2021-05-19 10:09:25.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/my_permissions_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      204 2021-05-19 10:09:25.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/permissions_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      301 2022-08-25 09:15:43.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/pubreg_audit_log_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      246 2022-04-27 09:26:47.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/pubreg_clients_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      201 2023-03-13 08:50:41.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/pubreg_multiple_client_keys_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      125 2023-03-13 08:50:41.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/pubreg_single_client_keys_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      354 2021-07-06 12:28:25.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/status_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      721 2021-07-06 12:28:25.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/status_history_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      183 2022-08-25 13:30:17.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/team_members_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      124 2022-08-25 09:06:50.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/teams_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      163 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/date.py
--rw-r--r--   0 simen     (1000) simen     (1000)      730 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/io.py
--rw-r--r--   0 simen     (1000) simen     (1000)     4802 2023-04-21 08:20:57.000000 okdata-cli-2.0.0/okdata/cli/output.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-04-24 11:07:40.861759 okdata-cli-2.0.0/okdata_cli.egg-info/
--rw-r--r--   0 simen     (1000) simen     (1000)     1045 2023-04-24 11:07:40.000000 okdata-cli-2.0.0/okdata_cli.egg-info/PKG-INFO
--rw-r--r--   0 simen     (1000) simen     (1000)     2211 2023-04-24 11:07:40.000000 okdata-cli-2.0.0/okdata_cli.egg-info/SOURCES.txt
--rw-r--r--   0 simen     (1000) simen     (1000)        1 2023-04-24 11:07:40.000000 okdata-cli-2.0.0/okdata_cli.egg-info/dependency_links.txt
--rw-r--r--   0 simen     (1000) simen     (1000)       52 2023-04-24 11:07:40.000000 okdata-cli-2.0.0/okdata_cli.egg-info/entry_points.txt
--rw-r--r--   0 simen     (1000) simen     (1000)        7 2023-04-24 11:07:40.000000 okdata-cli-2.0.0/okdata_cli.egg-info/namespace_packages.txt
--rw-r--r--   0 simen     (1000) simen     (1000)       80 2023-04-24 11:07:40.000000 okdata-cli-2.0.0/okdata_cli.egg-info/requires.txt
--rw-r--r--   0 simen     (1000) simen     (1000)       11 2023-04-24 11:07:40.000000 okdata-cli-2.0.0/okdata_cli.egg-info/top_level.txt
--rw-r--r--   0 simen     (1000) simen     (1000)      276 2020-04-30 07:54:22.000000 okdata-cli-2.0.0/pyproject.toml
--rw-r--r--   0 simen     (1000) simen     (1000)       38 2023-04-24 11:07:40.861759 okdata-cli-2.0.0/setup.cfg
--rw-r--r--   0 simen     (1000) simen     (1000)     1380 2023-04-24 11:06:10.000000 okdata-cli-2.0.0/setup.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-05-24 07:16:08.238551 okdata-cli-2.0.1/
+-rw-r--r--   0 simen     (1000) simen     (1000)     1077 2020-04-30 07:54:22.000000 okdata-cli-2.0.1/LICENSE
+-rw-r--r--   0 simen     (1000) simen     (1000)     1045 2023-05-24 07:16:08.238551 okdata-cli-2.0.1/PKG-INFO
+-rw-r--r--   0 simen     (1000) simen     (1000)      320 2023-04-21 08:20:57.000000 okdata-cli-2.0.1/README.md
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-05-24 07:16:08.234551 okdata-cli-2.0.1/okdata/
+-rw-r--r--   0 simen     (1000) simen     (1000)       56 2020-12-09 11:27:37.000000 okdata-cli-2.0.1/okdata/__init__.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-05-24 07:16:08.234551 okdata-cli-2.0.1/okdata/cli/
+-rw-r--r--   0 simen     (1000) simen     (1000)       27 2023-04-21 09:45:40.000000 okdata-cli-2.0.1/okdata/cli/__init__.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     2534 2023-04-21 10:35:45.000000 okdata-cli-2.0.1/okdata/cli/__main__.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     4400 2023-05-24 07:13:46.000000 okdata-cli-2.0.1/okdata/cli/command.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-05-24 07:16:08.234551 okdata-cli-2.0.1/okdata/cli/commands/
+-rw-r--r--   0 simen     (1000) simen     (1000)        0 2020-12-09 11:27:37.000000 okdata-cli-2.0.1/okdata/cli/commands/__init__.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-05-24 07:16:08.238551 okdata-cli-2.0.1/okdata/cli/commands/datasets/
+-rw-r--r--   0 simen     (1000) simen     (1000)       69 2023-03-21 06:17:16.000000 okdata-cli-2.0.1/okdata/cli/commands/datasets/__init__.py
+-rw-r--r--   0 simen     (1000) simen     (1000)    14871 2023-05-24 07:11:46.000000 okdata-cli-2.0.1/okdata/cli/commands/datasets/datasets.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     5669 2023-03-21 06:17:16.000000 okdata-cli-2.0.1/okdata/cli/commands/datasets/questions.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     4461 2023-03-21 06:17:16.000000 okdata-cli-2.0.1/okdata/cli/commands/datasets/validators.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     3699 2023-03-21 06:17:16.000000 okdata-cli-2.0.1/okdata/cli/commands/datasets/wizards.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     4568 2022-04-27 09:26:47.000000 okdata-cli-2.0.1/okdata/cli/commands/permissions.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-05-24 07:16:08.238551 okdata-cli-2.0.1/okdata/cli/commands/pubreg/
+-rw-r--r--   0 simen     (1000) simen     (1000)       89 2021-09-24 07:58:38.000000 okdata-cli-2.0.1/okdata/cli/commands/pubreg/__init__.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     2392 2023-03-21 06:10:29.000000 okdata-cli-2.0.1/okdata/cli/commands/pubreg/client.py
+-rw-r--r--   0 simen     (1000) simen     (1000)    11255 2023-04-24 08:36:09.000000 okdata-cli-2.0.1/okdata/cli/commands/pubreg/pubreg.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     5459 2023-03-13 08:50:41.000000 okdata-cli-2.0.1/okdata/cli/commands/pubreg/questions.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     3121 2023-03-13 08:50:41.000000 okdata-cli-2.0.1/okdata/cli/commands/pubreg/wizards.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     3067 2022-04-27 09:26:47.000000 okdata-cli-2.0.1/okdata/cli/commands/status.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-05-24 07:16:08.238551 okdata-cli-2.0.1/okdata/cli/commands/teams/
+-rw-r--r--   0 simen     (1000) simen     (1000)     2997 2023-02-17 13:22:37.000000 okdata-cli-2.0.1/okdata/cli/commands/teams/questions.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     5633 2023-04-24 08:36:09.000000 okdata-cli-2.0.1/okdata/cli/commands/teams/teams.py
+-rw-r--r--   0 simen     (1000) simen     (1000)      456 2022-12-09 07:24:37.000000 okdata-cli-2.0.1/okdata/cli/commands/teams/util.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     1223 2022-12-09 07:24:37.000000 okdata-cli-2.0.1/okdata/cli/commands/teams/wizards.py
+-rw-r--r--   0 simen     (1000) simen     (1000)      341 2023-02-17 13:22:37.000000 okdata-cli-2.0.1/okdata/cli/commands/wizard.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-05-24 07:16:08.234551 okdata-cli-2.0.1/okdata/cli/data/
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-05-24 07:16:08.238551 okdata-cli-2.0.1/okdata/cli/data/output-format/
+-rw-r--r--   0 simen     (1000) simen     (1000)      180 2020-12-09 11:27:37.000000 okdata-cli-2.0.1/okdata/cli/data/output-format/datasets_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      262 2023-05-24 07:11:46.000000 okdata-cli-2.0.1/okdata/cli/data/output-format/datasets_copy_file_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      206 2020-12-09 11:27:37.000000 okdata-cli-2.0.1/okdata/cli/data/output-format/datasets_copy_file_config_2.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      359 2020-12-09 11:27:37.000000 okdata-cli-2.0.1/okdata/cli/data/output-format/datasets_dataset_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      345 2020-12-09 11:27:37.000000 okdata-cli-2.0.1/okdata/cli/data/output-format/datasets_dataset_version_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      328 2020-12-09 11:27:37.000000 okdata-cli-2.0.1/okdata/cli/data/output-format/datasets_dataset_version_edition_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      119 2020-12-09 11:27:37.000000 okdata-cli-2.0.1/okdata/cli/data/output-format/datasets_dataset_version_edition_distributions_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      209 2020-12-09 11:27:37.000000 okdata-cli-2.0.1/okdata/cli/data/output-format/datasets_dataset_versions_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      146 2021-05-19 10:09:25.000000 okdata-cli-2.0.1/okdata/cli/data/output-format/my_permissions_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      204 2021-05-19 10:09:25.000000 okdata-cli-2.0.1/okdata/cli/data/output-format/permissions_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      301 2022-08-25 09:15:43.000000 okdata-cli-2.0.1/okdata/cli/data/output-format/pubreg_audit_log_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      246 2022-04-27 09:26:47.000000 okdata-cli-2.0.1/okdata/cli/data/output-format/pubreg_clients_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      201 2023-03-13 08:50:41.000000 okdata-cli-2.0.1/okdata/cli/data/output-format/pubreg_multiple_client_keys_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      125 2023-03-13 08:50:41.000000 okdata-cli-2.0.1/okdata/cli/data/output-format/pubreg_single_client_keys_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      354 2021-07-06 12:28:25.000000 okdata-cli-2.0.1/okdata/cli/data/output-format/status_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      721 2021-07-06 12:28:25.000000 okdata-cli-2.0.1/okdata/cli/data/output-format/status_history_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      183 2022-08-25 13:30:17.000000 okdata-cli-2.0.1/okdata/cli/data/output-format/team_members_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      124 2022-08-25 09:06:50.000000 okdata-cli-2.0.1/okdata/cli/data/output-format/teams_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      163 2020-12-09 11:27:37.000000 okdata-cli-2.0.1/okdata/cli/date.py
+-rw-r--r--   0 simen     (1000) simen     (1000)      730 2020-12-09 11:27:37.000000 okdata-cli-2.0.1/okdata/cli/io.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     4802 2023-04-21 08:20:57.000000 okdata-cli-2.0.1/okdata/cli/output.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-05-24 07:16:08.238551 okdata-cli-2.0.1/okdata_cli.egg-info/
+-rw-r--r--   0 simen     (1000) simen     (1000)     1045 2023-05-24 07:16:08.000000 okdata-cli-2.0.1/okdata_cli.egg-info/PKG-INFO
+-rw-r--r--   0 simen     (1000) simen     (1000)     2211 2023-05-24 07:16:08.000000 okdata-cli-2.0.1/okdata_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 simen     (1000) simen     (1000)        1 2023-05-24 07:16:08.000000 okdata-cli-2.0.1/okdata_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 simen     (1000) simen     (1000)       52 2023-05-24 07:16:08.000000 okdata-cli-2.0.1/okdata_cli.egg-info/entry_points.txt
+-rw-r--r--   0 simen     (1000) simen     (1000)        7 2023-05-24 07:16:08.000000 okdata-cli-2.0.1/okdata_cli.egg-info/namespace_packages.txt
+-rw-r--r--   0 simen     (1000) simen     (1000)       80 2023-05-24 07:16:08.000000 okdata-cli-2.0.1/okdata_cli.egg-info/requires.txt
+-rw-r--r--   0 simen     (1000) simen     (1000)       11 2023-05-24 07:16:08.000000 okdata-cli-2.0.1/okdata_cli.egg-info/top_level.txt
+-rw-r--r--   0 simen     (1000) simen     (1000)      276 2020-04-30 07:54:22.000000 okdata-cli-2.0.1/pyproject.toml
+-rw-r--r--   0 simen     (1000) simen     (1000)       38 2023-05-24 07:16:08.238551 okdata-cli-2.0.1/setup.cfg
+-rw-r--r--   0 simen     (1000) simen     (1000)     1380 2023-05-24 07:14:00.000000 okdata-cli-2.0.1/setup.py
```

### Comparing `okdata-cli-2.0.0/LICENSE` & `okdata-cli-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `okdata-cli-2.0.0/PKG-INFO` & `okdata-cli-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okdata-cli
-Version: 2.0.0
+Version: 2.0.1
 Summary: CLI for services provided by Oslo Origo
 Home-page: https://github.com/oslokommune/okdata-cli/
 Author: Oslo Origo
 Author-email: dataplattform@oslo.kommune.no
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `okdata-cli-2.0.0/okdata/cli/__main__.py` & `okdata-cli-2.0.1/okdata/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-2.0.0/okdata/cli/command.py` & `okdata-cli-2.0.1/okdata/cli/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   -h, --help                # Print this help
   -d, --debug               # Output debug information while executing task
   --format=<value>          # Output format: table OR json
   --env=<value>             # Environment to run command in: prod OR dev"""
 
 
 class BaseCommand:
-    version = "2.0.0"
+    version = "2.0.1"
     # TODO: Can use `importlib` in Python 3.8 and up instead of hard coding the
     #       version here:
     #
     # version = importlib.metadata.version("okdata-cli")
 
     __doc__ = f"""okdata-cli {version}
```

### Comparing `okdata-cli-2.0.0/okdata/cli/commands/datasets/datasets.py` & `okdata-cli-2.0.1/okdata/cli/commands/datasets/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,15 +346,24 @@
         data = {
             "dataset": dataset_id,
             "file": source,
             "uploaded": res["result"],
             "trace_id": res["trace_id"],
         }
         out.add_row(data)
-        self.print(f"Uploaded file to dataset: {dataset_id}", out)
+        self.print(
+            "\n".join(
+                [
+                    f"Uploaded file to dataset: {dataset_id}",
+                    str(out),
+                    "\nYou can check the data processing status by running:\n",
+                    f"  okdata status {res['trace_id']}",
+                ]
+            )
+        )
 
     def download_files(self, source, target):
         dataset_id, version, edition = self._dataset_components_from_uri(source)
         downloaded_files = self.download.download(
             dataset_id, version, edition, resolve_output_filepath(target)
         )
         self.log.info(f"Download returned: {downloaded_files}")
```

### Comparing `okdata-cli-2.0.0/okdata/cli/commands/datasets/questions.py` & `okdata-cli-2.0.1/okdata/cli/commands/datasets/questions.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-2.0.0/okdata/cli/commands/datasets/validators.py` & `okdata-cli-2.0.1/okdata/cli/commands/datasets/validators.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-2.0.0/okdata/cli/commands/datasets/wizards.py` & `okdata-cli-2.0.1/okdata/cli/commands/datasets/wizards.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-2.0.0/okdata/cli/commands/permissions.py` & `okdata-cli-2.0.1/okdata/cli/commands/permissions.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-2.0.0/okdata/cli/commands/pubreg/client.py` & `okdata-cli-2.0.1/okdata/cli/commands/pubreg/client.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-2.0.0/okdata/cli/commands/pubreg/pubreg.py` & `okdata-cli-2.0.1/okdata/cli/commands/pubreg/pubreg.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-2.0.0/okdata/cli/commands/pubreg/questions.py` & `okdata-cli-2.0.1/okdata/cli/commands/pubreg/questions.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-2.0.0/okdata/cli/commands/pubreg/wizards.py` & `okdata-cli-2.0.1/okdata/cli/commands/pubreg/wizards.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-2.0.0/okdata/cli/commands/status.py` & `okdata-cli-2.0.1/okdata/cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-2.0.0/okdata/cli/commands/teams/questions.py` & `okdata-cli-2.0.1/okdata/cli/commands/teams/questions.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-2.0.0/okdata/cli/commands/teams/teams.py` & `okdata-cli-2.0.1/okdata/cli/commands/teams/teams.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-2.0.0/okdata/cli/commands/teams/wizards.py` & `okdata-cli-2.0.1/okdata/cli/commands/teams/wizards.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-2.0.0/okdata/cli/data/output-format/status_history_config.json` & `okdata-cli-2.0.1/okdata/cli/data/output-format/status_history_config.json`

 * *Files identical despite different names*

### Comparing `okdata-cli-2.0.0/okdata/cli/io.py` & `okdata-cli-2.0.1/okdata/cli/io.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-2.0.0/okdata/cli/output.py` & `okdata-cli-2.0.1/okdata/cli/output.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-2.0.0/okdata_cli.egg-info/PKG-INFO` & `okdata-cli-2.0.1/okdata_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okdata-cli
-Version: 2.0.0
+Version: 2.0.1
 Summary: CLI for services provided by Oslo Origo
 Home-page: https://github.com/oslokommune/okdata-cli/
 Author: Oslo Origo
 Author-email: dataplattform@oslo.kommune.no
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `okdata-cli-2.0.0/okdata_cli.egg-info/SOURCES.txt` & `okdata-cli-2.0.1/okdata_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `okdata-cli-2.0.0/setup.py` & `okdata-cli-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="okdata-cli",
-    version="2.0.0",
+    version="2.0.1",
     author="Oslo Origo",
     author_email="dataplattform@oslo.kommune.no",
     description="CLI for services provided by Oslo Origo",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/oslokommune/okdata-cli/",
```

