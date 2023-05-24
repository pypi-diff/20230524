# Comparing `tmp/apache-airflow-providers-microsoft-azure-6.1.0rc2.tar.gz` & `tmp/apache-airflow-providers-microsoft-azure-6.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-microsoft-azure-6.1.0rc2.tar", last modified: Fri May 19 17:52:49 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-microsoft-azure-6.1.1rc1.tar", last modified: Wed May 24 07:20:24 2023, max compression
```

## Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2.tar` & `apache-airflow-providers-microsoft-azure-6.1.1rc1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:48.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    26802 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    25181 2023-05-19 17:52:48.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/
--rw-r--r--   0 root         (0) root         (0)     1540 2023-05-19 12:13:16.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16662 2023-05-19 17:52:48.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8720 2023-04-30 16:55:11.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/adx.py
--rw-r--r--   0 root         (0) root         (0)    10986 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/asb.py
--rw-r--r--   0 root         (0) root         (0)     4778 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/base_azure.py
--rw-r--r--   0 root         (0) root         (0)    15288 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/batch.py
--rw-r--r--   0 root         (0) root         (0)     6176 2023-05-03 19:47:07.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/container_instance.py
--rw-r--r--   0 root         (0) root         (0)     2458 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/container_registry.py
--rw-r--r--   0 root         (0) root         (0)     4058 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/container_volume.py
--rw-r--r--   0 root         (0) root         (0)    14222 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/cosmos.py
--rw-r--r--   0 root         (0) root         (0)    42973 2023-03-30 19:12:06.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/data_factory.py
--rw-r--r--   0 root         (0) root         (0)    21695 2023-03-10 19:32:05.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/data_lake.py
--rw-r--r--   0 root         (0) root         (0)    12985 2023-04-30 16:55:11.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/fileshare.py
--rw-r--r--   0 root         (0) root         (0)     7318 2023-03-16 20:46:35.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/synapse.py
--rw-r--r--   0 root         (0) root         (0)    27566 2023-04-01 16:40:04.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10038 2023-03-10 19:31:58.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/log/wasb_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3788 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/adls.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/adx.py
--rw-r--r--   0 root         (0) root         (0)    29576 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/asb.py
--rw-r--r--   0 root         (0) root         (0)    16252 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/batch.py
--rw-r--r--   0 root         (0) root         (0)    15967 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/container_instances.py
--rw-r--r--   0 root         (0) root         (0)     2766 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/cosmos.py
--rw-r--r--   0 root         (0) root         (0)    12432 2023-05-12 08:38:07.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     4422 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/synapse.py
--rw-r--r--   0 root         (0) root         (0)     2687 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7902 2023-05-03 19:47:07.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/secrets/key_vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2643 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/sensors/cosmos.py
--rw-r--r--   0 root         (0) root         (0)     5763 2023-05-03 19:47:07.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/sensors/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     7660 2023-05-03 19:47:07.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/sensors/wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4771 2023-04-21 10:05:41.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py
--rw-r--r--   0 root         (0) root         (0)     4815 2023-05-03 19:47:07.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/transfers/local_to_adls.py
--rw-r--r--   0 root         (0) root         (0)     2936 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/transfers/local_to_wasb.py
--rw-r--r--   0 root         (0) root         (0)     4575 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py
--rw-r--r--   0 root         (0) root         (0)     8215 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-03-14 06:24:40.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8859 2023-04-24 21:04:25.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/triggers/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     7381 2023-04-24 21:04:25.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/triggers/wasb.py
--rw-r--r--   0 root         (0) root         (0)     2804 2023-04-30 16:55:11.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/apache_airflow_providers_microsoft_azure.egg-info/
--rw-r--r--   0 root         (0) root         (0)    26802 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2944 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/apache_airflow_providers_microsoft_azure.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/apache_airflow_providers_microsoft_azure.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/apache_airflow_providers_microsoft_azure.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      609 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/apache_airflow_providers_microsoft_azure.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/apache_airflow_providers_microsoft_azure.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2359 2023-05-19 17:52:49.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1874 2023-05-19 17:52:48.000000 apache-airflow-providers-microsoft-azure-6.1.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-24 07:20:22.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    27035 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    25363 2023-05-24 07:20:22.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-05-24 07:09:22.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16683 2023-05-24 07:20:22.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:14.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8720 2023-05-23 11:35:14.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/adx.py
+-rw-r--r--   0 root         (0) root         (0)    10986 2023-05-23 11:35:14.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/asb.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2023-05-23 11:35:14.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/base_azure.py
+-rw-r--r--   0 root         (0) root         (0)    15288 2023-05-23 11:35:14.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/batch.py
+-rw-r--r--   0 root         (0) root         (0)     6176 2023-05-23 11:35:14.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/container_instance.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/container_registry.py
+-rw-r--r--   0 root         (0) root         (0)     4058 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/container_volume.py
+-rw-r--r--   0 root         (0) root         (0)    14222 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)    42973 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)    21695 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/data_lake.py
+-rw-r--r--   0 root         (0) root         (0)    12985 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/fileshare.py
+-rw-r--r--   0 root         (0) root         (0)     7318 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/synapse.py
+-rw-r--r--   0 root         (0) root         (0)    27566 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10038 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3788 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/adls.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/adx.py
+-rw-r--r--   0 root         (0) root         (0)    29576 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/asb.py
+-rw-r--r--   0 root         (0) root         (0)    16252 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/batch.py
+-rw-r--r--   0 root         (0) root         (0)    15967 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/container_instances.py
+-rw-r--r--   0 root         (0) root         (0)     2766 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)    12432 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     4422 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/synapse.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7902 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/secrets/key_vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2643 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/sensors/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)     5763 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/sensors/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     7838 2023-05-23 14:21:47.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/sensors/wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py
+-rw-r--r--   0 root         (0) root         (0)     4815 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py
+-rw-r--r--   0 root         (0) root         (0)     2936 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py
+-rw-r--r--   0 root         (0) root         (0)     4575 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py
+-rw-r--r--   0 root         (0) root         (0)     8215 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8859 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/triggers/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     7384 2023-05-23 14:21:47.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/triggers/wasb.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/apache_airflow_providers_microsoft_azure.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    27035 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2944 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/apache_airflow_providers_microsoft_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/apache_airflow_providers_microsoft_azure.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/apache_airflow_providers_microsoft_azure.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      609 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/apache_airflow_providers_microsoft_azure.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-23 11:35:15.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-05-24 07:20:24.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-05-24 07:20:22.000000 apache-airflow-providers-microsoft-azure-6.1.1rc1/setup.py
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/LICENSE` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/MANIFEST.in` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/PKG-INFO` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-azure
-Version: 6.1.0rc2
+Version: 6.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-azure package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.1.1/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -21,14 +21,15 @@
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
 Requires-Python: ~=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: google
 Provides-Extra: oracle
 Provides-Extra: sftp
 License-File: LICENSE
@@ -51,38 +52,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-azure``
 
-Release: ``6.1.0rc2``
+Release: ``6.1.1rc1``
 
 
 `Microsoft Azure <https://azure.microsoft.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.azure`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.azure`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-microsoft-azure``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ================================  ==================
 PIP package                       Version required
 ================================  ==================
@@ -149,14 +150,27 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.1.1
+.....
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Fix deferrable mode execution in WasbPrefixSensor (#31411)``
+
+Misc
+~~~~
+
+* ``Optimize deferred mode execution for wasb sensors (#31009)``
+
 6.1.0
 .....
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Features
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/README.rst` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-azure``
 
-Release: ``6.1.0rc2``
+Release: ``6.1.1rc1``
 
 
 `Microsoft Azure <https://azure.microsoft.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.azure`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.azure`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-microsoft-azure``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ================================  ==================
 PIP package                       Version required
 ================================  ==================
@@ -113,14 +113,27 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.1.1
+.....
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Fix deferrable mode execution in WasbPrefixSensor (#31411)``
+
+Misc
+~~~~
+
+* ``Optimize deferred mode execution for wasb sensors (#31009)``
+
 6.1.0
 .....
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Features
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/__init__.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "6.1.0"
+__version__ = "6.1.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/get_provider_info.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-microsoft-azure",
         "name": "Microsoft Azure",
         "description": "`Microsoft Azure <https://azure.microsoft.com/>`__\n",
         "suspended": False,
         "versions": [
+            "6.1.1",
             "6.1.0",
             "6.0.0",
             "5.3.1",
             "5.3.0",
             "5.2.1",
             "5.2.0",
             "5.1.0",
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/__init__.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/adx.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/adx.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/asb.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/asb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/base_azure.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/base_azure.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/batch.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/container_instance.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/container_instance.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/container_registry.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/container_registry.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/container_volume.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/container_volume.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/cosmos.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/data_lake.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/data_lake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/fileshare.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/fileshare.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/synapse.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/synapse.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/hooks/wasb.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/hooks/wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/log/__init__.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/log/wasb_task_handler.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/__init__.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/adls.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/adls.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/adx.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/adx.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/asb.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/asb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/batch.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/container_instances.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/container_instances.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/cosmos.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/synapse.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/synapse.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/secrets/__init__.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/secrets/key_vault.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/secrets/key_vault.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/sensors/__init__.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/sensors/cosmos.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/sensors/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/sensors/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/sensors/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/sensors/wasb.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/sensors/wasb.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,25 +74,26 @@
     def execute(self, context: Context) -> None:
         """Defers trigger class to poll for state of the job run until
         it reaches a failure state or success state
         """
         if not self.deferrable:
             super().execute(context=context)
         else:
-            self.defer(
-                timeout=timedelta(seconds=self.timeout),
-                trigger=WasbBlobSensorTrigger(
-                    container_name=self.container_name,
-                    blob_name=self.blob_name,
-                    wasb_conn_id=self.wasb_conn_id,
-                    public_read=self.public_read,
-                    poke_interval=self.poke_interval,
-                ),
-                method_name="execute_complete",
-            )
+            if not self.poke(context=context):
+                self.defer(
+                    timeout=timedelta(seconds=self.timeout),
+                    trigger=WasbBlobSensorTrigger(
+                        container_name=self.container_name,
+                        blob_name=self.blob_name,
+                        wasb_conn_id=self.wasb_conn_id,
+                        public_read=self.public_read,
+                        poke_interval=self.poke_interval,
+                    ),
+                    method_name="execute_complete",
+                )
 
     def execute_complete(self, context: Context, event: dict[str, str]) -> None:
         """
         Callback for when the trigger fires - returns immediately.
         Relies on trigger to throw an exception, otherwise it assumes execution was
         successful.
         """
@@ -168,24 +169,25 @@
     def execute(self, context: Context) -> None:
         """Defers trigger class to poll for state of the job run until it
         reaches a failure state or success state
         """
         if not self.deferrable:
             super().execute(context=context)
         else:
-            self.defer(
-                timeout=timedelta(seconds=self.timeout),
-                trigger=WasbPrefixSensorTrigger(
-                    container_name=self.container_name,
-                    prefix=self.prefix,
-                    wasb_conn_id=self.wasb_conn_id,
-                    poke_interval=self.poke_interval,
-                ),
-                method_name="execute_complete",
-            )
+            if not self.poke(context=context):
+                self.defer(
+                    timeout=timedelta(seconds=self.timeout),
+                    trigger=WasbPrefixSensorTrigger(
+                        container_name=self.container_name,
+                        prefix=self.prefix,
+                        wasb_conn_id=self.wasb_conn_id,
+                        poke_interval=self.poke_interval,
+                    ),
+                    method_name="execute_complete",
+                )
 
     def execute_complete(self, context: Context, event: dict[str, str]) -> None:
         """
         Callback for when the trigger fires - returns immediately.
         Relies on trigger to throw an exception, otherwise it assumes execution was
         successful.
         """
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/transfers/__init__.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/transfers/local_to_adls.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/transfers/local_to_wasb.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/triggers/__init__.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/triggers/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/triggers/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/triggers/wasb.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/triggers/wasb.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         )
 
     async def run(self) -> AsyncIterator[TriggerEvent]:
         """Makes async connection to Azure WASB and polls for existence of a blob with given prefix."""
         prefix_exists = False
         hook = WasbAsyncHook(wasb_conn_id=self.wasb_conn_id, public_read=self.public_read)
         try:
-            async with hook.blob_service_client:
+            async with await hook.get_async_conn():
                 while not prefix_exists:
                     prefix_exists = await hook.check_for_prefix_async(
                         container_name=self.container_name,
                         prefix=self.prefix,
                         include=self.include,
                         delimiter=self.delimiter,
                     )
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/airflow/providers/microsoft/azure/utils.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/airflow/providers/microsoft/azure/utils.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-azure
-Version: 6.1.0rc2
+Version: 6.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-azure package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.1.1/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -21,14 +21,15 @@
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
 Requires-Python: ~=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: google
 Provides-Extra: oracle
 Provides-Extra: sftp
 License-File: LICENSE
@@ -51,38 +52,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-azure``
 
-Release: ``6.1.0rc2``
+Release: ``6.1.1rc1``
 
 
 `Microsoft Azure <https://azure.microsoft.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.azure`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.azure`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-microsoft-azure``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ================================  ==================
 PIP package                       Version required
 ================================  ==================
@@ -149,14 +150,27 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.1.1
+.....
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Fix deferrable mode execution in WasbPrefixSensor (#31411)``
+
+Misc
+~~~~
+
+* ``Optimize deferred mode execution for wasb sensors (#31009)``
+
 6.1.0
 .....
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Features
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/apache_airflow_providers_microsoft_azure.egg-info/requires.txt` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/pyproject.toml` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/setup.cfg` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 	Framework :: Apache Airflow
 	Framework :: Apache Airflow :: Provider
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.1.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.1.1/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -69,10 +70,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.microsoft.azure.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.microsoft.azure
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-microsoft-azure-6.1.0rc2/setup.py` & `apache-airflow-providers-microsoft-azure-6.1.1rc1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-microsoft-azure package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "6.1.0"
+version = "6.1.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-microsoft-azure setup."""
     setup(
         version=version,
         extras_require={
```

