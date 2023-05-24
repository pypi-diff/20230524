# Comparing `tmp/automation_rest_server-3.7.3.tar.gz` & `tmp/automation_rest_server-3.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\automation_rest_server-3.7.3.tar", last modified: Fri May 19 01:43:39 2023, max compression
+gzip compressed data, was "dist\automation_rest_server-3.7.5.tar", last modified: Wed May 24 05:44:00 2023, max compression
```

## Comparing `automation_rest_server-3.7.3.tar` & `automation_rest_server-3.7.5.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/
--rw-rw-rw-   0        0        0     1098 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/LICENSE.txt
--rw-rw-rw-   0        0        0      687 2022-08-30 06:56:12.000000 automation_rest_server-3.7.3/MANIFEST.in
--rw-rw-rw-   0        0        0      551 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/configuration/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/configuration/__init__.py
--rw-rw-rw-   0        0        0      581 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/configuration/config.yaml
--rw-rw-rw-   0        0        0     1099 2022-12-13 11:04:16.000000 automation_rest_server-3.7.3/automation_rest_server/configuration/firmware_build.yaml
--rw-rw-rw-   0        0        0  1333232 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/configuration/pci.ids
--rw-rw-rw-   0        0        0      157 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/configuration/version.yaml
--rw-rw-rw-   0        0        0       83 2022-08-25 03:13:17.000000 automation_rest_server-3.7.3/automation_rest_server/configuration/web_server.yaml
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/rest_client/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:18:57.000000 automation_rest_server-3.7.3/automation_rest_server/rest_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/rest_client/resource/
--rw-rw-rw-   0        0        0        0 2022-08-10 09:04:38.000000 automation_rest_server-3.7.3/automation_rest_server/rest_client/resource/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/rest_client/resource/models/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:20:01.000000 automation_rest_server-3.7.3/automation_rest_server/rest_client/resource/models/__init__.py
--rw-rw-rw-   0        0        0     4257 2023-05-10 02:20:31.000000 automation_rest_server-3.7.3/automation_rest_server/rest_client/resource/models/helper.py
--rw-rw-rw-   0        0        0     1944 2022-08-17 05:58:24.000000 automation_rest_server-3.7.3/automation_rest_server/rest_client/resource/node_resource.py
--rw-rw-rw-   0        0        0     1374 2022-08-30 04:43:20.000000 automation_rest_server-3.7.3/automation_rest_server/rest_client/resource/test_resource.py
--rw-rw-rw-   0        0        0      340 2022-08-25 03:00:40.000000 automation_rest_server-3.7.3/automation_rest_server/rest_client/resource/web_resource.py
--rw-rw-rw-   0        0        0     2536 2023-02-21 08:02:23.000000 automation_rest_server-3.7.3/automation_rest_server/rest_client/web_rest_client.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/rest_server/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/rest_server/__init__.py
--rw-rw-rw-   0        0        0     1678 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/rest_server/reset_server.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/__init__.py
--rw-rw-rw-   0        0        0     2150 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/benchmark_resource.py
--rw-rw-rw-   0        0        0     1956 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/build_firmware_resource.py
--rw-rw-rw-   0        0        0      933 2022-12-12 01:57:01.000000 automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/git_resource.py
--rw-rw-rw-   0        0        0      850 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/models/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/models/__init__.py
--rw-rw-rw-   0        0        0     2044 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/models/ftp_server.py
--rw-rw-rw-   0        0        0     1732 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/models/helper.py
--rw-rw-rw-   0        0        0      958 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/oakgate_resource.py
--rw-rw-rw-   0        0        0      691 2022-08-11 02:31:16.000000 automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/operation_resource.py
--rw-rw-rw-   0        0        0     1641 2022-09-20 01:54:25.000000 automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/state_resource.py
--rw-rw-rw-   0        0        0     1085 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/stop_flag_resource.py
--rw-rw-rw-   0        0        0     6233 2022-12-03 07:36:31.000000 automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/test_resource.py
--rw-rw-rw-   0        0        0     1295 2023-05-10 02:20:31.000000 automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/upgrade_resource.py
--rw-rw-rw-   0        0        0     6063 2023-05-04 07:05:41.000000 automation_rest_server-3.7.3/automation_rest_server/run.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/__init__.py
--rw-rw-rw-   0        0        0     6679 2022-09-20 04:46:34.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/database.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/dut/
--rw-rw-rw-   0        0        0        0 2021-11-12 08:10:50.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/dut/__init__.py
--rw-rw-rw-   0        0        0     3082 2023-04-19 05:40:44.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/dut/slot.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/dut/sub_slot/
--rw-rw-rw-   0        0        0        0 2021-11-24 03:48:51.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/dut/sub_slot/__init__.py
--rw-rw-rw-   0        0        0     1434 2022-09-15 07:43:45.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py
--rw-rw-rw-   0        0        0     3541 2023-04-17 06:49:22.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py
--rw-rw-rw-   0        0        0      901 2023-04-19 03:39:13.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py
--rw-rw-rw-   0        0        0     8894 2023-05-09 09:27:56.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/engine/
--rw-rw-rw-   0        0        0      214 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/engine/__init__.py
--rw-rw-rw-   0        0        0     3336 2023-05-19 01:43:00.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/engine/nose_engine.py
--rw-rw-rw-   0        0        0     4926 2023-02-16 01:39:59.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/engine/oakgate_engine.py
--rw-rw-rw-   0        0        0     4007 2023-03-02 06:19:25.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/engine/perses_engine.py
--rw-rw-rw-   0        0        0     1489 2022-09-30 01:53:36.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py
--rw-rw-rw-   0        0        0      239 2023-04-07 02:04:12.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/engine/special_parameter.py
--rw-rw-rw-   0        0        0     3562 2022-09-20 07:48:14.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/engine/sse_engine.py
--rw-rw-rw-   0        0        0     3986 2023-05-12 01:47:10.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/engine/venus_engine.py
--rw-rw-rw-   0        0        0     1517 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_build.py
--rw-rw-rw-   0        0        0     3049 2023-05-10 02:58:49.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_download.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_engine/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_engine/__init__.py
--rw-rw-rw-   0        0        0     7168 2022-12-13 11:05:02.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py
--rw-rw-rw-   0        0        0     6204 2023-05-11 09:15:12.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_engine/logic_with_firmware_engine.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_engine/oakgate/
--rw-rw-rw-   0        0        0        0 2023-04-11 02:31:20.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_engine/oakgate/__init__.py
--rw-rw-rw-   0        0        0     2925 2023-04-11 02:43:50.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_engine/oakgate/nvme_download.py
--rw-rw-rw-   0        0        0     2691 2023-04-17 07:35:59.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_engine/oakgate/two_step_download.py
--rw-rw-rw-   0        0        0      671 2023-05-10 02:30:29.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py
--rw-rw-rw-   0        0        0     1996 2023-05-10 03:22:37.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py
--rw-rw-rw-   0        0        0     1585 2023-05-10 02:30:15.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py
--rw-rw-rw-   0        0        0     2344 2023-04-09 02:31:46.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py
--rw-rw-rw-   0        0        0     5139 2023-05-10 07:14:09.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/node_database.py
--rw-rw-rw-   0        0        0    10717 2023-04-19 03:38:41.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/performance_database.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/reboot_engine/
--rw-rw-rw-   0        0        0       50 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/reboot_engine/__init__.py
--rw-rw-rw-   0        0        0     2439 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py
--rw-rw-rw-   0        0        0     2055 2023-05-10 02:51:26.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/state.py
--rw-rw-rw-   0        0        0      672 2022-12-13 03:29:14.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/status_file.py
--rw-rw-rw-   0        0        0     5684 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/test_base.py
--rw-rw-rw-   0        0        0     1973 2023-02-14 08:06:21.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/test_benchmark.py
--rw-rw-rw-   0        0        0     3512 2023-02-07 07:54:27.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/test_benchmark_group.py
--rw-rw-rw-   0        0        0     1263 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/test_case.py
--rw-rw-rw-   0        0        0    22062 2023-05-10 02:21:32.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/test_pool.py
--rw-rw-rw-   0        0        0      892 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/test_reboot_handle.py
--rw-rw-rw-   0        0        0     4485 2023-05-12 02:37:27.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/test_result.py
--rw-rw-rw-   0        0        0     3757 2023-03-02 10:28:02.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/test_runner.py
--rw-rw-rw-   0        0        0     4717 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/test_framework/test_suite.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/tool/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/tool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/
--rw-rw-rw-   0        0        0        0 2021-11-12 06:54:04.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/dll/
--rw-rw-rw-   0        0        0        0 2021-10-23 02:17:43.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/dll/__init__.py
--rw-rw-rw-   0        0        0    24064 2021-10-23 02:17:43.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/dll/buf.dll
--rw-rw-rw-   0        0        0    12760 2021-10-23 02:17:43.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/dll/buf.so
--rw-rw-rw-   0        0        0      777 2021-10-23 02:17:43.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/dll/build.py
--rw-rw-rw-   0        0        0      861 2022-09-15 07:43:45.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/linux_nvme.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/
--rw-rw-rw-   0        0        0        0 2021-11-23 06:34:00.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/__init__.py
--rw-rw-rw-   0        0        0    14077 2021-11-23 06:29:25.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/buf.py
--rw-rw-rw-   0        0        0     4722 2021-11-23 06:25:09.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/ctype.py
--rw-rw-rw-   0        0        0    39204 2021-11-23 06:28:50.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/get_feature.py
--rw-rw-rw-   0        0        0    38547 2022-09-15 07:43:45.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/ioctl.py
--rw-rw-rw-   0        0        0    23303 2022-09-15 07:42:03.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/nvme.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/struct/
--rw-rw-rw-   0        0        0      256 2021-11-23 06:21:15.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/struct/__init__.py
--rw-rw-rw-   0        0        0    30449 2021-11-23 06:59:35.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/struct/command.py
--rw-rw-rw-   0        0        0    15322 2021-11-23 06:59:35.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/struct/features.py
--rw-rw-rw-   0        0        0     1104 2021-10-23 02:17:43.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/struct/hmb.py
--rw-rw-rw-   0        0        0    16135 2021-11-23 07:31:19.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/struct/identify.py
--rw-rw-rw-   0        0        0    13915 2021-11-23 06:59:59.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/struct/log_page.py
--rw-rw-rw-   0        0        0     2361 2021-11-12 10:37:37.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/struct/memory.py
--rw-rw-rw-   0        0        0    10510 2021-10-23 02:17:43.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/struct/pcie.py
--rw-rw-rw-   0        0        0    35527 2021-10-23 02:17:43.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/struct/registers.py
--rw-rw-rw-   0        0        0     9095 2021-11-24 06:24:21.000000 automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/utility_vu.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/tool/diskpart/
--rw-rw-rw-   0        0        0       56 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/tool/diskpart/__init__.py
--rw-rw-rw-   0        0        0      770 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/tool/diskpart/diskpart.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/tool/fio/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/tool/fio/__init__.py
--rw-rw-rw-   0        0        0    18967 2023-02-23 03:46:38.000000 automation_rest_server-3.7.3/automation_rest_server/tool/fio/fio.py
--rw-rw-rw-   0        0        0     5032 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/tool/fio/fio_linux.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/tool/fio/tool/
--rw-rw-rw-   0        0        0  4733892 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/tool/fio/tool/fio
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/tool/git/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/tool/git/__init__.py
--rw-rw-rw-   0        0        0     5645 2023-03-02 10:20:30.000000 automation_rest_server-3.7.3/automation_rest_server/tool/git/git_operator.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/tool/iometer/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/tool/iometer/__init__.py
--rw-rw-rw-   0        0        0     9223 2023-02-07 08:25:51.000000 automation_rest_server-3.7.3/automation_rest_server/tool/iometer/iometer.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server/utils/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/utils/__init__.py
--rw-rw-rw-   0        0        0    12385 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/utils/buf.py
--rw-rw-rw-   0        0        0     5636 2023-04-10 09:29:00.000000 automation_rest_server-3.7.3/automation_rest_server/utils/firmware_path.py
--rw-rw-rw-   0        0        0     3697 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/utils/log.py
--rw-rw-rw-   0        0        0      386 2023-02-23 02:34:33.000000 automation_rest_server-3.7.3/automation_rest_server/utils/message.py
--rw-rw-rw-   0        0        0     3532 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/utils/nose_xml.py
--rw-rw-rw-   0        0        0     1742 2022-09-20 07:22:33.000000 automation_rest_server-3.7.3/automation_rest_server/utils/pip_operation.py
--rw-rw-rw-   0        0        0     1823 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/utils/process.py
--rw-rw-rw-   0        0        0     3226 2023-05-11 09:28:31.000000 automation_rest_server-3.7.3/automation_rest_server/utils/serial_tool.py
--rw-rw-rw-   0        0        0     9222 2022-06-02 02:49:38.000000 automation_rest_server-3.7.3/automation_rest_server/utils/ssh.py
--rw-rw-rw-   0        0        0     5366 2022-12-22 01:47:58.000000 automation_rest_server-3.7.3/automation_rest_server/utils/system.py
-drwxrwxrwx   0        0        0        0 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server.egg-info/
--rw-rw-rw-   0        0        0      551 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7047 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      107 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/automation_rest_server.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       64 2023-05-19 01:43:39.000000 automation_rest_server-3.7.3/setup.cfg
--rw-rw-rw-   0        0        0     1248 2023-05-19 01:43:28.000000 automation_rest_server-3.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:44:00.000000 automation_rest_server-3.7.5/
+-rw-rw-rw-   0        0        0     1098 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      687 2022-08-30 06:56:12.000000 automation_rest_server-3.7.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      551 2023-05-24 05:44:00.000000 automation_rest_server-3.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-24 05:43:58.000000 automation_rest_server-3.7.5/automation_rest_server/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:43:59.000000 automation_rest_server-3.7.5/automation_rest_server/configuration/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/configuration/__init__.py
+-rw-rw-rw-   0        0        0      581 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/configuration/config.yaml
+-rw-rw-rw-   0        0        0     1099 2022-12-13 11:04:16.000000 automation_rest_server-3.7.5/automation_rest_server/configuration/firmware_build.yaml
+-rw-rw-rw-   0        0        0  1333232 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/configuration/pci.ids
+-rw-rw-rw-   0        0        0      157 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/configuration/version.yaml
+-rw-rw-rw-   0        0        0       83 2022-08-25 03:13:17.000000 automation_rest_server-3.7.5/automation_rest_server/configuration/web_server.yaml
+drwxrwxrwx   0        0        0        0 2023-05-24 05:43:59.000000 automation_rest_server-3.7.5/automation_rest_server/rest_client/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:18:57.000000 automation_rest_server-3.7.5/automation_rest_server/rest_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:43:59.000000 automation_rest_server-3.7.5/automation_rest_server/rest_client/resource/
+-rw-rw-rw-   0        0        0        0 2022-08-10 09:04:38.000000 automation_rest_server-3.7.5/automation_rest_server/rest_client/resource/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:43:59.000000 automation_rest_server-3.7.5/automation_rest_server/rest_client/resource/models/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:20:01.000000 automation_rest_server-3.7.5/automation_rest_server/rest_client/resource/models/__init__.py
+-rw-rw-rw-   0        0        0     4257 2023-05-10 02:20:31.000000 automation_rest_server-3.7.5/automation_rest_server/rest_client/resource/models/helper.py
+-rw-rw-rw-   0        0        0     1944 2022-08-17 05:58:24.000000 automation_rest_server-3.7.5/automation_rest_server/rest_client/resource/node_resource.py
+-rw-rw-rw-   0        0        0     1374 2022-08-30 04:43:20.000000 automation_rest_server-3.7.5/automation_rest_server/rest_client/resource/test_resource.py
+-rw-rw-rw-   0        0        0      340 2022-08-25 03:00:40.000000 automation_rest_server-3.7.5/automation_rest_server/rest_client/resource/web_resource.py
+-rw-rw-rw-   0        0        0     2536 2023-02-21 08:02:23.000000 automation_rest_server-3.7.5/automation_rest_server/rest_client/web_rest_client.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:43:59.000000 automation_rest_server-3.7.5/automation_rest_server/rest_server/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/rest_server/__init__.py
+-rw-rw-rw-   0        0        0     1678 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/rest_server/reset_server.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:43:59.000000 automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/__init__.py
+-rw-rw-rw-   0        0        0     2150 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/benchmark_resource.py
+-rw-rw-rw-   0        0        0     1956 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/build_firmware_resource.py
+-rw-rw-rw-   0        0        0      933 2022-12-12 01:57:01.000000 automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/git_resource.py
+-rw-rw-rw-   0        0        0      850 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:43:59.000000 automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/models/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/models/__init__.py
+-rw-rw-rw-   0        0        0     2044 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/models/ftp_server.py
+-rw-rw-rw-   0        0        0     1732 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/models/helper.py
+-rw-rw-rw-   0        0        0      958 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/oakgate_resource.py
+-rw-rw-rw-   0        0        0      691 2022-08-11 02:31:16.000000 automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/operation_resource.py
+-rw-rw-rw-   0        0        0     1641 2022-09-20 01:54:25.000000 automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/state_resource.py
+-rw-rw-rw-   0        0        0     1085 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/stop_flag_resource.py
+-rw-rw-rw-   0        0        0     6233 2022-12-03 07:36:31.000000 automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/test_resource.py
+-rw-rw-rw-   0        0        0     1295 2023-05-10 02:20:31.000000 automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/upgrade_resource.py
+-rw-rw-rw-   0        0        0     6063 2023-05-04 07:05:41.000000 automation_rest_server-3.7.5/automation_rest_server/run.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:43:59.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/__init__.py
+-rw-rw-rw-   0        0        0     6679 2022-09-20 04:46:34.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/database.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:43:59.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/dut/
+-rw-rw-rw-   0        0        0        0 2021-11-12 08:10:50.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/dut/__init__.py
+-rw-rw-rw-   0        0        0     3082 2023-04-19 05:40:44.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/dut/slot.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:43:59.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/dut/sub_slot/
+-rw-rw-rw-   0        0        0        0 2021-11-24 03:48:51.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/dut/sub_slot/__init__.py
+-rw-rw-rw-   0        0        0     1434 2022-09-15 07:43:45.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py
+-rw-rw-rw-   0        0        0     3541 2023-04-17 06:49:22.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py
+-rw-rw-rw-   0        0        0      901 2023-04-19 03:39:13.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py
+-rw-rw-rw-   0        0        0     8894 2023-05-09 09:27:56.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:43:59.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/engine/
+-rw-rw-rw-   0        0        0      214 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/engine/__init__.py
+-rw-rw-rw-   0        0        0     3336 2023-05-24 05:43:06.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/engine/nose_engine.py
+-rw-rw-rw-   0        0        0     4926 2023-02-16 01:39:59.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/engine/oakgate_engine.py
+-rw-rw-rw-   0        0        0     4007 2023-03-02 06:19:25.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/engine/perses_engine.py
+-rw-rw-rw-   0        0        0     1489 2022-09-30 01:53:36.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py
+-rw-rw-rw-   0        0        0      239 2023-04-07 02:04:12.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/engine/special_parameter.py
+-rw-rw-rw-   0        0        0     3562 2022-09-20 07:48:14.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/engine/sse_engine.py
+-rw-rw-rw-   0        0        0     3986 2023-05-12 01:47:10.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/engine/venus_engine.py
+-rw-rw-rw-   0        0        0     1517 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_build.py
+-rw-rw-rw-   0        0        0     3049 2023-05-10 02:58:49.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_download.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:43:59.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_engine/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_engine/__init__.py
+-rw-rw-rw-   0        0        0     7168 2022-12-13 11:05:02.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py
+-rw-rw-rw-   0        0        0     6204 2023-05-11 09:15:12.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_engine/logic_with_firmware_engine.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:43:59.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_engine/oakgate/
+-rw-rw-rw-   0        0        0        0 2023-04-11 02:31:20.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_engine/oakgate/__init__.py
+-rw-rw-rw-   0        0        0     2925 2023-04-11 02:43:50.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_engine/oakgate/nvme_download.py
+-rw-rw-rw-   0        0        0     2691 2023-04-17 07:35:59.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_engine/oakgate/two_step_download.py
+-rw-rw-rw-   0        0        0      671 2023-05-10 02:30:29.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py
+-rw-rw-rw-   0        0        0     1996 2023-05-10 03:22:37.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py
+-rw-rw-rw-   0        0        0     1585 2023-05-10 02:30:15.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py
+-rw-rw-rw-   0        0        0     2344 2023-04-09 02:31:46.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py
+-rw-rw-rw-   0        0        0     5139 2023-05-10 07:14:09.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/node_database.py
+-rw-rw-rw-   0        0        0    10717 2023-04-19 03:38:41.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/performance_database.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:43:59.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/reboot_engine/
+-rw-rw-rw-   0        0        0       50 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/reboot_engine/__init__.py
+-rw-rw-rw-   0        0        0     2439 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py
+-rw-rw-rw-   0        0        0     2055 2023-05-10 02:51:26.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/state.py
+-rw-rw-rw-   0        0        0      672 2022-12-13 03:29:14.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/status_file.py
+-rw-rw-rw-   0        0        0     5684 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/test_base.py
+-rw-rw-rw-   0        0        0     1973 2023-02-14 08:06:21.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/test_benchmark.py
+-rw-rw-rw-   0        0        0     3512 2023-02-07 07:54:27.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/test_benchmark_group.py
+-rw-rw-rw-   0        0        0     1263 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/test_case.py
+-rw-rw-rw-   0        0        0    22062 2023-05-10 02:21:32.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/test_pool.py
+-rw-rw-rw-   0        0        0      892 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/test_reboot_handle.py
+-rw-rw-rw-   0        0        0     4485 2023-05-12 02:37:27.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/test_result.py
+-rw-rw-rw-   0        0        0     3757 2023-03-02 10:28:02.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/test_runner.py
+-rw-rw-rw-   0        0        0     4717 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/test_framework/test_suite.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:43:59.000000 automation_rest_server-3.7.5/automation_rest_server/tool/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/tool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:44:00.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/
+-rw-rw-rw-   0        0        0        0 2021-11-12 06:54:04.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:44:00.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/dll/
+-rw-rw-rw-   0        0        0        0 2021-10-23 02:17:43.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/dll/__init__.py
+-rw-rw-rw-   0        0        0    24064 2021-10-23 02:17:43.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/dll/buf.dll
+-rw-rw-rw-   0        0        0    12760 2021-10-23 02:17:43.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/dll/buf.so
+-rw-rw-rw-   0        0        0      777 2021-10-23 02:17:43.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/dll/build.py
+-rw-rw-rw-   0        0        0      861 2022-09-15 07:43:45.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/linux_nvme.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:44:00.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/
+-rw-rw-rw-   0        0        0        0 2021-11-23 06:34:00.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/__init__.py
+-rw-rw-rw-   0        0        0    14077 2021-11-23 06:29:25.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/buf.py
+-rw-rw-rw-   0        0        0     4722 2021-11-23 06:25:09.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/ctype.py
+-rw-rw-rw-   0        0        0    39204 2021-11-23 06:28:50.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/get_feature.py
+-rw-rw-rw-   0        0        0    38547 2022-09-15 07:43:45.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/ioctl.py
+-rw-rw-rw-   0        0        0    23303 2022-09-15 07:42:03.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/nvme.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:44:00.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/struct/
+-rw-rw-rw-   0        0        0      256 2021-11-23 06:21:15.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/struct/__init__.py
+-rw-rw-rw-   0        0        0    30449 2021-11-23 06:59:35.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/struct/command.py
+-rw-rw-rw-   0        0        0    15322 2021-11-23 06:59:35.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/struct/features.py
+-rw-rw-rw-   0        0        0     1104 2021-10-23 02:17:43.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/struct/hmb.py
+-rw-rw-rw-   0        0        0    16135 2021-11-23 07:31:19.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/struct/identify.py
+-rw-rw-rw-   0        0        0    13915 2021-11-23 06:59:59.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/struct/log_page.py
+-rw-rw-rw-   0        0        0     2361 2021-11-12 10:37:37.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/struct/memory.py
+-rw-rw-rw-   0        0        0    10510 2021-10-23 02:17:43.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/struct/pcie.py
+-rw-rw-rw-   0        0        0    35527 2021-10-23 02:17:43.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/struct/registers.py
+-rw-rw-rw-   0        0        0     9095 2021-11-24 06:24:21.000000 automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/utility_vu.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:44:00.000000 automation_rest_server-3.7.5/automation_rest_server/tool/diskpart/
+-rw-rw-rw-   0        0        0       56 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/tool/diskpart/__init__.py
+-rw-rw-rw-   0        0        0      770 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/tool/diskpart/diskpart.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:44:00.000000 automation_rest_server-3.7.5/automation_rest_server/tool/fio/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/tool/fio/__init__.py
+-rw-rw-rw-   0        0        0    18967 2023-02-23 03:46:38.000000 automation_rest_server-3.7.5/automation_rest_server/tool/fio/fio.py
+-rw-rw-rw-   0        0        0     5032 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/tool/fio/fio_linux.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:44:00.000000 automation_rest_server-3.7.5/automation_rest_server/tool/fio/tool/
+-rw-rw-rw-   0        0        0  4733892 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/tool/fio/tool/fio
+drwxrwxrwx   0        0        0        0 2023-05-24 05:44:00.000000 automation_rest_server-3.7.5/automation_rest_server/tool/git/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/tool/git/__init__.py
+-rw-rw-rw-   0        0        0     5645 2023-03-02 10:20:30.000000 automation_rest_server-3.7.5/automation_rest_server/tool/git/git_operator.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:44:00.000000 automation_rest_server-3.7.5/automation_rest_server/tool/iometer/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/tool/iometer/__init__.py
+-rw-rw-rw-   0        0        0     9223 2023-02-07 08:25:51.000000 automation_rest_server-3.7.5/automation_rest_server/tool/iometer/iometer.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:44:00.000000 automation_rest_server-3.7.5/automation_rest_server/utils/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/utils/__init__.py
+-rw-rw-rw-   0        0        0    12385 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/utils/buf.py
+-rw-rw-rw-   0        0        0     5636 2023-04-10 09:29:00.000000 automation_rest_server-3.7.5/automation_rest_server/utils/firmware_path.py
+-rw-rw-rw-   0        0        0     3697 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/utils/log.py
+-rw-rw-rw-   0        0        0      386 2023-02-23 02:34:33.000000 automation_rest_server-3.7.5/automation_rest_server/utils/message.py
+-rw-rw-rw-   0        0        0     3532 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/utils/nose_xml.py
+-rw-rw-rw-   0        0        0     1742 2022-09-20 07:22:33.000000 automation_rest_server-3.7.5/automation_rest_server/utils/pip_operation.py
+-rw-rw-rw-   0        0        0     1823 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/utils/process.py
+-rw-rw-rw-   0        0        0     3226 2023-05-11 09:28:31.000000 automation_rest_server-3.7.5/automation_rest_server/utils/serial_tool.py
+-rw-rw-rw-   0        0        0     9222 2022-06-02 02:49:38.000000 automation_rest_server-3.7.5/automation_rest_server/utils/ssh.py
+-rw-rw-rw-   0        0        0     5366 2022-12-22 01:47:58.000000 automation_rest_server-3.7.5/automation_rest_server/utils/system.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:43:58.000000 automation_rest_server-3.7.5/automation_rest_server.egg-info/
+-rw-rw-rw-   0        0        0      551 2023-05-24 05:43:58.000000 automation_rest_server-3.7.5/automation_rest_server.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7047 2023-05-24 05:43:58.000000 automation_rest_server-3.7.5/automation_rest_server.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 05:43:58.000000 automation_rest_server-3.7.5/automation_rest_server.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-05-24 05:43:58.000000 automation_rest_server-3.7.5/automation_rest_server.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      107 2023-05-24 05:43:58.000000 automation_rest_server-3.7.5/automation_rest_server.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-05-24 05:43:58.000000 automation_rest_server-3.7.5/automation_rest_server.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       64 2023-05-24 05:44:00.000000 automation_rest_server-3.7.5/setup.cfg
+-rw-rw-rw-   0        0        0     1248 2023-05-24 05:43:41.000000 automation_rest_server-3.7.5/setup.py
```

### Comparing `automation_rest_server-3.7.3/LICENSE.txt` & `automation_rest_server-3.7.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/MANIFEST.in` & `automation_rest_server-3.7.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/PKG-INFO` & `automation_rest_server-3.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: automation_rest_server
-Version: 3.7.3
+Version: 3.7.5
 Summary: NVMe production server
 Home-page: https://pypi.org/project/automation_rest_server
 Author: yuwen123441
 Author-email: yuwen123441@126.com
 License: MIT License
 Description: UNKNOWN
 Keywords: runner,server
```

### Comparing `automation_rest_server-3.7.3/automation_rest_server/configuration/config.yaml` & `automation_rest_server-3.7.5/automation_rest_server/configuration/config.yaml`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/configuration/firmware_build.yaml` & `automation_rest_server-3.7.5/automation_rest_server/configuration/firmware_build.yaml`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/configuration/pci.ids` & `automation_rest_server-3.7.5/automation_rest_server/configuration/pci.ids`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/rest_client/resource/models/helper.py` & `automation_rest_server-3.7.5/automation_rest_server/rest_client/resource/models/helper.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/rest_client/resource/node_resource.py` & `automation_rest_server-3.7.5/automation_rest_server/rest_client/resource/node_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/rest_client/resource/test_resource.py` & `automation_rest_server-3.7.5/automation_rest_server/rest_client/resource/test_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/rest_client/web_rest_client.py` & `automation_rest_server-3.7.5/automation_rest_server/rest_client/web_rest_client.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/rest_server/reset_server.py` & `automation_rest_server-3.7.5/automation_rest_server/rest_server/reset_server.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/benchmark_resource.py` & `automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/benchmark_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/build_firmware_resource.py` & `automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/build_firmware_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/git_resource.py` & `automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/git_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py` & `automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/models/ftp_server.py` & `automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/models/ftp_server.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/models/helper.py` & `automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/models/helper.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/oakgate_resource.py` & `automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/oakgate_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/operation_resource.py` & `automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/operation_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/state_resource.py` & `automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/state_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/stop_flag_resource.py` & `automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/stop_flag_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/test_resource.py` & `automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/test_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/rest_server/resource/upgrade_resource.py` & `automation_rest_server-3.7.5/automation_rest_server/rest_server/resource/upgrade_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/run.py` & `automation_rest_server-3.7.5/automation_rest_server/run.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/database.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/database.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/dut/slot.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/dut/slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/engine/nose_engine.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/engine/nose_engine.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 
 class NoseEngine(object):
 
     def __init__(self):
         self.prun_port = os.environ.get("prun_port", 5000)
         self.working_path = os.environ["working_path"]
-        self.log_path = self.get_log_path()
         self.ip = get_ip_address()
+        self.log_path = self.get_log_path()
 
     def get_log_path(self):
         log_base_path = os.path.join(self.working_path, "log")
         if os.path.exists(log_base_path) is False:
             os.mkdir(log_base_path)
         if self.ip is not None:
             log_ip = os.path.join(log_base_path, self.ip)
```

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/engine/oakgate_engine.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/engine/oakgate_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/engine/perses_engine.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/engine/perses_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/engine/sse_engine.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/engine/sse_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/engine/venus_engine.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/engine/venus_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_build.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_build.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_download.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_download.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_engine/logic_with_firmware_engine.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_engine/logic_with_firmware_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_engine/oakgate/nvme_download.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_engine/oakgate/nvme_download.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_engine/oakgate/two_step_download.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_engine/oakgate/two_step_download.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/node_database.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/node_database.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/performance_database.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/performance_database.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/state.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/state.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/status_file.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/status_file.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/test_base.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/test_base.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/test_benchmark.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/test_benchmark_group.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/test_benchmark_group.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/test_case.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/test_case.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/test_pool.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/test_pool.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/test_reboot_handle.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/test_reboot_handle.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/test_result.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/test_result.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/test_runner.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/test_runner.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/test_framework/test_suite.py` & `automation_rest_server-3.7.5/automation_rest_server/test_framework/test_suite.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/device/dll/buf.dll` & `automation_rest_server-3.7.5/automation_rest_server/tool/device/dll/buf.dll`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/device/dll/buf.so` & `automation_rest_server-3.7.5/automation_rest_server/tool/device/dll/buf.so`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/device/dll/build.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/device/dll/build.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/device/linux_nvme.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/device/linux_nvme.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/buf.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/buf.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/ctype.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/ctype.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/get_feature.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/get_feature.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/ioctl.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/ioctl.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/nvme.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/nvme.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/struct/command.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/struct/command.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/struct/features.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/struct/features.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/struct/hmb.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/struct/hmb.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/struct/identify.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/struct/identify.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/struct/log_page.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/struct/log_page.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/struct/memory.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/struct/memory.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/struct/pcie.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/struct/pcie.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/struct/registers.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/struct/registers.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/device/nvme/utility_vu.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/device/nvme/utility_vu.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/diskpart/diskpart.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/diskpart/diskpart.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/fio/fio.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/fio/fio.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/fio/fio_linux.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/fio/fio_linux.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/fio/tool/fio` & `automation_rest_server-3.7.5/automation_rest_server/tool/fio/tool/fio`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/git/git_operator.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/git/git_operator.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/tool/iometer/iometer.py` & `automation_rest_server-3.7.5/automation_rest_server/tool/iometer/iometer.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/utils/buf.py` & `automation_rest_server-3.7.5/automation_rest_server/utils/buf.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/utils/firmware_path.py` & `automation_rest_server-3.7.5/automation_rest_server/utils/firmware_path.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/utils/log.py` & `automation_rest_server-3.7.5/automation_rest_server/utils/log.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/utils/nose_xml.py` & `automation_rest_server-3.7.5/automation_rest_server/utils/nose_xml.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/utils/pip_operation.py` & `automation_rest_server-3.7.5/automation_rest_server/utils/pip_operation.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/utils/process.py` & `automation_rest_server-3.7.5/automation_rest_server/utils/process.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/utils/serial_tool.py` & `automation_rest_server-3.7.5/automation_rest_server/utils/serial_tool.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/utils/ssh.py` & `automation_rest_server-3.7.5/automation_rest_server/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server/utils/system.py` & `automation_rest_server-3.7.5/automation_rest_server/utils/system.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/automation_rest_server.egg-info/PKG-INFO` & `automation_rest_server-3.7.5/automation_rest_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: automation-rest-server
-Version: 3.7.3
+Version: 3.7.5
 Summary: NVMe production server
 Home-page: https://pypi.org/project/automation_rest_server
 Author: yuwen123441
 Author-email: yuwen123441@126.com
 License: MIT License
 Description: UNKNOWN
 Keywords: runner,server
```

### Comparing `automation_rest_server-3.7.3/automation_rest_server.egg-info/SOURCES.txt` & `automation_rest_server-3.7.5/automation_rest_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.7.3/setup.py` & `automation_rest_server-3.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 packages = ["automation_rest_server"]
 #python setup.py sdist upload  
 #python setup.py bdist_wheel
 
 setup(
     name = 'automation_rest_server',
-    version = '3.7.3',
+    version = '3.7.5',
     keywords = ['runner', 'server'],
     description = 'NVMe production server',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'License :: OSI Approved :: MIT License',
```

