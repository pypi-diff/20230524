# Comparing `tmp/joulescope-1.1.4.tar.gz` & `tmp/joulescope-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joulescope-1.1.4.tar", last modified: Fri Apr 28 18:57:57 2023, max compression
+gzip compressed data, was "joulescope-1.1.5.tar", last modified: Wed May 24 19:33:40 2023, max compression
```

## Comparing `joulescope-1.1.4.tar` & `joulescope-1.1.5.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 18:57:57.580541 joulescope-1.1.4/
--rw-rw-rw-   0        0        0    21719 2023-04-28 18:43:33.000000 joulescope-1.1.4/CHANGELOG.md
--rw-rw-rw-   0        0        0     6771 2020-08-11 21:29:57.000000 joulescope-1.1.4/CREDITS.html
--rw-rw-rw-   0        0        0    11558 2020-05-30 15:27:09.000000 joulescope-1.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0      132 2022-11-07 18:35:15.000000 joulescope-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3628 2023-04-28 18:57:57.581543 joulescope-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1762 2020-11-25 13:12:14.000000 joulescope-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 18:57:57.544463 joulescope-1.1.4/joulescope/
--rw-rw-rw-   0        0        0     2291 2023-03-20 19:38:30.000000 joulescope-1.1.4/joulescope/__init__.py
--rw-rw-rw-   0        0        0      730 2020-05-30 15:27:09.000000 joulescope-1.1.4/joulescope/__main__.py
--rw-rw-rw-   0        0        0    54968 2023-03-11 15:21:25.000000 joulescope-1.1.4/joulescope/data_recorder.py
--rw-rw-rw-   0        0        0    26397 2022-09-09 13:37:25.000000 joulescope-1.1.4/joulescope/datafile.py
-drwxrwxrwx   0        0        0        0 2023-04-28 18:57:57.557995 joulescope-1.1.4/joulescope/entry_points/
--rw-rw-rw-   0        0        0        0 2020-05-30 15:27:09.000000 joulescope-1.1.4/joulescope/entry_points/__init__.py
--rw-rw-rw-   0        0        0     1325 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/entry_points/bootloader_go.py
--rw-rw-rw-   0        0        0     4040 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/entry_points/capture.py
--rw-rw-rw-   0        0        0     1530 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/entry_points/gpo_demo.py
--rw-rw-rw-   0        0        0     2103 2023-04-19 20:18:48.000000 joulescope-1.1.4/joulescope/entry_points/info.py
--rw-rw-rw-   0        0        0     2110 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/entry_points/parameter_set.py
--rw-rw-rw-   0        0        0     5043 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/entry_points/program.py
--rw-rw-rw-   0        0        0     6546 2022-09-10 13:15:16.000000 joulescope-1.1.4/joulescope/entry_points/recording.py
--rw-rw-rw-   0        0        0     3609 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/entry_points/runner.py
--rw-rw-rw-   0        0        0      865 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/entry_points/scan.py
--rw-rw-rw-   0        0        0     2883 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/entry_points/statistics.py
--rw-rw-rw-   0        0        0     2814 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/entry_points/stream_test.py
--rw-rw-rw-   0        0        0     3000 2020-05-30 15:27:09.000000 joulescope-1.1.4/joulescope/file_replace.py
--rw-rw-rw-   0        0        0     5532 2023-02-22 12:49:19.000000 joulescope-1.1.4/joulescope/jls_v2_writer.py
--rw-rw-rw-   0        0        0     3056 2022-09-09 13:37:25.000000 joulescope-1.1.4/joulescope/parameter.py
--rw-rw-rw-   0        0        0    11070 2022-11-07 22:01:01.000000 joulescope-1.1.4/joulescope/parameters_v1.py
--rw-rw-rw-   0        0        0     8797 2022-12-20 13:24:03.000000 joulescope-1.1.4/joulescope/span.py
--rw-rw-rw-   0        0        0      653 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/stream_buffer.py
-drwxrwxrwx   0        0        0        0 2023-04-28 18:57:57.561503 joulescope-1.1.4/joulescope/test/
--rw-rw-rw-   0        0        0        0 2020-05-30 15:27:09.000000 joulescope-1.1.4/joulescope/test/__init__.py
--rw-rw-rw-   0        0        0    16330 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/test/test_data_recorder.py
--rw-rw-rw-   0        0        0     5407 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/test/test_data_recorder_downsampled.py
--rw-rw-rw-   0        0        0     2484 2020-05-30 15:27:09.000000 joulescope-1.1.4/joulescope/test/test_file_replace.py
--rw-rw-rw-   0        0        0     4237 2022-11-21 18:21:24.000000 joulescope-1.1.4/joulescope/test/test_jls_v2_writer.py
--rw-rw-rw-   0        0        0     2902 2021-03-09 14:36:24.000000 joulescope-1.1.4/joulescope/test/test_span.py
--rw-rw-rw-   0        0        0     1179 2020-05-30 15:27:09.000000 joulescope-1.1.4/joulescope/test/test_time.py
--rw-rw-rw-   0        0        0     4631 2021-11-19 14:35:42.000000 joulescope-1.1.4/joulescope/test/test_units.py
--rw-rw-rw-   0        0        0    10876 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/test_datafile.py
--rw-rw-rw-   0        0        0     2189 2020-05-30 15:27:09.000000 joulescope-1.1.4/joulescope/time.py
--rw-rw-rw-   0        0        0     4736 2021-11-19 14:35:42.000000 joulescope-1.1.4/joulescope/units.py
-drwxrwxrwx   0        0        0        0 2023-04-28 18:57:57.565504 joulescope-1.1.4/joulescope/v0/
--rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/__init__.py
--rw-rw-rw-   0        0        0     6362 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/array_storage.py
--rw-rw-rw-   0        0        0    12568 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/bootloader.py
--rw-rw-rw-   0        0        0     9922 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/calibration.py
--rw-rw-rw-   0        0        0    85576 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/decimators.py
--rw-rw-rw-   0        0        0    58006 2023-03-20 19:36:21.000000 joulescope-1.1.4/joulescope/v0/driver.py
--rw-rw-rw-   0        0        0   957021 2023-04-26 20:01:19.000000 joulescope-1.1.4/joulescope/v0/filter_fir.c
--rw-rw-rw-   0        0        0     6132 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/firmware_manager.py
-drwxrwxrwx   0        0        0        0 2023-04-28 18:57:57.566003 joulescope-1.1.4/joulescope/v0/native/
--rw-rw-rw-   0        0        0     3763 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/native/filter_fir.c
--rw-rw-rw-   0        0        0     2904 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/native/filter_fir.h
--rw-rw-rw-   0        0        0     2647 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/native/running_statistics.c
--rw-rw-rw-   0        0        0     2891 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/native/running_statistics.h
-drwxrwxrwx   0        0        0        0 2023-04-28 18:57:57.567517 joulescope-1.1.4/joulescope/v0/native/test/
--rw-rw-rw-   0        0        0    57119 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/native/test/acutest.h
--rw-rw-rw-   0        0        0     2942 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/native/test/test_filter_fir.c
--rw-rw-rw-   0        0        0     1913 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/notification_handler.py
--rw-rw-rw-   0        0        0   433682 2023-04-26 20:01:19.000000 joulescope-1.1.4/joulescope/v0/pattern_buffer.c
--rw-rw-rw-   0        0        0     1245 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/public_keys.py
--rw-rw-rw-   0        0        0  2675267 2023-04-26 20:01:20.000000 joulescope-1.1.4/joulescope/v0/stream_buffer.c
-drwxrwxrwx   0        0        0        0 2023-04-28 18:57:57.571527 joulescope-1.1.4/joulescope/v0/test/
--rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/test/__init__.py
--rw-rw-rw-   0        0        0     2999 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/test/test_array_storage.py
--rw-rw-rw-   0        0        0     3717 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/test/test_calibration.py
--rw-rw-rw-   0        0        0     4551 2023-03-10 18:03:29.000000 joulescope-1.1.4/joulescope/v0/test/test_device.py
--rw-rw-rw-   0        0        0     2308 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/test/test_filter_fir.py
--rw-rw-rw-   0        0        0     1418 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/test/test_parameter.py
--rw-rw-rw-   0        0        0     3379 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/test/test_pattern_buffer.py
--rw-rw-rw-   0        0        0     3670 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/test/test_stats.py
--rw-rw-rw-   0        0        0    24677 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/test/test_stream_buffer.py
--rw-rw-rw-   0        0        0     1793 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/test/test_view.py
-drwxrwxrwx   0        0        0        0 2023-04-28 18:57:57.574030 joulescope-1.1.4/joulescope/v0/usb/
--rw-rw-rw-   0        0        0      758 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/usb/__init__.py
--rw-rw-rw-   0        0        0     8886 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/usb/api.py
--rw-rw-rw-   0        0        0     5114 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/usb/core.py
--rw-rw-rw-   0        0        0     8111 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/usb/device_thread.py
--rw-rw-rw-   0        0        0     4046 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/usb/hw_tests.py
--rw-rw-rw-   0        0        0     1542 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/usb/impl_tools.py
-drwxrwxrwx   0        0        0        0 2023-04-28 18:57:57.575034 joulescope-1.1.4/joulescope/v0/usb/libusb/
--rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/usb/libusb/__init__.py
--rw-rw-rw-   0        0        0    40907 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/usb/libusb/device.py
--rw-rw-rw-   0        0        0     2406 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/usb/scan_info.py
-drwxrwxrwx   0        0        0        0 2023-04-28 18:57:57.577037 joulescope-1.1.4/joulescope/v0/usb/winusb/
--rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/usb/winusb/__init__.py
--rw-rw-rw-   0        0        0    35453 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/usb/winusb/device.py
--rw-rw-rw-   0        0        0     8061 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/usb/winusb/kernel32.py
--rw-rw-rw-   0        0        0     6017 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/usb/winusb/setupapi.py
--rw-rw-rw-   0        0        0     5280 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v0/usb/winusb/win32_device_notify.py
-drwxrwxrwx   0        0        0        0 2023-04-28 18:57:57.580041 joulescope-1.1.4/joulescope/v1/
--rw-rw-rw-   0        0        0      690 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v1/__init__.py
--rw-rw-rw-   0        0        0    28152 2023-04-19 20:18:36.000000 joulescope-1.1.4/joulescope/v1/device.py
--rw-rw-rw-   0        0        0     7317 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v1/driver.py
--rw-rw-rw-   0        0        0     5627 2023-04-19 20:18:51.000000 joulescope-1.1.4/joulescope/v1/js110.py
--rw-rw-rw-   0        0        0     7534 2023-01-25 15:11:30.000000 joulescope-1.1.4/joulescope/v1/js220.py
--rw-rw-rw-   0        0        0     6630 2023-02-15 17:15:30.000000 joulescope-1.1.4/joulescope/v1/sample_buffer.py
--rw-rw-rw-   0        0        0   888760 2023-04-26 20:01:21.000000 joulescope-1.1.4/joulescope/v1/stats.c
--rw-rw-rw-   0        0        0    16328 2023-04-12 13:39:59.000000 joulescope-1.1.4/joulescope/v1/stream_buffer.py
-drwxrwxrwx   0        0        0        0 2023-04-28 18:57:57.580541 joulescope-1.1.4/joulescope/v1/test/
--rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.4/joulescope/v1/test/__init__.py
--rw-rw-rw-   0        0        0     3047 2022-11-10 15:29:05.000000 joulescope-1.1.4/joulescope/v1/test/test_sample_buffer.py
--rw-rw-rw-   0        0        0      470 2023-04-28 18:42:56.000000 joulescope-1.1.4/joulescope/version.py
--rw-rw-rw-   0        0        0    21187 2022-11-11 15:21:00.000000 joulescope-1.1.4/joulescope/view.py
-drwxrwxrwx   0        0        0        0 2023-04-28 18:57:57.548471 joulescope-1.1.4/joulescope.egg-info/
--rw-rw-rw-   0        0        0     3628 2023-04-28 18:57:57.000000 joulescope-1.1.4/joulescope.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3265 2023-04-28 18:57:57.000000 joulescope-1.1.4/joulescope.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 18:57:57.000000 joulescope-1.1.4/joulescope.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-04-28 18:57:57.000000 joulescope-1.1.4/joulescope.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      200 2023-04-28 18:57:57.000000 joulescope-1.1.4/joulescope.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-28 18:57:57.000000 joulescope-1.1.4/joulescope.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      851 2022-11-30 15:24:46.000000 joulescope-1.1.4/pyproject.toml
--rw-rw-rw-   0        0        0      117 2023-04-28 18:57:57.582045 joulescope-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     6882 2023-04-28 18:41:46.000000 joulescope-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.876642 joulescope-1.1.5/
+-rw-rw-rw-   0        0        0    21821 2023-05-24 14:34:53.000000 joulescope-1.1.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0     6771 2020-08-11 21:29:57.000000 joulescope-1.1.5/CREDITS.html
+-rw-rw-rw-   0        0        0    11558 2020-05-30 15:27:09.000000 joulescope-1.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      132 2022-11-07 18:35:15.000000 joulescope-1.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3628 2023-05-24 19:33:40.876642 joulescope-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1762 2020-11-25 13:12:14.000000 joulescope-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.816069 joulescope-1.1.5/joulescope/
+-rw-rw-rw-   0        0        0     2291 2023-03-20 19:38:30.000000 joulescope-1.1.5/joulescope/__init__.py
+-rw-rw-rw-   0        0        0      730 2020-05-30 15:27:09.000000 joulescope-1.1.5/joulescope/__main__.py
+-rw-rw-rw-   0        0        0    54968 2023-03-11 15:21:25.000000 joulescope-1.1.5/joulescope/data_recorder.py
+-rw-rw-rw-   0        0        0    26397 2022-09-09 13:37:25.000000 joulescope-1.1.5/joulescope/datafile.py
+drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.852582 joulescope-1.1.5/joulescope/entry_points/
+-rw-rw-rw-   0        0        0        0 2020-05-30 15:27:09.000000 joulescope-1.1.5/joulescope/entry_points/__init__.py
+-rw-rw-rw-   0        0        0     1325 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/entry_points/bootloader_go.py
+-rw-rw-rw-   0        0        0     4040 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/entry_points/capture.py
+-rw-rw-rw-   0        0        0     1530 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/entry_points/gpo_demo.py
+-rw-rw-rw-   0        0        0     2103 2023-04-19 20:18:48.000000 joulescope-1.1.5/joulescope/entry_points/info.py
+-rw-rw-rw-   0        0        0     2110 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/entry_points/parameter_set.py
+-rw-rw-rw-   0        0        0     5043 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/entry_points/program.py
+-rw-rw-rw-   0        0        0     6546 2022-09-10 13:15:16.000000 joulescope-1.1.5/joulescope/entry_points/recording.py
+-rw-rw-rw-   0        0        0     3609 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/entry_points/runner.py
+-rw-rw-rw-   0        0        0      865 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/entry_points/scan.py
+-rw-rw-rw-   0        0        0     2883 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/entry_points/statistics.py
+-rw-rw-rw-   0        0        0     2814 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/entry_points/stream_test.py
+-rw-rw-rw-   0        0        0     3000 2020-05-30 15:27:09.000000 joulescope-1.1.5/joulescope/file_replace.py
+-rw-rw-rw-   0        0        0     5532 2023-02-22 12:49:19.000000 joulescope-1.1.5/joulescope/jls_v2_writer.py
+-rw-rw-rw-   0        0        0     3056 2022-09-09 13:37:25.000000 joulescope-1.1.5/joulescope/parameter.py
+-rw-rw-rw-   0        0        0    11070 2022-11-07 22:01:01.000000 joulescope-1.1.5/joulescope/parameters_v1.py
+-rw-rw-rw-   0        0        0     8797 2022-12-20 13:24:03.000000 joulescope-1.1.5/joulescope/span.py
+-rw-rw-rw-   0        0        0      653 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/stream_buffer.py
+drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.856091 joulescope-1.1.5/joulescope/test/
+-rw-rw-rw-   0        0        0        0 2020-05-30 15:27:09.000000 joulescope-1.1.5/joulescope/test/__init__.py
+-rw-rw-rw-   0        0        0    16330 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/test/test_data_recorder.py
+-rw-rw-rw-   0        0        0     5407 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/test/test_data_recorder_downsampled.py
+-rw-rw-rw-   0        0        0     2484 2020-05-30 15:27:09.000000 joulescope-1.1.5/joulescope/test/test_file_replace.py
+-rw-rw-rw-   0        0        0     4237 2022-11-21 18:21:24.000000 joulescope-1.1.5/joulescope/test/test_jls_v2_writer.py
+-rw-rw-rw-   0        0        0     2902 2021-03-09 14:36:24.000000 joulescope-1.1.5/joulescope/test/test_span.py
+-rw-rw-rw-   0        0        0     1179 2020-05-30 15:27:09.000000 joulescope-1.1.5/joulescope/test/test_time.py
+-rw-rw-rw-   0        0        0     4631 2021-11-19 14:35:42.000000 joulescope-1.1.5/joulescope/test/test_units.py
+-rw-rw-rw-   0        0        0    10876 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/test_datafile.py
+-rw-rw-rw-   0        0        0     2189 2020-05-30 15:27:09.000000 joulescope-1.1.5/joulescope/time.py
+-rw-rw-rw-   0        0        0     4736 2021-11-19 14:35:42.000000 joulescope-1.1.5/joulescope/units.py
+drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.859599 joulescope-1.1.5/joulescope/v0/
+-rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/__init__.py
+-rw-rw-rw-   0        0        0     6362 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/array_storage.py
+-rw-rw-rw-   0        0        0    12568 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/bootloader.py
+-rw-rw-rw-   0        0        0     9922 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/calibration.py
+-rw-rw-rw-   0        0        0    85576 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/decimators.py
+-rw-rw-rw-   0        0        0    58006 2023-03-20 19:36:21.000000 joulescope-1.1.5/joulescope/v0/driver.py
+-rw-rw-rw-   0        0        0   957021 2023-04-26 20:01:19.000000 joulescope-1.1.5/joulescope/v0/filter_fir.c
+-rw-rw-rw-   0        0        0     6132 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/firmware_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.860599 joulescope-1.1.5/joulescope/v0/native/
+-rw-rw-rw-   0        0        0     3763 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/native/filter_fir.c
+-rw-rw-rw-   0        0        0     2904 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/native/filter_fir.h
+-rw-rw-rw-   0        0        0     2647 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/native/running_statistics.c
+-rw-rw-rw-   0        0        0     2891 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/native/running_statistics.h
+drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.862103 joulescope-1.1.5/joulescope/v0/native/test/
+-rw-rw-rw-   0        0        0    57119 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/native/test/acutest.h
+-rw-rw-rw-   0        0        0     2942 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/native/test/test_filter_fir.c
+-rw-rw-rw-   0        0        0     1913 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/notification_handler.py
+-rw-rw-rw-   0        0        0   433682 2023-04-26 20:01:19.000000 joulescope-1.1.5/joulescope/v0/pattern_buffer.c
+-rw-rw-rw-   0        0        0     1245 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/public_keys.py
+-rw-rw-rw-   0        0        0  2675267 2023-04-26 20:01:20.000000 joulescope-1.1.5/joulescope/v0/stream_buffer.c
+drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.866613 joulescope-1.1.5/joulescope/v0/test/
+-rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/test/__init__.py
+-rw-rw-rw-   0        0        0     2999 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/test/test_array_storage.py
+-rw-rw-rw-   0        0        0     3717 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/test/test_calibration.py
+-rw-rw-rw-   0        0        0     4551 2023-03-10 18:03:29.000000 joulescope-1.1.5/joulescope/v0/test/test_device.py
+-rw-rw-rw-   0        0        0     2308 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/test/test_filter_fir.py
+-rw-rw-rw-   0        0        0     1418 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/test/test_parameter.py
+-rw-rw-rw-   0        0        0     3379 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/test/test_pattern_buffer.py
+-rw-rw-rw-   0        0        0     3670 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/test/test_stats.py
+-rw-rw-rw-   0        0        0    24677 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/test/test_stream_buffer.py
+-rw-rw-rw-   0        0        0     1793 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/test/test_view.py
+drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.869116 joulescope-1.1.5/joulescope/v0/usb/
+-rw-rw-rw-   0        0        0      758 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/__init__.py
+-rw-rw-rw-   0        0        0     8886 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/api.py
+-rw-rw-rw-   0        0        0     5114 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/core.py
+-rw-rw-rw-   0        0        0     8111 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/device_thread.py
+-rw-rw-rw-   0        0        0     4046 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/hw_tests.py
+-rw-rw-rw-   0        0        0     1542 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/impl_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.870122 joulescope-1.1.5/joulescope/v0/usb/libusb/
+-rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/libusb/__init__.py
+-rw-rw-rw-   0        0        0    40907 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/libusb/device.py
+-rw-rw-rw-   0        0        0     2406 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/scan_info.py
+drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.872626 joulescope-1.1.5/joulescope/v0/usb/winusb/
+-rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/winusb/__init__.py
+-rw-rw-rw-   0        0        0    35453 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/winusb/device.py
+-rw-rw-rw-   0        0        0     8061 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/winusb/kernel32.py
+-rw-rw-rw-   0        0        0     6017 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/winusb/setupapi.py
+-rw-rw-rw-   0        0        0     5280 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/winusb/win32_device_notify.py
+drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.875643 joulescope-1.1.5/joulescope/v1/
+-rw-rw-rw-   0        0        0      690 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v1/__init__.py
+-rw-rw-rw-   0        0        0    28495 2023-05-24 15:39:07.000000 joulescope-1.1.5/joulescope/v1/device.py
+-rw-rw-rw-   0        0        0     7317 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v1/driver.py
+-rw-rw-rw-   0        0        0     5627 2023-04-19 20:18:51.000000 joulescope-1.1.5/joulescope/v1/js110.py
+-rw-rw-rw-   0        0        0     7534 2023-01-25 15:11:30.000000 joulescope-1.1.5/joulescope/v1/js220.py
+-rw-rw-rw-   0        0        0     6630 2023-02-15 17:15:30.000000 joulescope-1.1.5/joulescope/v1/sample_buffer.py
+-rw-rw-rw-   0        0        0   888760 2023-04-26 20:01:21.000000 joulescope-1.1.5/joulescope/v1/stats.c
+-rw-rw-rw-   0        0        0    16328 2023-04-12 13:39:59.000000 joulescope-1.1.5/joulescope/v1/stream_buffer.py
+drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.876642 joulescope-1.1.5/joulescope/v1/test/
+-rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v1/test/__init__.py
+-rw-rw-rw-   0        0        0     3047 2022-11-10 15:29:05.000000 joulescope-1.1.5/joulescope/v1/test/test_sample_buffer.py
+-rw-rw-rw-   0        0        0      470 2023-05-24 14:34:59.000000 joulescope-1.1.5/joulescope/version.py
+-rw-rw-rw-   0        0        0    21187 2022-11-11 15:21:00.000000 joulescope-1.1.5/joulescope/view.py
+drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.829095 joulescope-1.1.5/joulescope.egg-info/
+-rw-rw-rw-   0        0        0     3628 2023-05-24 19:33:40.000000 joulescope-1.1.5/joulescope.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3265 2023-05-24 19:33:40.000000 joulescope-1.1.5/joulescope.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 19:33:40.000000 joulescope-1.1.5/joulescope.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-05-24 19:33:40.000000 joulescope-1.1.5/joulescope.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      201 2023-05-24 19:33:40.000000 joulescope-1.1.5/joulescope.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-24 19:33:40.000000 joulescope-1.1.5/joulescope.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      851 2022-11-30 15:24:46.000000 joulescope-1.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0      117 2023-05-24 19:33:40.884675 joulescope-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     6883 2023-05-24 14:34:05.000000 joulescope-1.1.5/setup.py
```

### Comparing `joulescope-1.1.4/CHANGELOG.md` & `joulescope-1.1.5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to pyjoulescope.
 
 
+## 1.1.5
+
+2023 May 24
+
+* Added JS110 on-instrument (sensor) statistics option to v1 backend.
+
+
 ## 1.1.4
 
 2023 Apr 28
 
 * Bumped revisions for pyjls and pyjoulescope_driver to latest.
   Many improvements and fixes.  See projects for details.
```

### Comparing `joulescope-1.1.4/CREDITS.html` & `joulescope-1.1.5/CREDITS.html`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/LICENSE.txt` & `joulescope-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/PKG-INFO` & `joulescope-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope
-Version: 1.1.4
+Version: 1.1.5
 Summary: Joulescope™ host driver and utilities
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `joulescope-1.1.4/README.md` & `joulescope-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/__init__.py` & `joulescope-1.1.5/joulescope/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/__main__.py` & `joulescope-1.1.5/joulescope/__main__.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/data_recorder.py` & `joulescope-1.1.5/joulescope/data_recorder.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/datafile.py` & `joulescope-1.1.5/joulescope/datafile.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/entry_points/bootloader_go.py` & `joulescope-1.1.5/joulescope/entry_points/bootloader_go.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/entry_points/capture.py` & `joulescope-1.1.5/joulescope/entry_points/capture.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/entry_points/gpo_demo.py` & `joulescope-1.1.5/joulescope/entry_points/gpo_demo.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/entry_points/info.py` & `joulescope-1.1.5/joulescope/entry_points/info.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/entry_points/parameter_set.py` & `joulescope-1.1.5/joulescope/entry_points/parameter_set.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/entry_points/program.py` & `joulescope-1.1.5/joulescope/entry_points/program.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/entry_points/recording.py` & `joulescope-1.1.5/joulescope/entry_points/recording.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/entry_points/runner.py` & `joulescope-1.1.5/joulescope/entry_points/runner.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/entry_points/scan.py` & `joulescope-1.1.5/joulescope/entry_points/scan.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/entry_points/statistics.py` & `joulescope-1.1.5/joulescope/entry_points/statistics.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/entry_points/stream_test.py` & `joulescope-1.1.5/joulescope/entry_points/stream_test.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/file_replace.py` & `joulescope-1.1.5/joulescope/file_replace.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/jls_v2_writer.py` & `joulescope-1.1.5/joulescope/jls_v2_writer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/parameter.py` & `joulescope-1.1.5/joulescope/parameter.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/parameters_v1.py` & `joulescope-1.1.5/joulescope/parameters_v1.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/span.py` & `joulescope-1.1.5/joulescope/span.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/stream_buffer.py` & `joulescope-1.1.5/joulescope/stream_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/test/test_data_recorder.py` & `joulescope-1.1.5/joulescope/test/test_data_recorder.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/test/test_data_recorder_downsampled.py` & `joulescope-1.1.5/joulescope/test/test_data_recorder_downsampled.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/test/test_file_replace.py` & `joulescope-1.1.5/joulescope/test/test_file_replace.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/test/test_jls_v2_writer.py` & `joulescope-1.1.5/joulescope/test/test_jls_v2_writer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/test/test_span.py` & `joulescope-1.1.5/joulescope/test/test_span.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/test/test_time.py` & `joulescope-1.1.5/joulescope/test/test_time.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/test/test_units.py` & `joulescope-1.1.5/joulescope/test/test_units.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/test_datafile.py` & `joulescope-1.1.5/joulescope/test_datafile.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/time.py` & `joulescope-1.1.5/joulescope/time.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/units.py` & `joulescope-1.1.5/joulescope/units.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/array_storage.py` & `joulescope-1.1.5/joulescope/v0/array_storage.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/bootloader.py` & `joulescope-1.1.5/joulescope/v0/bootloader.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/calibration.py` & `joulescope-1.1.5/joulescope/v0/calibration.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/decimators.py` & `joulescope-1.1.5/joulescope/v0/decimators.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/driver.py` & `joulescope-1.1.5/joulescope/v0/driver.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/filter_fir.c` & `joulescope-1.1.5/joulescope/v0/filter_fir.c`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/firmware_manager.py` & `joulescope-1.1.5/joulescope/v0/firmware_manager.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/native/filter_fir.c` & `joulescope-1.1.5/joulescope/v0/native/filter_fir.c`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/native/filter_fir.h` & `joulescope-1.1.5/joulescope/v0/native/filter_fir.h`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/native/running_statistics.c` & `joulescope-1.1.5/joulescope/v0/native/running_statistics.c`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/native/running_statistics.h` & `joulescope-1.1.5/joulescope/v0/native/running_statistics.h`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/native/test/acutest.h` & `joulescope-1.1.5/joulescope/v0/native/test/acutest.h`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/native/test/test_filter_fir.c` & `joulescope-1.1.5/joulescope/v0/native/test/test_filter_fir.c`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/notification_handler.py` & `joulescope-1.1.5/joulescope/v0/notification_handler.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/pattern_buffer.c` & `joulescope-1.1.5/joulescope/v0/pattern_buffer.c`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/public_keys.py` & `joulescope-1.1.5/joulescope/v0/public_keys.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/stream_buffer.c` & `joulescope-1.1.5/joulescope/v0/stream_buffer.c`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/test/test_array_storage.py` & `joulescope-1.1.5/joulescope/v0/test/test_array_storage.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/test/test_calibration.py` & `joulescope-1.1.5/joulescope/v0/test/test_calibration.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/test/test_device.py` & `joulescope-1.1.5/joulescope/v0/test/test_device.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/test/test_filter_fir.py` & `joulescope-1.1.5/joulescope/v0/test/test_filter_fir.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/test/test_parameter.py` & `joulescope-1.1.5/joulescope/v0/test/test_parameter.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/test/test_pattern_buffer.py` & `joulescope-1.1.5/joulescope/v0/test/test_pattern_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/test/test_stats.py` & `joulescope-1.1.5/joulescope/v0/test/test_stats.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/test/test_stream_buffer.py` & `joulescope-1.1.5/joulescope/v0/test/test_stream_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/test/test_view.py` & `joulescope-1.1.5/joulescope/v0/test/test_view.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/usb/__init__.py` & `joulescope-1.1.5/joulescope/v0/usb/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/usb/api.py` & `joulescope-1.1.5/joulescope/v0/usb/api.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/usb/core.py` & `joulescope-1.1.5/joulescope/v0/usb/core.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/usb/device_thread.py` & `joulescope-1.1.5/joulescope/v0/usb/device_thread.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/usb/hw_tests.py` & `joulescope-1.1.5/joulescope/v0/usb/hw_tests.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/usb/impl_tools.py` & `joulescope-1.1.5/joulescope/v0/usb/impl_tools.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/usb/libusb/device.py` & `joulescope-1.1.5/joulescope/v0/usb/libusb/device.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/usb/scan_info.py` & `joulescope-1.1.5/joulescope/v0/usb/scan_info.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/usb/winusb/device.py` & `joulescope-1.1.5/joulescope/v0/usb/winusb/device.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/usb/winusb/kernel32.py` & `joulescope-1.1.5/joulescope/v0/usb/winusb/kernel32.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/usb/winusb/setupapi.py` & `joulescope-1.1.5/joulescope/v0/usb/winusb/setupapi.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v0/usb/winusb/win32_device_notify.py` & `joulescope-1.1.5/joulescope/v0/usb/winusb/win32_device_notify.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v1/__init__.py` & `joulescope-1.1.5/joulescope/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v1/device.py` & `joulescope-1.1.5/joulescope/v1/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,21 +180,27 @@
             if 'integral' in k:
                 k['∫'] = k['integral']
         for cbk in self._statistics_callbacks:
             cbk(value)
 
     def _statistics_start(self):
         if self.is_open:
-            self.publish('s/stats/ctrl', 1)
-            self.subscribe('s/stats/value', 'pub', self._on_stats_cbk)
+            if 'js110' in self.device_path and self.config == 'off':
+                self.subscribe('s/sstats/value', 'pub', self._on_stats_cbk)
+            else:
+                self.publish('s/stats/ctrl', 1)
+                self.subscribe('s/stats/value', 'pub', self._on_stats_cbk)
 
     def _statistics_stop(self):
         if self.is_open:
-            self.unsubscribe('s/stats/value', self._on_stats_cbk)
-            self.publish('s/stats/ctrl', 0)
+            if 'js110' in self.device_path and self.config == 'off':
+                self.unsubscribe('s/sstats/value', self._on_stats_cbk)
+            else:
+                self.unsubscribe('s/stats/value', self._on_stats_cbk)
+                self.publish('s/stats/ctrl', 0)
 
     def statistics_accumulators_clear(self):
         """Clear the charge and energy accumulators."""
         self._statistics_offsets.clear()
 
     def view_factory(self):
         """Construct a new View into the device's data.
```

### Comparing `joulescope-1.1.4/joulescope/v1/driver.py` & `joulescope-1.1.5/joulescope/v1/driver.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v1/js110.py` & `joulescope-1.1.5/joulescope/v1/js110.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v1/js220.py` & `joulescope-1.1.5/joulescope/v1/js220.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v1/sample_buffer.py` & `joulescope-1.1.5/joulescope/v1/sample_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v1/stats.c` & `joulescope-1.1.5/joulescope/v1/stats.c`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v1/stream_buffer.py` & `joulescope-1.1.5/joulescope/v1/stream_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/v1/test/test_sample_buffer.py` & `joulescope-1.1.5/joulescope/v1/test/test_sample_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope/view.py` & `joulescope-1.1.5/joulescope/view.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/joulescope.egg-info/PKG-INFO` & `joulescope-1.1.5/joulescope.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope
-Version: 1.1.4
+Version: 1.1.5
 Summary: Joulescope™ host driver and utilities
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `joulescope-1.1.4/joulescope.egg-info/SOURCES.txt` & `joulescope-1.1.5/joulescope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/pyproject.toml` & `joulescope-1.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.4/setup.py` & `joulescope-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 
     # See https://packaging.python.org/en/latest/requirements.html
     # https://numpy.org/neps/nep-0029-deprecation_policy.html
     install_requires=[
         'numpy',
         'psutil',
         'pyjls>=0.6.2',
-        'pyjoulescope_driver>=1.3.7',
+        'pyjoulescope_driver>=1.3.11',
         'python-dateutil>=2.7.3',
         'pymonocypher>=3.1.3',
         "pywin32; platform_system=='Windows'",
     ],
 
     extras_require={
         'dev': ['check-manifest', 'coverage', 'Cython', 'wheel', 'sphinx', 'myst-parser'],
```

