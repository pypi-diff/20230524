# Comparing `tmp/pyidevice-2.3.32.2.tar.gz` & `tmp/pyidevice-2.3.32.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyidevice-2.3.32.2.tar", last modified: Wed May 24 02:45:21 2023, max compression
+gzip compressed data, was "pyidevice-2.3.32.3.tar", last modified: Wed May 24 02:53:19 2023, max compression
```

## Comparing `pyidevice-2.3.32.2.tar` & `pyidevice-2.3.32.3.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:45:21.642094 pyidevice-2.3.32.2/
--rw-r--r--   0 rongcloud   (501) staff       (20)    35147 2022-09-26 09:47:22.000000 pyidevice-2.3.32.2/LICENSE
--rw-r--r--   0 rongcloud   (501) staff       (20)       24 2022-09-26 09:47:22.000000 pyidevice-2.3.32.2/MANIFEST.in
--rw-r--r--   0 rongcloud   (501) staff       (20)    11371 2023-05-24 02:45:21.641778 pyidevice-2.3.32.2/PKG-INFO
--rw-r--r--   0 rongcloud   (501) staff       (20)    10950 2023-05-24 02:33:49.000000 pyidevice-2.3.32.2/README.md
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:45:21.627580 pyidevice-2.3.32.2/demo/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 pyidevice-2.3.32.2/demo/__init__.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    18971 2022-12-08 06:20:36.000000 pyidevice-2.3.32.2/demo/afc.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1141 2022-12-08 06:20:36.000000 pyidevice-2.3.32.2/demo/crash_log.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     6471 2023-03-07 02:35:28.000000 pyidevice-2.3.32.2/demo/installation_proxy.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:45:21.630636 pyidevice-2.3.32.2/demo/instrument_demo/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 pyidevice-2.3.32.2/demo/instrument_demo/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      866 2022-09-26 09:47:22.000000 pyidevice-2.3.32.2/demo/instrument_demo/activity.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3290 2023-04-07 02:39:15.000000 pyidevice-2.3.32.2/demo/instrument_demo/app_lifecycle.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      536 2022-09-26 09:47:22.000000 pyidevice-2.3.32.2/demo/instrument_demo/applictionListing.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      362 2023-04-07 02:35:34.000000 pyidevice-2.3.32.2/demo/instrument_demo/channel.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4146 2023-05-22 07:56:02.000000 pyidevice-2.3.32.2/demo/instrument_demo/coreprofilesessiontap.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1535 2023-05-22 07:56:02.000000 pyidevice-2.3.32.2/demo/instrument_demo/coreprofilesessiontap_parse.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2174 2023-02-09 09:46:25.000000 pyidevice-2.3.32.2/demo/instrument_demo/deviceinfo.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      494 2023-05-22 07:56:02.000000 pyidevice-2.3.32.2/demo/instrument_demo/energy.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2199 2023-05-08 09:42:27.000000 pyidevice-2.3.32.2/demo/instrument_demo/gpu.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1085 2023-05-22 07:56:02.000000 pyidevice-2.3.32.2/demo/instrument_demo/graphics.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      748 2023-05-22 07:56:02.000000 pyidevice-2.3.32.2/demo/instrument_demo/launchAPP.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      851 2023-02-16 02:26:32.000000 pyidevice-2.3.32.2/demo/instrument_demo/mobileNotifications.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      533 2023-02-09 09:46:25.000000 pyidevice-2.3.32.2/demo/instrument_demo/netstatPID.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2835 2023-02-09 09:46:25.000000 pyidevice-2.3.32.2/demo/instrument_demo/networking.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2554 2023-04-20 02:17:26.000000 pyidevice-2.3.32.2/demo/instrument_demo/sysmontap.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     8873 2022-09-26 09:47:22.000000 pyidevice-2.3.32.2/demo/instrument_demo/xcuitest.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3608 2022-12-08 06:20:36.000000 pyidevice-2.3.32.2/demo/mobile_config.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     5368 2022-09-26 09:47:22.000000 pyidevice-2.3.32.2/demo/pcapd.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3089 2022-12-08 06:20:36.000000 pyidevice-2.3.32.2/demo/screenshotr.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4297 2022-12-08 06:20:36.000000 pyidevice-2.3.32.2/demo/syslog.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:45:21.625237 pyidevice-2.3.32.2/ios_device/
--rw-r--r--   0 rongcloud   (501) staff       (20)       37 2022-09-26 09:47:22.000000 pyidevice-2.3.32.2/ios_device/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)       25 2023-05-24 02:44:54.000000 pyidevice-2.3.32.2/ios_device/__version__.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:45:21.631987 pyidevice-2.3.32.2/ios_device/cli/
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 pyidevice-2.3.32.2/ios_device/cli/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    31554 2023-05-24 02:44:13.000000 pyidevice-2.3.32.2/ios_device/cli/base.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      988 2023-04-07 02:33:45.000000 pyidevice-2.3.32.2/ios_device/cli/cli.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    19122 2023-05-24 02:30:31.000000 pyidevice-2.3.32.2/ios_device/cli/instruments.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    11223 2023-04-26 06:21:46.000000 pyidevice-2.3.32.2/ios_device/cli/mobile.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      293 2022-09-26 09:47:22.000000 pyidevice-2.3.32.2/ios_device/main.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    23312 2023-04-07 02:39:15.000000 pyidevice-2.3.32.2/ios_device/py_ios_device.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:45:21.636330 pyidevice-2.3.32.2/ios_device/servers/
--rw-r--r--   0 rongcloud   (501) staff       (20)     7287 2023-04-26 03:35:04.000000 pyidevice-2.3.32.2/ios_device/servers/Installation.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1029 2023-04-20 02:15:07.000000 pyidevice-2.3.32.2/ios_device/servers/Instrument.py
--rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 pyidevice-2.3.32.2/ios_device/servers/__init__.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    19387 2022-12-08 06:20:36.000000 pyidevice-2.3.32.2/ios_device/servers/afc.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1238 2022-12-08 06:20:36.000000 pyidevice-2.3.32.2/ios_device/servers/amfi.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1155 2022-12-08 06:20:36.000000 pyidevice-2.3.32.2/ios_device/servers/crash_log.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      993 2023-05-22 06:59:19.000000 pyidevice-2.3.32.2/ios_device/servers/diagnostics_relay.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7844 2023-04-20 02:15:07.000000 pyidevice-2.3.32.2/ios_device/servers/dvt.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1223 2023-03-07 02:32:12.000000 pyidevice-2.3.32.2/ios_device/servers/house_arrest.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3536 2022-12-08 06:20:36.000000 pyidevice-2.3.32.2/ios_device/servers/image_mounter.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     1679 2023-03-17 09:31:16.000000 pyidevice-2.3.32.2/ios_device/servers/mc_install.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)    31263 2022-12-08 06:20:36.000000 pyidevice-2.3.32.2/ios_device/servers/notification_proxy.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     2834 2023-04-20 02:31:19.000000 pyidevice-2.3.32.2/ios_device/servers/os_trace.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3163 2022-12-08 06:20:36.000000 pyidevice-2.3.32.2/ios_device/servers/pcapd.py
--rwxr-xr-x   0 rongcloud   (501) staff       (20)     3102 2022-12-08 06:20:36.000000 pyidevice-2.3.32.2/ios_device/servers/screenshotr.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1083 2023-01-04 04:20:57.000000 pyidevice-2.3.32.2/ios_device/servers/simulate_location.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1596 2023-03-31 08:20:40.000000 pyidevice-2.3.32.2/ios_device/servers/spring_board.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3329 2023-01-04 03:41:43.000000 pyidevice-2.3.32.2/ios_device/servers/syslog.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      864 2023-04-17 09:44:17.000000 pyidevice-2.3.32.2/ios_device/servers/testmanagerd.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:45:21.640876 pyidevice-2.3.32.2/ios_device/util/
--rw-r--r--   0 rongcloud   (501) staff       (20)     1860 2022-09-26 09:47:22.000000 pyidevice-2.3.32.2/ios_device/util/__init__.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    11825 2022-12-08 06:20:36.000000 pyidevice-2.3.32.2/ios_device/util/api_util.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    24888 2022-12-08 06:30:13.000000 pyidevice-2.3.32.2/ios_device/util/bpylist2.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4657 2022-09-26 09:47:22.000000 pyidevice-2.3.32.2/ios_device/util/ca.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4585 2022-09-26 09:47:22.000000 pyidevice-2.3.32.2/ios_device/util/constants.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7921 2022-12-08 06:20:36.000000 pyidevice-2.3.32.2/ios_device/util/dtx_msg.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     1842 2022-09-26 09:47:22.000000 pyidevice-2.3.32.2/ios_device/util/exceptions.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3907 2022-09-26 09:47:22.000000 pyidevice-2.3.32.2/ios_device/util/forward.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     7443 2023-01-04 06:39:27.000000 pyidevice-2.3.32.2/ios_device/util/gpu_decode.py
--rw-r--r--   0 rongcloud   (501) staff       (20)   109555 2023-04-07 02:39:15.000000 pyidevice-2.3.32.2/ios_device/util/kc_data.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    41845 2023-04-07 02:39:15.000000 pyidevice-2.3.32.2/ios_device/util/kperf_data.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    16216 2023-04-07 02:39:15.000000 pyidevice-2.3.32.2/ios_device/util/lifecycle.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    16285 2023-04-20 02:30:51.000000 pyidevice-2.3.32.2/ios_device/util/lockdown.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     3131 2022-12-08 06:20:36.000000 pyidevice-2.3.32.2/ios_device/util/plist_service.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    27335 2023-04-26 02:45:02.000000 pyidevice-2.3.32.2/ios_device/util/plistlib.py
--rw-r--r--   0 rongcloud   (501) staff       (20)    12592 2023-03-31 09:19:13.000000 pyidevice-2.3.32.2/ios_device/util/usbmux.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     9513 2023-02-09 09:51:53.000000 pyidevice-2.3.32.2/ios_device/util/utils.py
--rw-r--r--   0 rongcloud   (501) staff       (20)     4261 2023-02-14 02:46:09.000000 pyidevice-2.3.32.2/ios_device/util/variables.py
-drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:45:21.641588 pyidevice-2.3.32.2/pyidevice.egg-info/
--rw-r--r--   0 rongcloud   (501) staff       (20)    11371 2023-05-24 02:45:21.000000 pyidevice-2.3.32.2/pyidevice.egg-info/PKG-INFO
--rw-r--r--   0 rongcloud   (501) staff       (20)     2486 2023-05-24 02:45:21.000000 pyidevice-2.3.32.2/pyidevice.egg-info/SOURCES.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)        1 2023-05-24 02:45:21.000000 pyidevice-2.3.32.2/pyidevice.egg-info/dependency_links.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       51 2023-05-24 02:45:21.000000 pyidevice-2.3.32.2/pyidevice.egg-info/entry_points.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)      141 2023-05-24 02:45:21.000000 pyidevice-2.3.32.2/pyidevice.egg-info/requires.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       10 2023-05-24 02:45:21.000000 pyidevice-2.3.32.2/pyidevice.egg-info/top_level.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)      140 2023-04-07 02:39:15.000000 pyidevice-2.3.32.2/requirements.txt
--rw-r--r--   0 rongcloud   (501) staff       (20)       38 2023-05-24 02:45:21.642154 pyidevice-2.3.32.2/setup.cfg
--rw-r--r--   0 rongcloud   (501) staff       (20)      976 2023-04-07 02:35:34.000000 pyidevice-2.3.32.2/setup.py
--rw-r--r--   0 rongcloud   (501) staff       (20)      959 2023-04-20 03:34:06.000000 pyidevice-2.3.32.2/setup2.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:53:19.330178 pyidevice-2.3.32.3/
+-rw-r--r--   0 rongcloud   (501) staff       (20)    35147 2022-09-26 09:47:22.000000 pyidevice-2.3.32.3/LICENSE
+-rw-r--r--   0 rongcloud   (501) staff       (20)       24 2022-09-26 09:47:22.000000 pyidevice-2.3.32.3/MANIFEST.in
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11371 2023-05-24 02:53:19.329899 pyidevice-2.3.32.3/PKG-INFO
+-rw-r--r--   0 rongcloud   (501) staff       (20)    10950 2023-05-24 02:33:49.000000 pyidevice-2.3.32.3/README.md
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:53:19.313427 pyidevice-2.3.32.3/demo/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 pyidevice-2.3.32.3/demo/__init__.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    18971 2022-12-08 06:20:36.000000 pyidevice-2.3.32.3/demo/afc.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1141 2022-12-08 06:20:36.000000 pyidevice-2.3.32.3/demo/crash_log.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     6471 2023-03-07 02:35:28.000000 pyidevice-2.3.32.3/demo/installation_proxy.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:53:19.317802 pyidevice-2.3.32.3/demo/instrument_demo/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 pyidevice-2.3.32.3/demo/instrument_demo/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      866 2022-09-26 09:47:22.000000 pyidevice-2.3.32.3/demo/instrument_demo/activity.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3290 2023-04-07 02:39:15.000000 pyidevice-2.3.32.3/demo/instrument_demo/app_lifecycle.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      536 2022-09-26 09:47:22.000000 pyidevice-2.3.32.3/demo/instrument_demo/applictionListing.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      362 2023-04-07 02:35:34.000000 pyidevice-2.3.32.3/demo/instrument_demo/channel.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4146 2023-05-22 07:56:02.000000 pyidevice-2.3.32.3/demo/instrument_demo/coreprofilesessiontap.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1535 2023-05-22 07:56:02.000000 pyidevice-2.3.32.3/demo/instrument_demo/coreprofilesessiontap_parse.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2174 2023-02-09 09:46:25.000000 pyidevice-2.3.32.3/demo/instrument_demo/deviceinfo.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      494 2023-05-22 07:56:02.000000 pyidevice-2.3.32.3/demo/instrument_demo/energy.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2199 2023-05-08 09:42:27.000000 pyidevice-2.3.32.3/demo/instrument_demo/gpu.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1085 2023-05-22 07:56:02.000000 pyidevice-2.3.32.3/demo/instrument_demo/graphics.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      748 2023-05-22 07:56:02.000000 pyidevice-2.3.32.3/demo/instrument_demo/launchAPP.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      851 2023-02-16 02:26:32.000000 pyidevice-2.3.32.3/demo/instrument_demo/mobileNotifications.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      533 2023-02-09 09:46:25.000000 pyidevice-2.3.32.3/demo/instrument_demo/netstatPID.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2835 2023-02-09 09:46:25.000000 pyidevice-2.3.32.3/demo/instrument_demo/networking.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2554 2023-04-20 02:17:26.000000 pyidevice-2.3.32.3/demo/instrument_demo/sysmontap.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     8873 2022-09-26 09:47:22.000000 pyidevice-2.3.32.3/demo/instrument_demo/xcuitest.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3608 2022-12-08 06:20:36.000000 pyidevice-2.3.32.3/demo/mobile_config.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     5368 2022-09-26 09:47:22.000000 pyidevice-2.3.32.3/demo/pcapd.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3089 2022-12-08 06:20:36.000000 pyidevice-2.3.32.3/demo/screenshotr.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4297 2022-12-08 06:20:36.000000 pyidevice-2.3.32.3/demo/syslog.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:53:19.310878 pyidevice-2.3.32.3/ios_device/
+-rw-r--r--   0 rongcloud   (501) staff       (20)       37 2022-09-26 09:47:22.000000 pyidevice-2.3.32.3/ios_device/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)       25 2023-05-24 02:53:19.000000 pyidevice-2.3.32.3/ios_device/__version__.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:53:19.319642 pyidevice-2.3.32.3/ios_device/cli/
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 pyidevice-2.3.32.3/ios_device/cli/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    31554 2023-05-24 02:44:13.000000 pyidevice-2.3.32.3/ios_device/cli/base.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      988 2023-04-07 02:33:45.000000 pyidevice-2.3.32.3/ios_device/cli/cli.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    19122 2023-05-24 02:30:31.000000 pyidevice-2.3.32.3/ios_device/cli/instruments.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11223 2023-04-26 06:21:46.000000 pyidevice-2.3.32.3/ios_device/cli/mobile.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      293 2022-09-26 09:47:22.000000 pyidevice-2.3.32.3/ios_device/main.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    23312 2023-04-07 02:39:15.000000 pyidevice-2.3.32.3/ios_device/py_ios_device.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:53:19.324066 pyidevice-2.3.32.3/ios_device/servers/
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7287 2023-04-26 03:35:04.000000 pyidevice-2.3.32.3/ios_device/servers/Installation.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1029 2023-04-20 02:15:07.000000 pyidevice-2.3.32.3/ios_device/servers/Instrument.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)        0 2022-09-26 09:47:22.000000 pyidevice-2.3.32.3/ios_device/servers/__init__.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    19387 2022-12-08 06:20:36.000000 pyidevice-2.3.32.3/ios_device/servers/afc.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1238 2022-12-08 06:20:36.000000 pyidevice-2.3.32.3/ios_device/servers/amfi.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1155 2022-12-08 06:20:36.000000 pyidevice-2.3.32.3/ios_device/servers/crash_log.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      993 2023-05-22 06:59:19.000000 pyidevice-2.3.32.3/ios_device/servers/diagnostics_relay.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7844 2023-04-20 02:15:07.000000 pyidevice-2.3.32.3/ios_device/servers/dvt.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1223 2023-03-07 02:32:12.000000 pyidevice-2.3.32.3/ios_device/servers/house_arrest.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3536 2022-12-08 06:20:36.000000 pyidevice-2.3.32.3/ios_device/servers/image_mounter.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     1679 2023-03-17 09:31:16.000000 pyidevice-2.3.32.3/ios_device/servers/mc_install.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)    31263 2022-12-08 06:20:36.000000 pyidevice-2.3.32.3/ios_device/servers/notification_proxy.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2834 2023-04-20 02:31:19.000000 pyidevice-2.3.32.3/ios_device/servers/os_trace.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3163 2022-12-08 06:20:36.000000 pyidevice-2.3.32.3/ios_device/servers/pcapd.py
+-rwxr-xr-x   0 rongcloud   (501) staff       (20)     3102 2022-12-08 06:20:36.000000 pyidevice-2.3.32.3/ios_device/servers/screenshotr.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1083 2023-01-04 04:20:57.000000 pyidevice-2.3.32.3/ios_device/servers/simulate_location.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1596 2023-03-31 08:20:40.000000 pyidevice-2.3.32.3/ios_device/servers/spring_board.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3329 2023-01-04 03:41:43.000000 pyidevice-2.3.32.3/ios_device/servers/syslog.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      864 2023-04-17 09:44:17.000000 pyidevice-2.3.32.3/ios_device/servers/testmanagerd.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:53:19.328915 pyidevice-2.3.32.3/ios_device/util/
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1860 2022-09-26 09:47:22.000000 pyidevice-2.3.32.3/ios_device/util/__init__.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11825 2022-12-08 06:20:36.000000 pyidevice-2.3.32.3/ios_device/util/api_util.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    24888 2022-12-08 06:30:13.000000 pyidevice-2.3.32.3/ios_device/util/bpylist2.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4657 2022-09-26 09:47:22.000000 pyidevice-2.3.32.3/ios_device/util/ca.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4585 2022-09-26 09:47:22.000000 pyidevice-2.3.32.3/ios_device/util/constants.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7921 2022-12-08 06:20:36.000000 pyidevice-2.3.32.3/ios_device/util/dtx_msg.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     1842 2022-09-26 09:47:22.000000 pyidevice-2.3.32.3/ios_device/util/exceptions.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3907 2022-09-26 09:47:22.000000 pyidevice-2.3.32.3/ios_device/util/forward.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     7443 2023-01-04 06:39:27.000000 pyidevice-2.3.32.3/ios_device/util/gpu_decode.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)   109555 2023-04-07 02:39:15.000000 pyidevice-2.3.32.3/ios_device/util/kc_data.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    41845 2023-04-07 02:39:15.000000 pyidevice-2.3.32.3/ios_device/util/kperf_data.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    16216 2023-04-07 02:39:15.000000 pyidevice-2.3.32.3/ios_device/util/lifecycle.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    16285 2023-04-20 02:30:51.000000 pyidevice-2.3.32.3/ios_device/util/lockdown.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     3131 2022-12-08 06:20:36.000000 pyidevice-2.3.32.3/ios_device/util/plist_service.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    27335 2023-04-26 02:45:02.000000 pyidevice-2.3.32.3/ios_device/util/plistlib.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)    12592 2023-03-31 09:19:13.000000 pyidevice-2.3.32.3/ios_device/util/usbmux.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     9513 2023-02-09 09:51:53.000000 pyidevice-2.3.32.3/ios_device/util/utils.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)     4261 2023-02-14 02:46:09.000000 pyidevice-2.3.32.3/ios_device/util/variables.py
+drwxr-xr-x   0 rongcloud   (501) staff       (20)        0 2023-05-24 02:53:19.329697 pyidevice-2.3.32.3/pyidevice.egg-info/
+-rw-r--r--   0 rongcloud   (501) staff       (20)    11371 2023-05-24 02:53:19.000000 pyidevice-2.3.32.3/pyidevice.egg-info/PKG-INFO
+-rw-r--r--   0 rongcloud   (501) staff       (20)     2486 2023-05-24 02:53:19.000000 pyidevice-2.3.32.3/pyidevice.egg-info/SOURCES.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)        1 2023-05-24 02:53:19.000000 pyidevice-2.3.32.3/pyidevice.egg-info/dependency_links.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       50 2023-05-24 02:53:19.000000 pyidevice-2.3.32.3/pyidevice.egg-info/entry_points.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)      141 2023-05-24 02:53:19.000000 pyidevice-2.3.32.3/pyidevice.egg-info/requires.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       10 2023-05-24 02:53:19.000000 pyidevice-2.3.32.3/pyidevice.egg-info/top_level.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)      140 2023-04-07 02:39:15.000000 pyidevice-2.3.32.3/requirements.txt
+-rw-r--r--   0 rongcloud   (501) staff       (20)       38 2023-05-24 02:53:19.330245 pyidevice-2.3.32.3/setup.cfg
+-rw-r--r--   0 rongcloud   (501) staff       (20)      976 2023-04-07 02:35:34.000000 pyidevice-2.3.32.3/setup.py
+-rw-r--r--   0 rongcloud   (501) staff       (20)      958 2023-05-24 02:53:19.000000 pyidevice-2.3.32.3/setup2.py
```

### Comparing `pyidevice-2.3.32.2/LICENSE` & `pyidevice-2.3.32.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/PKG-INFO` & `pyidevice-2.3.32.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyidevice
-Version: 2.3.32.2
+Version: 2.3.32.3
 Summary: Get ios data and operate ios devices
 Home-page: https://github.com/YueChen-C/py-ios-device
 Author: chenpeijie
 Author-email: cpjsf@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyidevice-2.3.32.2/README.md` & `pyidevice-2.3.32.3/README.md`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/afc.py` & `pyidevice-2.3.32.3/demo/afc.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/crash_log.py` & `pyidevice-2.3.32.3/demo/crash_log.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/installation_proxy.py` & `pyidevice-2.3.32.3/demo/installation_proxy.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/instrument_demo/activity.py` & `pyidevice-2.3.32.3/demo/instrument_demo/activity.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/instrument_demo/app_lifecycle.py` & `pyidevice-2.3.32.3/demo/instrument_demo/app_lifecycle.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/instrument_demo/applictionListing.py` & `pyidevice-2.3.32.3/demo/instrument_demo/applictionListing.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/instrument_demo/coreprofilesessiontap.py` & `pyidevice-2.3.32.3/demo/instrument_demo/coreprofilesessiontap.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/instrument_demo/coreprofilesessiontap_parse.py` & `pyidevice-2.3.32.3/demo/instrument_demo/coreprofilesessiontap_parse.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/instrument_demo/deviceinfo.py` & `pyidevice-2.3.32.3/demo/instrument_demo/deviceinfo.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/instrument_demo/gpu.py` & `pyidevice-2.3.32.3/demo/instrument_demo/gpu.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/instrument_demo/graphics.py` & `pyidevice-2.3.32.3/demo/instrument_demo/graphics.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/instrument_demo/launchAPP.py` & `pyidevice-2.3.32.3/demo/instrument_demo/launchAPP.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/instrument_demo/mobileNotifications.py` & `pyidevice-2.3.32.3/demo/instrument_demo/mobileNotifications.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/instrument_demo/netstatPID.py` & `pyidevice-2.3.32.3/demo/instrument_demo/netstatPID.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/instrument_demo/networking.py` & `pyidevice-2.3.32.3/demo/instrument_demo/networking.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/instrument_demo/sysmontap.py` & `pyidevice-2.3.32.3/demo/instrument_demo/sysmontap.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/instrument_demo/xcuitest.py` & `pyidevice-2.3.32.3/demo/instrument_demo/xcuitest.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/mobile_config.py` & `pyidevice-2.3.32.3/demo/mobile_config.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/pcapd.py` & `pyidevice-2.3.32.3/demo/pcapd.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/screenshotr.py` & `pyidevice-2.3.32.3/demo/screenshotr.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/demo/syslog.py` & `pyidevice-2.3.32.3/demo/syslog.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/cli/base.py` & `pyidevice-2.3.32.3/ios_device/cli/base.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/cli/cli.py` & `pyidevice-2.3.32.3/ios_device/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/cli/instruments.py` & `pyidevice-2.3.32.3/ios_device/cli/instruments.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/cli/mobile.py` & `pyidevice-2.3.32.3/ios_device/cli/mobile.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/py_ios_device.py` & `pyidevice-2.3.32.3/ios_device/py_ios_device.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/servers/Installation.py` & `pyidevice-2.3.32.3/ios_device/servers/Installation.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/servers/Instrument.py` & `pyidevice-2.3.32.3/ios_device/servers/Instrument.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/servers/afc.py` & `pyidevice-2.3.32.3/ios_device/servers/afc.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/servers/amfi.py` & `pyidevice-2.3.32.3/ios_device/servers/amfi.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/servers/crash_log.py` & `pyidevice-2.3.32.3/ios_device/servers/crash_log.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/servers/diagnostics_relay.py` & `pyidevice-2.3.32.3/ios_device/servers/diagnostics_relay.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/servers/dvt.py` & `pyidevice-2.3.32.3/ios_device/servers/dvt.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/servers/house_arrest.py` & `pyidevice-2.3.32.3/ios_device/servers/house_arrest.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/servers/image_mounter.py` & `pyidevice-2.3.32.3/ios_device/servers/image_mounter.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/servers/mc_install.py` & `pyidevice-2.3.32.3/ios_device/servers/mc_install.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/servers/notification_proxy.py` & `pyidevice-2.3.32.3/ios_device/servers/notification_proxy.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/servers/os_trace.py` & `pyidevice-2.3.32.3/ios_device/servers/os_trace.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/servers/pcapd.py` & `pyidevice-2.3.32.3/ios_device/servers/pcapd.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/servers/screenshotr.py` & `pyidevice-2.3.32.3/ios_device/servers/screenshotr.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/servers/simulate_location.py` & `pyidevice-2.3.32.3/ios_device/servers/simulate_location.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/servers/spring_board.py` & `pyidevice-2.3.32.3/ios_device/servers/spring_board.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/servers/syslog.py` & `pyidevice-2.3.32.3/ios_device/servers/syslog.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/servers/testmanagerd.py` & `pyidevice-2.3.32.3/ios_device/servers/testmanagerd.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/util/__init__.py` & `pyidevice-2.3.32.3/ios_device/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/util/api_util.py` & `pyidevice-2.3.32.3/ios_device/util/api_util.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/util/bpylist2.py` & `pyidevice-2.3.32.3/ios_device/util/bpylist2.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/util/ca.py` & `pyidevice-2.3.32.3/ios_device/util/ca.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/util/constants.py` & `pyidevice-2.3.32.3/ios_device/util/constants.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/util/dtx_msg.py` & `pyidevice-2.3.32.3/ios_device/util/dtx_msg.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/util/exceptions.py` & `pyidevice-2.3.32.3/ios_device/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/util/forward.py` & `pyidevice-2.3.32.3/ios_device/util/forward.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/util/gpu_decode.py` & `pyidevice-2.3.32.3/ios_device/util/gpu_decode.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/util/kc_data.py` & `pyidevice-2.3.32.3/ios_device/util/kc_data.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/util/kperf_data.py` & `pyidevice-2.3.32.3/ios_device/util/kperf_data.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/util/lifecycle.py` & `pyidevice-2.3.32.3/ios_device/util/lifecycle.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/util/lockdown.py` & `pyidevice-2.3.32.3/ios_device/util/lockdown.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/util/plist_service.py` & `pyidevice-2.3.32.3/ios_device/util/plist_service.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/util/plistlib.py` & `pyidevice-2.3.32.3/ios_device/util/plistlib.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/util/usbmux.py` & `pyidevice-2.3.32.3/ios_device/util/usbmux.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/util/utils.py` & `pyidevice-2.3.32.3/ios_device/util/utils.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/ios_device/util/variables.py` & `pyidevice-2.3.32.3/ios_device/util/variables.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/pyidevice.egg-info/PKG-INFO` & `pyidevice-2.3.32.3/pyidevice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyidevice
-Version: 2.3.32.2
+Version: 2.3.32.3
 Summary: Get ios data and operate ios devices
 Home-page: https://github.com/YueChen-C/py-ios-device
 Author: chenpeijie
 Author-email: cpjsf@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyidevice-2.3.32.2/pyidevice.egg-info/SOURCES.txt` & `pyidevice-2.3.32.3/pyidevice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/setup.py` & `pyidevice-2.3.32.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyidevice-2.3.32.2/setup2.py` & `pyidevice-2.3.32.3/setup2.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,11 +23,11 @@
       python_requires=">=3.7",
       classifiers=[
           "Programming Language :: Python :: 3",
           "Operating System :: OS Independent",
       ],
       entry_points={
           'console_scripts':{
-              'pyidevice=ios_device.main:cli'
+              'pyidevice=pyidevice.main:cli'
           }
       },
 )
```

