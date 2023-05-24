# Comparing `tmp/py_ios_device-2.3.32.1.tar.gz` & `tmp/py_ios_device-2.3.32.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ios_device-2.3.32.1.tar", last modified: Wed Apr 26 06:22:31 2023, max compression
+gzip compressed data, was "py_ios_device-2.3.32.2.tar", last modified: Wed May 24 02:44:55 2023, max compression
```

## Comparing `py_ios_device-2.3.32.1.tar` & `py_ios_device-2.3.32.2.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-26 06:22:31.779176 py_ios_device-2.3.32.1/
--rw-r--r--   0 rongcloud   (501) staff       (20)    35147 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/LICENSE
--rw-r--r--   0 rongcloud   (501) staff       (20)       24 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/MANIFEST.in
--rw-r--r--   0 rongcloud   (501) staff       (20)    11011 2023-04-26 06:22:31.778979 py_ios_device-2.3.32.1/PKG-INFO
--rw-r--r--   0 rongcloud   (501) staff       (20)    10544 2023-04-20 03:06:40.000000 py_ios_device-2.3.32.1/README.md
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-26 06:22:31.760948 py_ios_device-2.3.32.1/demo/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/demo/__init__.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    18971 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/demo/afc.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1141 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/demo/crash_log.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     6471 2023-03-07 02:35:28.000000 py_ios_device-2.3.32.1/demo/installation_proxy.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-26 06:22:31.764445 py_ios_device-2.3.32.1/demo/instrument_demo/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/demo/instrument_demo/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      866 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/demo/instrument_demo/activity.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3290 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.1/demo/instrument_demo/app_lifecycle.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      536 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/demo/instrument_demo/applictionListing.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      362 2023-04-07 02:35:34.000000 py_ios_device-2.3.32.1/demo/instrument_demo/channel.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4146 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.1/demo/instrument_demo/coreprofilesessiontap.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1535 2023-02-21 09:11:42.000000 py_ios_device-2.3.32.1/demo/instrument_demo/coreprofilesessiontap_parse.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2174 2023-02-09 09:46:25.000000 py_ios_device-2.3.32.1/demo/instrument_demo/deviceinfo.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      494 2023-04-07 02:35:34.000000 py_ios_device-2.3.32.1/demo/instrument_demo/energy.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2199 2023-03-17 08:58:28.000000 py_ios_device-2.3.32.1/demo/instrument_demo/gpu.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1085 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/demo/instrument_demo/graphics.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      748 2023-03-17 08:58:33.000000 py_ios_device-2.3.32.1/demo/instrument_demo/launchAPP.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      851 2023-02-16 02:26:32.000000 py_ios_device-2.3.32.1/demo/instrument_demo/mobileNotifications.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      533 2023-02-09 09:46:25.000000 py_ios_device-2.3.32.1/demo/instrument_demo/netstatPID.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2835 2023-02-09 09:46:25.000000 py_ios_device-2.3.32.1/demo/instrument_demo/networking.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2554 2023-04-20 02:17:26.000000 py_ios_device-2.3.32.1/demo/instrument_demo/sysmontap.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     8873 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/demo/instrument_demo/xcuitest.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3608 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/demo/mobile_config.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     5368 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/demo/pcapd.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3089 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/demo/screenshotr.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4297 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/demo/syslog.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-26 06:22:31.765039 py_ios_device-2.3.32.1/ios_device/
--rw-r--r--   0 rongcloud   (501) staff       (20)       37 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/ios_device/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)       25 2023-04-26 06:17:20.000000 py_ios_device-2.3.32.1/ios_device/__version__.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-26 06:22:31.767284 py_ios_device-2.3.32.1/ios_device/cli/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/ios_device/cli/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    29436 2023-04-20 02:52:36.000000 py_ios_device-2.3.32.1/ios_device/cli/base.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      988 2023-04-07 02:33:45.000000 py_ios_device-2.3.32.1/ios_device/cli/cli.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    19123 2023-04-20 03:02:09.000000 py_ios_device-2.3.32.1/ios_device/cli/instruments.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    11223 2023-04-26 06:21:46.000000 py_ios_device-2.3.32.1/ios_device/cli/mobile.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      293 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/ios_device/main.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    23312 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.1/ios_device/py_ios_device.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-26 06:22:31.773422 py_ios_device-2.3.32.1/ios_device/servers/
--rw-r--r--   0 rongcloud   (501) staff       (20)     7287 2023-04-26 03:35:04.000000 py_ios_device-2.3.32.1/ios_device/servers/Installation.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1029 2023-04-20 02:15:07.000000 py_ios_device-2.3.32.1/ios_device/servers/Instrument.py
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/ios_device/servers/__init__.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    19387 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/servers/afc.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1238 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/servers/amfi.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1155 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/servers/crash_log.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      993 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/servers/diagnostics_relay.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7844 2023-04-20 02:15:07.000000 py_ios_device-2.3.32.1/ios_device/servers/dvt.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1223 2023-03-07 02:32:12.000000 py_ios_device-2.3.32.1/ios_device/servers/house_arrest.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3536 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/servers/image_mounter.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     1679 2023-03-17 09:31:16.000000 py_ios_device-2.3.32.1/ios_device/servers/mc_install.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    31263 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/servers/notification_proxy.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2834 2023-04-20 02:31:19.000000 py_ios_device-2.3.32.1/ios_device/servers/os_trace.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3163 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/servers/pcapd.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3102 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/servers/screenshotr.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1083 2023-01-04 04:20:57.000000 py_ios_device-2.3.32.1/ios_device/servers/simulate_location.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1596 2023-03-31 08:20:40.000000 py_ios_device-2.3.32.1/ios_device/servers/spring_board.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3329 2023-01-04 03:41:43.000000 py_ios_device-2.3.32.1/ios_device/servers/syslog.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      864 2023-04-17 09:44:17.000000 py_ios_device-2.3.32.1/ios_device/servers/testmanagerd.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-26 06:22:31.778045 py_ios_device-2.3.32.1/ios_device/util/
--rw-r--r--   0 rongcloud   (501) staff       (20)     1860 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/ios_device/util/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    11825 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/util/api_util.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    24888 2022-12-08 06:30:13.000000 py_ios_device-2.3.32.1/ios_device/util/bpylist2.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4657 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/ios_device/util/ca.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4585 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/ios_device/util/constants.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7921 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/util/dtx_msg.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1842 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/ios_device/util/exceptions.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3907 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.1/ios_device/util/forward.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7443 2023-01-04 06:39:27.000000 py_ios_device-2.3.32.1/ios_device/util/gpu_decode.py
--rw-r--r--   0 rongcloud   (501) staff       (20)   109555 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.1/ios_device/util/kc_data.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    41845 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.1/ios_device/util/kperf_data.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    16216 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.1/ios_device/util/lifecycle.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    16285 2023-04-20 02:30:51.000000 py_ios_device-2.3.32.1/ios_device/util/lockdown.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3131 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.1/ios_device/util/plist_service.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    27335 2023-04-26 02:45:02.000000 py_ios_device-2.3.32.1/ios_device/util/plistlib.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    12592 2023-03-31 09:19:13.000000 py_ios_device-2.3.32.1/ios_device/util/usbmux.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     9513 2023-02-09 09:51:53.000000 py_ios_device-2.3.32.1/ios_device/util/utils.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4261 2023-02-14 02:46:09.000000 py_ios_device-2.3.32.1/ios_device/util/variables.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-04-26 06:22:31.778792 py_ios_device-2.3.32.1/py_ios_device.egg-info/
--rw-r--r--   0 rongcloud   (501) staff       (20)    11011 2023-04-26 06:22:31.000000 py_ios_device-2.3.32.1/py_ios_device.egg-info/PKG-INFO
--rw-r--r--   0 rongcloud   (501) staff       (20)     2406 2023-04-26 06:22:31.000000 py_ios_device-2.3.32.1/py_ios_device.egg-info/SOURCES.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)        1 2023-04-26 06:22:31.000000 py_ios_device-2.3.32.1/py_ios_device.egg-info/dependency_links.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       51 2023-04-26 06:22:31.000000 py_ios_device-2.3.32.1/py_ios_device.egg-info/entry_points.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)      141 2023-04-26 06:22:31.000000 py_ios_device-2.3.32.1/py_ios_device.egg-info/requires.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       16 2023-04-26 06:22:31.000000 py_ios_device-2.3.32.1/py_ios_device.egg-info/top_level.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)      140 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.1/requirements.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       38 2023-04-26 06:22:31.779216 py_ios_device-2.3.32.1/setup.cfg
--rw-r--r--   0 rongcloud   (501) staff       (20)      976 2023-04-07 02:35:34.000000 py_ios_device-2.3.32.1/setup.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      959 2023-04-20 03:34:06.000000 py_ios_device-2.3.32.1/setup2.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:44:55.186875 py_ios_device-2.3.32.2/
+-rw-r--r--   0 rongcloud   (501) staff       (20)    35147 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/LICENSE
+-rw-r--r--   0 rongcloud   (501) staff       (20)       24 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/MANIFEST.in
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11417 2023-05-24 02:44:55.186472 py_ios_device-2.3.32.2/PKG-INFO
+-rw-r--r--   0 rongcloud   (501) staff       (20)    10950 2023-05-24 02:33:49.000000 py_ios_device-2.3.32.2/README.md
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:44:55.168183 py_ios_device-2.3.32.2/demo/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/demo/__init__.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    18971 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/demo/afc.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1141 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/demo/crash_log.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     6471 2023-03-07 02:35:28.000000 py_ios_device-2.3.32.2/demo/installation_proxy.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:44:55.172827 py_ios_device-2.3.32.2/demo/instrument_demo/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/demo/instrument_demo/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      866 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/demo/instrument_demo/activity.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3290 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.2/demo/instrument_demo/app_lifecycle.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      536 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/demo/instrument_demo/applictionListing.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      362 2023-04-07 02:35:34.000000 py_ios_device-2.3.32.2/demo/instrument_demo/channel.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4146 2023-05-22 07:56:02.000000 py_ios_device-2.3.32.2/demo/instrument_demo/coreprofilesessiontap.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1535 2023-05-22 07:56:02.000000 py_ios_device-2.3.32.2/demo/instrument_demo/coreprofilesessiontap_parse.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2174 2023-02-09 09:46:25.000000 py_ios_device-2.3.32.2/demo/instrument_demo/deviceinfo.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      494 2023-05-22 07:56:02.000000 py_ios_device-2.3.32.2/demo/instrument_demo/energy.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2199 2023-05-08 09:42:27.000000 py_ios_device-2.3.32.2/demo/instrument_demo/gpu.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1085 2023-05-22 07:56:02.000000 py_ios_device-2.3.32.2/demo/instrument_demo/graphics.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      748 2023-05-22 07:56:02.000000 py_ios_device-2.3.32.2/demo/instrument_demo/launchAPP.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      851 2023-02-16 02:26:32.000000 py_ios_device-2.3.32.2/demo/instrument_demo/mobileNotifications.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      533 2023-02-09 09:46:25.000000 py_ios_device-2.3.32.2/demo/instrument_demo/netstatPID.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2835 2023-02-09 09:46:25.000000 py_ios_device-2.3.32.2/demo/instrument_demo/networking.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2554 2023-04-20 02:17:26.000000 py_ios_device-2.3.32.2/demo/instrument_demo/sysmontap.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     8873 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/demo/instrument_demo/xcuitest.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3608 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/demo/mobile_config.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     5368 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/demo/pcapd.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3089 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/demo/screenshotr.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4297 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/demo/syslog.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:44:55.173453 py_ios_device-2.3.32.2/ios_device/
+-rw-r--r--   0 rongcloud   (501) staff       (20)       37 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/ios_device/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)       25 2023-05-24 02:44:54.000000 py_ios_device-2.3.32.2/ios_device/__version__.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:44:55.175100 py_ios_device-2.3.32.2/ios_device/cli/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/ios_device/cli/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    31554 2023-05-24 02:44:13.000000 py_ios_device-2.3.32.2/ios_device/cli/base.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      988 2023-04-07 02:33:45.000000 py_ios_device-2.3.32.2/ios_device/cli/cli.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    19122 2023-05-24 02:30:31.000000 py_ios_device-2.3.32.2/ios_device/cli/instruments.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11223 2023-04-26 06:21:46.000000 py_ios_device-2.3.32.2/ios_device/cli/mobile.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      293 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/ios_device/main.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    23312 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.2/ios_device/py_ios_device.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:44:55.180186 py_ios_device-2.3.32.2/ios_device/servers/
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7287 2023-04-26 03:35:04.000000 py_ios_device-2.3.32.2/ios_device/servers/Installation.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1029 2023-04-20 02:15:07.000000 py_ios_device-2.3.32.2/ios_device/servers/Instrument.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/ios_device/servers/__init__.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    19387 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/ios_device/servers/afc.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1238 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/ios_device/servers/amfi.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1155 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/ios_device/servers/crash_log.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      993 2023-05-22 06:59:19.000000 py_ios_device-2.3.32.2/ios_device/servers/diagnostics_relay.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7844 2023-04-20 02:15:07.000000 py_ios_device-2.3.32.2/ios_device/servers/dvt.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1223 2023-03-07 02:32:12.000000 py_ios_device-2.3.32.2/ios_device/servers/house_arrest.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3536 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/ios_device/servers/image_mounter.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     1679 2023-03-17 09:31:16.000000 py_ios_device-2.3.32.2/ios_device/servers/mc_install.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    31263 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/ios_device/servers/notification_proxy.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2834 2023-04-20 02:31:19.000000 py_ios_device-2.3.32.2/ios_device/servers/os_trace.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3163 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/ios_device/servers/pcapd.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3102 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/ios_device/servers/screenshotr.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1083 2023-01-04 04:20:57.000000 py_ios_device-2.3.32.2/ios_device/servers/simulate_location.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1596 2023-03-31 08:20:40.000000 py_ios_device-2.3.32.2/ios_device/servers/spring_board.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3329 2023-01-04 03:41:43.000000 py_ios_device-2.3.32.2/ios_device/servers/syslog.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      864 2023-04-17 09:44:17.000000 py_ios_device-2.3.32.2/ios_device/servers/testmanagerd.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:44:55.185495 py_ios_device-2.3.32.2/ios_device/util/
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1860 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/ios_device/util/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11825 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/ios_device/util/api_util.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    24888 2022-12-08 06:30:13.000000 py_ios_device-2.3.32.2/ios_device/util/bpylist2.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4657 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/ios_device/util/ca.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4585 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/ios_device/util/constants.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7921 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/ios_device/util/dtx_msg.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1842 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/ios_device/util/exceptions.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3907 2022-09-26 09:47:22.000000 py_ios_device-2.3.32.2/ios_device/util/forward.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7443 2023-01-04 06:39:27.000000 py_ios_device-2.3.32.2/ios_device/util/gpu_decode.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)   109555 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.2/ios_device/util/kc_data.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    41845 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.2/ios_device/util/kperf_data.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    16216 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.2/ios_device/util/lifecycle.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    16285 2023-04-20 02:30:51.000000 py_ios_device-2.3.32.2/ios_device/util/lockdown.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3131 2022-12-08 06:20:36.000000 py_ios_device-2.3.32.2/ios_device/util/plist_service.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    27335 2023-04-26 02:45:02.000000 py_ios_device-2.3.32.2/ios_device/util/plistlib.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    12592 2023-03-31 09:19:13.000000 py_ios_device-2.3.32.2/ios_device/util/usbmux.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     9513 2023-02-09 09:51:53.000000 py_ios_device-2.3.32.2/ios_device/util/utils.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4261 2023-02-14 02:46:09.000000 py_ios_device-2.3.32.2/ios_device/util/variables.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:44:55.186294 py_ios_device-2.3.32.2/py_ios_device.egg-info/
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11417 2023-05-24 02:44:55.000000 py_ios_device-2.3.32.2/py_ios_device.egg-info/PKG-INFO
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2406 2023-05-24 02:44:55.000000 py_ios_device-2.3.32.2/py_ios_device.egg-info/SOURCES.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)        1 2023-05-24 02:44:55.000000 py_ios_device-2.3.32.2/py_ios_device.egg-info/dependency_links.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       51 2023-05-24 02:44:55.000000 py_ios_device-2.3.32.2/py_ios_device.egg-info/entry_points.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)      141 2023-05-24 02:44:55.000000 py_ios_device-2.3.32.2/py_ios_device.egg-info/requires.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       16 2023-05-24 02:44:55.000000 py_ios_device-2.3.32.2/py_ios_device.egg-info/top_level.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)      140 2023-04-07 02:39:15.000000 py_ios_device-2.3.32.2/requirements.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       38 2023-05-24 02:44:55.186930 py_ios_device-2.3.32.2/setup.cfg
+-rw-r--r--   0 rongcloud   (501) staff       (20)      976 2023-04-07 02:35:34.000000 py_ios_device-2.3.32.2/setup.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      959 2023-04-20 03:34:06.000000 py_ios_device-2.3.32.2/setup2.py
```

### Comparing `py_ios_device-2.3.32.1/LICENSE` & `py_ios_device-2.3.32.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/PKG-INFO` & `py_ios_device-2.3.32.2/py_ios_device.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py_ios_device
-Version: 2.3.32.1
+Name: py-ios-device
+Version: 2.3.32.2
 Summary: Get ios data and operate ios devices
 Home-page: https://github.com/YueChen-C/py-ios-device
 Author: chenpeijie
 Author-email: cpjsf@163.com
 Maintainer: chenpeijie
 Maintainer-email: 
 License: UNKNOWN
@@ -297,14 +297,31 @@
 
 #### enable developer mode
 ```bash
 $ pyidevice enable_developer_mode
 ```
 
 
+#### using python
+```python
+
+from ios_device.cli.base import InstrumentsBase
+from ios_device.util.dtx_msg import DTXMessage
+
+with InstrumentsBase() as rpc:
+    def sysmontap_callback(res: DTXMessage):
+        print(res.selector, res.auxiliaries)
+
+    rpc.process_attributes = ['name', 'pid']
+    rpc.system_attributes = rpc.device_info.sysmonSystemAttributes()
+    rpc.sysmontap(sysmontap_callback)
+
+
+```
+
 QQ ：37042417
 
 
 api : [document](./doc/使用文档.md)
 demo: [document](./test/test.py)
```

### Comparing `py_ios_device-2.3.32.1/README.md` & `py_ios_device-2.3.32.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -280,13 +280,30 @@
 
 #### enable developer mode
 ```bash
 $ pyidevice enable_developer_mode
 ```
 
 
+#### using python
+```python
+
+from ios_device.cli.base import InstrumentsBase
+from ios_device.util.dtx_msg import DTXMessage
+
+with InstrumentsBase() as rpc:
+    def sysmontap_callback(res: DTXMessage):
+        print(res.selector, res.auxiliaries)
+
+    rpc.process_attributes = ['name', 'pid']
+    rpc.system_attributes = rpc.device_info.sysmonSystemAttributes()
+    rpc.sysmontap(sysmontap_callback)
+
+
+```
+
 QQ ：37042417
 
 
 api : [document](./doc/使用文档.md)
 demo: [document](./test/test.py)
```

### Comparing `py_ios_device-2.3.32.1/demo/afc.py` & `py_ios_device-2.3.32.2/demo/afc.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/demo/crash_log.py` & `py_ios_device-2.3.32.2/demo/crash_log.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/demo/installation_proxy.py` & `py_ios_device-2.3.32.2/demo/installation_proxy.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/demo/instrument_demo/activity.py` & `py_ios_device-2.3.32.2/demo/instrument_demo/activity.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/demo/instrument_demo/app_lifecycle.py` & `py_ios_device-2.3.32.2/demo/instrument_demo/app_lifecycle.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/demo/instrument_demo/applictionListing.py` & `py_ios_device-2.3.32.2/demo/instrument_demo/applictionListing.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/demo/instrument_demo/coreprofilesessiontap.py` & `py_ios_device-2.3.32.2/demo/instrument_demo/coreprofilesessiontap.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/demo/instrument_demo/coreprofilesessiontap_parse.py` & `py_ios_device-2.3.32.2/demo/instrument_demo/coreprofilesessiontap_parse.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/demo/instrument_demo/deviceinfo.py` & `py_ios_device-2.3.32.2/demo/instrument_demo/deviceinfo.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/demo/instrument_demo/gpu.py` & `py_ios_device-2.3.32.2/demo/instrument_demo/gpu.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/demo/instrument_demo/graphics.py` & `py_ios_device-2.3.32.2/demo/instrument_demo/graphics.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/demo/instrument_demo/launchAPP.py` & `py_ios_device-2.3.32.2/demo/instrument_demo/launchAPP.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/demo/instrument_demo/mobileNotifications.py` & `py_ios_device-2.3.32.2/demo/instrument_demo/mobileNotifications.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/demo/instrument_demo/netstatPID.py` & `py_ios_device-2.3.32.2/demo/instrument_demo/netstatPID.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/demo/instrument_demo/networking.py` & `py_ios_device-2.3.32.2/demo/instrument_demo/networking.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/demo/instrument_demo/sysmontap.py` & `py_ios_device-2.3.32.2/demo/instrument_demo/sysmontap.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/demo/instrument_demo/xcuitest.py` & `py_ios_device-2.3.32.2/demo/instrument_demo/xcuitest.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/demo/mobile_config.py` & `py_ios_device-2.3.32.2/demo/mobile_config.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/demo/pcapd.py` & `py_ios_device-2.3.32.2/demo/pcapd.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/demo/screenshotr.py` & `py_ios_device-2.3.32.2/demo/screenshotr.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/demo/syslog.py` & `py_ios_device-2.3.32.2/demo/syslog.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/cli/base.py` & `py_ios_device-2.3.32.2/ios_device/cli/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,84 +27,86 @@
     def __exit__(self):
         self.rpc.stop()
 
     def __init__(self, rpc: InstrumentServer):
         self.rpc = rpc
 
     def runningProcesses(self):
-        """ 获取当前运行应用
+        """ Get a list of running applications; 获取当前运行应用
         :return:
         """
         parsed = self.rpc.call(InstrumentsService.DeviceInfo, "runningProcesses").selector
         return parsed
 
-    def execnameForPid(self, pid):
-        """ 获取应用路径
+    def execnameForPid(self, pid: str):
+        """ Get the application name running pid; 获取 pid 应用名称
         :param pid:
         :return:
         """
         parsed = self.rpc.call(InstrumentsService.DeviceInfo, "execnameForPid:", str(pid)).selector
         return parsed
 
-    def isRunningPid(self, pid):
-        """ 应用是否运行
+    def isRunningPid(self, pid: str):
+        """ Is the app running ; 应用是否运行
         :param pid:
         :return:
         """
         parsed = self.rpc.call(InstrumentsService.DeviceInfo, "isRunningPid:", str(pid)).selector
         return parsed
 
-    def nameForUID(self, uid):
+    def nameForUID(self, uid: str):
         parsed = self.rpc.call(InstrumentsService.DeviceInfo, "nameForUID:", str(uid)).selector
         return parsed
 
     def machTimeInfo(self):
         """ 时间校准，获取
-        :return: mach time 比例
+        :return: [mach_absolute_time, numer, denom]
         """
         parsed = self.rpc.call(InstrumentsService.DeviceInfo, "machTimeInfo").selector
         return parsed
 
     def traceCodesFile(self):
-        """ traceCodes 堆栈 code 码
-        :return:
+        """ code for stack data
+        :return: {code: name}
         """
         parsed = self.rpc.call(InstrumentsService.DeviceInfo, "traceCodesFile").selector
         return {int(k, 16): v for k, v in map(lambda l: l.split(), parsed.splitlines())}
 
     def networkInformation(self):
         """ 当前网络信息
-        :return:
+        :return: {'en0': 'Wi-Fi', 'en1': 'Ethernet Adaptor (en1)', 'lo0': 'Loopback'}
         """
         parsed = self.rpc.call(InstrumentsService.DeviceInfo, "networkInformation").selector
         return parsed
 
     def systemInformation(self):
-        """ 设备基本信息
+        """ system information
         :return:
         """
         parsed = self.rpc.call(InstrumentsService.DeviceInfo, "systemInformation").selector
         return parsed
 
     def hardwareInformation(self):
-        """ 硬件数据
+        """ hardware Information
         :return:
         """
         parsed = self.rpc.call(InstrumentsService.DeviceInfo, "hardwareInformation").selector
         return parsed
 
     def sysmonProcessAttributes(self):
-        """ 获取应用性能数据所需的参数
+        """ Parameters required to obtain application performance data, 获取应用性能数据所需的参数
+        for the 'com.apple.instruments.server.services.sysmontap' service.
         :return:
         """
         parsed = self.rpc.call(InstrumentsService.DeviceInfo, "sysmonProcessAttributes").selector
         return parsed
 
     def sysmonSystemAttributes(self):
-        """ 获取系统性能数据所需的参数
+        """ Parameters needed to obtain system performance data; 获取系统性能数据所需的参数
+        for the 'com.apple.instruments.server.services.sysmontap' service.
         :return:
         """
         parsed = self.rpc.call(InstrumentsService.DeviceInfo, "sysmonSystemAttributes").selector
         return parsed
 
     def symbolicatorSignaturesForExpiredPids(self):
         parsed = self.rpc.call(InstrumentsService.DeviceInfo,
@@ -131,15 +133,15 @@
         return parsed
 
     def kpepDatabase(self):
         parsed = self.rpc.call(InstrumentsService.DeviceInfo, "kpepDatabase").selector
         return plistlib.loads(parsed)
 
     def machKernelName(self):
-        parsed = self.rpc.call(InstrumentsService.DeviceInfo, "cpKDebugEventsAsXML").selector
+        parsed = self.rpc.call(InstrumentsService.DeviceInfo, "machKernelName").selector
         return parsed
 
 
 class InstrumentsBase:
     def __init__(self, udid=None, network=None, lockdown=None):
         self.udid = udid
         self.network = network
@@ -188,100 +190,118 @@
 
     @property
     def device_info(self) -> InstrumentDeviceInfo:
         rpc = self.instruments
         return InstrumentDeviceInfo(rpc)
 
     def launch_app(self, bundle_id,
-                   app_env=None,
-                   app_args: list = [],
+                   app_env: dict = None,
+                   app_args: list = None,
                    app_path: str = "",
-                   options: dict = {},
+                   options: {} = None,
                    callback: callable = None):
-
-        if app_env is None:
-            app_env = {}
-        else:
-            app_env = json.loads(app_env)
-            if not isinstance(app_env, dict):
-                log.info('app_env 参数异常应为 Json 格式')
-                return
-
+        """
+        launch app ; 启动应用
+        @param bundle_id: bundle id
+        @param app_env:  App running environment variables; 应用运行环境变量
+        @param app_args: Parameters required when the app starts; 应用启动时所需参数
+        @param app_path: The absolute path of the app usually does not need this parameter,which is used to prevent the
+        same bundle id
+        @param options:  startup options; 启动选项
+        @param callback: callback function will return the app log; 回调函数会持续返回 app 日志
+        @return:
+        """
         options = options or {
             "StartSuspendedKey": 0,
             "KillExisting": False,
         }
         if callback:
-            self.instruments.register_channel_callback(InstrumentsService.ProcessControl, callable)
+            self.instruments.register_channel_callback(InstrumentsService.ProcessControl, callback)
         pid = self.instruments.call(InstrumentsService.ProcessControl,
                                     "launchSuspendedProcessWithDevicePath:bundleIdentifier:environment:arguments"
                                     ":options:",
-                                    app_path, bundle_id, app_env, app_args, options).selector
+                                    app_path, bundle_id, app_env or {}, app_args or [], options or {}).selector
+        log.info(f'launch {bundle_id} pid: {pid}')
         return pid
 
-    def kill_app(self, pid):
+    def kill_app(self, pid: str):
+        """
+        kill app; 杀死应用
+        @param pid:
+        @return:
+        """
         parsed = self.instruments.call(InstrumentsService.ProcessControl, "killPid:", str(pid)).selector
         return parsed
 
-    def signal_app(self, sig, pid):
+    def signal_app(self, sig: str, pid: str):
+        """
+        send signal to app; 向应用发送信号
+        @param sig:
+        @param pid:
+        @return:
+        """
         parsed = self.instruments.call(InstrumentsService.ProcessControl, "sendSignal:toPid", str(sig),
                                        str(pid)).selector
         return parsed
 
     def application_listing(self, bundle_id=None):
-        """ _selector
-            - installedApplicationsMatching:registerUpdateToken:
-            - unregisterUpdateToken:
-        :return:
+        """
+        Get the list of installed applications; 获取已安装应用列表
+        @param bundle_id:  bundle id
+        @return:
         """
         applist = self.instruments.call(InstrumentsService.ApplicationListing,
                                         "installedApplicationsMatching:registerUpdateToken:",
                                         {}, "").selector
         if bundle_id:
             for app in applist:
                 if app.get('CFBundleIdentifier') == bundle_id:
                     return app
         return applist
 
     def sysmontap(self,
                   callback: callable,
                   time: int = 1000,
-                  stopSignal: threading.Event = threading.Event()):
+                  stopSignal: threading.Event = threading.Event(),
+                  system_attributes=None,
+                  process_attributes=None):
+        """
+        Get application performance data ; 获取性能数据
+        @param process_attributes:
+        @param system_attributes:
+        @param callback:
+        @param time: Output frequency (ms)
+        @param stopSignal:
+        @return:
         """
-        :param time: 获取时间间隔（ms）
-        :param stopSignal:
-        :param callback:
-        :return:
-        """
-
-        log.info(f'Sysmontap setConfig ...')
         config = {
-            'ur': time,  # 输出频率 ms
+            'ur': time,
             'bm': 0,
             'cpuUsage': True,
             'sampleInterval': time * 1000000}
-        if self.system_attributes:  # 系统信息字段
-            config['sysAttrs'] = self.system_attributes
-        if self.process_attributes:  # 进程信息字段
-            config['procAttrs'] = self.process_attributes
+        _system_attributes = self.system_attributes or system_attributes
+        config['sysAttrs'] = _system_attributes
+        process_attributes = self.process_attributes or process_attributes
+        config['procAttrs'] = process_attributes
         self.instruments.call(InstrumentsService.Sysmontap, "setConfig:", config)
         self.instruments.register_channel_callback(InstrumentsService.Sysmontap, callback)
         self.instruments.call(InstrumentsService.Sysmontap, "start")
         log.info(f'Sysmontap start ...')
         log.info(f'wait for data ...')
         while not stopSignal.wait(1):
             pass
         self.instruments.call(InstrumentsService.Sysmontap, "stop")
 
     def graphics(self,
                  callback: callable,
                  time=1000,
                  stopSignal: threading.Event = threading.Event()):
-        """ 获取 FPS 等数据
-        :param time: 获取时间间隔（ms）
+        """
+        get graphics
+        :param time: Output frequency (ms)
         :param callback:
         :param stopSignal:
         :return:
         """
         self.instruments.register_channel_callback(InstrumentsService.GraphicsOpengl, callback)
         log.info(self.instruments.call(InstrumentsService.GraphicsOpengl, "availableStatistics").selector)
         log.info(self.instruments.call(InstrumentsService.GraphicsOpengl, "driverNames").selector)
@@ -291,28 +311,35 @@
                               "startSamplingAtTimeInterval:",
                               0.0)
         while not stopSignal.wait(1):
             pass
         self.instruments.call(InstrumentsService.GraphicsOpengl, "stopSampling")
 
     def xcode_network(self, pid, stopSignal: threading.Event = threading.Event()):
+        """
+        Get the network data of the launched application
+        @param pid:
+        @param stopSignal:
+        @return:
+        """
         channel = "com.apple.xcode.debug-gauge-data-providers.NetworkStatistics"
         attr = {}
         self.instruments.call(channel, "startSamplingForPIDs:", {pid})
         while not stopSignal.wait(1):
             ret = self.instruments.call(channel, "sampleAttributes:forPIDs:", attr, {pid})
             print(ret.selector)
 
     def networking(self,
                    callback: callable,
                    stopSignal: threading.Event = threading.Event()):
-        """ 获取网络数据
-        :param callback:
-        :param stopSignal:
-        :return:
+        """
+        Get system network data
+        @param callback:
+        @param stopSignal:
+        @return:
         """
         self.instruments.register_channel_callback(InstrumentsService.Networking, callback)
 
         self.instruments.call(InstrumentsService.Networking, "replayLastRecordedSession")
         log.info(msg=f'networking replayLastRecordedSession')
         self.instruments.call(InstrumentsService.Networking, "startMonitoring")
         log.info(msg=f'networking startMonitoring networking')
@@ -321,14 +348,20 @@
             pass
         self.instruments.call(InstrumentsService.Networking, "stopMonitoring")
         log.info(msg=f'networking stopMonitoring ')
 
     def mobile_notifications(self,
                              callback: callable,
                              stopSignal: threading.Event = threading.Event()):
+        """
+        get mobile notifications
+        @param callback:
+        @param stopSignal:
+        @return:
+        """
 
         self.instruments.register_undefined_callback(callback)
         self.instruments.call(InstrumentsService.MobileNotifications,
                               'setApplicationStateNotificationsEnabled:', str(True))
         log.info(msg='Waiting for action app')
         while not stopSignal.wait(1):
             pass
@@ -350,14 +383,20 @@
         while not stopSignal.wait(1):
             pass
         self.instruments.call(InstrumentsService.CoreProfileSessionTap, "stop")
 
     def gpu_counters(self,
                      callback: callable,
                      stopSignal: threading.Event = threading.Event()):
+        """
+        get gpu counters
+        @param callback:
+        @param stopSignal:
+        @return:
+        """
         self.instruments.register_undefined_callback(callback)
         requestDeviceGPUInfo = self.instruments.call(InstrumentsService.GPU, 'requestDeviceGPUInfo').selector
 
         min_collection_interval = requestDeviceGPUInfo[0].get('min-collection-interval')
         self.instruments.call(InstrumentsService.GPU,
                               "configureCounters:counterProfile:interval:windowLimit:tracingPID:",
                               RawInt64sl(min_collection_interval, 3, 1, 0), RawInt32sl(-1))
@@ -366,50 +405,68 @@
         while not stopSignal.wait(1):
             pass
         self.instruments.call(InstrumentsService.GPU, 'stopCollectingCounters')
         data = self.instruments.call(InstrumentsService.GPU, 'flushRemainingData').selector
         return data
 
     def screenshot(self):
+        """
+        screenshot
+        @return:
+        """
         var = self.instruments.call(InstrumentsService.Screenshot, "takeScreenshot").selector
         return var
 
     def power(self,
               callback: callable,
               stopSignal: threading.Event = threading.Event()):
+        """
+        get power  ios < 14
+        @param callback:
+        @param stopSignal:
+        @return:
+        """
         channel = "com.apple.instruments.server.services.power"
         self.instruments.register_channel_callback(channel, callback)
         stream_num = self.instruments.call(channel, "openStreamForPath:", "live/level.dat").selector
         print("open", stream_num)
         print("start", self.instruments.call(channel, "startStreamTransfer:", float(stream_num)).selector)
         print("[!] wait a few seconds, be patient...")
         while not stopSignal.wait(1):
             pass
         log.info(f"stop{self.instruments.call(channel, 'endStreamTransfer:', float(stream_num)).selector}")
 
     def xcode_energy(self, pid, stopSignal: threading.Event = threading.Event()):
+        """
+        get energy
+        @param pid:
+        @param stopSignal:
+        @return:
+        """
         self.instruments.call(InstrumentsService.XcodeEnergy, "startSamplingForPIDs:", {pid})
         while not stopSignal.wait(1):
             ret = self.instruments.call(InstrumentsService.XcodeEnergy, "sampleAttributes:forPIDs:", {}, {pid})
             print(ret.selector)
 
     def get_condition_inducer(self):
-        """ 获取网络配置参数，用于 condition_inducer
+        """ Get condition data configuration 获取压力数据配置数据
         :return:
         """
         ret = self.instruments.call(InstrumentsService.ConditionInducer, "availableConditionInducers").selector
         return ret
 
     def set_condition_inducer(self,
                               condition_identifier,
                               profile_identifier,
                               stopSignal: threading.Event = threading.Event()):
-        """ 设置手机状态，模拟网络，手机压力数据等
-        :param condition_identifier:
-        :param profile_identifier:
+        """ Set mobile phone status, simulated network, mobile cpu pressure, etc; 设置手机状态，模拟网络，手机压力数据等
+        @param condition_identifier:
+        @param profile_identifier:
+        @param stopSignal: thread event control
+
         :return:
         """
         ret = self.instruments.call(InstrumentsService.ConditionInducer,
                                     'enableConditionWithIdentifier:profileIdentifier:',
                                     condition_identifier, profile_identifier).selector
         log.info(
             f"Condition configuration enabled [{profile_identifier}] successfully, please do not stop the command...")
```

### Comparing `py_ios_device-2.3.32.1/ios_device/cli/cli.py` & `py_ios_device-2.3.32.2/ios_device/cli/cli.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/cli/instruments.py` & `py_ios_device-2.3.32.2/ios_device/cli/instruments.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,15 @@
                 print("Memory  >>", Memory.decode(data))
                 print("Network >>", Network.decode(data))
                 print("Disk    >>", disk.decode(data))
                 print("CPU     >>", SystemCPUUsage)
 
     with InstrumentsBase(udid=udid, network=network) as rpc:
         rpc.process_attributes = ['name', 'pid']
-        rpc.system_attributes = rpc.device_info.sysmonProcessAttributes()
+        rpc.system_attributes = rpc.device_info.sysmonSystemAttributes()
         rpc.sysmontap(on_callback_message)
 
 
 @instruments.group()
 def condition():
     """
     Set system running condition
```

### Comparing `py_ios_device-2.3.32.1/ios_device/cli/mobile.py` & `py_ios_device-2.3.32.2/ios_device/cli/mobile.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/py_ios_device.py` & `py_ios_device-2.3.32.2/ios_device/py_ios_device.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/servers/Installation.py` & `py_ios_device-2.3.32.2/ios_device/servers/Installation.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/servers/Instrument.py` & `py_ios_device-2.3.32.2/ios_device/servers/Instrument.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/servers/afc.py` & `py_ios_device-2.3.32.2/ios_device/servers/afc.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/servers/amfi.py` & `py_ios_device-2.3.32.2/ios_device/servers/amfi.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/servers/crash_log.py` & `py_ios_device-2.3.32.2/ios_device/servers/crash_log.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/servers/diagnostics_relay.py` & `py_ios_device-2.3.32.2/ios_device/servers/diagnostics_relay.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/servers/dvt.py` & `py_ios_device-2.3.32.2/ios_device/servers/dvt.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/servers/house_arrest.py` & `py_ios_device-2.3.32.2/ios_device/servers/house_arrest.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/servers/image_mounter.py` & `py_ios_device-2.3.32.2/ios_device/servers/image_mounter.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/servers/mc_install.py` & `py_ios_device-2.3.32.2/ios_device/servers/mc_install.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/servers/notification_proxy.py` & `py_ios_device-2.3.32.2/ios_device/servers/notification_proxy.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/servers/os_trace.py` & `py_ios_device-2.3.32.2/ios_device/servers/os_trace.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/servers/pcapd.py` & `py_ios_device-2.3.32.2/ios_device/servers/pcapd.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/servers/screenshotr.py` & `py_ios_device-2.3.32.2/ios_device/servers/screenshotr.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/servers/simulate_location.py` & `py_ios_device-2.3.32.2/ios_device/servers/simulate_location.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/servers/spring_board.py` & `py_ios_device-2.3.32.2/ios_device/servers/spring_board.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/servers/syslog.py` & `py_ios_device-2.3.32.2/ios_device/servers/syslog.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/servers/testmanagerd.py` & `py_ios_device-2.3.32.2/ios_device/servers/testmanagerd.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/util/__init__.py` & `py_ios_device-2.3.32.2/ios_device/util/__init__.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/util/api_util.py` & `py_ios_device-2.3.32.2/ios_device/util/api_util.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/util/bpylist2.py` & `py_ios_device-2.3.32.2/ios_device/util/bpylist2.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/util/ca.py` & `py_ios_device-2.3.32.2/ios_device/util/ca.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/util/constants.py` & `py_ios_device-2.3.32.2/ios_device/util/constants.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/util/dtx_msg.py` & `py_ios_device-2.3.32.2/ios_device/util/dtx_msg.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/util/exceptions.py` & `py_ios_device-2.3.32.2/ios_device/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/util/forward.py` & `py_ios_device-2.3.32.2/ios_device/util/forward.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/util/gpu_decode.py` & `py_ios_device-2.3.32.2/ios_device/util/gpu_decode.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/util/kc_data.py` & `py_ios_device-2.3.32.2/ios_device/util/kc_data.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/util/kperf_data.py` & `py_ios_device-2.3.32.2/ios_device/util/kperf_data.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/util/lifecycle.py` & `py_ios_device-2.3.32.2/ios_device/util/lifecycle.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/util/lockdown.py` & `py_ios_device-2.3.32.2/ios_device/util/lockdown.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/util/plist_service.py` & `py_ios_device-2.3.32.2/ios_device/util/plist_service.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/util/plistlib.py` & `py_ios_device-2.3.32.2/ios_device/util/plistlib.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/util/usbmux.py` & `py_ios_device-2.3.32.2/ios_device/util/usbmux.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/util/utils.py` & `py_ios_device-2.3.32.2/ios_device/util/utils.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/ios_device/util/variables.py` & `py_ios_device-2.3.32.2/ios_device/util/variables.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/py_ios_device.egg-info/PKG-INFO` & `py_ios_device-2.3.32.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py-ios-device
-Version: 2.3.32.1
+Name: py_ios_device
+Version: 2.3.32.2
 Summary: Get ios data and operate ios devices
 Home-page: https://github.com/YueChen-C/py-ios-device
 Author: chenpeijie
 Author-email: cpjsf@163.com
 Maintainer: chenpeijie
 Maintainer-email: 
 License: UNKNOWN
@@ -297,14 +297,31 @@
 
 #### enable developer mode
 ```bash
 $ pyidevice enable_developer_mode
 ```
 
 
+#### using python
+```python
+
+from ios_device.cli.base import InstrumentsBase
+from ios_device.util.dtx_msg import DTXMessage
+
+with InstrumentsBase() as rpc:
+    def sysmontap_callback(res: DTXMessage):
+        print(res.selector, res.auxiliaries)
+
+    rpc.process_attributes = ['name', 'pid']
+    rpc.system_attributes = rpc.device_info.sysmonSystemAttributes()
+    rpc.sysmontap(sysmontap_callback)
+
+
+```
+
 QQ ：37042417
 
 
 api : [document](./doc/使用文档.md)
 demo: [document](./test/test.py)
```

### Comparing `py_ios_device-2.3.32.1/py_ios_device.egg-info/SOURCES.txt` & `py_ios_device-2.3.32.2/py_ios_device.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/setup.py` & `py_ios_device-2.3.32.2/setup.py`

 * *Files identical despite different names*

### Comparing `py_ios_device-2.3.32.1/setup2.py` & `py_ios_device-2.3.32.2/setup2.py`

 * *Files identical despite different names*

