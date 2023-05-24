# Comparing `tmp/aio_dt_protocol-0.9.5.tar.gz` & `tmp/aio_dt_protocol-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_dt_protocol-0.9.5.tar", last modified: Fri May 19 17:25:15 2023, max compression
+gzip compressed data, was "aio_dt_protocol-1.0.0.tar", last modified: Wed May 24 15:40:18 2023, max compression
```

## Comparing `aio_dt_protocol-0.9.5.tar` & `aio_dt_protocol-1.0.0.tar`

### file list

```diff
@@ -1,41 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 17:25:15.055277 aio_dt_protocol-0.9.5/
--rw-rw-rw-   0        0        0     1526 2023-04-05 18:37:56.000000 aio_dt_protocol-0.9.5/LICENSE
--rw-rw-rw-   0        0        0     6559 2023-05-19 17:25:15.056277 aio_dt_protocol-0.9.5/PKG-INFO
--rw-rw-rw-   0        0        0     5815 2023-04-06 13:39:16.000000 aio_dt_protocol-0.9.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 17:25:14.839353 aio_dt_protocol-0.9.5/aio_dt_protocol/
--rw-rw-rw-   0        0        0    34959 2023-04-05 07:22:52.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/Actions.py
--rw-rw-rw-   0        0        0    50180 2023-05-19 08:54:16.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/Browser.py
--rw-rw-rw-   0        0        0     9971 2023-04-04 10:33:45.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/BrowserEx.py
--rw-rw-rw-   0        0        0    35317 2023-04-05 07:22:52.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/DOMElement.py
--rw-rw-rw-   0        0        0    32529 2023-04-05 17:29:55.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/Data.py
--rw-rw-rw-   0        0        0    22749 2023-04-06 07:01:02.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/Page.py
--rw-rw-rw-   0        0        0    10249 2023-05-19 09:09:36.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/PageEx.py
--rw-rw-rw-   0        0        0      363 2023-05-19 08:54:16.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 17:25:15.055277 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/
--rw-rw-rw-   0        0        0     3631 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/BackgroundService.py
--rw-rw-rw-   0        0        0    13809 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Browser.py
--rw-rw-rw-   0        0        0     7070 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/CSS.py
--rw-rw-rw-   0        0        0     2045 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Console.py
--rw-rw-rw-   0        0        0    16735 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/DOM.py
--rw-rw-rw-   0        0        0     1846 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/DeviceOrientation.py
--rw-rw-rw-   0        0        0    24645 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Emulation.py
--rw-rw-rw-   0        0        0    23665 2023-05-19 15:17:07.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Fetch.py
--rw-rw-rw-   0        0        0     2066 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Log.py
--rw-rw-rw-   0        0        0    22099 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Network.py
--rw-rw-rw-   0        0        0     2124 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Overlay.py
--rw-rw-rw-   0        0        0    35374 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Page.py
--rw-rw-rw-   0        0        0    32897 2023-04-05 17:56:11.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Runtime.py
--rw-rw-rw-   0        0        0     1712 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/SystemInfo.py
--rw-rw-rw-   0        0        0    17569 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Target.py
--rw-rw-rw-   0        0        0        0 2021-06-02 19:57:07.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/domains/__init__.py
--rw-rw-rw-   0        0        0     3409 2023-05-19 09:15:55.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/exceptions.py
--rw-rw-rw-   0        0        0     5156 2023-05-19 08:54:16.000000 aio_dt_protocol-0.9.5/aio_dt_protocol/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-19 17:25:14.844352 aio_dt_protocol-0.9.5/aio_dt_protocol.egg-info/
--rw-rw-rw-   0        0        0     6559 2023-05-19 17:25:14.000000 aio_dt_protocol-0.9.5/aio_dt_protocol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1083 2023-05-19 17:25:14.000000 aio_dt_protocol-0.9.5/aio_dt_protocol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 17:25:14.000000 aio_dt_protocol-0.9.5/aio_dt_protocol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-19 17:25:14.000000 aio_dt_protocol-0.9.5/aio_dt_protocol.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-19 17:25:14.000000 aio_dt_protocol-0.9.5/aio_dt_protocol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-04-06 10:50:43.000000 aio_dt_protocol-0.9.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 17:25:15.057276 aio_dt_protocol-0.9.5/setup.cfg
--rw-rw-rw-   0        0        0     1503 2023-04-06 10:09:07.000000 aio_dt_protocol-0.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:40:18.121229 aio_dt_protocol-1.0.0/
+-rw-rw-rw-   0        0        0     1526 2023-04-05 18:37:56.000000 aio_dt_protocol-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     6496 2023-05-24 15:40:18.122228 aio_dt_protocol-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5752 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 15:40:18.051253 aio_dt_protocol-1.0.0/aio_dt_protocol/
+-rw-rw-rw-   0        0        0      369 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/__init__.py
+-rw-rw-rw-   0        0        0    10780 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/actions.py
+-rw-rw-rw-   0        0        0    56871 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/browser.py
+-rw-rw-rw-   0        0        0    22851 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/connection.py
+-rw-rw-rw-   0        0        0    25804 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/data.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:40:18.074246 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/
+-rw-rw-rw-   0        0        0        0 2021-06-02 19:57:07.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:40:18.077245 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/background_service/
+-rw-rw-rw-   0        0        0      107 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/background_service/__init__.py
+-rw-rw-rw-   0        0        0     3279 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/background_service/background_service.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/background_service/types.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:40:18.080243 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/browser/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/browser/__init__.py
+-rw-rw-rw-   0        0        0    13585 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/browser/browser.py
+-rw-rw-rw-   0        0        0     1346 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/browser/types.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:40:18.083242 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/css/
+-rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/css/__init__.py
+-rw-rw-rw-   0        0        0     6353 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/css/css.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/css/types.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:40:18.086241 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/device_orientation/
+-rw-rw-rw-   0        0        0       51 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/device_orientation/__init__.py
+-rw-rw-rw-   0        0        0     1455 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/device_orientation/device_orientation.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/device_orientation/types.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:40:18.090239 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/dom/
+-rw-rw-rw-   0        0        0       80 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/dom/__init__.py
+-rw-rw-rw-   0        0        0    16508 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/dom/dom.py
+-rw-rw-rw-   0        0        0    35576 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/dom/dom_element.py
+-rw-rw-rw-   0        0        0      798 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/dom/types.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:40:18.093238 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/emulation/
+-rw-rw-rw-   0        0        0       73 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/emulation/__init__.py
+-rw-rw-rw-   0        0        0    24489 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/emulation/emulation.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/emulation/types.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:40:18.096237 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/fetch/
+-rw-rw-rw-   0        0        0       57 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/fetch/__init__.py
+-rw-rw-rw-   0        0        0    17264 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/fetch/fetch.py
+-rw-rw-rw-   0        0        0     5210 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/fetch/types.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:40:18.099236 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/input/
+-rw-rw-rw-   0        0        0       26 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/input/__init__.py
+-rw-rw-rw-   0        0        0    23645 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/input/input.py
+-rw-rw-rw-   0        0        0     2778 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/input/types.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:40:18.102235 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/log/
+-rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/log/__init__.py
+-rw-rw-rw-   0        0        0     1701 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/log/log.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/log/types.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:40:18.105235 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/network/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/network/__init__.py
+-rw-rw-rw-   0        0        0    18941 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/network/network.py
+-rw-rw-rw-   0        0        0     3522 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/network/types.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:40:18.109233 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/overlay/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/overlay/__init__.py
+-rw-rw-rw-   0        0        0     1731 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/overlay/overlay.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/overlay/types.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:40:18.111232 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/page/
+-rw-rw-rw-   0        0        0       53 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/page/__init__.py
+-rw-rw-rw-   0        0        0    33541 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/page/page.py
+-rw-rw-rw-   0        0        0     3104 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/page/types.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:40:18.114231 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/runtime/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/runtime/__init__.py
+-rw-rw-rw-   0        0        0    23769 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/runtime/runtime.py
+-rw-rw-rw-   0        0        0     7629 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/runtime/types.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:40:18.118229 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/system_info/
+-rw-rw-rw-   0        0        0       37 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/system_info/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/system_info/system_info.py
+-rw-rw-rw-   0        0        0      784 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/system_info/types.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:40:18.121229 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/target/
+-rw-rw-rw-   0        0        0       61 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/target/__init__.py
+-rw-rw-rw-   0        0        0    17276 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/target/target.py
+-rw-rw-rw-   0        0        0      408 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/domains/target/types.py
+-rw-rw-rw-   0        0        0     3409 2023-05-19 09:15:55.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/exceptions.py
+-rw-rw-rw-   0        0        0     7275 2023-05-24 15:34:41.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/extend_connection.py
+-rw-rw-rw-   0        0        0     5156 2023-05-19 08:54:16.000000 aio_dt_protocol-1.0.0/aio_dt_protocol/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:40:18.073246 aio_dt_protocol-1.0.0/aio_dt_protocol.egg-info/
+-rw-rw-rw-   0        0        0     6496 2023-05-24 15:40:17.000000 aio_dt_protocol-1.0.0/aio_dt_protocol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2504 2023-05-24 15:40:17.000000 aio_dt_protocol-1.0.0/aio_dt_protocol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 15:40:17.000000 aio_dt_protocol-1.0.0/aio_dt_protocol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-24 15:40:17.000000 aio_dt_protocol-1.0.0/aio_dt_protocol.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-24 15:40:17.000000 aio_dt_protocol-1.0.0/aio_dt_protocol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-04-06 10:50:43.000000 aio_dt_protocol-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 15:40:18.122228 aio_dt_protocol-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1503 2023-04-06 10:09:07.000000 aio_dt_protocol-1.0.0/setup.py
```

### Comparing `aio_dt_protocol-0.9.5/LICENSE` & `aio_dt_protocol-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.5/PKG-INFO` & `aio_dt_protocol-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio_dt_protocol
-Version: 0.9.5
+Version: 1.0.0
 Summary: Asynchronous wrapper over Chromium browser debugger protocol.
 Home-page: https://github.com/PieceOfGood/aio_dt_protocol
 Author: PieceOfGood
 Author-email: 78sanchezz@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
@@ -30,17 +30,17 @@
 И так как всё общение через протокол основано на формате JSON, по желанию можно установить ujson:
 https://github.com/ultrajson/ultrajson
 
 ### Примеры:
 
 ```python
 import asyncio
-from aio_dt_protocol import BrowserEx as Browser
+from aio_dt_protocol import Browser
 from aio_dt_protocol import find_instances
-from aio_dt_protocol.Data import KeyEvents
+from aio_dt_protocol.data import KeyEvents
 
 DEBUG_PORT: int = 9222
 BROWSER_NAME: str = "chrome"
 
 
 async def main() -> None:
     # ? Если на указанном порту есть запущенный браузер, происходит подключение.
@@ -56,42 +56,42 @@
         msg = f"[- LAUNCH NEW BROWSER ON {DEBUG_PORT} PORT -]"
     print(msg)
 
     # ? Будет печатать в консоль всё, что приходит по соединению со страницей.
     # ? Полезно при разработке.
     # async def action_printer(data: dict) -> None:
     #     print(data)
-    # page = await browser.GetPage(callback=action_printer)
-    page = await browser.GetPage()
+    # conn = await browser.getPage(callback=action_printer)
+    conn = await browser.getPage()
 
     print("[- GO TO GOOGLE ... -]")
-    await page.Navigate("https://www.google.com")
+    await conn.Page.navigate("https://www.google.com")
 
-    input_node = await page.QuerySelector("input")
-    await input_node.Click()
+    input_node = await conn.DOM.querySelector("input")
+    await input_node.click()
     await asyncio.sleep(1)
-    await page.action.InsertText("github PieceOfGood")
+    await conn.extend.action.insertText("github PieceOfGood")
     await asyncio.sleep(1)
-    await page.action.SendKeyEvent(KeyEvents.enter)
+    await conn.extend.action.sendKeyEvent(KeyEvents.enter)
     await asyncio.sleep(1)
 
     submit_button_selector = "div:not([jsname])>center>[type=submit]:not([jsaction])"
 
-    submit_button = await page.QuerySelector(submit_button_selector)
-    await submit_button.Click()
+    submit_button = await conn.DOM.querySelector(submit_button_selector)
+    await submit_button.click()
 
     # ? Или выполнить клик используя JS
     # click_code = f"""\
     # document.querySelector("{submit_button_selector}").click();
     # """
-    # await page.InjectJS(click_code)
+    # await conn.extend.injectJS(click_code)
 
     print("[- WAIT FOR CLOSE PAGE ... -]")
     # ? Пока соединение существует, цикл выполняется.
-    await page.WaitForClose()
+    await conn.waitForClose()
     print("[- DONE -]")
 
 
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
@@ -114,55 +114,59 @@
                  func_name: "test_func",
                  args: [1, "test"]
             }))
         });
     </script>
     </html>"""
 
-    # ? number и text будут переданы из браузера, а bind_arg указан при регистрации
-    async def test_func(number: int, text: str, bind_arg: dict) -> None:
-        print(f"[- test_func -] Called with args:\n\tnumber: {number}\n\ttext: {text}\n\tbing_arg: {bind_arg}")
-
-    await page.AddListener(
-        test_func,                          # ! слушатель
-        {"name": "test", "value": True}     # ! bind_arg
-    )
 
-    # ? Если ожидается внушительный функционал прикрутить к странице, то это можно
-    # ? сделать за один раз.
-    # await page.AddListeners(
-    #     (test_func, [ {"name": "test", "value": True} ]),
-    #     # (any_awaitable1, [1, 2, 3])
-    #     # (any_awaitable2, [])
-    # )
+# ? number и text будут переданы из браузера, а bind_arg указан при регистрации
+async def test_func(number: int, text: str, bind_arg: dict) -> None:
+    print(f"[- test_func -] Called with args:\n\tnumber: {number}\n\ttext: {text}\n\tbing_arg: {bind_arg}")
+
+
+await conn.addListener(
+    test_func,  # ! слушатель
+    {"name": "test", "value": True}  # ! bind_arg
+)
+
+# ? Если ожидается внушительный функционал прикрутить к странице, то это можно
+# ? сделать за один раз.
+# await conn.addListeners(
+#     (test_func, [ {"name": "test", "value": True} ]),
+#     # (any_awaitable1, [1, 2, 3])
+#     # (any_awaitable2, [])
+# )
 
-    await page.Navigate(html)
+await conn.Page.navigate(html)
 ```
 ### Headless
 Чтобы запустить браузер в `безголовом` режиме, нужно передать аргументу принимающему путь к папке профиля пустую строку.
+
 ```python
 import asyncio
-from aio_dt_protocol import BrowserEx as Browser
+from aio_dt_protocol import Browser
 from aio_dt_protocol.utils import save_img_as, async_util_call
 
 
 async def main() -> None:
     print("[- HEADLESS RUN -]")
     browser = Browser(profile_path="")
     print("[- WAITING PAGE -]")
-    page = await browser.WaitFirstTab()
+    conn = await browser.waitFirstTab()
     print("[- GO TO GOOGLE -]")
-    await page.Navigate("https://www.google.com")
-    
+    await conn.Page.navigate("https://www.google.com")
+
     print("[- MAKE SCREENSHOT -]")
     await async_util_call(
-        save_img_as, "google.png", await page.MakeScreenshot()
+        save_img_as, "google.png", await conn.Page.makeScreenshot()
     )
-    
+
     print("[- CLOSE BROWSER -]")
-    await page.CloseBrowser()
+    await conn.Browser.close()
     print("[- DONE -]")
 
+
 if __name__ == '__main__':
     asyncio.run(main())
 
 ```
```

### Comparing `aio_dt_protocol-0.9.5/README.md` & `aio_dt_protocol-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 И так как всё общение через протокол основано на формате JSON, по желанию можно установить ujson:
 https://github.com/ultrajson/ultrajson
 
 ### Примеры:
 
 ```python
 import asyncio
-from aio_dt_protocol import BrowserEx as Browser
+from aio_dt_protocol import Browser
 from aio_dt_protocol import find_instances
-from aio_dt_protocol.Data import KeyEvents
+from aio_dt_protocol.data import KeyEvents
 
 DEBUG_PORT: int = 9222
 BROWSER_NAME: str = "chrome"
 
 
 async def main() -> None:
     # ? Если на указанном порту есть запущенный браузер, происходит подключение.
@@ -37,42 +37,42 @@
         msg = f"[- LAUNCH NEW BROWSER ON {DEBUG_PORT} PORT -]"
     print(msg)
 
     # ? Будет печатать в консоль всё, что приходит по соединению со страницей.
     # ? Полезно при разработке.
     # async def action_printer(data: dict) -> None:
     #     print(data)
-    # page = await browser.GetPage(callback=action_printer)
-    page = await browser.GetPage()
+    # conn = await browser.getPage(callback=action_printer)
+    conn = await browser.getPage()
 
     print("[- GO TO GOOGLE ... -]")
-    await page.Navigate("https://www.google.com")
+    await conn.Page.navigate("https://www.google.com")
 
-    input_node = await page.QuerySelector("input")
-    await input_node.Click()
+    input_node = await conn.DOM.querySelector("input")
+    await input_node.click()
     await asyncio.sleep(1)
-    await page.action.InsertText("github PieceOfGood")
+    await conn.extend.action.insertText("github PieceOfGood")
     await asyncio.sleep(1)
-    await page.action.SendKeyEvent(KeyEvents.enter)
+    await conn.extend.action.sendKeyEvent(KeyEvents.enter)
     await asyncio.sleep(1)
 
     submit_button_selector = "div:not([jsname])>center>[type=submit]:not([jsaction])"
 
-    submit_button = await page.QuerySelector(submit_button_selector)
-    await submit_button.Click()
+    submit_button = await conn.DOM.querySelector(submit_button_selector)
+    await submit_button.click()
 
     # ? Или выполнить клик используя JS
     # click_code = f"""\
     # document.querySelector("{submit_button_selector}").click();
     # """
-    # await page.InjectJS(click_code)
+    # await conn.extend.injectJS(click_code)
 
     print("[- WAIT FOR CLOSE PAGE ... -]")
     # ? Пока соединение существует, цикл выполняется.
-    await page.WaitForClose()
+    await conn.waitForClose()
     print("[- DONE -]")
 
 
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
@@ -95,55 +95,59 @@
                  func_name: "test_func",
                  args: [1, "test"]
             }))
         });
     </script>
     </html>"""
 
-    # ? number и text будут переданы из браузера, а bind_arg указан при регистрации
-    async def test_func(number: int, text: str, bind_arg: dict) -> None:
-        print(f"[- test_func -] Called with args:\n\tnumber: {number}\n\ttext: {text}\n\tbing_arg: {bind_arg}")
-
-    await page.AddListener(
-        test_func,                          # ! слушатель
-        {"name": "test", "value": True}     # ! bind_arg
-    )
 
-    # ? Если ожидается внушительный функционал прикрутить к странице, то это можно
-    # ? сделать за один раз.
-    # await page.AddListeners(
-    #     (test_func, [ {"name": "test", "value": True} ]),
-    #     # (any_awaitable1, [1, 2, 3])
-    #     # (any_awaitable2, [])
-    # )
+# ? number и text будут переданы из браузера, а bind_arg указан при регистрации
+async def test_func(number: int, text: str, bind_arg: dict) -> None:
+    print(f"[- test_func -] Called with args:\n\tnumber: {number}\n\ttext: {text}\n\tbing_arg: {bind_arg}")
+
+
+await conn.addListener(
+    test_func,  # ! слушатель
+    {"name": "test", "value": True}  # ! bind_arg
+)
+
+# ? Если ожидается внушительный функционал прикрутить к странице, то это можно
+# ? сделать за один раз.
+# await conn.addListeners(
+#     (test_func, [ {"name": "test", "value": True} ]),
+#     # (any_awaitable1, [1, 2, 3])
+#     # (any_awaitable2, [])
+# )
 
-    await page.Navigate(html)
+await conn.Page.navigate(html)
 ```
 ### Headless
 Чтобы запустить браузер в `безголовом` режиме, нужно передать аргументу принимающему путь к папке профиля пустую строку.
+
 ```python
 import asyncio
-from aio_dt_protocol import BrowserEx as Browser
+from aio_dt_protocol import Browser
 from aio_dt_protocol.utils import save_img_as, async_util_call
 
 
 async def main() -> None:
     print("[- HEADLESS RUN -]")
     browser = Browser(profile_path="")
     print("[- WAITING PAGE -]")
-    page = await browser.WaitFirstTab()
+    conn = await browser.waitFirstTab()
     print("[- GO TO GOOGLE -]")
-    await page.Navigate("https://www.google.com")
-    
+    await conn.Page.navigate("https://www.google.com")
+
     print("[- MAKE SCREENSHOT -]")
     await async_util_call(
-        save_img_as, "google.png", await page.MakeScreenshot()
+        save_img_as, "google.png", await conn.Page.makeScreenshot()
     )
-    
+
     print("[- CLOSE BROWSER -]")
-    await page.CloseBrowser()
+    await conn.Browser.close()
     print("[- DONE -]")
 
+
 if __name__ == '__main__':
     asyncio.run(main())
 
 ```
```

### Comparing `aio_dt_protocol-0.9.5/aio_dt_protocol/Actions.py` & `aio_dt_protocol-1.0.0/aio_dt_protocol/domains/input/input.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import time
-import asyncio
-import random
-from typing import Tuple, List, Optional, Literal
-from .Data import WINDOWS_KEY_SET, WindowBounds, TouchPoint, KeyModifiers, KeyEvents
+from .types import TouchPoint
+from typing import Optional, List, Literal
 
 
-class Actions:
-    def __init__(self, page_instance):
-        self.page_instance = page_instance
+class Input:
+    """
+    #   https://chromedevtools.github.io/devtools-protocol/tot/Input
+    """
+    __slots__ = ("_connection",)
+
+    def __init__(self, conn) -> None:
 
+        from ...connection import Connection
+
+        self._connection: Connection = conn
 
 # region [ |>*<|=== Domains ===|>*<| ] Input [ |>*<|=== Domains ===|>*<| ]
-    #   https://chromedevtools.github.io/devtools-protocol/tot/Input
     #   https://godoc.org/github.com/unixpickle/muniverse/chrome
 
-    async def DispatchKeyEvent(
+    async def dispatchKeyEvent(
         self, type_: str,
         modifiers:             int = 0,
         timestamp:             Optional[int] = None,
         text:                  str = "",
         unmodifiedText:        str = "",
         keyIdentifier:         str = "",
         code:                  str = "",
@@ -73,17 +77,17 @@
             "autoRepeat": autoRepeat, "isKeypad": isKeypad, "isSystemKey": isSystemKey, "location": location,
             "commands": (commands if commands else [])
         }
         if timestamp is not None:
             args.update({"timestamp": timestamp})
         else:
             args.update({"timestamp": int(time.time() * 1000)})
-        await self.page_instance.Call("Input.dispatchKeyEvent", args)
+        await self._connection.call("Input.dispatchKeyEvent", args)
 
-    async def DispatchMouseEvent(
+    async def dispatchMouseEvent(
         self, type_: str, x: float, y: float,
         modifiers:            int = 0,
         timestamp:            Optional[int] = None,
         button:               str = "none",
         buttons:              int = 0,
         clickCount:           int = 1,
         force:              float = 0,
@@ -142,17 +146,17 @@
             "clickCount": clickCount, "force": force, "tangentialPressure": tangentialPressure, "tiltX": tiltX,
             "tiltY": tiltY, "twist": twist, "deltaX": deltaX, "deltaY": deltaY, "pointerType": pointerType
         }
         if timestamp is not None:
             args.update({"timestamp": timestamp})
         else:
             args.update({"timestamp": int(time.time() * 1000)})
-        await self.page_instance.Call("Input.dispatchMouseEvent", args)
+        await self._connection.call("Input.dispatchMouseEvent", args)
 
-    async def DispatchTouchEvent(
+    async def dispatchTouchEvent(
         self, type_: str,
         touchPoints: Optional[List[TouchPoint]] = None,
         modifiers:                int = 0,
         timestamp:                Optional[int] = None
     ) -> None:
         """
         Отправляет событие прикосновения на страницу.
@@ -175,28 +179,28 @@
             if len(touchPoints) == 0 or touchPoints is None:
                 raise ValueError(f"Для действия '{type_}', аргумент 'touchPoints' должен получить хотя-бы одну координату")
             args.update({"touchPoints": [point.to_dict() for point in touchPoints]})
 
         if timestamp is not None: args.update({"timestamp": timestamp})
         else: args.update({"timestamp": int(time.time() * 1000)})
 
-        await self.page_instance.Call("Input.dispatchTouchEvent", args)
+        await self._connection.call("Input.dispatchTouchEvent", args)
 
-    async def InsertText(self, text: str) -> None:
+    async def insertText(self, text: str) -> None:
         """
         (EXPERIMENTAL)
         Этот метод эмулирует вставку текста, который не поступает от нажатия клавиши, например,
             клавиатуры Emoji или IME.
         https://chromedevtools.github.io/devtools-protocol/tot/Input/#method-insertText
         :param text:                    Текст для вставки.
         :return:
         """
-        await self.page_instance.Call("Input.insertText", {"text": text})
+        await self._connection.call("Input.insertText", {"text": text})
 
-    async def SynthesizePinchGesture(
+    async def synthesizePinchGesture(
             self, x: float, y: float, scaleFactor: float,
                 relativeSpeed: Optional[int] = None,
             gestureSourceType: Optional[Literal["touch", "mouse"]] = None
     ) -> None:
         """
         (EXPERIMENTAL)
         Синтезирует жест щипка за период времени, генерируя соответствующие сенсорные события.
@@ -212,17 +216,17 @@
         :return:
         """
         args = {"x": x, "y": y, "scaleFactor": scaleFactor}
         if relativeSpeed is not None:
             args.update({"relativeSpeed": relativeSpeed})
         if gestureSourceType is not None:
             args.update({"gestureSourceType": gestureSourceType})
-        await self.page_instance.Call("Input.synthesizePinchGesture", args)
+        await self._connection.call("Input.synthesizePinchGesture", args)
 
-    async def SynthesizeScrollGesture(
+    async def synthesizeScrollGesture(
             self, x: float, y: float,
                       xDistance: Optional[float] = None,
                       yDistance: Optional[float] = None,
                     xOverscroll: Optional[float] = None,
                     yOverscroll: Optional[float] = None,
                     preventFling: Optional[bool] = None,
                             speed: Optional[int] = None,
@@ -271,17 +275,17 @@
             args.update({"gestureSourceType": gestureSourceType})
         if repeatCount is not None:
             args.update({"repeatCount": repeatCount})
         if repeatDelayMs is not None:
             args.update({"repeatDelayMs": repeatDelayMs})
         if interactionMarkerName is not None:
             args.update({"interactionMarkerName": interactionMarkerName})
-        await self.page_instance.Call("Input.synthesizeScrollGesture", args)
+        await self._connection.call("Input.synthesizeScrollGesture", args)
 
-    async def SynthesizeTapGesture(
+    async def synthesizeTapGesture(
             self, x: float, y: float,
             duration:          Optional[int] = None,
             tapCount:          Optional[int] = None,
             gestureSourceType: Optional[Literal["touch", "mouse"]] = None
     ) -> None:
         """
         (EXPERIMENTAL)
@@ -299,209 +303,10 @@
         args = {"x": x, "y": y}
         if duration is not None:
             args.update({"duration": duration})
         if tapCount is not None:
             args.update({"tapCount": tapCount})
         if gestureSourceType is not None:
             args.update({"gestureSourceType": gestureSourceType})
-        await self.page_instance.Call("Input.synthesizeTapGesture", args)
-
-    async def ActivateTarget(self, targetId: Optional[str] = None) -> None:
-        """
-        Активирует (создаёт фокус) "target".
-        https://chromedevtools.github.io/devtools-protocol/tot/Target#method-activateTarget
-        :param targetId:        Строка, представляющая идентификатор созданной страницы.
-        :return:
-        """
-        if targetId is None: targetId = self.page_instance.page_id
-        await self.page_instance.Call("Target.activateTarget", {"targetId": targetId})
-
-    async def BringToFront(self) -> None:
-        """
-        Выводит страницу на передний план (активирует вкладку).
-        https://chromedevtools.github.io/devtools-protocol/tot/Page#method-bringToFront
-        :return:
-        """
-        await self.page_instance.Call("Page.bringToFront")
+        await self._connection.call("Input.synthesizeTapGesture", args)
 
     # endregion
-
-    # ==================================================================================================================
-
-    async def SwipeTo(
-        self,
-        direction: Literal["up", "down", "left", "right"],
-        x:            float = 0,
-        y:            float = 0,
-        distance:     Optional[float] = None,
-        speed:        Optional[float] = None,
-        overscroll:   Optional[float] = None,
-        repeat_count:   Optional[int] = None,
-        repeat_delay: Optional[float] = None,
-        gestureSourceType: Literal["touch", "mouse"] = "mouse"
-    ) -> None:
-        """
-        Скроллит вьюпорт жестом "touch" на всю его длину/высоту.
-            Возвращает управление только после выполнения жеста!
-        :param direction:           (optional) Направление. Может быть следующим:
-                                        up — пальцем вверх(прокрутка вниз)
-                                        down — пальцем вниз(прокрутка вверх)
-                                        left — пальцем влево(прокрутка вправо)
-                                        right — пальцем вправо(прокрутка влево)
-        :param x:                   (optional) X-координата начальной точки.
-        :param y:                   (optional) Y-координата начальной точки.
-        :param distance:            (optional) Дистанция движения.
-        :param speed:               (optional) Скорость движения(по умолчанию = 800).
-        :param overscroll:          (optional) Дополнительная дистанция в пикселях.
-        :param repeat_count:        (optional) Кол-во повторений сделанного жеста.
-        :param repeat_delay:        (optional) Задержка между повторениями.
-        :param gestureSourceType:   (optional) Задержка между повторениями.
-        :return:
-        """
-        if direction not in ["up", "down", "left", "right"]:
-            raise ValueError("'direction' must be one from — up; down; left; right")
-        sign = -1 if direction in ["up", "left"] else 1
-        rect = None
-        if x is None:
-            rect = await self.page_instance.GetViewportRect()
-            x = 10 if direction == "right" else rect.width - 10 if direction == "left" else rect.height / 2
-
-        if y is None:
-            rect = await self.page_instance.GetViewportRect()
-            y = 10 if direction == "down" else rect.height - 10 if direction == "up" else rect.width / 2
-
-        if distance is None:
-            rect = rect or await self.page_instance.GetViewportRect()
-            distance = (rect.height if direction in ["up", "down"] else rect.width) - 10
-
-        overscroll = overscroll if overscroll is not None else 0
-
-        args = {
-            "x": x, "y": y, "speed": speed, "repeatCount": repeat_count,
-            "repeatDelayMs": repeat_delay, "gestureSourceType": gestureSourceType,
-            "xDistance": distance * sign if direction in ["left", "right"] else None,
-            "yDistance": distance * sign if direction in ["up", "down"] else None,
-            "xOverscroll": overscroll * -sign if direction in ["left", "right"] else None,
-            "yOverscroll": overscroll * -sign if direction in ["up", "down"] else None,
-        }
-        await self.SynthesizeScrollGesture(**args)
-
-    async def ClickTo(self, x: int, y: int, delay: float = None) -> None:
-        """
-        Эмулирует клик мыши по координатам.
-        :param x:               x - координата
-        :param y:               y - координата
-        :param delay:           задержка перед отпусканием
-        :return:
-        """
-        await self.DispatchMouseEvent("mousePressed", x, y, button="left")
-        if delay: await asyncio.sleep(delay)
-        await self.DispatchMouseEvent("mouseReleased", x, y, button="left")
-
-    async def MouseMoveTo(self, x: int, y: int) -> None:
-        await self.DispatchMouseEvent("mouseMoved", x, y)
-
-    async def MouseWheel(self, x: float, y: float, deltaX: float = 0, deltaY: float = 0) -> None:
-        """
-        Крутит колесо мышки.
-        :param x:               Положение
-        :param y:               указателя мыши.
-        :param deltaX:          Скроллит по-горизонтали.
-        :param deltaY:          Скроллит по-вертикали, положительное значение == вниз.
-        :return:
-        """
-        await self.DispatchMouseEvent("mouseWheel", x, y, button="middle", deltaX=deltaX, deltaY=deltaY)
-
-    async def WheelTo(self, direction: str = "down") -> None:
-        sign = -1 if direction in ["up", "left"] else 1
-        rect = await self.page_instance.GetViewportRect()
-        x = 10 if direction == "right" else rect.width - 10 if direction == "left" else rect.height / 2
-        y = 10 if direction == "down" else rect.height - 10 if direction == "up" else rect.width / 2
-        distance = ((rect.height if direction in ["up", "down"] else rect.width) - 10) * sign
-        delta = {"deltaX": distance} if direction in ["left", "rigth"] else {"deltaY": distance}
-        await self.MouseWheel(x, y, **delta)
-
-
-    async def MouseMoveToCoordinatesAndClick(self, x: int, y: int) -> None:
-        await self.MouseMoveTo(x, y)
-        await self.ClickTo(x, y)
-
-    async def SendChar(self, char: str) -> None:
-        """
-        Эмулирует ввод символа нажатием соответствующей кнопки клавиатуры.
-            Внимание! Курсор должен быть установлен в эдит-боксе!
-        :param char:             Символ для ввода.
-        :return:
-        """
-        upper_key = char.upper()
-        args = {
-            "text": char, "key": char, "keyIdentifier": f"U+{WINDOWS_KEY_SET[upper_key]:X}",
-            "windowsVirtualKeyCode": WINDOWS_KEY_SET[upper_key],
-            "nativeVirtualKeyCode": WINDOWS_KEY_SET[upper_key]
-        }
-        if len(char) > 1: raise ValueError(f"Передаваемая строка: '{char}' — должна быть из одного символа!")
-        await self.DispatchKeyEvent("char", **args)
-
-    async def SendText(
-            self, text: str, interval: Optional[Tuple[float, float]] = None
-    ) -> None:
-        """
-        Эмулирует последовательный набор текста.
-            Внимание! Курсор должен быть установлен в эдит-боксе!
-        :param text:             Последовательность символов для ввода.
-        :param interval:         Задержка после нажатия кнопки. None - отключает задержку.
-                                     Кортеж из двух чисел описывает интервал, вычисляемый рандомно.
-                                     Кортеж (10, None) — устанавливает фиксированное ожидание в 10 секунд
-        :return:
-        """
-        for letter in text:
-            await self.SendChar(letter)
-            if interval is not None: await asyncio.sleep(random.uniform(interval[0], interval[1]))
-
-    async def SendKeyEvent(self, event: dict, *modifiers: KeyModifiers) -> None:
-        args = {}
-        if modifiers:
-            s = 0
-            for m in modifiers: s += m.value
-            args.update({"modifiers": s})
-
-        args.update(event)
-        await self.DispatchKeyEvent("keyDown", **args)
-        await self.DispatchKeyEvent("keyUp", **args)
-
-    async def ControlA(self) -> None:
-        """ Выделить весь текст(Ctrl+A). """
-        await self.SendKeyEvent(KeyEvents.keyA, KeyModifiers.ctrl)
-
-    async def BackspaceText(
-            self, count: int = 1, modifier: KeyModifiers = KeyModifiers.none) -> None:
-        """
-        Удаляет текст в текстовом поле с позиции курсора по направлению в лево, или полностью очистить,
-            эмулируя нажатие клавиши 'Backspace'.
-            Внимание! Курсор должен быть установлен в эдит-боксе!
-        :param count:                   (optional) Количество нажатий. Не имеет воздействия при полной очистке.
-        :param modifier:                (optional) none - удалить один символ, alt - слово, включая стоящие перед
-                                            ним пробелы, ctrl — полностью очистить эдит-бокс.
-        :return:
-        """
-
-        if modifier.name == "ctrl":
-            await self.ControlA()
-            await self.SendKeyEvent(KeyEvents.backspace)
-            return
-
-        for i in range(count):
-            await self.SendKeyEvent(KeyEvents.backspace, modifier.value)
-
-    async def SetWindowBounds(self, bounds: WindowBounds, windowId: Optional[int] = None) -> None:
-        """
-        (EXPERIMENTAL)
-        Устанавливает позицию и/или размер окна.
-        https://chromedevtools.github.io/devtools-protocol/tot/Browser#method-setWindowBounds
-        :param bounds:          Новые границы окна, а так же состояние.
-        :param windowId:        Идентификатор окна.
-
-        :return:        None
-        """
-        if windowId is None:
-            windowId = (await self.page_instance.GetWindowForTarget()).windowId
-        await self.page_instance.Call("Browser.setWindowBounds", {"windowId": windowId, "bounds": bounds.to_dict()})
```

### Comparing `aio_dt_protocol-0.9.5/aio_dt_protocol/Browser.py` & `aio_dt_protocol-1.0.0/aio_dt_protocol/browser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
+import asyncio
+from urllib.error import URLError
+
 try:
     import ujson as json
     HAS_UJSON = True
 except ModuleNotFoundError:
     HAS_UJSON = False
     import json
 import warnings
 import re, os, sys, signal, subprocess
 from urllib.parse import quote
 from os.path import expanduser
 from inspect import iscoroutinefunction
 from typing import List, Dict, Union, Optional, Tuple
 from collections.abc import Sequence
 from enum import Enum
-from .Page import Page
-from .Data import TargetConnectionInfo, TargetConnectionType, CommonCallback
-from .exceptions import FlagArgumentContainError
+from .connection import Connection
+from .data import TargetConnectionInfo, TargetConnectionType, CommonCallback
+from .exceptions import FlagArgumentContainError, NoTargetWithGivenIdFound
 from .utils import get_request, registry_read_key, log, async_util_call
 
 
 class Browser:
 
     def __init__(
             self,
@@ -267,41 +270,39 @@
 
         if flags is not None:
             flag_box += flags
 
         run_args += flag_box.flags()
         return subprocess.Popen(run_args).pid
 
-    def KillBrowser(self) -> None:
-        """
-        "Убивает" процесс браузера. Рекомендуется только в крайних случаях.
-            Лучше всего вызывать метод Call("Browser.close") у инстанса страницы
-        :return:
-        """
-        try: os.kill(self.browser_pid, signal.SIGTERM)
-        except PermissionError: pass
+    def kill(self) -> None:
+        """  Убивает процесс браузера. """
+        try:
+            os.kill(self.browser_pid, signal.SIGTERM)
+        except PermissionError:
+            pass
 
-    async def GetTargetConnectionInfoList(self) -> List[TargetConnectionInfo]:
-        return [TargetConnectionInfo(**i) for i in await self.GetPageList()]
+    async def getTargetConnectionInfoList(self) -> List[TargetConnectionInfo]:
+        return [TargetConnectionInfo(**i) for i in await self.getPageList()]
 
-    async def GetTargetConnectionInfo(
+    async def getTargetConnectionInfo(
             self, key: str = "type",
             connection_type: Union[str, TargetConnectionType] = "page") -> TargetConnectionInfo:
         v = connection_type if type(connection_type) is str else connection_type.value
-        for page_data in await self.GetPageList():
+        for page_data in await self.getPageList():
             data = page_data[key]
             if v in data: return TargetConnectionInfo(**page_data)
         raise ValueError(f"No have value {v} for key {key} in active target list")
 
-    async def GetConnectionsByType(
+    async def getConnectionsByType(
             self, connection_type: Union[str, TargetConnectionType]) -> List[TargetConnectionInfo]:
         t = connection_type if type(connection_type) is str else connection_type.value
-        return [ti for ti in await self.GetTargetConnectionInfoList() if ti.type == t]
+        return [ti for ti in await self.getTargetConnectionInfoList() if ti.type == t]
 
-    async def GetPageList(self) -> List[dict]:
+    async def getPageList(self) -> List[dict]:
         """
         Запрашивает у браузера список всех его дочерних процессов,
         включая табы(вкладки/страницы), воркеры, расширения, сервисы и прочее.
 
         :return: [ {
                     "description": "",
                     "devtoolsFrontendUrl": "/devtools/inspector.html?ws=localhost:9222/devtools/page/DAB7FB6187B554E10B0BD18821265734",
@@ -314,21 +315,21 @@
         """
         result = await async_util_call(
             get_request, f"http://127.0.0.1:{self.debug_port}/json/list")
 
         if self.verbose: log("GetPageList() => " + result)
         return json.loads(result)
 
-    async def GetPageBy(
+    async def getPageBy(
             self, key: Union[str, int],
             value: Union[str, int],
             match_mode: str = "exact",
             index: int = 0,
             callback: CommonCallback = None
-    ) -> Union[Page, None]:
+    ) -> Optional[Connection]:
         """
         Организует выбор нужного инстанса из процессов браузера по следующим критериям:
         :param key:                 По ключу из словаря. Список ключей смотри
                                         в возвращаемых значениях GetPageList()
         :param value:               Значение ключа, которому должен соответствовать выбор
         :param match_mode:          Значение ключа:
                                         "exact"      - полностью совпадает с value,
@@ -338,114 +339,240 @@
                                         быть несколько, предоставляется возможность выбрать
                                         по индексу. По умолчанию = 0
         :param callback:            Корутина, которой будет передаваться контекст абсолютно
                                         всех событий страницы в виде словаря. Если передан,
                                         включает уведомления домена "Runtime" для общения
                                         со страницей.
 
-        :return:        <Page> - инстанс страницы с подключением по WebSocket или None, если не найдено
+        :return:        <Connection>
         """
 
         if callback is not None and not iscoroutinefunction(callback):
             raise TypeError("Argument 'callback' must be a coroutine")
 
         counter = 0; v = value.lower()
-        for page_data in await self.GetPageList():
+        for page_data in await self.getPageList():
             data = page_data[key]
             if ((match_mode == "exact" and data == v)
                 or (match_mode == "contains" and data.find(v) > -1 )
                     or (match_mode == "startswith" and data.find(v) == 0)):
                 if counter == index:
-                    page = Page(
+                    conn = Connection(
                         page_data["webSocketDebuggerUrl"],
                         page_data["id"],
                         page_data["devtoolsFrontendUrl"],
                         callback,
                         self.profile_path == "",
                         self.verbose,
                         self.browser_name
                     )
-                    await page.Activate()
-                    return page
+
+                    await conn.activate()
+                    return conn
                 counter += 1
         return None
 
-    async def GetPage(
+    async def getPage(
             self,
             index: int = 0, page_type: str = "page",
             callback: CommonCallback = None
-    ) -> "Page":
+    ) -> "Connection":
         """
         Получает страницу браузера по индексу. По умолчанию, первую.
         :param index:       - Желаемый индекс страницы начиная с нуля.
-        :param page_type:   - Тип "Page" | 'background_page' | 'service_worker' | ???
+        :param page_type:   - Тип "page" | 'background_page' | 'service_worker' | ???
         :param callback:    - Корутина, которой будет передаваться контекст абсолютно
                                 всех событий страницы в виде словаря.
-        :return:        <Page>
+        :return:        <Connection>
         """
-        return await self.GetPageBy("type", page_type, "exact", index, callback)
+        return await self.getPageBy("type", page_type, "exact", index, callback)
 
-    async def GetPageByID(
-            self, page_id: str,
+    async def getPageByID(
+            self, conn_id: str,
             callback: CommonCallback = None
-    ) -> "Page":
+    ) -> "Connection":
         """
         Получает страницу браузера по уникальному идентификатору.
-        :param page_id:     - Желаемый идентификатор страницы. Метод GetPageList()
+        :param conn_id:     - Желаемый идентификатор страницы. Метод GetPageList()
                                 возвращает список доступных инстансов и словарь
                                 каждого из них содержит 'id'. Так же создание инстансов
                                 страниц через домен 'Target' возвращает 'targetId',
                                 который используется с этой же целью.
         :param callback:    - Корутина, которой будет передаваться контекст абсолютно
                                 всех событий страницы в виде словаря.
-        :return:        <Page>
+        :return:        <Connection>
         """
-        return await self.GetPageBy("id", page_id, "exact", 0, callback)
+        return await self.getPageBy("id", conn_id, "exact", 0, callback)
 
-    async def GetPageByTitle(
+    async def getPageByTitle(
             self, value: str,
             match_mode: str = "startswith",
             index: int = 0,
             callback: CommonCallback = None
-    ) -> "Page":
+    ) -> "Connection":
         """
         Получает страницу браузера по заголовку. По умолчанию, первую.
         :param value:       - Текст, который будет сопоставляться при поиске.
         :param match_mode:  - Тип сопоставления(по умолчанию 'startswith').
                                 Может быть только:
                                     * exact      - полное соответствие заголовка и value
                                     * contains   - заголовок содержит value
                                     * startswith - заголовок начинается с value
         :param index:       - Желаемый индекс страницы начиная с нуля.
         :param callback:    - Корутина, которой будет передаваться контекст абсолютно
                                 всех событий страницы в виде словаря.
-        :return:        <Page>
+        :return:        <Connection>
         """
-        return await self.GetPageBy("title", value, match_mode, index, callback)
+        return await self.getPageBy("title", value, match_mode, index, callback)
 
-    async def GetPageByURL(
+    async def getPageByURL(
             self, value: str,
             match_mode: str = "startswith",
             index: int = 0,
             callback: CommonCallback = None
-    ) -> "Page":
+    ) -> "Connection":
         """
         Получает страницу браузера по её URL. По умолчанию, первую.
         :param value:       - Текст, который будет сопоставляться при поиске.
         :param match_mode:  - Тип сопоставления(по умолчанию 'startswith').
                                 Может быть только:
                                     * exact      - полное соответствие URL и value
                                     * contains   - URL содержит value
                                     * startswith - URL начинается с value
         :param index:       - Желаемый индекс страницы начиная с нуля.
         :param callback:    - Корутина, которой будет передаваться контекст абсолютно
                                 всех событий страницы в виде словаря.
-        :return:        <Page>
+        :return:        <Connection>
+        """
+        return await self.getPageBy("url", value, match_mode, index, callback)
+
+    async def createPage(
+            self, url: str = "about:blank",
+            newWindow: bool = False,
+            background: bool = False,
+            wait_for_create: bool = True,
+            callback: CommonCallback = None
+    ) -> Optional[Connection]:
+        """
+        Создаёт новую вкладку в браузере.
+        :param url:                     - (optional) Адрес будет открыт при создании.
+        :param newWindow:               - (optional) Если 'True' — страница будет открыта в новом окне.
+        :param background:              - (optional) Если 'True' — страница будет открыта в фоне.
+        :return:                    * <Connection>
+        """
+        while not (tmp := await self.getPage(callback=callback)):
+            await asyncio.sleep(.5)
+        page_id = await tmp.Target.createTarget(url, newWindow=newWindow, background=background)
+        if wait_for_create:
+            while not (page := await self.getPageByID(page_id)):
+                await asyncio.sleep(.5)
+        else:
+            page = await self.getPageByID(page_id)
+        return page
+    
+    async def showInspector(self, conn: Connection, new_window: bool = True,
+                            callback: CommonCallback = None) -> Optional[Connection]:
+        """
+        Открывает новую вкладку с дебаггером для инспектируемой страницы.
+        :param conn:            - Инспектируемая страница. Может принадлежать любому браузеру.
+        :param new_window:      - Создать target в отдельном окне?
+        :return:        <Connection>
         """
-        return await self.GetPageBy("url", value, match_mode, index, callback)
+        return await self.createPage(
+            "http://127.0.0.1:" + str(self.debug_port) + conn.frontend_url, new_window, callback=callback
+        )
+
+    async def createPopupWindow(self, conn: Connection, url: str = "about:blank",
+                                callback: CommonCallback = None) -> Optional[Connection]:
+        """
+        Создаёт всплывающее окно с минимумом интерфейса браузера".
+        :param url:             - Адрес, ресурс которого будет загружен
+        :param conn:            - Родительская страница, инициатор
+        :return:        Connection or None
+        """
+        await conn.extend.injectJS(f'window.open("{url}", "blank_window_name", "popup,noopener,noreferrer");')
+        return await self.getPageByOpener(conn, callback=callback)
+
+    async def getPageByOpener(self, conn: Connection, callback: CommonCallback = None) -> Optional[Connection]:
+        """
+        Возвращает последний созданный инстанс страницы, открытие которого инициировано с конкретной страницы.
+            Например, при использовании JavaScript "window.open()".
+        :param conn:            - Родительская страница, инициатор
+        :return:        Connection or None
+        """
+        for target_info in await conn.Target.getTargets():
+            if target_info.openerId == conn.conn_id:
+                return await self.getPageByID(target_info.targetId, callback=callback)
+        return None
+
+    async def getPagesByOpener(self, conn: Connection, callback: CommonCallback = None) -> List[Connection]:
+        """
+        Возвращает список всех инстансов страниц, открытие которых инициировано с конкретной страницы.
+            Например, при использовании JavaScript "window.open()".
+        :param conn:            - Родительская страница, инициатор открытых окон
+        :return:        List[Connection]
+        """
+        pages = []
+        for target_info in await conn.Target.getTargets():
+            if target_info.openerId == conn.conn_id:
+                pages.append(await self.getPageByID(target_info.targetId, callback=callback))
+        return pages
+
+    async def waitFirstTab(self, timeout: float = 20.0, callback: CommonCallback = None) -> Connection:
+        """
+        Вызывает исключение 'asyncio.exceptions.TimeoutError' по истечении таймаута, или возвращает инстанс.
+        """
+        return await asyncio.wait_for(self.getFirstTab(callback), timeout)
+
+    async def getFirstTab(self, callback: CommonCallback = None) -> Connection:
+        """
+        Безусловно дожидается соединения со страницей.
+        """
+        while True:
+            try:
+                while (conn := await self.getPage(callback=callback)) is None:
+                    await asyncio.sleep(.5)
+                return conn
+            except URLError: await asyncio.sleep(1)
+
+    async def close(self) -> None:
+        """ Корректно закрывает браузер если остались ещё его инстансы """
+        if conn := await self.getPage():
+            await conn.Browser.close()
+
+    async def closeAllPagesExcept(self, *except_list: Connection) -> None:
+        """ Закрывает все страницы браузера, кроме переданных """
+        for conn in await self.getTargetConnectionInfoList():
+            if conn.type == "page":
+                condition = False
+                for conn in except_list:
+                    condition |= conn.conn_id == conn._id
+                if not condition:
+                    i = 4
+                    try:
+                        while (tab := await self.getPageByID(conn._id)) is None and i:
+                            await asyncio.sleep(.5)
+                            i -= 1
+                        if tab: await tab.Target.close()
+                    except NoTargetWithGivenIdFound:
+                        pass
+
+    async def getFramesFor(self, conn: Connection) -> List[Connection]:
+        """ Возвращает список iFrame для указанного инстанса """
+        result = []
+        for data in await self.getPageList():
+            if data["type"] == "iframe" and data["parentId"] == conn.conn_id:
+                result.append(await self.getPageByID(data["id"]))
+        return result
+
+    def __eq__(self, other: "Browser") -> bool:
+        return self.debug_port == other.debug_port
+
+    def __hash__(self) -> int:
+        return hash(self.debug_port)
 
 
 class FlagBuilder:
     """ Обеспечивает последовательность неповторяющихся флагов
     для запуска браузера.
     """
     def __init__(self):
```

### Comparing `aio_dt_protocol-0.9.5/aio_dt_protocol/BrowserEx.py` & `aio_dt_protocol-1.0.0/aio_dt_protocol/actions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,208 +1,193 @@
 import asyncio
-from asyncio import sleep, wait_for
-from urllib.error import URLError
-from inspect import iscoroutinefunction
-
-from .Data import CommonCallback
-from .Browser import Browser
-from .PageEx import PageEx
-from .exceptions import NoTargetWithGivenIdFound
-
-from urllib.parse import urlparse
-import re
-from typing import Optional, List
-
-
-class BrowserEx(Browser):
-    """
-    Расширение для 'Browser'. Включает в себя один новый метод CreatePage()
-        создающий новые вкладки(процессы страниц), а так же, все методы
-        получения инстансов вкладок, возвращают их с расширенным функционалом.
-    """
-
-    @staticmethod
-    def get_domain(url):
-        if url == "about:blank":
-            return "about:blank"
-        return re.search(r"^[^.]+", urlparse(url).netloc)[0]
-
-    async def GetPageBy(
-            self, key: str,
-            value: str,
-            match_mode: str = "exact",
-            index: int = 0,
-            callback: CommonCallback = None
-    ) -> Optional[PageEx]:
-
-        if callback is not None and not iscoroutinefunction(callback):
-            raise TypeError("Argument 'callback' must be a coroutine")
-
-        counter = 0; v = value.lower()
-        for page_data in await self.GetPageList():
-            data = page_data[key].lower()
-            if ((match_mode == "exact" and data == v)
-                or (match_mode == "contains" and data.find(v) > -1)
-                    or (match_mode == "startswith" and data.find(v) == 0)):
-                if counter == index:
-                    page = PageEx(
-                        page_data["webSocketDebuggerUrl"],
-                        page_data["id"],
-                        page_data["devtoolsFrontendUrl"],
-                        callback,
-                        self.profile_path == "",
-                        self.verbose,
-                        self.browser_name
-                    )
-                    await page.Activate()
-                    return page
-                counter += 1
-        return None
-
-    async def GetPage(
-            self, index: int = 0, page_type: str = "page",
-            callback: CommonCallback = None
-    ) -> Optional[PageEx]:
-        return await self.GetPageBy("type", page_type, "exact", index, callback)
-
-    async def GetPageByID(
-            self, page_id: str, index: int = 0,
-            callback: CommonCallback = None
-    ) -> Optional[PageEx]:
-        return await self.GetPageBy("id", page_id, "exact", index, callback)
-
-    async def GetPageByTitle(
-            self, value: any, match_mode: str = "startswith",
-            index: int = 0, callback: CommonCallback = None
-    ) -> Optional[PageEx]:
-        return await self.GetPageBy("title", value, match_mode, index, callback)
-
-    async def GetPageByURL(
-            self, value: any, match_mode: str = "startswith",
-            index: int = 0, callback: CommonCallback = None
-    ) -> Optional[PageEx]:
-        return await self.GetPageBy("url", value, match_mode, index, callback)
-
-    async def CreatePage(
-            self,  url: str = "about:blank",
-            newWindow: bool = False,
-            background: bool = False,
-            wait_for_create: bool = True,
-            callback: CommonCallback = None
-    ) -> Optional[PageEx]:
-        """
-        Создаёт новую вкладку в браузере.
-        :param url:                     - (optional) Адрес будет открыт при создании.
-        :param newWindow:               - (optional) Если 'True' — страница будет открыта в новом окне.
-        :param background:              - (optional) Если 'True' — страница будет открыта в фоне.
-        :return:                    * Инстанс страницы <PageEx>
-        """
-        while not (tmp := await self.GetPage(callback=callback)):
-            await sleep(.5)
-        page_id = await tmp.CreateTarget(url, newWindow=newWindow, background=background)
-        if wait_for_create:
-            while not(page := await self.GetPageByID(page_id)):
-                await sleep(.5)
-        else:
-            page = await self.GetPageByID(page_id)
-        return page
-
-    async def ShowInspector(self, page: PageEx, new_window: bool = True,
-                            callback: CommonCallback = None) -> Optional[PageEx]:
-        """
-        Открывает новую вкладку с дебаггером для инспектируемой страницы.
-        :param page:            - Инспектируемая страница. Может принадлежать любому браузеру.
-        :param new_window:      - Создать target в отдельном окне?
-        :return:        <PageEx>
-        """
-        return await self.CreatePage(
-            "http://127.0.0.1:" + str(self.debug_port) + page.frontend_url, new_window, callback=callback
-        )
-
-    async def CreatePopupWindow(self, page: PageEx, url: str = "about:blank",
-                                callback: CommonCallback = None) -> Optional[PageEx]:
-        """
-        Создаёт всплывающее окно с минимумом интерфейса браузера".
-        :param url:             - Адрес, ресурс которого будет загружен
-        :param page:            - Родительская страница, инициатор
-        :return:        PageEx or None
-        """
-        await page.InjectJS(f'window.open("{url}", "blank_window_name", "popup,noopener,noreferrer");')
-        return await self.GetPageByOpener(page, callback=callback)
-
-    async def GetPageByOpener(self, page: PageEx, callback: CommonCallback = None) -> Optional[PageEx]:
-        """
-        Возвращает последний созданный инстанс страницы, открытие которого инициировано с конкретной страницы.
-            Например, при использовании JavaScript "window.open()".
-        :param page:            - Родительская страница, инициатор
-        :return:        PageEx or None
-        """
-        for target_info in await page.GetTargets():
-            if target_info.openerId == page.page_id:
-                return await self.GetPageByID(target_info.targetId, callback=callback)
-        return None
-
-    async def GetPagesByOpener(self, page: PageEx, callback: CommonCallback = None) -> List[PageEx]:
-        """
-        Возвращает список всех инстансов страниц, открытие которых инициировано с конкретной страницы.
-            Например, при использовании JavaScript "window.open()".
-        :param page:            - Родительская страница, инициатор открытых окон
-        :return:        List[PageEx]
-        """
-        pages = []
-        for target_info in await page.GetTargets():
-            if target_info.openerId == page.page_id:
-                pages.append(await self.GetPageByID(target_info.targetId, callback=callback))
-        return pages
-
-    async def WaitFirstTab(self, timeout: float = 20.0, callback: CommonCallback = None) -> PageEx:
-        """
-        Вызывает исключение 'asyncio.exceptions.TimeoutError' по истечении таймаута, или возвращает инстанс.
-        """
-        return await wait_for(self.GetFirstTab(callback), timeout)
-
-    async def GetFirstTab(self, callback: CommonCallback = None) -> PageEx:
-        """
-        Безусловно дожидается соединения со страницей.
-        """
-        while True:
-            try:
-                while (page := await self.GetPage(callback=callback)) is None:
-                    await sleep(.5)
-                return page
-            except URLError: await sleep(1)
-
-    async def Close(self) -> None:
-        """ Корректно закрывает браузер если остались ещё его инстансы """
-        if page := await self.GetPage():
-            await page.CloseBrowser()
-
-    async def CloseAllPagesExcept(self, *except_list: PageEx) -> None:
-        """ Закрывает все страницы браузера, кроме переданных """
-        for conn in await self.GetTargetConnectionInfoList():
-            if conn.type == "page":
-                condition = False
-                for page in except_list:
-                    condition |= page.page_id == conn.id
-                if not condition:
-                    i = 4
-                    try:
-                        while (tab := await self.GetPageByID(conn.id)) is None and i:
-                            await asyncio.sleep(.5)
-                            i -= 1
-                        if tab: await tab.Close()
-                    except NoTargetWithGivenIdFound:
-                        pass
-
-    async def GetFramesFor(self, page: PageEx) -> List[PageEx]:
-        """ Возвращает список iFrame для указанного инстанса """
-        result = []
-        for conn in await self.GetPageList():
-            if conn["type"] == "iframe" and conn["parentId"] == page.page_id:
-                result.append( await self.GetPageByID(conn["id"]) )
-        return result
-
-    def __eq__(self, other: "BrowserEx") -> bool:
-        return self.debug_port == other.debug_port
-
-    def __hash__(self) -> int:
-        return hash(self.debug_port)
+import random
+from typing import Tuple, Optional, Literal
+from .data import WINDOWS_KEY_SET, KeyModifiers, KeyEvents
+from .domains.browser.types import Bounds
+
+
+class Actions:
+    __slots__ = ("_connection",)
+
+    def __init__(self, conn) -> None:
+        from .connection import Connection
+
+        self._connection: Connection = conn
+
+    async def swipeTo(
+        self,
+        direction: Literal["up", "down", "left", "right"],
+        x:            float = 0,
+        y:            float = 0,
+        distance:     Optional[float] = None,
+        speed:        Optional[float] = None,
+        overscroll:   Optional[float] = None,
+        repeat_count:   Optional[int] = None,
+        repeat_delay: Optional[float] = None,
+        gestureSourceType: Literal["touch", "mouse"] = "mouse"
+    ) -> None:
+        """
+        Скроллит вьюпорт жестом "touch" на всю его длину/высоту.
+            Возвращает управление только после выполнения жеста!
+        :param direction:           (optional) Направление. Может быть следующим:
+                                        up — пальцем вверх(прокрутка вниз)
+                                        down — пальцем вниз(прокрутка вверх)
+                                        left — пальцем влево(прокрутка вправо)
+                                        right — пальцем вправо(прокрутка влево)
+        :param x:                   (optional) X-координата начальной точки.
+        :param y:                   (optional) Y-координата начальной точки.
+        :param distance:            (optional) Дистанция движения.
+        :param speed:               (optional) Скорость движения(по умолчанию = 800).
+        :param overscroll:          (optional) Дополнительная дистанция в пикселях.
+        :param repeat_count:        (optional) Кол-во повторений сделанного жеста.
+        :param repeat_delay:        (optional) Задержка между повторениями.
+        :param gestureSourceType:   (optional) Задержка между повторениями.
+        :return:
+        """
+        if direction not in ["up", "down", "left", "right"]:
+            raise ValueError("'direction' must be one from — up; down; left; right")
+        sign = -1 if direction in ["up", "left"] else 1
+        rect = None
+        if x is None:
+            rect = await self._connection.extend.getViewportRect()
+            x = 10 if direction == "right" else rect.width - 10 if direction == "left" else rect.height / 2
+
+        if y is None:
+            rect = await self._connection.extend.getViewportRect()
+            y = 10 if direction == "down" else rect.height - 10 if direction == "up" else rect.width / 2
+
+        if distance is None:
+            rect = rect or await self._connection.extend.getViewportRect()
+            distance = (rect.height if direction in ["up", "down"] else rect.width) - 10
+
+        overscroll = overscroll if overscroll is not None else 0
+
+        args = {
+            "x": x, "y": y, "speed": speed, "repeatCount": repeat_count,
+            "repeatDelayMs": repeat_delay, "gestureSourceType": gestureSourceType,
+            "xDistance": distance * sign if direction in ["left", "right"] else None,
+            "yDistance": distance * sign if direction in ["up", "down"] else None,
+            "xOverscroll": overscroll * -sign if direction in ["left", "right"] else None,
+            "yOverscroll": overscroll * -sign if direction in ["up", "down"] else None,
+        }
+        await self._connection.Input.synthesizeScrollGesture(**args)
+
+    async def clickTo(self, x: int, y: int, delay: float = None) -> None:
+        """
+        Эмулирует клик мыши по координатам.
+        :param x:               x - координата
+        :param y:               y - координата
+        :param delay:           задержка перед отпусканием
+        :return:
+        """
+        await self._connection.Input.dispatchMouseEvent("mousePressed", x, y, button="left")
+        if delay: await asyncio.sleep(delay)
+        await self._connection.Input.dispatchMouseEvent("mouseReleased", x, y, button="left")
+
+    async def mouseMoveTo(self, x: int, y: int) -> None:
+        await self._connection.Input.dispatchMouseEvent("mouseMoved", x, y)
+
+    async def mouseWheel(self, x: float, y: float, deltaX: float = 0, deltaY: float = 0) -> None:
+        """
+        Крутит колесо мышки.
+        :param x:               Положение
+        :param y:               указателя мыши.
+        :param deltaX:          Скроллит по-горизонтали.
+        :param deltaY:          Скроллит по-вертикали, положительное значение == вниз.
+        :return:
+        """
+        await self._connection.Input.dispatchMouseEvent("mouseWheel", x, y, button="middle", deltaX=deltaX, deltaY=deltaY)
+
+    async def wheelTo(self, direction: str = "down") -> None:
+        sign = -1 if direction in ["up", "left"] else 1
+        rect = await self._connection.extend.getViewportRect()
+        x = 10 if direction == "right" else rect.width - 10 if direction == "left" else rect.height / 2
+        y = 10 if direction == "down" else rect.height - 10 if direction == "up" else rect.width / 2
+        distance = ((rect.height if direction in ["up", "down"] else rect.width) - 10) * sign
+        delta = {"deltaX": distance} if direction in ["left", "rigth"] else {"deltaY": distance}
+        await self.mouseWheel(x, y, **delta)
+
+
+    async def mouseMoveToCoordinatesAndClick(self, x: int, y: int) -> None:
+        await self.mouseMoveTo(x, y)
+        await self.clickTo(x, y)
+
+    async def sendChar(self, char: str) -> None:
+        """
+        Эмулирует ввод символа нажатием соответствующей кнопки клавиатуры.
+            Внимание! Курсор должен быть установлен в эдит-боксе!
+        :param char:             Символ для ввода.
+        :return:
+        """
+        upper_key = char.upper()
+        args = {
+            "text": char, "key": char, "keyIdentifier": f"U+{WINDOWS_KEY_SET[upper_key]:X}",
+            "windowsVirtualKeyCode": WINDOWS_KEY_SET[upper_key],
+            "nativeVirtualKeyCode": WINDOWS_KEY_SET[upper_key]
+        }
+        if len(char) > 1: raise ValueError(f"Передаваемая строка: '{char}' — должна быть из одного символа!")
+        await self._connection.Input.dispatchKeyEvent("char", **args)
+
+    async def sendText(
+            self, text: str, interval: Optional[Tuple[float, float]] = None
+    ) -> None:
+        """
+        Эмулирует последовательный набор текста.
+            Внимание! Курсор должен быть установлен в эдит-боксе!
+        :param text:             Последовательность символов для ввода.
+        :param interval:         Задержка после нажатия кнопки. None - отключает задержку.
+                                     Кортеж из двух чисел описывает интервал, вычисляемый рандомно.
+                                     Кортеж (10, None) — устанавливает фиксированное ожидание в 10 секунд
+        :return:
+        """
+        for letter in text:
+            await self.sendChar(letter)
+            if interval is not None: await asyncio.sleep(random.uniform(interval[0], interval[1]))
+
+    async def sendKeyEvent(self, event: dict, *modifiers: KeyModifiers) -> None:
+        args = {}
+        if modifiers:
+            s = 0
+            for m in modifiers: s += m.value
+            args.update({"modifiers": s})
+
+        args.update(event)
+        await self._connection.Input.dispatchKeyEvent("keyDown", **args)
+        await self._connection.Input.dispatchKeyEvent("keyUp", **args)
+
+    async def controlA(self) -> None:
+        """ Выделить весь текст(Ctrl+A). """
+        await self.sendKeyEvent(KeyEvents.keyA, KeyModifiers.ctrl)
+
+    async def backspaceText(
+            self, count: int = 1, modifier: KeyModifiers = KeyModifiers.none) -> None:
+        """
+        Удаляет текст в текстовом поле с позиции курсора по направлению в лево, или полностью очистить,
+            эмулируя нажатие клавиши 'Backspace'.
+            Внимание! Курсор должен быть установлен в эдит-боксе!
+        :param count:                   (optional) Количество нажатий. Не имеет воздействия при полной очистке.
+        :param modifier:                (optional) none - удалить один символ, alt - слово, включая стоящие перед
+                                            ним пробелы, ctrl — полностью очистить эдит-бокс.
+        :return:
+        """
+
+        if modifier.name == "ctrl":
+            await self.controlA()
+            await self.sendKeyEvent(KeyEvents.backspace)
+            return
+
+        for i in range(count):
+            await self.sendKeyEvent(KeyEvents.backspace, modifier.value)
+
+    async def setWindowBounds(self, bounds: Bounds, windowId: Optional[int] = None) -> None:
+        """
+        (EXPERIMENTAL)
+        Устанавливает позицию и/или размер окна.
+        https://chromedevtools.github.io/devtools-protocol/tot/Browser#method-setWindowBounds
+        :param bounds:          Новые границы окна, а так же состояние.
+        :param windowId:        Идентификатор окна.
+
+        :return:        None
+        """
+        if windowId is None:
+            windowId = (await self._connection.Target.getWindowForTarget()).windowId
+        await self._connection.call("Browser.setWindowBounds", {"windowId": windowId, "bounds": bounds.to_dict()})
```

### Comparing `aio_dt_protocol-0.9.5/aio_dt_protocol/DOMElement.py` & `aio_dt_protocol-1.0.0/aio_dt_protocol/domains/dom/dom_element.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import re
 import asyncio
 from typing import List, Dict, Optional, Union, Literal
-from .Data import NodeCenter, NodeRect, StyleProp, BoxModel
-from .domains.Runtime import RuntimeType, Script
-from .exceptions import (
+from .types import NodeCenter, NodeRect, BoxModel, StyleProp
+from ...domains.runtime.types import Script, RemoteObject
+from ...exceptions import (
     CouldNotFindNodeWithGivenID, RootIDNoLongerExists, NodeNotResolved, NodeNotDescribed,
     StateError
 )
 
 def to_dict_attrs(a: list) -> Union[dict, None]:
     if not a: return None
     return {a[i]: a[i+1] for i in range(0, len(a), 2)}
 
 class Node:
     __slots__ = (
-        "page_instance", "nodeId", "parentId", "backendNodeId", "nodeType", "nodeName", "localName", "nodeValue",
+        "_connection", "nodeId", "parentId", "backendNodeId", "nodeType", "nodeName", "localName", "nodeValue",
         "childNodeCount", "children", "attributes", "documentURL", "baseURL", "publicId", "systemId", "internalSubset",
         "xmlVersion", "name", "value", "pseudoType", "frameId", "shadowRootType", "contentDocument", "shadowRoots",
         "templateContent", "pseudoElements", "importedDocument", "distributedNodes", "isSVG", "compatibilityMode",
         "remote_object", "isolated_id"
     )
 
     def __init__(
-        self, page_instance, nodeId: int,
+        self, conn, nodeId: int,
         parentId:              Optional[int] = None,
         backendNodeId:         Optional[int] = None,
         nodeType:              Optional[int] = None,
         nodeName:              Optional[str] = None,
         localName:             Optional[str] = None,
         nodeValue:             Optional[str] = None,
         childNodeCount:        Optional[int] = None,
@@ -48,147 +48,154 @@
         templateContent:    Optional["Node"] = None,
         pseudoElements: Optional[List["Node"]] = None,
         importedDocument:    Optional["Node"] = None,
         distributedNodes: Optional[List[dict]] = None,  #
         isSVG:                Optional[bool] = None,    # является ли элемент SVG-элементом
         compatibilityMode: Optional[Literal["QuirksMode", "LimitedQuirksMode", "NoQuirksMode"]] = None
 
-    ):
-        self.page_instance = page_instance  # PageEx
+    ) -> None:
+
+        from ...connection import Connection
+
+        self._connection: Connection = conn
         self.nodeId = nodeId
         self.backendNodeId = backendNodeId
         self.nodeType = nodeType
         self.nodeName = nodeName
         self.localName = localName
         self.nodeValue = nodeValue
 
         self.parentId = parentId
         self.publicId = publicId
         self.systemId = systemId
         self.internalSubset = internalSubset
 
         self.childNodeCount = childNodeCount
-        self.children = self._AddChildren(children)
+        self.children = self._addChildren(children)
         self.attributes = to_dict_attrs(attributes)
         self.frameId = frameId
         self.documentURL = documentURL
         self.baseURL = baseURL
         self.xmlVersion = xmlVersion
         self.name = name
         self.value = value
         self.pseudoType = pseudoType
 
-        self.shadowRoots = self._AddChildren(shadowRoots)
+        self.shadowRoots = self._addChildren(shadowRoots)
         self.shadowRootType = shadowRootType
 
-        self.contentDocument = self._AddChild(contentDocument)
-        self.templateContent = self._AddChild(templateContent)
-        self.pseudoElements = self._AddChildren(pseudoElements)
-        self.importedDocument = self._AddChild(importedDocument)
+        self.contentDocument = self._addChild(contentDocument)
+        self.templateContent = self._addChild(templateContent)
+        self.pseudoElements = self._addChildren(pseudoElements)
+        self.importedDocument = self._addChild(importedDocument)
         self.distributedNodes = distributedNodes
         self.isSVG = isSVG
         self.compatibilityMode = compatibilityMode
 
-        self.remote_object: Optional['RemoteObject'] = None
+        self.remote_object: Optional[RemoteObject] = None
         self.isolated_id = None                                         # идентификатор изолированного контекста
 
     def __str__(self) -> str:
         return f"<Node id={self.nodeId} localName={self.localName} childNodeCount={self.childNodeCount}>"
 
-    def _AddChildren(self, children_list: Optional[List[dict]] = None) -> List["Node"]:
+    def _addChildren(self, children_list: Optional[List[dict]] = None) -> List["Node"]:
         """
         Вызывается рекурсивно всякий раз, когда описание нового узла содержит
             список потомков, а так же, когда уже созданному узлу запрашиваются
-            его потомки посредством метода GetChildNodes().
+            его потомки посредством метода getChildNodes().
         :param children_list:        Список словарей, описывающих свойства потомков.
         :return:        List[Node]
         """
         if not children_list: return []
         list_nodes = []
         for child in children_list:
-            list_nodes.append(Node(self.page_instance, **child))
+            list_nodes.append(Node(self._connection, **child))
         return list_nodes
 
-    def _AddChild(self, child: Union[dict, "Node", None] = None) -> Optional["Node"]:
+    def _addChild(self, child: Union[dict, "Node", None] = None) -> Optional["Node"]:
         if not child: return None
-        return Node(self.page_instance, **child) if type(child) is dict else child
+        return Node(self._connection, **child) if type(child) is dict else child
 
-    async def QuerySelector(self, selector: str, ignore_root_id_exists: bool = False) -> Optional["Node"]:
+    async def querySelector(self, selector: str, ignore_root_id_exists: bool = False) -> Optional["Node"]:
         """
         Выполняет DOM-запрос, возвращая объект найденного узла, или None.
             Эквивалент  === element.querySelector()
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-querySelector
         :param selector:                    Селектор.
         :param ignore_root_id_exists:       Игнорировать исключение при отсутствии родительского элемента.
                                                 Полезно при запросах на загружающихся страницах.
         :return:        <Node>
         """
         try:
             node_id = (
-                await self.page_instance.Call("DOM.querySelector", {
+                await self._connection.call("DOM.querySelector", {
                     "nodeId": self.nodeId, "selector": selector
                 }))["nodeId"]
         except CouldNotFindNodeWithGivenID as e:
             if match := re.search(r"nodeId\': (\d+)", str(e)):
                 if match.group(1) == str(self.nodeId):
                     if ignore_root_id_exists:
                         return None
                     raise RootIDNoLongerExists
             raise
-        return Node(self.page_instance, node_id) if node_id else None
+        return Node(self._connection, node_id) if node_id else None
 
-    async def QuerySelectorAll(self, selector: str, ignore_root_id_exists: bool = False) -> List["Node"]:
+    async def querySelectorAll(self, selector: str, ignore_root_id_exists: bool = False) -> List["Node"]:
         """
         Выполняет DOM-запрос, возвращая список объектов найденных узлов, или пустой список.
             Эквивалент  === element.querySelectorAll()
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-querySelectorAll
         :param selector:                    Селектор.
         :param ignore_root_id_exists:       Игнорировать исключение при отсутствии родительского элемента.
                                                 Полезно при запросах на загружающихся страницах.
         :return:        [ <Node>, <Node>, ... ]
         """
         nodes = []
         try:
-            for node_id in (await self.page_instance.Call("DOM.querySelectorAll", {
+            for node_id in (await self._connection.call("DOM.querySelectorAll", {
                         "nodeId": self.nodeId, "selector": selector
                     }))["nodeIds"]:
-                nodes.append(Node(self.page_instance, node_id))
+                nodes.append(Node(self._connection, node_id))
         except CouldNotFindNodeWithGivenID as e:
             if match := re.search(r"nodeId\': (\d+)", str(e)):
                 if match.group(1) == str(self.nodeId):
                     if ignore_root_id_exists:
                         return []
                     raise RootIDNoLongerExists
             raise
         return nodes
 
-    async def GetChildNodes(self, depth: int = -1, pierce: bool = False) -> None:
-        """
-        Запрашивает событие 'DOM.setChildNodes' для собственного узла и устанавливает слушателя.
-            Как только событие будет сгенерировано для текущего идентификатора узла, слушатель
-            будет отменён. Список полученных потомков узла, включая текстовые будет доступен
-            через его свойство 'children'.
+    async def getChildNodes(self, depth: int = -1, pierce: bool = False) -> asyncio.Event:
+        """ Запрашивает событие 'DOM.setChildNodes' для собственного узла и устанавливает
+        слушателя и возвращает ожидаемый объект события, который получит уведомление о том,
+        что ожидаемое событие произошло и все данные уже обработаны.
+        Как только 'DOM.setChildNodes' случится для текущего идентификатора узла, слушатель
+        будет отменён. Список полученных потомков узла, включая текстовые будет доступен
+        через его свойство 'children'.
 
         !ВНИМАНИЕ! Запрос потомков у <input /> не генерирует событие 'DOM.setChildNodes',
             потому как это одиночный тег, внутри которого не может быть потомков.
         :param depth:           Глубина иерархии, до которой будут получены все потомки.
                                     По умолчанию -1 == все. Чтобы задать конкретное значение,
                                     укажите любое целое число больше нуля.
         :param pierce:          Получать содержимое теневых узлов(shadowRoots, shadowDOM)?
-        :return:        None
+        :return:        asyncio.Event
         """
+        event = asyncio.Event()
         async def catch(data: dict) -> None:
             if data["parentId"] == self.nodeId:
-                self.page_instance.RemoveListenerForEvent("DOM.setChildNodes", catch)
-                self.children = self._AddChildren(data["nodes"])
+                self._connection.removeListenerForEvent("DOM.setChildNodes", catch)
+                self.children = self._addChildren(data["nodes"])
+                event.set()
 
         self.children = None
-        await self.page_instance.AddListenerForEvent("DOM.setChildNodes", catch)
-        await self.RequestChildNodes(depth, pierce)
-        while self.children is None: await asyncio.sleep(.01)
+        await self._connection.addListenerForEvent("DOM.setChildNodes", catch)
+        await self.requestChildNodes(depth, pierce)
+        return event
+
 
     async def ScrollIntoView(self, rect: dict = None) -> None:
         """
         (EXPERIMENTAL)
         Прокручивает указанный прямоугольник, в котором находится узел, если он еще не виден. После применения
             идентификатор узла становится недействителен и его придётся запрашивать вновь.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-scrollIntoViewIfNeeded
@@ -197,100 +204,102 @@
                                 центр узла, аналогично Element.scrollIntoView.
                                 Ожидается словарь, вида: {"x": 100, "y": 100, "width", 200, "height": 200}
         :return:        None
         """
         args = {"nodeId": self.nodeId}
         if rect:
             args.update({"rect": rect})
-        await self.page_instance.Call("DOM.scrollIntoViewIfNeeded", args)
+        await self._connection.call("DOM.scrollIntoViewIfNeeded", args)
 
-    async def FocusNode(self) -> bool:
+    async def focusNode(self) -> bool:
         """
         Фокусируется на элементе.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-focus
         :return:            Была ли фокусировка успешной
         """
         try:
-            await self.page_instance.Call("DOM.focus", {"nodeId": self.nodeId})
+            await self._connection.call("DOM.focus", {"nodeId": self.nodeId})
             return True
         except:
             return False
 
-    async def GetAttributes(self) -> Dict[str, str]:
+    async def getAttributes(self) -> Dict[str, str]:
         """
         Возвращает список атрибутов элемента.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-getAttributes
         :return:            {'id': 'element-id', 'style': 'position:absolute;...', ...}
         """
-        return to_dict_attrs((await self.page_instance.Call("DOM.getAttributes", {"nodeId": self.nodeId}))["attributes"])
+        return to_dict_attrs(
+            (await self._connection.call("DOM.getAttributes", {"nodeId": self.nodeId}))["attributes"])
 
-    async def RemoveAttribute(self, name: str) -> None:
+    async def removeAttribute(self, name: str) -> None:
         """
         Удаляет атрибут по 'name'.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-removeAttribute
         :param name:        Имя удаляемого атрибута.
         :return:
         """
-        await self.page_instance.Call("DOM.removeAttribute", {"nodeId": self.nodeId, "name": name})
+        await self._connection.call("DOM.removeAttribute", {"nodeId": self.nodeId, "name": name})
 
-    async def RemoveNode(self) -> None:
+    async def removeNode(self) -> None:
         """
         Удаляет себя из документа.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-removeNode
         :return:
         """
-        await self.page_instance.Call("DOM.removeNode", {"nodeId": self.nodeId})
+        await self._connection.call("DOM.removeNode", {"nodeId": self.nodeId})
 
-    async def GetBoxModel(self) -> BoxModel:
+    async def getBoxModel(self) -> BoxModel:
         """
         Возвращает 'box-model' элемента.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-getBoxModel
         :return:            <BoxModel>
         """
-        return BoxModel(**(await self.page_instance.Call("DOM.getBoxModel", {"nodeId": self.nodeId}))["model"])
+        return BoxModel(
+            **(await self._connection.call("DOM.getBoxModel", {"nodeId": self.nodeId}))["model"])
 
-    async def GetOuterHTML(self) -> str:
+    async def getOuterHTML(self) -> str:
         """
         Возвращает HTML-разметку элемента включая внешние границы тега.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-getOuterHTML
         :return:            Строка HTML-разметки. '<div>Inner div text</div>'.
         """
-        return (await self.page_instance.Call("DOM.getOuterHTML", {"nodeId": self.nodeId}))["outerHTML"]
+        return (await self._connection.call("DOM.getOuterHTML", {"nodeId": self.nodeId}))["outerHTML"]
 
-    async def GetInnerHTML(self) -> str:
+    async def getInnerHTML(self) -> str:
         """
         Возвращает HTML-разметку элемента НЕ включая внешние границы тега.
         :return:            Строка HTML-разметки. 'Inner div <div>text</div> with HTML'.
         """
-        html = await self.GetOuterHTML()
+        html = await self.getOuterHTML()
         if m := re.match(r"^<.*?>(.*)<.*?>$", html):
             return m.group(1)
         return html
 
-    async def GetInnerText(self, with_new_line_symbols: bool = True) -> str:
+    async def getInnerText(self, with_new_line_symbols: bool = True) -> str:
         """
         Возвращает текстовое содержимое элемента.
         :param with_new_line_symbols:     (optional) — Оставлять символы новой строки?
         :return:                        Текст.
         """
         pattern = r"<.*?>" if with_new_line_symbols else r"(<.*?>)|\n"
-        html = await self.GetOuterHTML()
+        html = await self.getOuterHTML()
         return re.sub(pattern, "", html).strip()
 
-    async def SetOuterHTML(self, outerHTML: str) -> None:
+    async def setOuterHTML(self, outerHTML: str) -> None:
         """
         Устанавливает HTML-разметку для элемента. !Внимание! После этого преобразования, элемент
             получит новый идентификатор и повтороно обратиться к нему уже не получится.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-setOuterHTML
         :param outerHTML:       Строка HTML-разметки. '<div>Inner div text</div>'.
         :return:
         """
-        await self.page_instance.Call("DOM.setOuterHTML", {"nodeId": self.nodeId, "outerHTML": outerHTML})
+        await self._connection.call("DOM.setOuterHTML", {"nodeId": self.nodeId, "outerHTML": outerHTML})
 
-    async def MoveTo(
+    async def moveTo(
             self, targetNodeId: int,
             insertBeforeNodeId: Optional[int] = None
     ) -> None:
         """
         Перемещает узел в новый контейнер, помещает его перед заданным якорем. В результате,
             внутренний идентификатор узла будет сменён.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-moveTo
@@ -299,17 +308,17 @@
                                         не будет найден, то перемещаемый элемент становится
                                         последним дочерним элементом 'targetNodeId'.
         :return:
         """
         args = {"nodeId": self.nodeId, "targetNodeId": targetNodeId}
         if insertBeforeNodeId:
             args.update({"insertBeforeNodeId": insertBeforeNodeId})
-        self.nodeId = (await self.page_instance.Call("DOM.moveTo", args))["nodeId"]
+        self.nodeId = (await self._connection.call("DOM.moveTo", args))["nodeId"]
 
-    async def CopyTo(
+    async def copyTo(
             self, targetNodeId: int, insertBeforeNodeId: Optional[int] = None
     ) -> "Node":
         """
         Создает глубокую копию текущего узла и помещает ее в 'targetNodeId' перед 'insertBeforeNodeId',
             если последний указан и будет найден. Возвращает склонированный узел.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-moveTo
         :param targetNodeId:        Идентификатор элемента, куда будет скопирован текущий элемент.
@@ -317,18 +326,18 @@
                                         не будет найден, то копируемый элемент становится
                                         последним дочерним элементом 'targetNodeId'.
         :return:                    <Node> - клона.
         """
         args = {"nodeId": self.nodeId, "targetNodeId": targetNodeId}
         if insertBeforeNodeId:
             args.update({"insertBeforeNodeId": insertBeforeNodeId})
-        node_id = (await self.page_instance.Call("DOM.copyTo", args))["nodeId"]
-        return Node(node_id, self.page_instance)
+        node_id = (await self._connection.call("DOM.copyTo", args))["nodeId"]
+        return Node(self._connection, node_id)
 
-    async def GetContentQuads(
+    async def getContentQuads(
             self,
             backendNodeId: Optional[int] = None,
                  objectId: Optional[str] = None
     ) -> List[List[int]]:
         """
         (EXPERIMENTAL)
         Возвращает квадраты, которые описывают положение узла на странице. Этот метод может вернуть
@@ -341,106 +350,106 @@
         """
         args = {"nodeId": self.nodeId}
         if not args and backendNodeId is not None:
             args.update({"backendNodeId": backendNodeId})
         if not args and objectId is not None:
             args.update({"objectId": objectId})
         if args:
-            return (await self.page_instance.Call("DOM.getContentQuads", args))["quads"]
+            return (await self._connection.call("DOM.getContentQuads", args))["quads"]
 
-    async def SetAttributeValue(self, attributeName: str, value: str) -> None:
+    async def setAttributeValue(self, attributeName: str, value: str) -> None:
         """
         Устанавливает атрибут для элемента с данным идентификатором.
             Например: await node.SetAttributeValue('class', 'class-name')
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-setAttributeValue
         :param attributeName:   Attribute name.
         :param value:           Attribute value.
         :return:
         """
-        await self.page_instance.Call("DOM.setAttributeValue", {"nodeId": self.nodeId, "name": attributeName, "value": value})
+        await self._connection.call(
+            "DOM.setAttributeValue", {"nodeId": self.nodeId, "name": attributeName, "value": value})
 
-    async def RequestChildNodes(self, depth: int = 1, pierce: bool = False) -> None:
-        """
-        Запрашивает, чтобы дочерние элементы узла с данным идентификатором возвращались
-            вызывающей стороне в форме событий DOM.setChildNodes, при которых извлекаются
-            не только непосредственные дочерние элементы, но и все дочерние элементы до
-            указанной глубины.
+    async def requestChildNodes(self, depth: int = 1, pierce: bool = False) -> None:
+        """ Запрашивает, чтобы дочерние элементы узла с данным идентификатором возвращались
+        вызывающей стороне в форме событий DOM.setChildNodes, при которых извлекаются
+        не только непосредственные дочерние элементы, но и все дочерние элементы до
+        указанной глубины.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-requestChildNodes
         :param depth:           (optional) - Максимальная глубина, на которой должны быть получены
                                     дочерние элементы, по умолчанию равна 1. Используйте -1 для
                                     всего поддерева или укажите целое число больше 0.
         :param pierce:           (optional) - Должны ли проходить фреймы и теневые корни при
                                     возврате поддерева (по умолчанию false).
         :return:
         """
         args = {"nodeId": self.nodeId, "depth": depth, "pierce": pierce}
-        await self.page_instance.Call("DOM.requestChildNodes", args)
+        await self._connection.call("DOM.requestChildNodes", args)
 
-    async def SetAttributesAsText(self, text: str, name: str = "") -> None:
+    async def setAttributesAsText(self, text: str, name: str = "") -> None:
         """
         Устанавливает атрибуты для элемента с заданным идентификатором. Этот метод полезен, когда пользователь
             редактирует некоторые существующие значения и типы атрибутов в нескольких парах имя/значение атрибута.
             Например(!не проверено!): await node.SetAttributesAsText("'class: class-name' 'data-id: new data-id'")
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-setAttributesAsText
         :param text:            Текст с рядом атрибутов. Будет анализировать этот текст с помощью HTML-парсера.
         :param name:            (optional) Имя атрибута для замены новыми атрибутами, полученными из текста,
                                     в случае успешного анализа текста.
         :return:
         """
         args = {"nodeId": self.nodeId, "text": text}
         if name:
             args.update({"name": name})
-        await self.page_instance.Call("DOM.setAttributesAsText", args)
+        await self._connection.call("DOM.setAttributesAsText", args)
 
-    async def SetFileInputFiles(self, files: List[str]) -> None:
+    async def setFileInputFiles(self, files: List[str]) -> None:
         """
         Устанавливает файлы для '<input />'- элемента с заданным идентификатором.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-setFileInputFiles
         :param files:           Список файлов. [ "path", "path", ... ]
         :return:
         """
-        await self.page_instance.Call("DOM.setFileInputFiles", {"nodeId": self.nodeId, "files": files})
+        await self._connection.call("DOM.setFileInputFiles", {"nodeId": self.nodeId, "files": files})
 
-    async def SetNewName(self, name: str) -> None:
+    async def setNodeName(self, name: str) -> None:
         """
         Устанавливает новое имя узла для узла. В результате узел получит новый иденификатор.
             Например: await node.SetNewName('span')
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-setNodeName
         :param name:            Новое имя элемента(узла).
         :return:
         """
-        self.nodeId = (await self.page_instance.Call("DOM.setNodeName", {"nodeId": self.nodeId, "name": name}))["nodeId"]
+        self.nodeId = (await self._connection.call("DOM.setNodeName", {"nodeId": self.nodeId, "name": name}))["nodeId"]
 
-    async def SetNewValue(self, value: str) -> None:
+    async def setNodeValue(self, value: str) -> None:
         """
         Устанавливает значение.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-setNodeValue
         :param value:           Новое значение элемента(узла).
         :return:
         """
-        await self.page_instance.Call("DOM.setNodeValue", {"nodeId": self.nodeId, "value": value})
+        await self._connection.call("DOM.setNodeValue", {"nodeId": self.nodeId, "value": value})
 
-    async def SetInspectedNode(self) -> None:
+    async def setInspectedNode(self) -> None:
         """
         Позволяет консоли обращаться к этому узлу с через $ x (см. Более подробную
             информацию о функциях $ x в API командной строки).
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-setInspectedNode
         :return:        None
         """
-        await self.page_instance.Call("DOM.setInspectedNode", {"nodeId": self.nodeId})
+        await self._connection.call("DOM.setInspectedNode", {"nodeId": self.nodeId})
 
-    async def CollectClassNames(self) -> List[str]:
+    async def collectClassNames(self) -> List[str]:
         """
         Собирает имена классов для выбранного узла и всех его потомков.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM/#method-collectClassNamesFromSubtree
         :return:                Список имён классов.
         """
-        return (await self.page_instance.Call("DOM.collectClassNamesFromSubtree", {"nodeId": self.nodeId}))["classNames"]
+        return (await self._connection.call("DOM.collectClassNamesFromSubtree", {"nodeId": self.nodeId}))["classNames"]
 
-    async def GetNodesForSubtreeByStyle(
+    async def getNodesForSubtreeByStyle(
             self, computedStyles: List[dict],
             pierce: bool = False
     ) -> List["Node"]:
         """
         Находит узлы с заданным вычисленным стилем в поддереве текущего узла.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM/#method-getNodesForSubtreeByStyle
         :param computedStyles:  Список вычисляемых CSS-свойств, соответствие которым будет проверяться.
@@ -448,132 +457,130 @@
                                     [{'name': 'width', 'value': '50px'}, {'name': 'height', 'value': '15px'}]
         :param pierce:          (optional) - Следует ли исследовать так же фреймы и shadow-DOM.
         :return:                Список узлов.
         """
         args = {"nodeId": self.nodeId, "computedStyles": computedStyles}
         if pierce: args.update({"pierce": True})
         nodes = []
-        for node_id in (await self.page_instance.Call("DOM.getNodesForSubtreeByStyle", args))["nodeIds"]:
-            nodes.append(Node(node_id, self.page_instance))
+        for node_id in (await self._connection.call("DOM.getNodesForSubtreeByStyle", args))["nodeIds"]:
+            nodes.append(Node(self._connection, node_id))
         return nodes
 
-    async def GetComputedStyle(self) -> List[StyleProp]:
+    async def getComputedStyle(self) -> List[StyleProp]:
         """
         Возвращает список <NodeProp> описывающих свойства указанного Узла.
         https://chromedevtools.github.io/devtools-protocol/tot/CSS/#method-getComputedStyleForNode
         :return:            [ <StyleProp>, ... ]
         """
-        r = (await self.page_instance.Call("CSS.getComputedStyleForNode", {"nodeId": self.nodeId}))["computedStyle"]
+        r = (await self._connection.call("CSS.getComputedStyleForNode", {"nodeId": self.nodeId}))["computedStyle"]
         return [StyleProp(**i) for i in r]
 
-    async def GetInlineStyles(self) -> Dict[str, dict]:
+    async def getInlineStyles(self) -> Dict[str, dict]:
         """
         Возвращает стили, определенные встроенными (явно в атрибуте style и неявно, используя атрибуты DOM) для
             узла DOM, идентифицированного с помощью nodeId.
             !ВНИМАНИЕ! Требует включения уведомлений домена CSS и DOM.
         https://chromedevtools.github.io/devtools-protocol/tot/CSS/#method-getInlineStylesForNode
         :return:            { inlineStyle: {}, attributeStyle: {} }
         """
-        return await self.page_instance.Call("CSS.getInlineStylesForNode", {"nodeId": self.nodeId})
+        return await self._connection.call("CSS.getInlineStylesForNode", {"nodeId": self.nodeId})
 
     # ==================================================================================================================
 
-    async def GetCenter(self) -> NodeCenter:
+    async def getCenter(self) -> NodeCenter:
         """ Возвращает координаты центра узла """
-        quad = (await self.GetContentQuads())[0]
+        quad = (await self.getContentQuads())[0]
         x = (quad[2] - quad[0]) // 2 + quad[0]
         y = (quad[7] - quad[1]) // 2 + quad[1]
         return NodeCenter(x, y)
 
-    async def GetRect(self) -> NodeRect:
+    async def getRect(self) -> NodeRect:
         """ Возвращает <NodeRect> свойств, описывающих пространственное положение узла """
-        q = (await self.GetContentQuads())[0]
+        q = (await self.getContentQuads())[0]
         return NodeRect(q[0], q[1], q[2] - q[0], q[7] - q[1], q[0], q[2], q[1], q[7])
 
-    async def Click(self, delay: float = None, has_link: bool = False) -> None:
+    async def click(self, delay: float = None, has_link: bool = False) -> None:
         """ Кликает в середину себя """
         if has_link:
-            self.page_instance.loading_state = "do_navigate"
-        center = await self.GetCenter()
-        await self.page_instance.action.MouseMoveTo(center.x, center.y)
-        await self.page_instance.action.ClickTo(center.x, center.y, delay)
+            self._connection.Page.loading_state = "do_navigate"
+        center = await self.getCenter()
+        await self._connection.extend.action.mouseMoveTo(center.x, center.y)
+        await self._connection.extend.action.clickTo(center.x, center.y, delay)
 
-    async def Describe(self, depth: Optional[int] = None, pierce: Optional[bool] = None) -> None:
+    async def describeNode(self, depth: Optional[int] = None, pierce: Optional[bool] = None) -> None:
         """
         Переописывает себя получая больше подробностей. Не требует включения домена. Не начинает
             отслеживать какие-либо объекты, можно использовать для автоматизации.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM/#method-describeNode
         :param depth:               Максимальная глубина, на которой должны быть извлечены
                                         дочерние элементы, по умолчанию равна 1. Используйте
                                         -1 для всего поддерева или укажите целое число больше 0.
         :param pierce:              Должны ли проходиться iframes и теневые корни при возврате
                                         поддерева (по умолчанию false).
         :return:            <Node>
         """
         args = dict(nodeId=self.nodeId)
         if depth is not None: args.update(depth=depth)
         if pierce is not None: args.update(pierce=pierce)
-        result = await self.page_instance.Call("DOM.describeNode", args)
+        result = await self._connection.call("DOM.describeNode", args)
         # print("DOM.describeNode", result)
 
         for k, v in result["node"].items():
             if k in ["children", "shadowRoots", "pseudoElements"]:
-                setattr(self, k, self._AddChildren(v))
+                setattr(self, k, self._addChildren(v))
             elif k in ["contentDocument", "templateContent", "importedDocument"]:
-                setattr(self, k, self._AddChild(v))
+                setattr(self, k, self._addChild(v))
             else:
                 setattr(self, k, v)
 
-    async def Resolve(self) -> None:
+    async def resolve(self) -> None:
         """ Получает ссылку на объект JavaScript для ноды. """
         if self.backendNodeId is None:
             raise NodeNotDescribed
         args = dict(backendNodeId=self.contentDocument.backendNodeId)
-        result: dict = await self.page_instance.Call("DOM.resolveNode", args)
+        result: dict = await self._connection.call("DOM.resolveNode", args)
         # print("DOM.resolveNode", result)
-        self.remote_object = RuntimeType.RemoteObject(**result.get("object"))
+        self.remote_object = RemoteObject(**result.get("object"))
 
-    async def Request(self) -> "Node":
+    async def request(self) -> "Node":
         """ Запрашивает ноду по ссылке на её оригинальный JavaScript объект. """
         if self.remote_object is None:
             raise NodeNotResolved
         args = dict(objectId=self.remote_object.objectId)
-        result: dict = await self.page_instance.Call("DOM.requestNode", args)
+        result: dict = await self._connection.call("DOM.requestNode", args)
         # print(result)
         return Node(
-            self.page_instance, result.get("nodeId"),
+            self._connection, result.get("nodeId"),
             frameId=self.frameId,
             nodeName=self.nodeName,
             localName=self.localName,
             attributes=self.attributes,
             contentDocument=self.contentDocument
         )
 
-    async def RequestMirror(self) -> "Node":
+    async def requestMirror(self) -> "Node":
         """
         Создаёт JavaScript-объект для этой ноды и запрашивает ноду по ссылке на этот объект.
             Таким образом можно получать ноды для изолированных DOM-элементов, вроде iframe.
             Например:
                 frame_node = await page.QuerySelector("iframe")     # находим iframe
                 resolved_node = await frame_node.RequestMirror()    # получаем доступ к нему
                 needle_node = resolved_node.QuerySelector("#needle-selector-in-iframe")
         """
-        await self.Describe()
-        await self.Resolve()
-        return await self.Request()
+        await self.describeNode()
+        await self.resolve()
+        return await self.request()
 
-    async def BuildScript(self, expression: str) -> "Script":
-        if not self.page_instance.runtime_enabled:
+    async def buildScript(self, expression: str) -> Script:
+        if not self._connection.Runtime.enabled:
             raise StateError("Domain 'Runtime' — must be enabled. Like: "
-                             "await instance.RuntimeEnable(True)")
-        if not self.page_instance.context_manager.is_watch:
+                             "await conn.Runtime.enable(True)")
+        if not self._connection.context_manager.is_watch:
             raise StateError("Watch for execution contexts must be enabled with domain 'Runtime'. Like: "
-                             "await instance.RuntimeEnable(True)")
+                             "await conn.Runtime.enable(True)")
         if not self.frameId:
-            await self.Describe()
-        if not (context := self.page_instance.context_manager.GetDefaultContext(
-                self.frameId or self.page_instance.page_id)):
+            await self.describeNode()
+        if not (context := self._connection.context_manager.GetDefaultContext(
+                self.frameId or self._connection.conn_id)):
             raise StateError("Something went wrong, or context was not obtained on creation.")
 
-        return Script(self.page_instance, expression, context)
-
-
+        return Script(self._connection, expression, context)
```

### Comparing `aio_dt_protocol-0.9.5/aio_dt_protocol/Page.py` & `aio_dt_protocol-1.0.0/aio_dt_protocol/connection.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,154 +1,173 @@
 try:
     import ujson as json
 except ModuleNotFoundError:
     import json
 import asyncio
-import websockets.client
+from websockets.client import WebSocketClientProtocol, connect
 
 from .exceptions import EvaluateError, get_cdtp_error, highlight_eval_error, PromiseEvaluateError, \
     highlight_promise_error
 from .utils import log
 
 from websockets.exceptions import ConnectionClosedError
 from inspect import iscoroutinefunction
 from typing import Callable, Awaitable, Optional, Union, Tuple, List, Dict
-from abc import ABC
-from .Data import DomainEvent, Sender, Receiver, CommonCallback
+from .data import DomainEvent, Sender, Receiver, CommonCallback
+from .extend_connection import Extend
 
-
-class AbsPage(ABC):
+from .domains.background_service import BackgroundService
+from .domains.browser import Browser
+from .domains.css import CSS
+from .domains.device_orientation import DeviceOrientation
+from .domains.dom import DOM
+from .domains.emulation import Emulation
+from .domains.fetch import Fetch
+from .domains.input import Input
+from .domains.log import Log
+from .domains.network import Network
+from .domains.overlay import Overlay
+from .domains.page import Page
+from .domains.runtime import Runtime
+from .domains.system_info import SystemInfo
+from .domains.target import Target
+
+
+class Connection:
+    """ Если инстанс страницы более не нужен, например, при перезаписи в него нового
+    инстанса, перед этим [-!-] ОБЯЗАТЕЛЬНО [-!-] - вызовите у него метод
+    Detach(), или закройте вкладку/страницу браузера, с которой он связан,
+    тогда это будет выполнено автоматом. Иначе в цикле событий останутся
+    задачи связанные с поддержанием соединения, которое более не востребовано.
+    """
     __slots__ = (
-        "ws_url", "page_id", "frontend_url", "callback", "is_headless_mode", "verbose", "browser_name", "id",
-        "responses", "connected", "ws_session", "receiver", "on_detach_listener", "listeners", "listeners_for_event",
-        "runtime_enabled", "on_close_event", "context_manager", "_connected", "_page_id", "_verbose",
-        "_browser_name", "_is_headless_mode"
-    )
+        "ws_url", "frontend_url", "callback", "_id", "extend",
+        "responses", "ws_session", "receiver", "on_detach_listener", "listeners", "listeners_for_event",
+        "on_close_event", "context_manager", "_connected", "_conn_id", "_verbose",
+        "_browser_name", "_is_headless_mode",
 
-    def __init__(
-        self,
-        ws_url:           str,
-        page_id:          str,
-        frontend_url:     str,
-        callback:         CommonCallback,
-        is_headless_mode: bool,
-        verbose:          bool,
-        browser_name:     str
-    ) -> None:
-        self.ws_url            = ws_url
-        self.page_id           = page_id
-        self.frontend_url      = frontend_url
-        self.callback          = callback
-        self.is_headless_mode  = is_headless_mode
-
-        self.verbose           = verbose
-        self.browser_name      = browser_name
-
-        self.id                = 0
-        self.connected         = False
-        self.ws_session        = None
-        self.receiver          = None
-        self.on_detach_listener: List[Callable[[any], Awaitable[None]], list, dict] = []
-        self.listeners         = {}
-        self.listeners_for_event = {}
-        self.runtime_enabled     = False
-        self.on_close_event = asyncio.Event()
-        self.responses: Dict[int, Optional[Sender[dict]]] = {}
-
-
-class Page(AbsPage):
-    """
-    Инстанс страницы должен быть активирован после создания вызовом метода Activate(),
-        это создаст подключение по WebSocket и запустит задачи обеспечивающие
-        обратную связь. Метод GetPageBy() инстанса браузера, заботится об этом
-        по умолчанию.
-
-    Если инстанс страницы более не нужен, например, при перезаписи в него нового
-        инстанса, перед этим [-!-] ОБЯЗАТЕЛЬНО [-!-] - вызовите у него метод
-        Detach(), или закройте вкладку/страницу браузера, с которой он связан,
-        тогда это будет выполнено автоматом. Иначе в цикле событий останутся
-        задачи связанные с поддержанием соединения, которое более не востребовано.
-    """
-    __slots__ = ()
+        "BackgroundService", "Browser", "CSS", "DeviceOrientation", "DOM", "Emulation", "Fetch", "Input",
+        "Log", "Network", "Overlay", "Page", "Runtime", "SystemInfo", "Target",
+    )
 
     def __init__(
-        self,
-        ws_url:           str,
-        page_id:          str,
-        frontend_url:     str,
-        callback:         CommonCallback,
-        is_headless_mode: bool,
-        verbose:          bool,
-        browser_name:     str
+            self,
+            ws_url: str,
+            conn_id: str,
+            frontend_url: str,
+            callback: CommonCallback,
+            is_headless_mode: bool,
+            verbose: bool,
+            browser_name: str
     ) -> None:
         """
         :param ws_url:              Адрес WebSocket
-        :param page_id:             Идентификатор страницы
+        :param conn_id:             Идентификатор страницы
         :param frontend_url:        devtoolsFrontendUrl по которому происходит подключение к дебаггеру
         :param callback:            Колбэк, который будет получать все данные,
                                         приходящие по WebSocket в виде словарей
         :param is_headless_mode:    "Headless" включён?
         :param verbose:             Печатать некие подробности процесса?
         :param browser_name:        Имя браузера
         """
-        AbsPage.__init__(self, ws_url, page_id, frontend_url, callback, is_headless_mode, verbose, browser_name)
 
-    @property
-    def connected(self) -> bool: return self._connected
+        self.ws_url = ws_url
+        self._conn_id = conn_id
+        self.frontend_url = frontend_url
+        self.callback = callback
+        self._is_headless_mode = is_headless_mode
+
+        self._verbose = verbose
+        self._browser_name = browser_name
+
+        self._id = 0
+        self._connected = False
+        self.ws_session: Optional[WebSocketClientProtocol] = None
+        self.receiver: Optional[asyncio.Task] = None
+        self.on_detach_listener: List[Callable[[any], Awaitable[None]], list, dict] = []
+        self.listeners = {}
+        self.listeners_for_event = {}
+        self.on_close_event = asyncio.Event()
+        self.responses: Dict[int, Optional[Sender[dict]]] = {}
+
+        self.extend = Extend(self)
+
+        self.BackgroundService = BackgroundService(self)
+        self.Browser = Browser(self)
+        self.CSS = CSS(self)
+        self.DeviceOrientation = DeviceOrientation(self)
+        self.DOM = DOM(self)
+        self.Emulation = Emulation(self)
+        self.Fetch = Fetch(self)
+        self.Input = Input(self)
+        self.Log = Log(self)
+        self.Network = Network(self)
+        self.Overlay = Overlay(self)
+        self.Page = Page(self)
+        self.Runtime = Runtime(self)
+        self.SystemInfo = SystemInfo(self)
+        self.Target = Target(self)
 
-    @connected.setter
-    def connected(self, value) -> None: self._connected = value
 
     @property
-    def page_id(self) -> str: return self._page_id
+    def connected(self) -> bool:
+        return self._connected
 
-    @page_id.setter
-    def page_id(self, value) -> None: self._page_id = value
+    @property
+    def conn_id(self) -> str:
+        return self._conn_id
 
     @property
-    def verbose(self) -> bool: return self._verbose
+    def verbose(self) -> bool:
+        return self._verbose
 
     @verbose.setter
-    def verbose(self, value) -> None: self._verbose = value
+    def verbose(self, value: bool) -> None:
+        self._verbose = value
 
     @property
-    def browser_name(self) -> str: return self._browser_name
-
-    @browser_name.setter
-    def browser_name(self, value) -> None: self._browser_name = value
+    def browser_name(self) -> str:
+        return self._browser_name
 
     @property
-    def is_headless_mode(self) -> bool: return self._is_headless_mode
+    def is_headless_mode(self) -> bool:
+        return self._is_headless_mode
 
-    @is_headless_mode.setter
-    def is_headless_mode(self, value) -> None: self._is_headless_mode = value
+    def __str__(self) -> str:
+        return f"<Connection targetId={self.conn_id!r}>"
 
-    async def Call(
+    def __eq__(self, other: "Connection") -> bool:
+        return self.conn_id == other.conn_id
+
+    def __hash__(self) -> int:
+        return hash(self.conn_id)
+
+    async def call(
         self, domain_and_method: str,
         params:  Optional[dict] = None,
         wait_for_response: bool = True
     ) -> Optional[dict]:
-        self.id += 1
-        _id = self.id
+        self._id += 1
+        _id = self._id
         data = {
             "id": _id,
             "params": params if params else {},
             "method": domain_and_method
         }
 
         if not wait_for_response:
             self.responses[_id] = None
-            await self._Send(json.dumps(data))
+            await self._send(json.dumps(data))
             return
 
         que = asyncio.Queue()
         sender, receiver = Sender[dict](que), Receiver[dict](que)
         self.responses[_id] = sender
 
-        await self._Send(json.dumps(data))
+        await self._send(json.dumps(data))
 
         response = await receiver.recv()
         if "error" in response:
 
             if ex := get_cdtp_error(response['error']['message']):
                 raise ex(f"domain_and_method = '{domain_and_method}' | params = '{str(params)}'")
 
@@ -157,24 +176,24 @@
                 f"error code -> '{response['error']['code']}';\n" +
                 f"error message -> '{response['error']['message']}'\n"+
                 f"domain_and_method = '{domain_and_method}' | params = '{str(params)}'"
             )
 
         return response["result"]
 
-    async def Eval(
+    async def eval(
         self, expression: str,
         objectGroup:            str = "console",
         includeCommandLineAPI: bool = True,
         silent:                bool = False,
         returnByValue:         bool = False,
         userGesture:           bool = True,
         awaitPromise:          bool = False
     ) -> dict:
-        response = await self.Call(
+        response = await self.call(
             "Runtime.evaluate", {
                 "expression": expression,
                 "objectGroup": objectGroup,
                 "includeCommandLineAPI": includeCommandLineAPI,
                 "silent": silent,
                 "returnByValue": returnByValue,
                 "userGesture": userGesture,
@@ -183,32 +202,32 @@
         )
         if "exceptionDetails" in response:
             raise EvaluateError(
                 highlight_eval_error(response["result"]["description"], expression)
             )
         return response["result"]
 
-    async def _Send(self, data: str) -> None:
+    async def _send(self, data: str) -> None:
         if self.connected:
             await self.ws_session.send(data)
 
-    async def _Recv(self) -> None:
+    async def _recv(self) -> None:
         while self.connected:
             try:
                 data_msg: dict = json.loads(await self.ws_session.recv())
             # ! Браузер разорвал соединение
             except ConnectionClosedError as e:
                 if self.verbose: log(f"ConnectionClosedError {e!r}")
-                await self.Detach()
+                await self.detach()
                 return
 
             if ("method" in data_msg and data_msg["method"] == "Inspector.detached"
                     and data_msg["params"]["reason"] == "target_closed"):
                 self.on_close_event.set()
-                await self.Detach()
+                await self.detach()
                 return
 
             # Ожидающие ответов вызовы API получают ответ по id входящих сообщений.
             if sender := self.responses.pop(data_msg.get("id"), None):
                 await sender.send(data_msg)
 
             # Если коллбэк функция была определена, она будет получать все
@@ -265,77 +284,77 @@
                     asyncio.create_task(
                         listener(                                           # корутина
                             p if p is not None else {},                     # её "params" — всегда передаётся
                             *args                                           # список bind-агрументов
                         )
                     )
 
-    async def EvalPromise(self, script: str) -> dict:
+    async def evalPromise(self, script: str) -> dict:
         """ Выполняет асинхронный код на странице и возвращает результат.
         !!! ВАЖНО !!! Выполняемый код не может возвращать какие-либо JS
         типы, поэтому должен возвращать JSON-сериализованный набор данных.
         """
-        result = await self.Eval(script)
+        result = await self.eval(script)
         args = dict(
             promiseObjectId=result["objectId"],
             returnByValue=False,
             generatePreview=False
         )
-        response = await self.Call("Runtime.awaitPromise", args)
+        response = await self.Runtime.awaitPromise(**args)
         if "exceptionDetails" in response:
             raise PromiseEvaluateError(
                 highlight_promise_error(response["result"]["description"]) +
                 "\n" + json.dumps(response["exceptionDetails"])
             )
         return json.loads(response["result"]["value"])
 
-    async def WaitForClose(self) -> None:
+    async def waitForClose(self) -> None:
         """ Дожидается, пока не будет потеряно соединение со страницей. """
         await self.on_close_event.wait()
 
-    async def Detach(self) -> None:
+    async def activate(self) -> None:
+        self.ws_session = await connect(self.ws_url, ping_interval=None)
+        self._connected = True
+        self.receiver = asyncio.create_task(self._recv())
+        if self.callback is not None:
+            await self.Runtime.enable()
+
+    async def detach(self) -> None:
         """
         Отключается от инстанса страницы. Вызывается автоматически при закрытии браузера,
             или инстанса текущей страницы. Принудительный вызов не закрывает страницу,
             а лишь разрывает с ней соединение.
         """
         if not self.connected:
             return
 
         self.receiver.cancel()
-        if self.verbose: log(f"[ DETACH ] {self.page_id}")
-        self.connected = False
+        if self.verbose: log(f"[ DETACH ] {self.conn_id}")
+        self._connected = False
 
         if self.on_detach_listener:
             function, args, kvargs = self.on_detach_listener
             await function(*args, **kvargs)
 
-    def RemoveOnDetach(self) -> None:
+    def removeOnDetach(self) -> None:
         self.on_detach_listener = []
 
-    def SetOnDetach(self, function: Callable[[any], Awaitable[None]], *args, **kvargs) -> bool:
+    def setOnDetach(self, function: Callable[[any], Awaitable[None]], *args, **kvargs) -> bool:
         """
         Регистрирует асинхронный коллбэк, который будет вызван с соответствующими аргументами
             при разрыве соединения со страницей.
         """
         if not iscoroutinefunction(function):
             raise TypeError("OnDetach-listener must be a async callable object!")
-        if not self.connected: return False
+        if not self.connected:
+            return False
         self.on_detach_listener = [function, args, kvargs]
         return True
 
-    async def Activate(self) -> None:
-        self.ws_session = await websockets.client.connect(self.ws_url, ping_interval=None)
-        self.connected = True
-        self.receiver = asyncio.create_task(self._Recv())
-        if self.callback is not None:
-            await self.Call("Runtime.enable")
-            self.runtime_enabled = True
-
-    async def AddListener(self, listener: Callable[[any], Awaitable[None]], *args: any) -> None:
+    async def addListener(self, listener: Callable[[any], Awaitable[None]], *args: any) -> None:
         """
         Добавляет 'слушателя', который будет ожидать свой вызов по имени функции.
             Вызов слушателей из контекста страницы осуществляется за счёт
             JSON-сериализованного объекта, отправленного сообщением в консоль,
             через домен 'info'. Объект должен содержать два обязательных свойства:
                 funcName — имя вызываемого слушателя
                 args:    — массив аргументов
@@ -359,48 +378,46 @@
                                     в функцию последними.
         :return:        None
         """
         if not iscoroutinefunction(listener):
             raise TypeError("Listener must be a async callable object!")
         if listener.__name__ not in self.listeners:
             self.listeners[ listener.__name__ ] = {"function": listener, "args": args}
-            if not self.runtime_enabled:
-                await self.Call("Runtime.enable")
-                self.runtime_enabled = True
+            if not self.Runtime.enabled:
+                await self.Runtime.enable()
 
-    async def AddListeners(
+    async def addListeners(
             self, *list_of_tuple_listeners_and_args: Tuple[Callable[[any], Awaitable[None]], list]) -> None:
         """
         Делает то же самое, что и AddListener(), но может зарегистрировать сразу несколько слушателей.
             Принимает список кортежей с двумя элементами, вида (async_func_or_method, list_args), где:
                 async_func_or_method    - асинхронная фукция или метод
                 list_args               - список её аргументов(может быть пустым)
         """
         for action in list_of_tuple_listeners_and_args:
             listener, args = action
             if not iscoroutinefunction(listener):
                 raise TypeError("Listener must be a async callable object!")
             if listener.__name__ not in self.listeners:
                 self.listeners[listener.__name__] = {"function": listener, "args": args}
-                if not self.runtime_enabled:
-                    await self.Call("Runtime.enable")
-                    self.runtime_enabled = True
+                if not self.Runtime.enabled:
+                    await self.Runtime.enable()
 
-    def RemoveListener(self, listener: Callable[[any], Awaitable[None]]) -> None:
+    def removeListener(self, listener: Callable[[any], Awaitable[None]]) -> None:
         """
         Удаляет слушателя.
         :param listener:        Колбэк-функция.
         :return:        None
         """
         if not iscoroutinefunction(listener):
             raise TypeError("Listener must be a async callable object!")
         if listener.__name__ in self.listeners:
             del self.listeners[ listener.__name__ ]
 
-    async def AddListenerForEvent(
+    async def addListenerForEvent(
         self, event: Union[str, DomainEvent], listener: Callable[[any], Awaitable[None]], *args) -> None:
         """
         Регистирует слушателя, который будет вызываться при вызове определённых событий
             в браузере. Список таких событий можно посмотреть в разделе "Events" почти
             у каждого домена по адресу: https://chromedevtools.github.io/devtools-protocol/
             Например: 'DOM.attributeModified'
         !Внимание! Каждый такой слушатель должен иметь один обязательный 'data'-аргумент,
@@ -415,38 +432,37 @@
         """
         e = event if type(event) is str else event.value
         if not iscoroutinefunction(listener):
             raise TypeError("Listener must be a async callable object!")
         if e not in self.listeners_for_event:
             self.listeners_for_event[ e ]: dict = {}
         self.listeners_for_event[ e ][listener] = args
-        if not self.runtime_enabled:
-            await self.Call("Runtime.enable")
-            self.runtime_enabled = True
+        if not self.Runtime.enabled:
+            await self.Runtime.enable()
 
-    def RemoveListenerForEvent(
+    def removeListenerForEvent(
             self, event: Union[str, DomainEvent], listener: Callable[[any], Awaitable[None]]) -> None:
         """
         Удаляет регистрацию слушателя для указанного события.
         :param event:           Имя метода, для которого была регистрация.
         :param listener:        Колбэк-функция, которую нужно удалить.
         :return:        None
         """
         e = event if type(event) is str else event.value
         if not iscoroutinefunction(listener):
             raise TypeError("Listener must be a async callable object!")
         if m := self.listeners_for_event.get( e ):
             if listener in m: m.pop(listener)
 
 
-    def RemoveListenersForEvent(self, event: Union[str, DomainEvent]) -> None:
+    def removeListenersForEvent(self, event: Union[str, DomainEvent]) -> None:
         """
         Удаляет регистрацию метода и слушателей вместе с ним для указанного события.
         :param event:          Имя метода, для которого была регистрация.
         :return:        None
         """
         e = event if type(event) is str else event.value
         if e in self.listeners_for_event:
             self.listeners_for_event.pop(e)
 
     def __del__(self) -> None:
-        if self.verbose: log(f"[ DELETED ] {self.page_id}")
+        if self.verbose: log(f"[ DELETED ] {self.conn_id}")
```

### Comparing `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/BackgroundService.py` & `aio_dt_protocol-1.0.0/aio_dt_protocol/domains/background_service/background_service.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,65 @@
-from abc import ABC, abstractmethod
-from typing import Optional, Union
-from ..Data import DomainEvent
+from ...data import DomainEvent
 
-class BackgroundService(ABC):
+class BackgroundService:
     """
     #   https://chromedevtools.github.io/devtools-protocol/tot/BackgroundService
     """
-    __slots__ = ()
+    __slots__ = ("_connection", "observing_started", "recording_started")
 
-    def __init__(self):
+    def __init__(self, conn) -> None:
+
+        from ...connection import Connection
+
+        self._connection: Connection = conn
         self.observing_started = False
         self.recording_started = False
 
-    @property
-    def connected(self) -> bool:
-        return False
-
-    @property
-    def verbose(self) -> bool:
-        return False
-
-    @property
-    def page_id(self) -> str:
-        return ""
-
-    async def BackgroundClearEvents(self, service: str) -> None:
+    async def backgroundClearEvents(self, service: str) -> None:
         """
         Удаляет все сохраненные данные для service.
         https://chromedevtools.github.io/devtools-protocol/tot/BackgroundService/#method-clearEvents
         :param service:         Фоновая служба, которая будет связана с командами / событиями. Каждая фоновая
                                     служба работает независимо, но использует один и тот же API.
                                 Допустимые значения:
                                     backgroundFetch, backgroundSync, pushMessaging, notifications,
                                     paymentHandler,periodicBackgroundSync
         :return:
         """
-        await self.Call("BackgroundService.clearEvents", {"service": service})
+        await self._connection.call("BackgroundService.clearEvents", {"service": service})
 
-    async def BackgroundSetRecording(self, shouldRecord: bool, service: str) -> None:
+    async def backgroundSetRecording(self, shouldRecord: bool, service: str) -> None:
         """
         Включает, или выключает запись для service.
         https://chromedevtools.github.io/devtools-protocol/tot/BackgroundService/#method-setRecording
         :param shouldRecord:    True == включить
         :param service:         ---------------------
         :return:
         """
-        await self.Call("BackgroundService.clearEvents", {"shouldRecord": shouldRecord, "service": service})
+        await self._connection.call("BackgroundService.clearEvents", {"shouldRecord": shouldRecord, "service": service})
         self.recording_started = shouldRecord
 
-    async def BackgroundStartObserving(self, service: str) -> None:
+    async def backgroundStartObserving(self, service: str) -> None:
         """
         Включает обновления событий для service.
         https://chromedevtools.github.io/devtools-protocol/tot/BackgroundService/#method-startObserving
         :param service:         ---------------------
         :return:
         """
         if not self.observing_started:
-            await self.Call("BackgroundService.startObserving", {"service": service})
+            await self._connection.call("BackgroundService.startObserving", {"service": service})
             self.observing_started = True
 
-    async def BackgroundStopObserving(self, service: str) -> None:
+    async def backgroundStopObserving(self, service: str) -> None:
         """
         Выключает обновления событий для service.
         https://chromedevtools.github.io/devtools-protocol/tot/BackgroundService/#method-stopObserving
         :param service:         ---------------------
         :return:
         """
         if self.observing_started:
-            await self.Call("BackgroundService.stopObserving", {"service": service})
+            await self._connection.call("BackgroundService.stopObserving", {"service": service})
             self.observing_started = False
 
-    @abstractmethod
-    async def Call(
-            self, domain_and_method: str,
-            params: Optional[dict] = None,
-            wait_for_response: bool = True
-    ) -> Union[dict, None]: raise NotImplementedError("async method Call() — is not implemented")
-
 class BackgroundServiceEvent(DomainEvent):
     backgroundServiceEventReceived = "BackgroundService.backgroundServiceEventReceived"
     recordingStateChanged = "BackgroundService.recordingStateChanged"
```

### Comparing `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Browser.py` & `aio_dt_protocol-1.0.0/aio_dt_protocol/domains/browser/browser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,25 @@
-from abc import ABC, abstractmethod
-from typing import Optional, Union, Dict, List
-from ..Data import WindowBounds, WindowInfo
-from ..Data import DomainEvent
+from typing import Optional, List
+from ...data import DomainEvent
+from .types import Version, Bounds, WindowInfo
 
-class Browser(ABC):
+
+class Browser:
     """
     #   https://chromedevtools.github.io/devtools-protocol/tot/Browser/
     """
-    __slots__ = ()
+    __slots__ = ("_connection",)
 
-    @property
-    def connected(self) -> bool:
-        return False
+    def __init__(self, conn) -> None:
 
-    @property
-    def verbose(self) -> bool:
-        return False
+        from ...connection import Connection
 
-    @property
-    def page_id(self) -> str:
-        return ""
+        self._connection: Connection = conn
 
-    async def SetPermission(
+    async def setPermission(
             self, permission: dict, setting: str, origin: str = None,
             browserContextId: str = None
     ) -> None:
         """
         (EXPERIMENTAL)
         Устанавливает настройки разрешений для данного источника.
         https://chromedevtools.github.io/devtools-protocol/tot/Browser#method-setPermission
@@ -55,17 +49,17 @@
         :return:
         """
         args = {"permission": permission, "setting": setting}
         if origin is not None:
             args.update({"origin": origin})
         if browserContextId is not None:
             args.update({"browserContextId": browserContextId})
-        await self.Call("Browser.setPermission", args)
+        await self._connection.call("Browser.setPermission", args)
 
-    async def GrantPermissions(
+    async def grantPermissions(
             self, permissions: List[str],
             origin: Optional[str] = None,
             browserContextId: Optional[str] = None
     ) -> None:
         """
         (EXPERIMENTAL)
         Предоставляет определенные разрешения данному источнику, отклоняя все остальные.
@@ -83,44 +77,45 @@
         :return:
         """
         args = {"permissions": permissions}
         if origin is not None:
             args.update({"origin": origin})
         if browserContextId is not None:
             args.update({"browserContextId": browserContextId})
-        await self.Call("Browser.grantPermissions", args)
+        await self._connection.call("Browser.grantPermissions", args)
 
-    async def ResetPermissions(self, browserContextId: Optional[str] = None) -> None:
+    async def resetPermissions(self, browserContextId: Optional[str] = None) -> None:
         """
         Сбросить все управление разрешениями для всех источников.
         https://chromedevtools.github.io/devtools-protocol/tot/Browser#method-resetPermissions
         :param browserContextId:    (optional) Контекст для переопределения. Если не указано, используется
                                         контекст браузера по умолчанию.
         :return:
         """
         args = {}
         if browserContextId is not None:
             args.update({"browserContextId": browserContextId})
-        await self.Call("Browser.resetPermissions", args)
+        await self._connection.call("Browser.resetPermissions", args)
 
-    async def GetVersion(self) -> Dict[str, str]:
+    async def getVersion(self) -> Version:
         """
         Возвращает словарь с информацией о текущем билде браузера.
         https://chromedevtools.github.io/devtools-protocol/tot/Browser#method-getVersion
         :return:                {
                                     "protocolVersion":  str( ... ), -> Protocol version.
                                     "product":          str( ... ), -> Product name.
                                     "revision":         str( ... ), -> Product revision.
                                     "userAgent":        str( ... ), -> User-Agent.
                                     "jsVersion":        str( ... )  -> V8 version.
                                 }
         """
-        return await self.Call("Browser.getVersion")
+        return Version(
+            **(await self._connection.call("Browser.getVersion")))
 
-    async def GetWindowBounds(self, windowId: int = None) -> WindowBounds:
+    async def getWindowBounds(self, windowId: int = None) -> Bounds:
         """
         (EXPERIMENTAL)
         Возвращает позицию и размер окна.
         https://chromedevtools.github.io/devtools-protocol/tot/Browser#method-getWindowBounds
         :param windowId:        Идентификатор окна браузера.
         :return:                {
                                     "left":       int(), -> (optional) Смещение от левого
@@ -130,35 +125,36 @@
                                     "width":      int(), -> (optional) Ширина окна в пикселях.
                                     "height":     int(), -> (optional) Высота окна в пикселях
                                     "windowState": str() -> (optional) normal, minimized,
                                                                 maximized, fullscreen
                                 }
         """
         if windowId is None:
-            windowId = (await self.GetWindowForTarget()).windowId
-        return WindowBounds(**(await self.Call("Browser.getWindowBounds", {"windowId": windowId}))["bounds"])
+            windowId = (await self._connection.Target.getWindowForTarget()).windowId
+        return Bounds(
+            **(await self._connection.call("Browser.getWindowBounds", {"windowId": windowId}))["bounds"])
 
-    async def GetWindowForTarget(self, targetId: Optional[str] = None) -> WindowInfo:
+    async def getWindowForTarget(self, targetId: Optional[str] = None) -> WindowInfo:
         """
         (EXPERIMENTAL)
         Возвращает идентификатор, а так же позицию и размер окна.
         https://chromedevtools.github.io/devtools-protocol/tot/Browser#method-getWindowForTarget
         :param targetId:        (optional) Идентификатор хоста агента Devtools. Если вызывается
                                     как часть сеанса, используется связанный targetId.
         :return:                {
                                     "windowId": int(), -> Идентификатор окна.
                                     "bounds":   dict() -> То же, что возвращает GetWindowBounds().
                                 }
         """
         if targetId is None:
-            targetId = self.page_id
-        result = await self.Call("Browser.getWindowForTarget", {"targetId": targetId})
-        return WindowInfo(windowId=result["windowId"], bounds=WindowBounds(**result["bounds"]))
+            targetId = self._connection.conn_id
+        result = await self._connection.call("Browser.getWindowForTarget", {"targetId": targetId})
+        return WindowInfo(windowId=result["windowId"], bounds=Bounds(**result["bounds"]))
 
-    async def SetDockTile(self, badgeLabel: Optional[str] = None, image: Optional[str] = None) -> None:
+    async def setDockTile(self, badgeLabel: Optional[str] = None, image: Optional[str] = None) -> None:
         """
         (EXPERIMENTAL)
         Задать сведения о док-плитке для конкретной платформы.
         https://chromedevtools.github.io/devtools-protocol/tot/Browser#method-setDockTile
         :param badgeLabel:      (optional) Значок метки(?)
         :param image:           (optional) PNG кодированное изображение.
         :return:
@@ -166,17 +162,17 @@
         args = {}
         if badgeLabel is not None:
             args.update({"badgeLabel": badgeLabel})
         if image is not None:
             args.update({"image": image})
         if not args:
             return
-        await self.Call("Browser.setDockTile", args)
+        await self._connection.call("Browser.setDockTile", args)
 
-    async def SetDownloadBehavior(
+    async def setDownloadBehavior(
             self, behavior: str,
             browserContextId: Optional[str] = None,
             downloadPath: Optional[str] = None,
             eventsEnabled: Optional[bool] = None
     ) -> None:
         """
         Устанавливает поведение при загрузке файлов.
@@ -191,30 +187,24 @@
         :param eventsEnabled:       (optional) Если не указано, используется контекст браузера по умолчанию.
         :return:
         """
         args = {"behavior": behavior}
         if browserContextId is not None: args.update(browserContextId=browserContextId)
         if downloadPath is not None: args.update(downloadPath=downloadPath)
         if eventsEnabled is not None: args.update(eventsEnabled=eventsEnabled)
-        await self.Call("Browser.setDownloadBehavior", args)
+        await self._connection.call("Browser.setDownloadBehavior", args)
 
-    async def CloseBrowser(self) -> bool:
+    async def close(self) -> bool:
         """
         Изящно завершает работу браузера.
         https://chromedevtools.github.io/devtools-protocol/tot/Browser#method-close
         :return:        Закрылся/был закрыт
         """
-        if self.connected:
-            await self.Call("Browser.close")
+        if self._connection.connected:
+            await self._connection.call("Browser.close")
             return True
         return False
 
-    @abstractmethod
-    async def Call(
-            self, domain_and_method: str,
-            params: Optional[dict] = None,
-            wait_for_response: bool = True
-    ) -> Union[dict, None]: raise NotImplementedError("async method Call() — is not implemented")
 
 class BrowserEvent(DomainEvent):
     downloadProgress = "Browser.downloadProgress"
     downloadWillBegin = "Browser.downloadWillBegin"
```

### Comparing `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/CSS.py` & `aio_dt_protocol-1.0.0/aio_dt_protocol/domains/css/css.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,71 +1,64 @@
-from abc import ABC, abstractmethod
-from typing import Optional, Union, Callable, List
-from ..Data import DomainEvent
+from typing import List
+from ...data import DomainEvent
 
-class CSS(ABC):
+
+class CSS:
     """
     #   https://chromedevtools.github.io/devtools-protocol/tot/Log
     #   LogEntry -> https://chromedevtools.github.io/devtools-protocol/tot/Log#type-LogEntry
     """
-    __slots__ = ()
-
-    def __init__(self):
-        self.css_domain_enabled = False
-        self.style_sheets = []  # Если домен CSS активирован, сюда попадут все 'styleSheetId' страницы
+    __slots__ = ("_connection", "enabled", "_style_sheets")
 
-    @property
-    def connected(self) -> bool:
-        return False
+    def __init__(self, conn) -> None:
 
-    @property
-    def verbose(self) -> bool:
-        return False
+        from ...connection import Connection
 
-    @property
-    def page_id(self) -> str:
-        return ""
+        self._connection: Connection = conn
+        self.enabled = False
+        self._style_sheets: List[str] = []  # Если домен CSS активирован, сюда попадут все 'styleSheetId' страницы
 
     @property
-    def style_sheets(self) -> list:
+    def style_sheets(self) -> List[str]:
         return self._style_sheets
 
     @style_sheets.setter
     def style_sheets(self, value) -> None:
         self._style_sheets = value
 
     async def _CSS_sheet_catcher(self, data: dict) -> None:
         """
         Колбэк вызываемый для каждого 'CSS.styleSheetAdded'-события, если
             включён агент домена 'CSS'.
         """
-        self.style_sheets.append(data["header"]["styleSheetId"])
+        self._style_sheets.append(data["header"]["styleSheetId"])
 
     async def CSSEnable(self) -> None:
         """
         Включает агент CSS. Клиент не должен предполагать, что агент CSS включен,
             пока не будет получен результат этой команды.
         https://chromedevtools.github.io/devtools-protocol/tot/CSS/#method-disable
         :return:
         """
-        if not self.css_domain_enabled:
-            await self.AddListenerForEvent("CSS.styleSheetAdded", self._CSS_sheet_catcher)
-            await self.Call("CSS.enable")
-            self.css_domain_enabled = True
+        if not self.enabled:
+            await self._connection.addListenerForEvent("CSS.styleSheetAdded", self._CSS_sheet_catcher)
+            await self._connection.call("CSS.enable")
+            self.enabled = True
 
     async def CSSDisable(self) -> None:
         """
         Отключает агент CSS.
         https://chromedevtools.github.io/devtools-protocol/tot/CSS/#method-disable
         :return:
         """
-        if self.css_domain_enabled:
-            self.RemoveListenerForEvent("CSS.styleSheetAdded", self._CSS_sheet_catcher)
-            await self.Call("CSS.disable")
-            self.css_domain_enabled = False
+        if self.enabled:
+            self._connection.removeListenerForEvent("CSS.styleSheetAdded", self._CSS_sheet_catcher)
+            await self._connection.call("CSS.disable")
+            self.style_sheets = []
+            self.enabled = False
 
     async def AddRule(
         self, styleSheetId: str, ruleText: str,
         startLine:   int = 0,
         startColumn: int = 0,
         endLine:     int = 0,
         endColumn:   int = 0
@@ -86,63 +79,47 @@
         """
         location = {"startLine": startLine, "startColumn": startColumn, "endLine": endLine, "endColumn": endColumn}
         args = {
             "styleSheetId": styleSheetId,
             "ruleText": ruleText,
             "location": location
         }
-        return (await self.Call("CSS.addRule", args))["rule"]
+        return (await self._connection.call("CSS.addRule", args))["rule"]
 
     async def CollectClassNames(self, styleSheetId: str) -> List[str]:
         """
         Возвращает список всех имён классов для указанного ID.
         https://chromedevtools.github.io/devtools-protocol/tot/CSS/#method-collectClassNames
         :param styleSheetId:            Идентификатор стилей.
         :return:
         """
-        return (await self.Call("CSS.collectClassNames", {"styleSheetId": styleSheetId}))["classNames"]
+        return (await self._connection.call("CSS.collectClassNames", {"styleSheetId": styleSheetId}))["classNames"]
 
     async def CreateStyleSheet(self, frameId: str = None) -> str:
         """
         Создает новую специальную таблицу стилей через "инспектор" во фрейме с заданным frameId.
             Если frameId не указан, будет использован frameId главного фрейма текущей страницы.
             Возвращает ID созданного styleSheet.
         https://chromedevtools.github.io/devtools-protocol/tot/CSS/#method-createStyleSheet
         :param frameId:                 Идентификатор фрейма, в котором будет создан styleSheet.
         :return:                styleSheetId
         """
-        frameId = frameId if frameId else self.page_id
-        styleSheetId = (await self.Call("CSS.createStyleSheet", {"frameId": frameId}))["styleSheetId"]
-        self.style_sheets.append(styleSheetId)
+        frameId = frameId if frameId else self._connection.conn_id
+        styleSheetId = (await self._connection.call("CSS.createStyleSheet", {"frameId": frameId}))["styleSheetId"]
+        self._style_sheets.append(styleSheetId)
         return styleSheetId
 
     async def GetStyleSheetText(self, styleSheetId: str) -> str:
         """
         Возвращает текстовый контент стилей для указанного ID.
         https://chromedevtools.github.io/devtools-protocol/tot/CSS/#method-getStyleSheetText
         :param styleSheetId:            Идентификатор стилей.
         :return:
         """
-        return (await self.Call("CSS.getStyleSheetText", {"styleSheetId": styleSheetId}))["text"]
-
-    @abstractmethod
-    async def AddListenerForEvent(
-            self, event: str, listener: Callable, *args: any) -> None:
-        raise NotImplementedError("async method AddListenerForEvent() — is not implemented")
-
-    @abstractmethod
-    def RemoveListenerForEvent(self, event: str, listener: Callable) -> None:
-        raise NotImplementedError("method RemoveListenerForEvent() — is not implemented")
-
-    @abstractmethod
-    async def Call(
-            self, domain_and_method: str,
-            params: Optional[dict] = None,
-            wait_for_response: bool = True
-    ) -> Union[dict, None]: raise NotImplementedError("async method Call() — is not implemented")
+        return (await self._connection.call("CSS.getStyleSheetText", {"styleSheetId": styleSheetId}))["text"]
 
 class CSSEvent(DomainEvent):
     fontsUpdated = "CSS.fontsUpdated"
     mediaQueryResultChanged = "CSS.mediaQueryResultChanged"
     styleSheetAdded = "CSS.styleSheetAdded"
     styleSheetChanged = "CSS.styleSheetChanged"
     styleSheetRemoved = "CSS.styleSheetRemoved"
```

### Comparing `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/DOM.py` & `aio_dt_protocol-1.0.0/aio_dt_protocol/domains/dom/dom.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,49 @@
 import re
-from abc import ABC, abstractmethod
 from typing import Optional, Union, List
-from ..DOMElement import Node
-from ..domains.Runtime import RuntimeType
-from ..exceptions import CouldNotFindNodeWithGivenID, RootIDNoLongerExists
-from ..Data import DomainEvent
+from .dom_element import Node
+from ..runtime.types import RemoteObject
+from ...exceptions import CouldNotFindNodeWithGivenID, RootIDNoLongerExists
+from ...data import DomainEvent
 
-class DOM(ABC):
+
+class DOM:
     """
     #   https://chromedevtools.github.io/devtools-protocol/tot/DOM
     """
-    __slots__ = ()
-
-    def __init__(self):
-        self.dom_domain_enabled = False
+    __slots__ = ("_connection", "enabled")
 
-    @property
-    def connected(self) -> bool:
-        return False
+    def __init__(self, conn) -> None:
 
-    @property
-    def verbose(self) -> bool:
-        return False
+        from ...connection import Connection
 
-    @property
-    def page_id(self) -> str:
-        return ""
+        self._connection: Connection = conn
+        self.enabled = False
 
-    async def DOMEnable(self) -> None:
+    async def enable(self) -> None:
         """
         Включает DOM-агент для данной страницы.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-enable
         :return:
         """
-        await self.Call("DOM.enable")
-        self.dom_domain_enabled = True
+        if not self.enabled:
+            await self._connection.call("DOM.enable")
+            self.enabled = True
 
-    async def DOMDisable(self) -> None:
+    async def disable(self) -> None:
         """
         Отключает DOM-агент для данной страницы.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-disable
         :return:
         """
-        await self.Call("DOM.disable")
-        self.dom_domain_enabled = False
+        if self.enabled:
+            await self._connection.call("DOM.disable")
+            self.enabled = False
 
-    async def GetRoot(self, depth: Optional[int] = None, pierce: Optional[bool] = None) -> Node:
+    async def getRoot(self, depth: Optional[int] = None, pierce: Optional[bool] = None) -> Node:
         """
         Возвращает корневой узел документа.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-getDocument
         Корневой элемент ВСЕГДА имеет подобную структуру:
         'root': {
             'nodeId': 19,
             'backendNodeId': 2,
@@ -118,18 +112,18 @@
         :param pierce:          Должны ли проходиться iframes и теневые корни при возврате
                                     поддерева (по умолчанию false).
         :return:            <Node>.
         """
         args = {}
         if depth is not None: args.update(depth=depth)
         if pierce is not None: args.update(pierce=pierce)
-        node: dict = (await self.Call("DOM.getDocument", args))["root"]
-        return Node(self, **node)
+        node: dict = (await self._connection.call("DOM.getDocument", args))["root"]
+        return Node(self._connection, **node)
 
-    async def QuerySelector(
+    async def querySelector(
             self, selector: str,
             ignore_root_id_exists: bool = False,
             in_frames: bool = False
     ) -> Union[Node, None]:
         """
         Выполняет DOM-запрос, возвращая объект найденного узла, или None.
             Эквивалент  === document.querySelector()
@@ -137,30 +131,30 @@
         :param selector:                    Селектор.
         :param ignore_root_id_exists:       Игнорировать исключение при отсутствии родительского элемента.
                                                 Полезно при запросах на загружающихся страницах.
         :param in_frames:                   Опрашивать документ вкючая shadow-root и iframe?
         :return:                <Node>
         """
         args = {} if not in_frames else dict(depth=-1, pierce=True)
-        root_node_id = (await self.Call("DOM.getDocument", args))["root"]["nodeId"]
+        root_node_id = (await self._connection.call("DOM.getDocument", args))["root"]["nodeId"]
         try:
-            node: dict = await self.Call("DOM.querySelector", {
+            node: dict = await self._connection.call("DOM.querySelector", {
                 "nodeId": root_node_id, "selector": selector
             })
         except CouldNotFindNodeWithGivenID as e:
             if match := re.search(r"nodeId\': (\d+)", str(e)):
                 if match.group(1) == str(root_node_id):
                     if ignore_root_id_exists:
                         return None
                     raise RootIDNoLongerExists
             raise
-        return Node(self, **node) if node["nodeId"] > 0 else None
+        return Node(self._connection, **node) if node["nodeId"] > 0 else None
 
 
-    async def QuerySelectorAll(
+    async def querySelectorAll(
             self, selector: str,
             ignore_root_id_exists: bool = False,
             in_frames: bool = False
     ) -> List[Node]:
         """
         Выполняет DOM-запрос, возвращая список объектов найденных узлов, или пустой список.
             Эквивалент  === document.querySelectorAll()
@@ -169,30 +163,30 @@
         :param ignore_root_id_exists:       Игнорировать исключение при отсутствии родительского элемента.
                                                 Полезно при запросах на загружающихся страницах.
         :param in_frames:                   Опрашивать документ вкючая shadow-root и iframe?
         :return:                [ <Node>, <Node>, ... ]
         """
         nodes = []
         args = {} if not in_frames else dict(depth=-1, pierce=True)
-        root_node_id = (await self.Call("DOM.getDocument", args))["root"]["nodeId"]
+        root_node_id = (await self._connection.call("DOM.getDocument", args))["root"]["nodeId"]
         try:
-            for node in (await self.Call("DOM.querySelectorAll", {
+            for node in (await self._connection.call("DOM.querySelectorAll", {
                 "nodeId": root_node_id, "selector": selector
             }))["nodeIds"]:
-                nodes.append(Node(self, node))
+                nodes.append(Node(self._connection, node))
         except CouldNotFindNodeWithGivenID as e:
             if match := re.search(r"nodeId\': (\d+)", str(e)):
                 if match.group(1) == str(root_node_id):
                     if ignore_root_id_exists:
                         return []
                     raise RootIDNoLongerExists
             raise
         return nodes
 
-    async def PerformSearch(self, query: str, searchInShadowDOM: Optional[bool] = None) -> dict:
+    async def performSearch(self, query: str, searchInShadowDOM: Optional[bool] = None) -> dict:
         """
         (EXPERIMENTAL)
         Ищет заданную строку в дереве DOM. Используйте 'GetSearchResults()' для доступа к результатам
             поиска или 'CancelSearch()'( !не найдено! ), чтобы завершить этот сеанс поиска. DOM-агент
             должен быть влючён.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-performSearch
         :param query:               Обычный текст, селектор, или поисковый запрос XPath.
@@ -200,17 +194,17 @@
         :return:                    {"searchId": str(searchId), "resultCount": int(resultCount)}
                                         searchId    - уникальный идентификатор сессии поиска.
                                         resultCount - кол-во результатов удовлетворяющих запрос.
         """
         args = {"query": query}
         if searchInShadowDOM is not None:
             args.update({"includeUserAgentShadowDOM": searchInShadowDOM})
-        return await self.Call("DOM.performSearch", args)
+        return await self._connection.call("DOM.performSearch", args)
 
-    async def GetSearchResults(
+    async def getSearchResults(
             self, searchId: str,
             fromIndex: int = 0,
             toIndex:   int = 0
     ) -> List[Node]:
         """
         (EXPERIMENTAL)
         Возвращает список результатов поиска для поисковой сессии 'searchId', в интервале от 'fromIndex'
@@ -219,48 +213,46 @@
         :param searchId:        Уникальный идентификатор сессии поиска.
         :param fromIndex:       Начальный индекс результата поиска, который будет возвращен.
         :param toIndex:         Конечный индекс результата поиска, который будет возвращен.
         :return:                [ <Node>, <Node>, ... ]
         """
         nodes = []
         args = {"searchId": searchId, "fromIndex": fromIndex, "toIndex": toIndex}
-        for node_id in (await self.Call("DOM.getSearchResults", args))["nodeIds"]:
-            if self.verbose:
-                print("[SearchResults] node_id =", node_id)
-            nodes.append(Node(self, node_id, ""))
+        for node_id in (await self._connection.call("DOM.getSearchResults", args))["nodeIds"]:
+            nodes.append(Node(self._connection, node_id))
         return nodes
 
-    async def Undo(self) -> None:
+    async def undo(self) -> None:
         """
         (EXPERIMENTAL)
         Отменяет последнее выполненное действие.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM#method-undo
         :return:
         """
-        await self.Call("DOM.undo")
+        await self._connection.call("DOM.undo")
 
-    async def Redo(self) -> None:
+    async def redo(self) -> None:
         """
         (EXPERIMENTAL)
         Повторно выполняет последнее отмененное действие.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM/#method-redo
         :return:
         """
-        await self.Call("DOM.redo")
+        await self._connection.call("DOM.redo")
 
-    async def MarkUndoableState(self) -> None:
+    async def markUndoableState(self) -> None:
         """
         (EXPERIMENTAL)
         Отмечает последнее состояние, которое нельзя изменить.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM/#method-markUndoableState
         :return:
         """
-        await self.Call("DOM.markUndoableState")
+        await self._connection.call("DOM.markUndoableState")
 
-    async def DescribeNode(
+    async def describeNode(
             self, nodeId: Optional[int] = None,
             backendNodeId: Optional[int] = None,
             objectId: Optional[str] = None,
             depth: Optional[int] = None,
             pierce: Optional[bool] = None
     ) -> Node:
         """
@@ -273,56 +265,49 @@
             raise ValueError("Один из nodeId, backendNodeId, или objectId — должен присутствовать!")
         args = {}
         if nodeId is not None: args.update(nodeId=nodeId)
         if backendNodeId is not None: args.update(backendNodeId=backendNodeId)
         if objectId is not None: args.update(objectId=objectId)
         if depth is not None: args.update(depth=depth)
         if pierce is not None: args.update(pierce=pierce)
-        result = await self.Call("DOM.describeNode", args)
-        return Node(self, **result["node"])
+        result = await self._connection.call("DOM.describeNode", args)
+        return Node(self._connection, **result["node"])
 
-    async def ResolveNode(
+    async def resolveNode(
             self, nodeId: Optional[int] = None,
             backendNodeId: Optional[int] = None,
             objectGroup: Optional[str] = None,
             executionContextId: Optional[str] = None
-    ) -> RuntimeType.RemoteObject:
+    ) -> RemoteObject:
         """
         Создаёт JavaScript-объект для указанной ноды и возвращает его описание.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM/#method-resolveNode
         :return:
         """
         if not ((nodeId != None) | (backendNodeId != None)):
             raise ValueError("Один из nodeId, или backendNodeId — должен присутствовать!")
         args = {}
         if nodeId is not None: args.update(nodeId=nodeId)
         if backendNodeId is not None: args.update(backendNodeId=backendNodeId)
         if objectGroup is not None: args.update(objectGroup=objectGroup)
         if executionContextId is not None: args.update(executionContextId=executionContextId)
-        result: dict = await self.Call("DOM.resolveNode", args)
-        return RuntimeType.RemoteObject(**result.get("object"))
+        result: dict = await self._connection.call("DOM.resolveNode", args)
+        return RemoteObject(**result.get("object"))
 
-    async def RequestNode(self, objectId: str) -> Node:
+    async def requestNode(self, objectId: str) -> Node:
         """
         Запрашивает, чтобы узел был отправлен вызывающей стороне с учетом ссылки на объект узла JavaScript.
             Все узлы, формирующие путь от узла к корню, также отправляются клиенту в виде серии
             setChildNodes-уведомлений.
         https://chromedevtools.github.io/devtools-protocol/tot/DOM/#method-requestNode
         :return:
         """
         args = {"objectId": objectId}
-        result: dict = await self.Call("DOM.requestNode", args)
-        return Node(self, result.get("nodeId"))
-
-    @abstractmethod
-    async def Call(
-            self, domain_and_method: str,
-            params: Optional[dict] = None,
-            wait_for_response: bool = True
-    ) -> Union[dict, None]: raise NotImplementedError("async method Call() — is not implemented")
+        result: dict = await self._connection.call("DOM.requestNode", args)
+        return Node(self._connection, result.get("nodeId"))
 
 
 class DOMEvent(DomainEvent):
     attributeModified = "DOM.attributeModified"
     attributeRemoved = "DOM.attributeRemoved"
     characterDataModified = "DOM.characterDataModified"
     childNodeCountUpdated = "DOM.childNodeCountUpdated"
```

### Comparing `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/DeviceOrientation.py` & `aio_dt_protocol-1.0.0/aio_dt_protocol/domains/device_orientation/device_orientation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,30 @@
-from abc import ABC, abstractmethod
-from typing import Optional, Union
 
-class DeviceOrientation(ABC):
+
+class DeviceOrientation:
     """
     #   https://chromedevtools.github.io/devtools-protocol/tot/DeviceOrientation
     """
-    __slots__ = ()
-
-    @property
-    def connected(self) -> bool:
-        return False
+    __slots__ = ("_connection",)
 
-    @property
-    def verbose(self) -> bool:
-        return False
+    def __init__(self, conn) -> None:
+        from ...connection import Connection
 
-    @property
-    def page_id(self) -> str:
-        return ""
+        self._connection: Connection = conn
 
-    async def ClearDeviceOrientationOverride(self) -> None:
+    async def clearDeviceOrientationOverride(self) -> None:
         """
         Очищает переопределенную ориентацию устройства.
         https://chromedevtools.github.io/devtools-protocol/tot/DeviceOrientation/#method-clearDeviceOrientationOverride
         :return:
         """
-        await self.Call("DeviceOrientation.clearDeviceOrientationOverride")
+        await self._connection.call("DeviceOrientation.clearDeviceOrientationOverride")
 
-    async def SetDeviceOrientationOverride(self, alpha: float, beta: float, gamma: float) -> None:
+    async def setDeviceOrientationOverride(self, alpha: float, beta: float, gamma: float) -> None:
         """
         Переопределяет ориентацию устройства, принудительно изменяя значения сенсоров, котоые так же
             можно найти в консоли браузера по Ctrl+Shift+P и в поиске ввести 'Show Sensors'.
         https://chromedevtools.github.io/devtools-protocol/tot/DeviceOrientation/#method-setDeviceOrientationOverride
         :return:
         """
         args = {"alpha": alpha, "beta": beta, "gamma": gamma}
-        await self.Call("DeviceOrientation.setDeviceOrientationOverride", args)
-
-    @abstractmethod
-    async def Call(
-            self, domain_and_method: str,
-            params: Optional[dict] = None,
-            wait_for_response: bool = True
-    ) -> Union[dict, None]: raise NotImplementedError("async method Call() — is not implemented")
+        await self._connection.call("DeviceOrientation.setDeviceOrientationOverride", args)
```

### Comparing `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Emulation.py` & `aio_dt_protocol-1.0.0/aio_dt_protocol/domains/emulation/emulation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,97 +1,91 @@
-from abc import ABC, abstractmethod
-from typing import Optional, Union
-from ..Data import DomainEvent
+from typing import Optional
+from ...data import DomainEvent
 
-class Emulation(ABC):
+
+class Emulation:
     """
     #   https://chromedevtools.github.io/devtools-protocol/tot/Emulation
     """
-    __slots__ = ()
+    __slots__ = ("_connection",)
 
-    @property
-    def connected(self) -> bool:
-        return False
+    def __init__(self, conn) -> None:
 
-    @property
-    def verbose(self) -> bool:
-        return False
+        from ...connection import Connection
 
-    @property
-    def page_id(self) -> str:
-        return ""
+        self._connection: Connection = conn
 
-    async def CanEmulate(self) -> bool:
+    async def canEmulate(self) -> bool:
         """
         Сообщает, поддерживается ли эмуляция.
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-canEmulate
         :return:                result -> True если эмуляция поддерживается
         """
-        return (await self.Call("Emulation.canEmulate"))["result"]
+        return (await self._connection.call("Emulation.canEmulate"))["result"]
 
-    async def ClearDeviceMetricsOverride(self) -> None:
+    async def clearDeviceMetricsOverride(self) -> None:
         """
         Очищает переопределённые метрики устройства.
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-clearDeviceMetricsOverride
         :return:
         """
-        await self.Call("Emulation.clearDeviceMetricsOverride")
+        await self._connection.call("Emulation.clearDeviceMetricsOverride")
 
-    async def ClearGeolocationOverride(self) -> None:
+    async def clearGeolocationOverride(self) -> None:
         """
         Очищает переопределённые позицию геолокации и ошибку.
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-clearGeolocationOverride
         :return:
         """
-        await self.Call("Emulation.clearGeolocationOverride")
+        await self._connection.call("Emulation.clearGeolocationOverride")
 
-    async def ResetPageScaleFactor(self) -> None:
+    async def resetPageScaleFactor(self) -> None:
         """
         Запрашивает сброс масштабирования страницы до начальных значений.
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-resetPageScaleFactor
         :return:
         """
-        await self.Call("Emulation.resetPageScaleFactor")
+        await self._connection.call("Emulation.resetPageScaleFactor")
 
-    async def SetFocusEmulationEnabled(self, enabled: bool) -> None:
+    async def setFocusEmulationEnabled(self, enabled: bool) -> None:
         """
         Включает или отключает симуляцию фокуса(когда страница активна).
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-setFocusEmulationEnabled
         :param enabled:         Включает, или отключает эмуляцию фокуса.
         :return:
         """
-        await self.Call("Emulation.setFocusEmulationEnabled", {"enabled": enabled})
+        await self._connection.call("Emulation.setFocusEmulationEnabled", {"enabled": enabled})
 
-    async def SetCPUThrottlingRate(self, rate: float) -> None:
+    async def setCPUThrottlingRate(self, rate: float) -> None:
         """
         Включает CPU "throttling", эмулируя медленный процессор.
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-setCPUThrottlingRate
         :param rate:            Коэффициент замедления(1 - без замедления; 2 - 2х кратное, и т.д.).
         :return:
         """
-        await self.Call("Emulation.setCPUThrottlingRate", {"rate": rate})
+        await self._connection.call("Emulation.setCPUThrottlingRate", {"rate": rate})
 
-    async def SetDefaultBackgroundColorOverride(self, color: dict) -> None:
+    async def setDefaultBackgroundColorOverride(self, color: dict) -> None:
         """
         Устанавливает или очищает переопределение цвета фона фрейма по умолчанию. Это переопределение
             используется, если в содержимом оно не указано.
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-setDefaultBackgroundColorOverride
         :param color:            (optional) RGBA цвета фона по умолчанию. Если не указано, любое
                                     существующее переопределение будет очищено. Словарь вида:
                                         {
                                             "r": int[0-255],
                                             "g": int[0-255],
                                             "b": int[0-255],
                                             "a": float[0-1] -> опционально. По умолчанию: 1.
                                         }
         :return:
         """
-        await self.Call("Emulation.setDefaultBackgroundColorOverride", {"color": color})
+        await self._connection.call("Emulation.setDefaultBackgroundColorOverride", {"color": color})
 
-    async def SetDeviceMetricsOverride(
+    async def setDeviceMetricsOverride(
             self, width: int, height: int,
             deviceScaleFactor: float = 0,
                         mobile: bool = False,
                         scale: Optional[float] = None,
                     screenWidth: Optional[int] = None,
                    screenHeight: Optional[int] = None,
                       positionX: Optional[int] = None,
@@ -167,50 +161,50 @@
             args.update({"positionY": positionY})
         if dontSetVisibleSize is not None:
             args.update({"dontSetVisibleSize": dontSetVisibleSize})
         if screenOrientation is not None:
             args.update({"screenOrientation": screenOrientation})
         if viewport is not None:
             args.update({"viewport": viewport})
-        await self.Call("Emulation.setDeviceMetricsOverride", args)
+        await self._connection.call("Emulation.setDeviceMetricsOverride", args)
 
-    async def SetScrollbarsHidden(self, hidden: bool) -> None:
+    async def setScrollbarsHidden(self, hidden: bool) -> None:
         """
         (EXPERIMENTAL)
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-setScrollbarsHidden
         :param hidden:              Должны ли полосы прокрутки быть всегда скрыты.
         :return:
         """
-        await self.Call("Emulation.setScrollbarsHidden", {"hidden": hidden})
+        await self._connection.call("Emulation.setScrollbarsHidden", {"hidden": hidden})
 
-    async def SetDocumentCookieDisabled(self, disabled: bool) -> None:
+    async def s(self, disabled: bool) -> None:
         """
         (EXPERIMENTAL)
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-setDocumentCookieDisabled
         :param disabled:            Должен ли API document.cookie быть отключен.
         :return:
         """
-        await self.Call("Emulation.setDocumentCookieDisabled", {"disabled": disabled})
+        await self._connection.call("Emulation.setDocumentCookieDisabled", {"disabled": disabled})
 
-    async def SetEmitTouchEventsForMouse(self, enabled: bool, configuration: Optional[str] = None) -> None:
+    async def setEmitTouchEventsForMouse(self, enabled: bool, configuration: Optional[str] = None) -> None:
         """
         (EXPERIMENTAL)
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-setEmitTouchEventsForMouse
         :param enabled:             Должна ли быть включена эмуляция касания на основе ввода от мыши.
         :param configuration:       (optional) Конфигурация событий касания / жеста.
                                         По умолчанию: текущая платформа. Допустимые значения:
                                             mobile, desktop
         :return:
         """
         args = {"enabled": enabled}
         if configuration is not None:
             args.update({"configuration": configuration})
-        await self.Call("Emulation.setEmitTouchEventsForMouse", args)
+        await self._connection.call("Emulation.setEmitTouchEventsForMouse", args)
 
-    async def SetEmulatedMedia(self, media: str = "", features: Optional[list] = None) -> None:
+    async def setEmulatedMedia(self, media: str = "", features: Optional[list] = None) -> None:
         """
         Эмулирует переданный тип медиа или медиа-функцию для медиа-запросов CSS.
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-setEmulatedMedia
         :param media:               (optional) Тип медиа для эмуляции. Пустая строка отключает переопределение.
         :param features:            (optional) Список медиа-функций для эмуляции. Допустимые значения:
                                         [{
                                             "name": str,
@@ -218,28 +212,28 @@
                                         }, { ... }, ... ]
                                         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#type-MediaFeature
         :return:
         """
         args = {"media": media}
         if features is not None:
             args.update({"features": features})
-        await self.Call("Emulation.setEmulatedMedia", args)
+        await self._connection.call("Emulation.setEmulatedMedia", args)
 
-    async def SetEmulatedVisionDeficiency(self, type_: str = "none") -> None:
+    async def setEmulatedVisionDeficiency(self, type_: str = "none") -> None:
         """
         (EXPERIMENTAL)
         Эмулирует переданный дефицит зрения.
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-setEmulatedVisionDeficiency
         :param type_:                (optional) Недостаток зрения для эмуляции. Допустимые значения:
                                         none, achromatopsia, blurredVision, deuteranopia, protanopia, tritanopia
         :return:
         """
-        await self.Call("Emulation.setEmulatedVisionDeficiency", {"type": type_})
+        await self._connection.call("Emulation.setEmulatedVisionDeficiency", {"type": type_})
 
-    async def SetGeolocationOverride(
+    async def setGeolocationOverride(
             self,
              latitude: Optional[float] = None,
             longitude: Optional[float] = None,
              accuracy: Optional[float] = None
     ) -> None:
         """
         Переопределяет Положение или Ошибку Геолокации. Пропуск любого из параметров эмулирует положение недоступно.
@@ -252,50 +246,50 @@
         args = {}
         if latitude is not None:
             args.update({"latitude": latitude})
         if longitude is not None:
             args.update({"longitude": longitude})
         if accuracy is not None:
             args.update({"accuracy": accuracy})
-        await self.Call("Emulation.setGeolocationOverride", args)
+        await self._connection.call("Emulation.setGeolocationOverride", args)
 
-    async def SetPageScaleFactor(self, pageScaleFactor: float) -> None:
+    async def setPageScaleFactor(self, pageScaleFactor: float) -> None:
         """
         (EXPERIMENTAL)
         Устанавливает переданный коэффициент масштабирования страницы.
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-setPageScaleFactor
         :param pageScaleFactor:     Коэффициент масштабирования страницы.
         :return:
         """
-        await self.Call("Emulation.setPageScaleFactor", {"pageScaleFactor": pageScaleFactor})
+        await self._connection.call("Emulation.setPageScaleFactor", {"pageScaleFactor": pageScaleFactor})
 
-    async def SetScriptExecutionDisabled(self, value: bool) -> None:
+    async def setScriptExecutionDisabled(self, value: bool) -> None:
         """
         Переключает выполнение скриптов на странице.
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-setScriptExecutionDisabled
         :param value:               Должно ли выполнение скриптов быть отключено на странице.
         :return:
         """
-        await self.Call("Emulation.setScriptExecutionDisabled", {"value": value})
+        await self._connection.call("Emulation.setScriptExecutionDisabled", {"value": value})
 
-    async def SetTouchEmulationEnabled(self, enabled: bool, maxTouchPoints: Optional[int] = None) -> None:
+    async def setTouchEmulationEnabled(self, enabled: bool, maxTouchPoints: Optional[int] = None) -> None:
         """
         Включает "касания" для платформ, которые их не поддерживают.
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-setTouchEmulationEnabled
         :param enabled:             Должна ли эмуляция сенсорного события быть включена.
         :param maxTouchPoints:      (optional) Максимальное количество поддерживаемых точек касания.
                                         По умолчанию 1.
         :return:
         """
         args = {"enabled": enabled}
         if maxTouchPoints is not None:
             args.update({"maxTouchPoints": maxTouchPoints})
-        await self.Call("Emulation.setTouchEmulationEnabled", args)
+        await self._connection.call("Emulation.setTouchEmulationEnabled", args)
 
-    async def SetLocaleOverride(self, locale: Optional[str] = None) -> None:
+    async def setLocaleOverride(self, locale: Optional[str] = None) -> None:
         """
         Не работает.
         https://bugs.chromium.org/p/chromium/issues/detail?id=1073363
         Починили с версии Хромиум == 83.0.4103.97
 
         (EXPERIMENTAL)
         Переопределяет языковой стандарт хост-системы на указанную.
@@ -305,44 +299,44 @@
                                         локаль системы хоста по умолчанию.
                                         https://stackoverflow.com/questions/3191664/list-of-all-locales-and-their-short-codes
         :return:
         """
         args = {}
         if locale is not None:
             args.update({"locale": locale})
-        await self.Call("Emulation.setLocaleOverride", args)
+        await self._connection.call("Emulation.setLocaleOverride", args)
 
-    async def SetTimezoneOverride(self, timezoneId: str = "") -> None:
+    async def setTimezoneOverride(self, timezoneId: str = "") -> None:
         """
         (EXPERIMENTAL)
         Переопределяет часовой пояс хост-системы на указанный.
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-setTimezoneOverride
         :param timezoneId:          Идентификатор часового пояса("Europe/Moscow"). Если пусто,
                                         отключает переопределение и восстанавливает часовой пояс
                                         хост-системы по умолчанию.
                                         https://en.wikipedia.org/wiki/List_of_tz_database_time_zones
         :return:
         """
-        await self.Call("Emulation.setTimezoneOverride", {"timezoneId": timezoneId})
+        await self._connection.call("Emulation.setTimezoneOverride", {"timezoneId": timezoneId})
 
-    async def SetVisibleSize(self, width: int, height: int) -> None:
+    async def setVisibleSize(self, width: int, height: int) -> None:
         """
         (DEPRECATED)
         (EXPERIMENTAL)
         Изменяет размер фрейма / области просмотра страницы. Обратите внимание, что это не влияет
             на контейнер фрейма (например, окно браузера). Может использоваться для создания
             скриншотов указанного размера. Не поддерживается на Android.
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-setVisibleSize
         :param width:               Ширина фрейма (DIP).
         :param height:              Высота фрейма (DIP).
         :return:            None
         """
-        await self.Call("Emulation.setVisibleSize", {"width": width, "height": height})
+        await self._connection.call("Emulation.setVisibleSize", {"width": width, "height": height})
 
-    async def EmulationSetUserAgent(
+    async def setUserAgentOverride(
             self, userAgent: str,
                 acceptLanguage: Optional[str] = None,
                       platform: Optional[str] = None,
             userAgentMetadata: Optional[dict] = None
     ) -> None:
         """
         Переопределяет юзер-агент переданной строкой.
@@ -369,18 +363,11 @@
         args = {"userAgent": userAgent}
         if acceptLanguage is not None:
             args.update({"acceptLanguage": acceptLanguage})
         if platform is not None:
             args.update({"platform": platform})
         if userAgentMetadata is not None:
             args.update({"userAgentMetadata": userAgentMetadata})
-        await self.Call("Emulation.setUserAgentOverride", args)
-
-    @abstractmethod
-    async def Call(
-            self, domain_and_method: str,
-            params: Optional[dict] = None,
-            wait_for_response: bool = True
-    ) -> Union[dict, None]: raise NotImplementedError("async method Call() — is not implemented")
+        await self._connection.call("Emulation.setUserAgentOverride", args)
 
 class EmulationEvent(DomainEvent):
     virtualTimeBudgetExpired = "Emulation.virtualTimeBudgetExpired"
```

### Comparing `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Fetch.py` & `aio_dt_protocol-1.0.0/aio_dt_protocol/domains/runtime/runtime.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,360 +1,356 @@
-from abc import ABC, abstractmethod
-from typing import Optional, Union, List, Callable, Awaitable
-from ..Data import DomainEvent
-from ..domains.Network import NetworkType
-from dataclasses import dataclass, field
+try:
+    import ujson as json
+except ModuleNotFoundError:
+    import json
+
+from typing import Optional, List
+from .types import PropertyDescriptor, ContextManager, ContextDescription, Script
+from ...data import DomainEvent
+from ...exceptions import PromiseEvaluateError, highlight_promise_error
 
 
-class Fetch(ABC):
+class Runtime:
     """
-    #   https://chromedevtools.github.io/devtools-protocol/tot/Fetch
+    #   https://chromedevtools.github.io/devtools-protocol/tot/Runtime
     """
-    __slots__ = ()
+    __slots__ = ("_connection", "enabled", "context_manager")
 
-    def __init__(self):
-        self.fetch_domain_enabled = False
+    def __init__(self, conn) -> None:
 
-    @property
-    def connected(self) -> bool:
-        return False
-
-    @property
-    def verbose(self) -> bool:
-        return False
-
-    @property
-    def page_id(self) -> str:
-        return ""
-
-    async def FetchEnable(
-        self,
-        patterns: Optional[List["FetchType.RequestPattern"]] = None,
-        handleAuthRequests: bool = False,
-        on_pause: Optional[Callable[['FetchType.EventRequestPaused'], Awaitable[None]]] = None,
-        on_auth:  Optional[Callable[['FetchType.EventAuthRequired'], Awaitable[None]]] = None,
-    ) -> None:
-        """
-        Включает выдачу событий requestPaused. Запрос будет приостановлен до тех пор,
-            пока клиент не вызовет одну из функций failRequest, fulfillRequest или
-            continueRequest / continueWithAuth.
-        https://chromedevtools.github.io/devtools-protocol/tot/Fetch#method-enable
-        :param patterns:            (optional) Если указано, только запросы,
-                                        соответствующие любому из этих шаблонов, будут
-                                        вызывать событие fetchRequested и будут
-                                        приостановлены до ответа клиента. Если не
-                                        установлен, все запросы будут затронуты.
-                                            https://chromedevtools.github.io/devtools-protocol/tot/Fetch#type-RequestPattern
-        :param handleAuthRequests:  (optional) Если True - события authRequired будут
-                                        выдаваться и запросы будут приостановлены в
-                                        ожидании вызова continueWithAuth.
-        :param on_pause:            (optional) Корутина, которая будет получать все события "requestPaused".
-        :param on_auth:             (optional) Корутина, которая будет получать все события "authRequired".
+        from ...connection import Connection
+
+        self._connection: Connection = conn
+        self.enabled = False
+        self.context_manager = ContextManager()
+
+    async def getProperties(
+            self, objectId: str,
+            skip_complex_types: bool = True,
+            ownProperties: Optional[bool] = None,
+            accessorPropertiesOnly: Optional[bool] = None,
+            generatePreview: Optional[bool] = None,
+            nonIndexedPropertiesOnly: Optional[bool] = None,
+    ) -> List[PropertyDescriptor]:
+        """ Возвращает свойства заданного объекта. Группа объектов результата наследуется
+        от целевого объекта.
+        https://chromedevtools.github.io/devtools-protocol/tot/Runtime/#method-getProperties
+        :param objectId:                    Идентификатор объекта, для которого возвращаются свойства.
+        :param ownProperties:               Если true, возвращает свойства, принадлежащие только самому
+                                                элементу, а не его цепочке прототипов.
+        :param accessorPropertiesOnly:      Если true, возвращает только свойства доступа (с геттером/сеттером);
+                                                внутренние свойства также не возвращаются.
+        :param generatePreview:             Должен ли быть создан предварительный просмотр для результатов.
+        :param nonIndexedPropertiesOnly:    Если true, возвращает только неиндексированные свойства.
+        :return:    {
+            "result": array[ PropertyDescriptor ],
+            "internalProperties":  list[ InternalPropertyDescriptor ],
+            "privateProperties":  list[ PrivatePropertyDescriptor ],
+            "exceptionDetails": dict{ ExceptionDetails }
+        }
+        """
+        args = {"objectId": objectId}
+        if ownProperties: args.update({"ownProperties": ownProperties})
+        if accessorPropertiesOnly: args.update({"accessorPropertiesOnly": accessorPropertiesOnly})
+        if generatePreview: args.update({"generatePreview": generatePreview})
+        if nonIndexedPropertiesOnly: args.update({"nonIndexedPropertiesOnly": nonIndexedPropertiesOnly})
+        response = await self._connection.call("Runtime.getProperties", args)
+        if "exceptionDetails" in response:
+            raise PromiseEvaluateError(
+                highlight_promise_error(response["result"]["description"]) +
+                "\n" + json.dumps(response["exceptionDetails"])
+            )
+        if not skip_complex_types:
+            return [PropertyDescriptor(**p) for p in response["result"]]
+
+        result = []
+        for p in response["result"]:
+            if (subtype := p["value"].get("type")) and subtype == "function":
+                continue
+            result.append(PropertyDescriptor(**p))
+        return result
+
+
+    async def awaitPromise(
+            self, promiseObjectId: str, returnByValue: bool = False, generatePreview: bool = False
+    ) -> dict:
+        """
+        Добавляет обработчик к промису с переданным идентификатором.
+        https://chromedevtools.github.io/devtools-protocol/tot/Runtime#method-awaitPromise
+        :param promiseObjectId:     Идентификатор промиса.
+        :param returnByValue:       (optional) Ожидается ли результат в виде объекта JSON,
+                                        который должен быть отправлен по значению.
+        :param generatePreview:     (optional) Должен ли предварительный просмотр
+                                        генерироваться для результата.
+        :return:                    {
+                                        "result": dict(https://chromedevtools.github.io/devtools-protocol/tot/Runtime#type-RemoteObject)
+                                        "exceptionDetails": dict(https://chromedevtools.github.io/devtools-protocol/tot/Runtime#type-ExceptionDetails)
+                                    }
+        """
+        args = {"promiseObjectId": promiseObjectId, "returnByValue": returnByValue, "generatePreview": generatePreview}
+        response = await self._connection.call("Runtime.awaitPromise", args)
+        if "exceptionDetails" in response:
+            raise PromiseEvaluateError(
+                highlight_promise_error(response["result"]["description"]) +
+                "\n" + json.dumps(response["exceptionDetails"])
+            )
+        return response["result"]
+
+    async def callFunctionOn(
+            self, functionDeclaration: str,
+            objectId: Optional[str] = None,
+            arguments: Optional[list] = None,
+            silent: Optional[bool] = None,
+            returnByValue: Optional[bool] = None,
+            generatePreview: Optional[bool] = None,
+            userGesture: Optional[bool] = None,
+            awaitPromise: Optional[bool] = None,
+            executionContextId: Optional[int] = None,
+            objectGroup: Optional[str] = None
+    ) -> dict:
+        """
+        Вызывает функцию с заданным объявлением для данного объекта. Группа объектов результата
+            наследуется от целевого объекта.
+        https://chromedevtools.github.io/devtools-protocol/tot/Runtime#method-callFunctionOn
+        :param functionDeclaration:     Объявление функции для вызова.
+        :param objectId:                (optional) Идентификатор объекта для вызова функции.
+                                            Должен быть указан либо objectId, либо executeContextId.
+        :param arguments:               (optional) Аргументы. Все аргументы вызова должны
+                                            принадлежать тому же миру JavaScript, что и целевой
+                                            объект.
+        :param silent:                  (optional) В тихом режиме исключения, выданные во время оценки,
+                                            не регистрируются и не приостанавливают выполнение.
+                                            Переопределяет 'setPauseOnException' состояние.
+        :param returnByValue:           (optional) Ожидается ли результат в виде объекта JSON,
+                                            который должен быть отправлен по значению.
+        :param generatePreview:         (optional, EXPERIMENTAL) Должен ли предварительный
+                                            просмотр генерироваться для результата.
+        :param userGesture:             (optional) Должно ли выполнение рассматриваться как
+                                            инициированное пользователем в пользовательском интерфейсе.
+        :param awaitPromise:            (optional) Решено ли выполнение await для полученного значения
+                                            и возврата после ожидаемого обещания.
+        :param executionContextId:      (optional) Определяет контекст выполнения, в котором будет
+                                            использоваться глобальный объект для вызова функции.
+                                            Должен быть указан либо executeContextId, либо objectId.
+        :param objectGroup:             (optional) Символическое имя группы, которое можно
+                                            использовать для освобождения нескольких объектов. Если
+                                            objectGroup не указан, а objectId равен, objectGroup
+                                            будет унаследован от объекта.
+        :return:                        { ... } - https://chromedevtools.github.io/devtools-protocol/tot/Runtime/#type-RemoteObject
+        """
+        args = {"functionDeclaration": functionDeclaration}
+        if objectId is not None:
+            args.update({"objectId": objectId})
+        if arguments is not None:
+            args.update({"arguments": arguments})
+        if silent is not None:
+            args.update({"silent": silent})
+        if returnByValue is not None:
+            args.update({"returnByValue": returnByValue})
+        if generatePreview is not None:
+            args.update({"generatePreview": generatePreview})
+        if userGesture is not None:
+            args.update({"userGesture": userGesture})
+        if awaitPromise is not None:
+            args.update({"awaitPromise": awaitPromise})
+        if executionContextId is not None:
+            args.update({"executionContextId": executionContextId})
+        if objectGroup is not None:
+            args.update({"objectGroup": objectGroup})
+        response = await self._connection.call("Runtime.callFunctionOn", args)
+        if "exceptionDetails" in response:
+            raise Exception(response["result"]["description"] + "\n" + json.dumps(response["exceptionDetails"]))
+        return response["result"]
+
+    async def enable(self, watch_for_execution_contexts: bool = False) -> None:
+        """
+        Включает создание отчетов о создании контекстов выполнения с помощью события executeContextCreated.
+            При включении, событие будет отправлено немедленно для каждого существующего контекста выполнения.
+
+        Позволяет так же организовать обратную связь со страницей, посылая из её контекста, данные, в консоль.
+            В этом случае будет генерироваться событие 'Runtime.consoleAPICalled':
+            https://chromedevtools.github.io/devtools-protocol/tot/Runtime#event-consoleAPICalled
+            {
+                'method': 'Runtime.consoleAPICalled',
+                'params': {
+                    'type': 'log',
+                    'args': [{'type': 'string', 'value': 'you console data passed was be here'}],
+                    'executionContextId': 2,
+                    'timestamp': 1583582949679.153,
+                    'stackTrace': {
+                        'callFrames': [{'functionName': '', 'scriptId': '48', 'url': '', 'lineNumber': 0, 'columnNumber': 8}]
+                    }
+                }
+            }
+
+        https://chromedevtools.github.io/devtools-protocol/tot/Runtime#method-enable
+        :param watch_for_execution_contexts:    Регистрирует слушателей, ожидающих события создания/уничтожения
+                                                    контекстов, которые можно запрашивать через
+                                                    page_instance.context_manager.GetDefaultContext(frameId: str).
+                                                    Должен быть включён ПЕРЕД переходом на целевой адрес.
         :return:
         """
-        async def on_pause_decorator(
-                params: dict, func: Callable[["FetchType.EventRequestPaused"], Awaitable[None]]) -> None:
-            await func(FetchType.EventRequestPaused(**params))
-
-        async def on_auth_decorator(
-                params: dict, func: Callable[["FetchType.EventAuthRequired"], Awaitable[None]]) -> None:
-            await func(FetchType.EventAuthRequired(**params))
-
-        if on_pause is not None:
-            await self.AddListenerForEvent(
-                FetchEvent.requestPaused, on_pause_decorator, on_pause)
-
-        if on_auth is not None:
-            await self.AddListenerForEvent(
-                FetchEvent.authRequired, on_auth_decorator, on_auth)
-
-        args = {}
-        patterns = patterns if patterns is not None else []
-        if patterns:
-            args.update({"patterns": [p.dict() for p in patterns]})
-        if handleAuthRequests: args.update({"handleAuthRequests": handleAuthRequests})
-        await self.Call("Fetch.enable", args)
-        self.fetch_domain_enabled = True
+        if not self.enabled:
+            await self._connection.call("Runtime.enable")
+            self.enabled = True
+
+        if watch_for_execution_contexts and not self.context_manager.is_watch:
+            await self._connection.addListenerForEvent(
+                RuntimeEvent.executionContextCreated, self.context_manager.on_create)
+            await self._connection.addListenerForEvent(
+                RuntimeEvent.executionContextsCleared, self.context_manager.on_clear)
+            await self._connection.addListenerForEvent(
+                RuntimeEvent.executionContextDestroyed, self.context_manager.on_destroy)
+            self.context_manager.is_watch = True
 
-    async def FetchDisable(self) -> None:
+    async def disable(self) -> None:
         """
-        Отключает взаимодействие с доменом.
-        https://chromedevtools.github.io/devtools-protocol/tot/Fetch#method-disable
+        Отключает создание отчетов о создании контекстов выполнения.
+        https://chromedevtools.github.io/devtools-protocol/tot/Runtime#method-disable
         :return:
         """
-        await self.Call("Fetch.disable")
-        self.fetch_domain_enabled = False
+        if self.enabled:
+            await self._connection.call("Runtime.disable")
+            self.enabled = False
+
+        if self.context_manager.is_watch:
+            self._connection.removeListenerForEvent(
+                RuntimeEvent.executionContextCreated, self.context_manager.on_create)
+            self._connection.removeListenerForEvent(
+                RuntimeEvent.executionContextsCleared, self.context_manager.on_clear)
+            self._connection.removeListenerForEvent(
+                RuntimeEvent.executionContextDestroyed, self.context_manager.on_destroy)
+            self.context_manager.is_watch = False
 
-    async def FailRequest(self, requestId: str, errorReason: str) -> None:
+    async def discardConsoleEntries(self) -> None:
         """
-        Вызывает сбой запроса по указанной причине.
-        https://chromedevtools.github.io/devtools-protocol/tot/Fetch#method-failRequest
-        :param requestId:           Идентификатор, полученный клиентом в событии requestPaused.
-        :param errorReason:         Причина сбоя выборки на уровне сети. Возможные значения:
-                                        Failed, Aborted, TimedOut, AccessDenied,
-                                        ConnectionClosed, ConnectionReset,
-                                        ConnectionRefused, ConnectionAborted,
-                                        ConnectionFailed, NameNotResolved,
-                                        InternetDisconnected, AddressUnreachable,
-                                        BlockedByClient, BlockedByResponse
+        Отбрасывает собранные исключения и вызовы API консоли.
+        https://chromedevtools.github.io/devtools-protocol/tot/Runtime#method-discardConsoleEntries
         :return:
         """
-        await self.Call("Fetch.failRequest", {"requestId": requestId, "errorReason": errorReason})
+        await self._connection.call("Runtime.discardConsoleEntries")
 
-    async def FulfillRequest(
-            self, requestId: str,
-            responseCode:                     int = 200,
-            responseHeaders: Optional[List[dict]] = None,
-            binaryResponseHeaders:  Optional[str] = None,
-            body:                   Optional[str] = None,
-            responsePhrase:         Optional[str] = None,
-            wait_for_response:               bool = False
-    ) -> None:
-        """
-        Предоставляет браузеру ответ на запрос.
-        https://chromedevtools.github.io/devtools-protocol/tot/Fetch#method-fulfillRequest
-        :param requestId:               Идентификатор, полученный клиентом в событии requestPaused.
-        :param responseCode:            Код ответа HTTP(например - 200).
-        :param responseHeaders:         (optional) Заголовки ответа. Например:
-                                            [
-                                                { "name": "User-Agent", "value": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.149 Safari/537.36" },
-                                                { "name": "Content-Type", "value": "application/json; charset=UTF-8" }
-                                            ]
-        :param binaryResponseHeaders:   (optional) Альтернативный способ указания заголовков ответа в
-                                            виде разделенных \0 серий пар имя-значение. Описанный выше
-                                            метод предпочтительней, если вам не нужно представлять
-                                            некоторые значения, отличные от UTF8, которые не могут быть
-                                            переданы по протоколу, в виде текста.
-        :param body:                    (optional) Тело ответа, кодированное в строку формата base64.
-        :param responsePhrase:          (optional) Текстовое представление responseCode. Если
-                                            отсутствует, используется стандартная фраза,
-                                            соответствующая responseCode.
-        :param wait_for_response:       (optional) Дожидаться ответа?
-        :return:
+    async def releaseObjectGroup(self, objectGroup: str) -> None:
         """
-        args = {"requestId": requestId, "responseCode": responseCode}
-        if responseHeaders is not None: args.update({"responseHeaders": responseHeaders})
-        if binaryResponseHeaders is not None: args.update({"binaryResponseHeaders": binaryResponseHeaders})
-        if body is not None: args.update({"body": body})
-        if responsePhrase is not None: args.update({"responsePhrase": responsePhrase})
-        # print("fulfillRequest args", json.dumps(args, indent=4))
-        await self.Call("Fetch.fulfillRequest", args, wait_for_response=wait_for_response)
-
-    async def ContinueRequest(
-        self, requestId: str,
-        url:                Optional[str] = None,
-        method:             Optional[str] = None,
-        postData:           Optional[str] = None,
-        headers:     Optional[List[dict]] = None,
-        interceptResponse: Optional[bool] = None,
-        wait_for_response:           bool = False
-    ) -> None:
-        """
-        Продолжает запрос, дополнительно изменяя некоторые его параметры.
-        https://chromedevtools.github.io/devtools-protocol/tot/Fetch#method-continueRequest
-        :param requestId:           Идентификатор, полученный клиентом в событии requestPaused.
-        :param url:                 (optional) Если установлено, URL-адрес запроса будет изменен так,
-                                        чтобы страница не наблюдалась.
-        :param method:              (optional) Переопределяет метод запроса переданным значением.
-        :param postData:            (optional) Переопределяет данные запроса переданными.
-        :param headers:             (optional) Переопределяет заголовки запроса переданными. . Например:
-                                        [
-                                            { "name": "User-Agent", "value": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.149 Safari/537.36" },
-                                            { "name": "Content-Type", "value": "application/json; charset=UTF-8" }
-                                        ]
-        :param interceptResponse:   (optional) Если установлено, переопределяет поведение перехвата ответа для этого запроса.
-        :param wait_for_response:   (optional) Дожидаться ответа?
+        Освобождает все удаленные объекты, принадлежащие данной группе.
+        https://chromedevtools.github.io/devtools-protocol/tot/Runtime#method-releaseObjectGroup
+        :param objectGroup:             Символическое имя группы.
         :return:
         """
-        args = {"requestId": requestId}
-        if url is not None: args.update({"url": url})
-        if method is not None: args.update({"method": method})
-        if postData is not None: args.update({"postData": postData})
-        if headers is not None: args.update({"headers": headers})
-        if interceptResponse is not None: args.update({"interceptResponse": interceptResponse})
-        await self.Call("Fetch.continueRequest", args, wait_for_response=wait_for_response)
-
-    async def ContinueWithAuth(self, requestId: str, authChallengeResponse: list) -> None:
-        """
-        Продолжает запрос, предоставляющий authChallengeResponse после события authRequired.
-        https://chromedevtools.github.io/devtools-protocol/tot/Fetch#method-continueWithAuth
-        :param requestId:               Идентификатор, полученный клиентом в событии requestPaused.
-        :param authChallengeResponse:   Ответ с помощью authChallenge.
-                                            {
-                                                "response": str(), -> Решение о том, что делать в ответ
-                                                    на запрос авторизации. По умолчанию означает
-                                                    использование стандартного поведения сетевого стека,
-                                                    что, скорее всего, приведет к отмене проверки
-                                                    подлинности или появлению всплывающего диалогового
-                                                    окна. Возможные значения:
-                                                        Default, CancelAuth, ProvideCredentials
-                                                "username": str(), -> (optional) Имя пользователя для
-                                                    предоставления, может быть пустым. Устанавливается,
-                                                    только если ответом является ProvideCredentials.
-                                                "password": str(), -> (optional) Пароль пользователя для
-                                                    предоставления, может быть пустым. Устанавливается,
-                                                    только если ответом является ProvideCredentials.
-                                            }
-        :return:
-        """
-        args = {"requestId": requestId, "authChallengeResponse": authChallengeResponse}
-        await self.Call("Fetch.continueWithAuth", args)
+        await self._connection.call("Runtime.releaseObjectGroup", {"objectGroup": objectGroup})
 
-    async def GetResponseBody(self, requestId: str) -> dict:
-        """
-        Вызывает тело ответа, получаемого от сервера и возвращаемого в виде одной строки. Может
-            выдаваться только для запроса, который приостановлен на этапе ответа и является
-            взаимоисключающим с "takeResponseBodyForInterceptionAsStream". Вызов других методов,
-            влияющих на запрос, или отключение домена выборки до получения тела приводит к
-            неопределенному поведению.
-        https://chromedevtools.github.io/devtools-protocol/tot/Fetch#method-getResponseBody
-        :param requestId:               Идентификатор перехваченного запроса для получения его тела.
+    async def compileScript(
+            self, expression: str,
+            sourceURL: str = "",
+            persistScript: bool = True,
+            executionContextId: Optional[int] = None
+    ) -> str:
+        """
+        Компилирует выражение.
+        https://chromedevtools.github.io/devtools-protocol/tot/Runtime#method-compileScript
+        :param expression:              Выражение для компиляции.
+        :param sourceURL:               Исходный URL для скрипта.
+        :param persistScript:           Указывает, следует ли сохранить скомпилированный скрипт.
+        :param executionContextId:      (optional) Указывает, в каком контексте выполнения выполнять сценарий.
+                                            Если параметр не указан, выражение будет выполняться в контексте
+                                            проверяемой страницы.
         :return:                        {
-                                            "body": str(),        -> Тело ответа.
-                                            "base64Encoded": bool -> True - если контент кодирован
-                                                                        как base64.
+                                            "scriptId": str()
+                                            "exceptionDetails": dict(https://chromedevtools.github.io/devtools-protocol/tot/Runtime#type-ExceptionDetails)
                                         }
         """
-        return await self.Call("Fetch.getResponseBody", {"requestId": requestId})
-
-    async def TakeResponseBodyAsStream(self, requestId: str) -> dict:
-        """
-        Возвращает дескриптор потока, представляющего тело ответа. Запрос должен быть приостановлен
-            на этапе HeadersReceived. Обратите внимание, что после этой команды запрос не может быть
-            продолжен как есть - клиент должен либо отменить его, либо предоставить тело ответа.
-            Поток поддерживает только последовательное чтение, IO.read потерпит неудачу, если указана
-            позиция. Этот метод является взаимоисключающим с getResponseBody. Вызов других методов,
-            влияющих на запрос, или отключение домена выборки до получения тела приводит к
-            неопределенному поведению.
-        https://chromedevtools.github.io/devtools-protocol/tot/Fetch#method-takeResponseBodyAsStream
-        :param requestId:               Идентификатор перехваченного запроса для получения его тела.
+        args = {"expression": expression, "sourceURL": sourceURL, "persistScript": persistScript}
+        if executionContextId is not None:
+            args.update({"executionContextId": executionContextId})
+
+        response = await self._connection.call("Runtime.compileScript", args)
+        if "exceptionDetails" in response:
+            raise Exception(response["exceptionDetails"]["text"] + "\n" + json.dumps(response["exceptionDetails"]))
+        return response["scriptId"]
+
+    async def buildScript(self, expression: str, context: Optional[ContextDescription] = None) -> Script:
+        return Script(self._connection, expression, context)
+
+    async def runIfWaitingForDebugger(self) -> None:
+        """
+        Сообщает инспектируемой странице, что можно запуститься, если она ожидает этого после
+            Target.setAutoAttach.
+        """
+        await self._connection.call("Runtime.runIfWaitingForDebugger")
+
+    async def runScript(
+            self, scriptId: str,
+            executionContextId: Optional[int] = None,
+            objectGroup: str = "console",
+            silent: bool = False,
+            includeCommandLineAPI: bool = True,
+            returnByValue: bool = False,
+            generatePreview: bool = False,
+            awaitPromise: bool = True
+    ) -> dict:
+        """
+        Запускает скрипт с заданным идентификатором в заданном контексте.
+        https://chromedevtools.github.io/devtools-protocol/tot/Runtime#method-runScript
+        :param scriptId:                ID сценария для запуска.
+        :param executionContextId:      (optional) Указывает, в каком контексте выполнения выполнять сценарий.
+                                            Если параметр не указан, выражение будет выполняться в контексте
+                                            проверяемой страницы.
+        :param objectGroup:             (optional) Символическое имя группы, которое можно использовать для
+                                            освобождения нескольких объектов.
+        :param silent:                  (optional) В тихом режиме исключения, выданные во время оценки, не
+                                            сообщаются и не приостанавливают выполнение. Переопределяет
+                                            состояние setPauseOnException.
+        :param includeCommandLineAPI:   (optional) Определяет, должен ли API командной строки быть доступным
+                                            во время оценки.
+        :param returnByValue:           (optional) Ожидается ли результат в виде объекта JSON, который должен
+                                            быть отправлен по значению.
+        :param generatePreview:         (optional) Должен ли предварительный просмотр генерироваться для результата.
+        :param awaitPromise:            (optional) Будет ли выполнено ожидание выполнения для полученного значения
+                                            и возврата после ожидаемого 'promise'.
         :return:                        {
-                                            "stream": str(), -> Это либо получается из другого метода,
-                                                либо указывается как blob <uuid> это UUID Blob.
-                                                    IO.StreamHandle:
-                                                    https://chromedevtools.github.io/devtools-protocol/tot/IO#type-StreamHandle
+                                            "result": dict(https://chromedevtools.github.io/devtools-protocol/tot/Runtime#type-RemoteObject)
+                                            "exceptionDetails": dict(https://chromedevtools.github.io/devtools-protocol/tot/Runtime#type-ExceptionDetails)
                                         }
         """
-        return await self.Call("Fetch.takeResponseBodyAsStream", {"requestId": requestId})
-
-    @abstractmethod
-    async def Call(
-        self, domain_and_method: str,
-        params: Optional[dict] = None,
-        wait_for_response: bool = True
-    ) -> Union[dict, None]: raise NotImplementedError("async method Call() — is not implemented")
-
-    @abstractmethod
-    async def AddListenerForEvent(
-            self, event: Union[str, DomainEvent], listener: Callable, *args: any) -> None:
-        raise NotImplementedError("async method AddListenerForEvent() — is not implemented")
-
-    @abstractmethod
-    def RemoveListenersForEvent(self, event: str) -> None:
-        raise NotImplementedError("method RemoveListenersForEvent() — is not implemented")
-
-
-class FetchEvent(DomainEvent):
-    authRequired = "Fetch.authRequired"
-    requestPaused = "Fetch.requestPaused"
-
-
-class FetchType:
-
-    @dataclass
-    class EventRequestPaused:
-        requestId: str
-        frameId: str
-        resourceType: str                               # ! Allowed Values: Document, Stylesheet, Image, Media, Font,
-                                                        # !     Script, TextTrack, XHR, Fetch, EventSource, WebSocket,
-                                                        # !     Manifest, SignedExchange, Ping, CSPViolationReport,
-                                                        # !     Preflight, Other
-        request: NetworkType.Request
-        responseHeaders: list["FetchType.HeaderEntry"]
-        responseErrorReason: Optional[str] = None       # ! Allowed Values: Failed, Aborted, TimedOut, AccessDenied,
-                                                        # !     ConnectionClosed, ConnectionReset, ConnectionRefused,
-                                                        # !     ConnectionAborted, ConnectionFailed, NameNotResolved,
-                                                        # !     InternetDisconnected, AddressUnreachable,
-                                                        # !     BlockedByClient, BlockedByResponse
-        responseStatusCode: Optional[int] = None
-        responseStatusText: Optional[str] = None
-        networkId: Optional[str] = None                 # ! id of request
-        redirectedRequestId: Optional[str] = None       # ! id запроса вызвавшего редирект
-        _request: NetworkType.Request = field(init=False, repr=False, default=None)
-        _responseHeaders: Optional[list["FetchType.HeaderEntry"]] = field(init=False, repr=False, default=None)
-
-        @property
-        def request(self) -> NetworkType.Request:
-            return self._request
-
-        @request.setter
-        def request(self, data: dict) -> None:
-            self._request = NetworkType.Request(**data)
-
-        @property
-        def responseHeaders(self) -> Optional[list["FetchType.HeaderEntry"]]:
-            return self._responseHeaders
-
-        @responseHeaders.setter
-        def responseHeaders(self, data: list[dict[str, str]]) -> None:
-            if not isinstance(data, property):
-                self._responseHeaders = [FetchType.HeaderEntry(**item) for item in data]
-            else:
-                self._responseHeaders = None
-
-
-    @dataclass
-    class EventAuthRequired:
-        requestId: str
-        request: NetworkType.Request
-        frameId: str
-        resourceType: str                               # ! Allowed Values: Document, Stylesheet, Image, Media, Font,
-                                                        # !     Script, TextTrack, XHR, Fetch, EventSource, WebSocket,
-                                                        # !     Manifest, SignedExchange, Ping, CSPViolationReport,
-                                                        # !     Preflight, Other
-        authChallenge: "FetchType.AuthChallenge"
-        _authChallenge: "FetchType.AuthChallenge" = field(init=False, repr=False, default=None)
-
-        @property
-        def authChallenge(self) -> "FetchType.AuthChallenge":
-            return self._authChallenge
-
-        @authChallenge.setter
-        def authChallenge(self, data: dict) -> None:
-            self._authChallenge = FetchType.AuthChallenge(**data)
-
-
-    @dataclass
-    class AuthChallenge:
-        origin: str
-        scheme: str
-        realm: str                                      # ! May be empty.
-        source: Optional[str] = None
-
-
-    @dataclass
-    class HeaderEntry:
-        name: str
-        value: str
-
-
-    @dataclass
-    class RequestPattern:
-        urlPattern: str = "*"                           # ? Подстановочные знаки ( '*'-> ноль или более, '?'-> ровно
-                                                        # ?     один) допускаются. Экранирующий символ — обратная
-                                                        # ?     косая черта(\).
-        resourceType: Optional[str] = None              # ? Если установлено, будут перехватываться только соответствующие
-                                                        # ?     указанным типам.
-                                                        # ! Allowed Values: Document, Stylesheet, Image, Media, Font,
-                                                        # !     Script, TextTrack, XHR, Fetch, EventSource, WebSocket,
-                                                        # !     Manifest, SignedExchange, Ping, CSPViolationReport,
-                                                        # !     Preflight, Other
-        requestStage: Optional[str] = None              # ? Стадия перехвата запроса. Запрос будет перехвачен до того,
-                                                        # ?     как запрос будет отправлен. Ответ будет перехвачен после
-                                                        # ?     получения ответа (но до получения тела ответа).
-                                                        # ! Allowed Values: Request, Response
-
-        def dict(self) -> dict:
-            result = {}
-            for k, v in self.__dict__.items():
-                if v: result[k] = v
-            return result
+        args = {
+            "scriptId": scriptId, "objectGroup": objectGroup, "silent": silent,
+            "includeCommandLineAPI": includeCommandLineAPI, "returnByValue": returnByValue,
+            "generatePreview": generatePreview, "awaitPromise": awaitPromise
+        }
+        if executionContextId is not None:
+            args.update({"executionContextId": executionContextId})
+
+        response = await self._connection.call("Runtime.runScript", args)
+        if "exceptionDetails" in response:
+            raise Exception(response["result"]["description"] + "\n" + json.dumps(response["exceptionDetails"]))
+        return response["result"]
+
+    async def addBinding(self, name: str, executionContextName: Optional[int] = None) -> None:
+        """
+        (EXPERIMENTAL)
+        Если executeContextId пуст, добавляет привязку с заданным именем к глобальным объектам всех
+            проверенных контекстов, включая созданные позже, привязки переживают перезагрузки. Если
+            указан executeContextId, добавляет привязку только к глобальному объекту данного
+            контекста выполнения. Функция привязки принимает ровно один аргумент, этот аргумент
+            должен быть строкой, в случае любого другого ввода функция выдает исключение. Каждый
+            вызов функции привязки создает уведомление Runtime.bindingCalled.
+        https://chromedevtools.github.io/devtools-protocol/tot/Runtime#method-addBinding
+        :param name:                    Имя привязки.
+        :param executionContextName:      (optional) Идентификатор контекста исполнения.
+        :return:
+        """
+        args = {"name": name}
+        if executionContextName is not None:
+            args.update({"executionContextName": executionContextName})
+
+        await self._connection.call("Runtime.addBinding", args)
+
+
+class RuntimeEvent(DomainEvent):
+    consoleAPICalled = "Runtime.consoleAPICalled"
+    exceptionRevoked = "Runtime.exceptionRevoked"
+    exceptionThrown = "Runtime.exceptionThrown"
+    executionContextCreated = "Runtime.executionContextCreated"
+    executionContextDestroyed = "Runtime.executionContextDestroyed"
+    executionContextsCleared = "Runtime.executionContextsCleared"
+    inspectRequested = "Runtime.inspectRequested"
+    bindingCalled = "Runtime.bindingCalled"                       # ! EXPERIMENTAL
```

### Comparing `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Network.py` & `aio_dt_protocol-1.0.0/aio_dt_protocol/domains/network/network.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,27 @@
-from abc import ABC, abstractmethod
-from typing import Optional, Union, List
-from dataclasses import dataclass, field
-from ..Data import Cookie, ConnectionType, DomainEvent
+from typing import Optional, List
+from ...data import DomainEvent
+from .types import ConnectionType, LoadNetworkResourcePageResult, Cookie
 
 
-class Network(ABC):
+class Network:
     """
     #   https://chromedevtools.github.io/devtools-protocol/tot/Network
     """
-    __slots__ = ()
+    __slots__ = ("_connection", "enabled")
 
-    def __init__(self):
-        self.network_domain_enabled   = False
+    def __init__(self, conn) -> None:
 
-    @property
-    def connected(self) -> bool:
-        return False
+        from ...connection import Connection
 
-    @property
-    def verbose(self) -> bool:
-        return False
+        self._connection: Connection = conn
+        self.enabled   = False
 
-    @property
-    def page_id(self) -> str:
-        return ""
 
-    async def NetworkEnable(
+    async def enable(
             self,
             maxTotalBufferSize:    Optional[int] = None,
             maxResourceBufferSize: Optional[int] = None,
             maxPostDataSize:       Optional[int] = None
     ) -> None:
         """
         Включает отслеживание сети, сетевые события теперь будут доставляться клиенту.
@@ -39,31 +31,33 @@
         :param maxResourceBufferSize:   (optional, EXPERIMENTAL) Размер буфера для каждого ресурса в
                                             байтах для использования при сохранении полезных данных сети
                                             (XHR и т. Д.).
         :param maxPostDataSize:         (optional) Самый длинный размер тела сообщения (в байтах),
                                             который будет включен в уведомление "requestWillBeSent".
         :return:
         """
-        args = {}
-        if maxTotalBufferSize is not None: args.update({"maxTotalBufferSize": maxTotalBufferSize})
-        if maxResourceBufferSize is not None: args.update({"maxResourceBufferSize": maxResourceBufferSize})
-        if maxPostDataSize is not None: args.update({"maxPostDataSize": maxPostDataSize})
-        await self.Call("Network.enable", args)
-        self.network_domain_enabled = True
+        if not self.enabled:
+            args = {}
+            if maxTotalBufferSize is not None: args.update({"maxTotalBufferSize": maxTotalBufferSize})
+            if maxResourceBufferSize is not None: args.update({"maxResourceBufferSize": maxResourceBufferSize})
+            if maxPostDataSize is not None: args.update({"maxPostDataSize": maxPostDataSize})
+            await self._connection.call("Network.enable", args)
+            self.enabled = True
 
-    async def NetworkDisable(self) -> None:
+    async def disable(self) -> None:
         """
         Отключает отслеживание сети, запрещает отправку сетевых событий клиенту.
         https://chromedevtools.github.io/devtools-protocol/tot/Network#method-disable
         :return:
         """
-        await self.Call("Network.disable")
-        self.network_domain_enabled = False
+        if self.enabled:
+            await self._connection.call("Network.disable")
+            self.enabled = False
 
-    async def EmulateNetworkConditions(
+    async def emulateNetworkConditions(
         self, latency: int,
         downloadThroughput: int = -1,
         uploadThroughput:   int = -1,
         offline:           bool = False,
         connectionType: Optional[ConnectionType] = None
     ) -> None:
         """
@@ -82,82 +76,82 @@
                                         bluetooth, ethernet, wifi, wimax, other
         :return:
         """
         args = {"latency": latency, "offline": offline}
         if downloadThroughput > -1: args.update({"downloadThroughput": downloadThroughput})
         if uploadThroughput > -1: args.update({"uploadThroughput": uploadThroughput})
         if connectionType: args.update({"connectionType": connectionType.value})
-        await self.Call("Network.emulateNetworkConditions", args)
+        await self._connection.call("Network.emulateNetworkConditions", args)
 
-    async def ClearBrowserCache(self) -> None:
+    async def clearBrowserCache(self) -> None:
         """
         Clears browser cache.
         https://chromedevtools.github.io/devtools-protocol/tot/Network#method-clearBrowserCache
         :return:
         """
-        await self.Call("Network.clearBrowserCache")
+        await self._connection.call("Network.clearBrowserCache")
 
-    async def ClearBrowserCookies(self) -> None:
+    async def clearBrowserCookies(self) -> None:
         """
         Clears browser cookies.
         https://chromedevtools.github.io/devtools-protocol/tot/Network#method-clearBrowserCookies
         :return:
         """
-        await self.Call("Network.clearBrowserCookies")
+        await self._connection.call("Network.clearBrowserCookies")
 
-    async def SetBlockedURLs(self, urls: List[str]) -> None:
+    async def setBlockedURLs(self, urls: List[str]) -> None:
         """
         (EXPERIMENTAL)
         Блокирует загрузку URL-адресов.
         !!!ВНИМАНИЕ!!! Требует активации доменов Page и Network!
         https://chromedevtools.github.io/devtools-protocol/tot/Network#method-setBlockedURLs
         :param urls:            Шаблоны URL для блокировки. Подстановочные знаки ('*') разрешены.
         :return:
         """
-        if not self.network_domain_enabled:
-            await self.NetworkEnable()
-        await self.Call("Network.setBlockedURLs", {"urls": urls})
+        if not self.enabled:
+            await self.enable()
+        await self._connection.call("Network.setBlockedURLs", {"urls": urls})
 
-    async def SetCacheDisabled(self, cacheDisabled: bool = True) -> None:
+    async def setCacheDisabled(self, cacheDisabled: bool = True) -> None:
         """
         Включает игнорирование кеша для каждого запроса. Если 'true', кеш не будет использоваться.
         https://chromedevtools.github.io/devtools-protocol/tot/Network#method-setCacheDisabled
         :param cacheDisabled:    Состояние.
         :return:
         """
-        await self.Call("Network.setCacheDisabled", {"cacheDisabled": cacheDisabled})
+        await self._connection.call("Network.setCacheDisabled", {"cacheDisabled": cacheDisabled})
 
-    async def GetAllCookies(self) -> List[Cookie]:
+    async def getAllCookies(self) -> List[Cookie]:
         """
         Возвращает все куки браузера. В зависимости от поддержки бэкэнда, вернет подробную
             информацию о куки в поле куки.
         https://chromedevtools.github.io/devtools-protocol/tot/Network#method-getAllCookies
         :return: cookies -> (array Cookie) Array of cookie objects.
         """
         cookies = []
-        for c in (await self.Call("Network.getAllCookies"))["cookies"]:
+        for c in (await self._connection.call("Network.getAllCookies"))["cookies"]:
             cookies.append(Cookie(**c))
         return cookies
 
-    async def GetCookies(self, urls: Optional[list] = None) -> List[Cookie]:
+    async def getCookies(self, urls: Optional[list] = None) -> List[Cookie]:
         """
         Возвращает все куки браузера для текущего URL. В зависимости от поддержки бэкэнда,
             вернет подробную информацию о куки в поле куки.
         https://chromedevtools.github.io/devtools-protocol/tot/Network#method-getCookies
         :param urls: список строк содержащих адреса, для которых будут извлечены Cookies [ "https://google.com", ... ]
         :return: cookies -> (array Cookie) Array of cookie objects.
         """
         args = {}
         if urls: args.update({"urls": urls})
         cookies = []
-        for c in (await self.Call("Network.getCookies", args))["cookies"]:
+        for c in (await self._connection.call("Network.getCookies", args))["cookies"]:
             cookies.append(Cookie(**c))
         return cookies
 
-    async def DeleteCookies(
+    async def deleteCookies(
             self, name: str,
             url:    str = "",
             domain: str = "",
             path:   str = ""
     ) -> None:
         """
         Удаляет файлы cookie браузера с соответствующими именами и URL-адресами или парой домен / путь.
@@ -169,17 +163,17 @@
         :param path:    (optional) Если указан, удаляет только те куки, что точно соответствуют 'path'.
         :return:
         """
         args = {"name": name}
         if url: args.update({"url": url})
         if domain: args.update({"domain": domain})
         if path: args.update({"path": path})
-        await self.Call("Network.deleteCookies", args)
+        await self._connection.call("Network.deleteCookies", args)
 
-    async def SetCookie(
+    async def setCookie(
             self, name: str, value: str,
             url:       str = "",
             domain:    str = "",
             path:      str = "",
             secure:   Optional[bool] = None,
             httpOnly: Optional[bool] = None,
             sameSite:  str = "",
@@ -213,36 +207,36 @@
         if domain: args.update({"domain": domain})
         if path: args.update({"path": path})
         if secure is not None: args.update({"secure": secure})
         if secure is not None: args.update({"httpOnly": httpOnly})
         if sameSite: args.update({"sameSite": sameSite})
         if expires > -1: args.update({"expires": expires})
         if priority: args.update({"priority": priority})
-        return (await self.Call("Network.setCookie", args))["success"]
+        return (await self._connection.call("Network.setCookie", args))["success"]
 
-    async def SetCookies(self, list_cookies: list) -> None:
+    async def setCookies(self, list_cookies: list) -> None:
         """
         Устанавливает сразу список кук
         https://chromedevtools.github.io/devtools-protocol/tot/Network#method-setCookies
         :param list_cookies:        список куки-параметров
         :return:
         """
-        await self.Call("Network.setCookies", {"cookies": list_cookies})
+        await self._connection.call("Network.setCookies", {"cookies": list_cookies})
 
-    async def SetExtraHeaders(self, headers: dict) -> None:
+    async def setExtraHTTPHeaders(self, headers: dict) -> None:
         """
         Устанавливает дополнительные заголовки, которые всегда будут отправляться в запросах
             от инстанса текущей страницы.
         https://chromedevtools.github.io/devtools-protocol/tot/Network#method-setExtraHTTPHeaders
         :param headers:        Заголовки запроса / ответа в виде ключей / значений объекта JSON.
         :return:
         """
-        await self.Call("Network.setExtraHTTPHeaders", {"headers": headers})
+        await self._connection.call("Network.setExtraHTTPHeaders", {"headers": headers})
 
-    async def NetworkSetUserAgent(
+    async def setUserAgentOverride(
         self, userAgent: str,
         acceptLanguage:     Optional[str] = None,
         platform:           Optional[str] = None,
         userAgentMetadata: Optional[dict] = None
     ) -> None:
         """
         Позволяет переопределить пользовательский агент с заданной строкой. Функционал ничем не
@@ -266,111 +260,37 @@
                                         }
         :return:            None
         """
         args = {"userAgent": userAgent}
         if acceptLanguage: args.update({"acceptLanguage": acceptLanguage})
         if platform: args.update({"platform": platform})
         if userAgentMetadata: args.update({"userAgentMetadata": userAgentMetadata})
-        await self.Call("Network.setUserAgentOverride", args)
+        await self._connection.call("Network.setUserAgentOverride", args)
 
-    async def LoadNetworkResource(
+    async def loadNetworkResource(
         self,
         url:      Optional[str] = None,
         options: Optional[dict] = None,
         frameId:  Optional[str] = None
-    ) -> "NetworkType.LoadNetworkResourcePageResult":
+    ) -> LoadNetworkResourcePageResult:
         """
         Выбирает ресурс и возвращает контент.
         https://chromedevtools.github.io/devtools-protocol/tot/Network#method-loadNetworkResource
         :param url:             (optional) URL ресурса, для которого нужно получить контент.
         :param options:         (optional) Опции запроса
         :param frameId:         (optional) Идентификатор фрейма
         :return:
         """
-        if url is None: url = await self.GetUrl()
+        if url is None: url = await self._connection.extend.getUrl()
         if options is None: options = {"disableCache": False, "includeCredentials": True}
-        if frameId is None: frameId = self.page_id
+        if frameId is None: frameId = self._connection.conn_id
         args = { "url": url, "options": options, "frameId": frameId }
-        resource = (await self.Call("Network.loadNetworkResource", args))["resource"]
-        return NetworkType.LoadNetworkResourcePageResult(**resource)
+        resource = (await self._connection.call("Network.loadNetworkResource", args))["resource"]
+        return LoadNetworkResourcePageResult(**resource)
 
-    @abstractmethod
-    async def GetUrl(self) -> str:
-        raise NotImplementedError("async method GetUrl() — is not implemented")
-
-    @abstractmethod
-    async def Call(
-        self, domain_and_method: str,
-        params:            Optional[dict] = None,
-        wait_for_response: bool = True
-    ) -> Union[dict, None]: raise NotImplementedError("async method Call() — is not implemented")
-
-
-class NetworkType:
-
-    @dataclass
-    class LoadNetworkResourcePageResult:
-        success: bool
-        netError: Optional[int] = None
-        netErrorName: Optional[str] = None
-        httpStatusCode: Optional[int] = None
-        stream: Optional[str] = None                # ! IO.StreamHandle
-        headers: Optional[dict] = None
-
-
-    @dataclass
-    class Request:
-        url: str
-        method: str
-        headers: dict
-        initialPriority: str                        # ! Allowed Values: VeryLow, Low, Medium, High, VeryHigh
-        referrerPolicy: str                         # ! Allowed Values: unsafe-url, no-referrer-when-downgrade,
-                                                    # !     no-referrer, origin, origin-when-cross-origin, same-origin,
-                                                    # !     strict-origin, strict-origin-when-cross-origin
-        trustTokenParams: Optional["NetworkType.TrustTokenParams"]
-        postDataEntries: Optional[list["NetworkType.PostDataEntry"]]
-        urlFragment: Optional[str] = None
-        postData: Optional[str] = None
-        hasPostData: Optional[bool] = None          # ! true if postData is present
-        _postDataEntries: Optional[list["NetworkType.PostDataEntry"]] = field(init=False, repr=False, default=None)
-        mixedContentType: Optional[str] = None      # ! Allowed Values: blockable, optionally-blockable, none
-        isLinkPreload: Optional[bool] = None
-        _trustTokenParams: Optional["NetworkType.TrustTokenParams"] = field(init=False, repr=False, default=None)
-        isSameSite: Optional[bool] = None
-
-        @property
-        def postDataEntries(self) -> list["NetworkType.PostDataEntry"]:
-            return self._postDataEntries
-
-        @postDataEntries.setter
-        def postDataEntries(self, data: list[dict[str, Union[str, None]]]) -> None:
-            if not isinstance(data, property):
-                self._postDataEntries = [NetworkType.PostDataEntry(**item) for item in data]
-            else:
-                self._postDataEntries = None
-
-        @property
-        def trustTokenParams(self) -> "NetworkType.TrustTokenParams":
-            return self._trustTokenParams
-
-        @trustTokenParams.setter
-        def trustTokenParams(self, data: dict) -> None:
-            self._trustTokenParams = NetworkType.TrustTokenParams(**data) if not isinstance(data, property) else None
-
-
-    @dataclass
-    class PostDataEntry:
-        bytes: Optional[str] = None
-
-
-    @dataclass
-    class TrustTokenParams:
-        type: str                                   # ! Allowed Values: Issuance, Redemption, Signing
-        refreshPolicy: str                          # ! Allowed Values: UseCached, Refresh
-        issuers: Optional[list[str]] = None
 
 class NetworkEvent(DomainEvent):
     dataReceived = "Network.dataReceived"
     eventSourceMessageReceived = "Network.eventSourceMessageReceived"
     loadingFailed = "Network.loadingFailed"
     loadingFinished = "Network.loadingFinished"
     requestServedFromCache = "Network.requestServedFromCache"
```

### Comparing `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Page.py` & `aio_dt_protocol-1.0.0/aio_dt_protocol/domains/page/page.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,245 +1,233 @@
 import asyncio
 from urllib.parse import quote
-from abc import ABC, abstractmethod
-from typing import Optional, Union, Callable, List, Literal
-from ..Data import DomainEvent
-from dataclasses import dataclass, field
+from typing import Optional, Union, Callable, Awaitable
+from ...data import DomainEvent
+from .types import FrameTree, LifecycleEventData
 
 
-class Page(ABC):
+class Page:
     """
     #   https://chromedevtools.github.io/devtools-protocol/tot/Page
     """
-    __slots__ = ()
+    __slots__ = (
+        "_connection", "enabled", "loading_state_watcher_enabled", "network_idle_state_watcher_enabled",
+        "lifecycle_events_enabled", "loading_state", "network_idle_state"
+    )
+    def __init__(self, conn) -> None:
+
+        from ...connection import Connection
+
+        self._connection: Connection = conn
+        self.enabled = False
+        self.loading_state_watcher_enabled = False
+        self.network_idle_state_watcher_enabled = False
+        self.loading_state = asyncio.Event()
+        self.lifecycle_events_enabled = False
+        self.network_idle_state = asyncio.Event()
 
-    def __init__(self):
-        self.page_domain_enabled = False
-
-    @property
-    def connected(self) -> bool:
-        return False
-
-    @property
-    def verbose(self) -> bool:
-        return False
-
-    @property
-    def page_id(self) -> str:
-        return ""
-
-    @property
-    def browser_name(self) -> str: return ""
-
-    async def PageEnable(self) -> None:
+    async def enable(self) -> None:
         """
         Включает уведомления домена 'Page'.
         https://chromedevtools.github.io/devtools-protocol/tot/Page#method-enable
-        :return:
         """
-        if not self.page_domain_enabled:
-            await self.AddListenerForEvent("Page.frameStartedLoading", self._StateLoadWatcher, "started")
-            await self.AddListenerForEvent("Page.frameNavigated", self._StateLoadWatcher, "navigated")
-            await self.AddListenerForEvent("Page.frameStoppedLoading", self._StateLoadWatcher, "stopped")
-            await self.Call("Page.enable")
-            self.page_domain_enabled = True
+        if not self.enabled:
+            await self._connection.call("Page.enable")
+            self.enabled = True
 
-    async def PageDisable(self) -> None:
+    async def disable(self) -> None:
         """
         Выключает уведомления домена 'Page'.
         https://chromedevtools.github.io/devtools-protocol/tot/Page#method-disable
-        :return:
         """
-        if self.page_domain_enabled:
-            self.RemoveListenerForEvent("Page.frameStartedLoading", self._StateLoadWatcher)
-            self.RemoveListenerForEvent("Page.frameNavigated", self._StateLoadWatcher)
-            self.RemoveListenerForEvent("Page.frameStoppedLoading", self._StateLoadWatcher)
-            await self.Call("Page.disable")
-            self.page_domain_enabled = False
-
-    async def _StateLoadWatcher(self, params: dict, state: str) -> None:
-        """
-        Устанавливает состояние загрузки фрейма страницы, если включены уведомления
-            домена Page.
-        """
-        frame_id = params["frameId"] if state != "navigated" else params["frame"]["id"]
-        if frame_id == self.page_id:
-            self.loading_state = state
+        if self.enabled:
+            if self.loading_state_watcher_enabled:
+                await self.enableLoadWatcher(False)
+            if self.network_idle_state_watcher_enabled:
+                await self.enableNetworkIdleWatcher(False)
+            await self._connection.call("Page.disable")
+            self.enabled = False
+
+    async def enableLoadWatcher(self, state: bool) -> None:
+        """ Уведомляет событие loading_state, что основной фрейм страницы завершил загрузку.
+        :param state:           Вкл/выкл
+        """
+        async def load_watcher_wrapper(params: dict) -> None:
+            if params["frameId"] == self._connection.conn_id:
+                self.loading_state.set()
+
+        if state != self.loading_state_watcher_enabled:
+            if state:
+                await self._connection.addListenerForEvent(
+                    PageEvent.frameStoppedLoading, load_watcher_wrapper)
+            else:
+                self._connection.removeListenerForEvent(
+                    PageEvent.frameStoppedLoading, load_watcher_wrapper)
+            self.loading_state_watcher_enabled = state
 
-    async def CreateIsolatedWorld(
+    async def createIsolatedWorld(
             self, frameId: str, worldName: Optional[str] = None, grantUniversalAccess: Optional[bool] = None) -> int:
         """
         Создаёт изолированный мир для указанного фрейма.
         https://chromedevtools.github.io/devtools-protocol/1-3/Page/#method-createIsolatedWorld
         :param frameId:                 Идентификатор фрейма, в котором должен быть создан изолированный мир.
         :param worldName:               Необязательное имя, о котором сообщается в контексте выполнения.
         :param grantUniversalAccess:    Должен ли быть предоставлен универсальный доступ к изолированному миру.
                                             Это мощная опция, используйте ее с осторожностью.
         :return:            Runtime.ExecutionContextId
         """
         args = dict(frameId=frameId)
         if worldName is not None: args.update(worldName=worldName)
         if grantUniversalAccess is not None: args.update(grantUniversalAccess=grantUniversalAccess)
-        result: dict = await self.Call("Page.createIsolatedWorld", args)
+        result: dict = await self._connection.call("Page.createIsolatedWorld", args)
         return result.get("executionContextId")
 
-    async def GetFrameTree(self) -> 'FrameTree':
+    async def getFrameTree(self) -> 'FrameTree':
         """
         Возвращает структуру присутствующих на странице фреймов. !!! Справедливо только в рамках одного домена.
         https://chromedevtools.github.io/devtools-protocol/tot/Page/#method-getFrameTree
         """
-        result = await self.Call("Page.getFrameTree")
-        # print("Page.getFrameTree", result)
+        result = await self._connection.call("Page.getFrameTree")
         return FrameTree(**result.get("frameTree"))
 
     # async def GetFrameFor
 
-    async def HandleJavaScriptDialog(self, accept: bool, promptText: str = "") -> None:
+    async def handleJavaScriptDialog(self, accept: bool, promptText: str = "") -> None:
         """
         Подтверждает или закрывает диалоговое окно, инициированное JavaScript (alert, confirm,
             prompt или для onbeforeunload).
         https://chromedevtools.github.io/devtools-protocol/tot/Page#method-handleJavaScriptDialog
         :param accept:          'True' — принять, 'False' — отклонить диалог.
         :param promptText:      (optional) Текст для ввода в диалоговом окне, прежде чем принять.
                                     Используется, только если это диалоговое окно с подсказкой.
         :return:
         """
         args = {"accept": accept}
         if promptText: args.update({"promptText": promptText})
-        await self.Call("Page.handleJavaScriptDialog", args)
+        await self._connection.call("Page.handleJavaScriptDialog", args)
 
-    async def Navigate(
+    async def navigate(
             self,
-            url:  Union[str, bytes] = "about:blank",
-            wait_for_load:     bool = True,
-            wait_for_complete: bool = False
+            url:  Union[str,     bytes] = "about:blank",
+            wait_for_load:         bool = False,
+            wait_for_network_idle: bool = True,
     ) -> None:
         """
         Переходит на адрес указанного 'url'.
         https://chromedevtools.github.io/devtools-protocol/tot/Page#method-navigate
         :param url:                 Адрес, по которому происходит навигация.
-        :param wait_for_load:       (optional) Если 'True' - ожидает 'complete' у 'document.readyState'
-                                        страницы, на которую осуществляется переход, а так же состояния остановки
-                                        газрузки ресурсов, если активны уведомления домена Page.
-        :param wait_for_complete:   (optional) Если 'True' - ожидает 'complete' у 'document.readyState'
-                                        страницы, на которую осуществляется переход.
+        :param wait_for_load:       (optional) Если 'True' - ожидает состояния остановки
+                                        загрузки ресурсов, если активны уведомления домена Page.
         :return:
         """
-        b_name_len = len(self.browser_name)
+        b_name_len = len(self._connection.browser_name)
         is_url = (
             "http" == url[:4] or
             "chrome" == url[:6] or
-            self.browser_name == url[:b_name_len] or
+            self._connection.browser_name == url[:b_name_len] or
             url == "about:blank"
         )
-        if self.page_domain_enabled: self.loading_state = "do_navigate"
+
+        if self.enabled:
+            self.loading_state.clear()
+        if self.lifecycle_events_enabled:
+            self.network_idle_state.clear()
+
         _url_ = ("data:text/html," + quote(url)
              # передать разметку как data-url, если начало этой строки
              # не содержит признаков url-адреса или передать "как есть",
              if type(url) is str and not is_url else url
                  # раз это строка содержащая url, или переход на пустую страницу
                  if type(url) is str and is_url else
                      # иначе декодировать и установить её как Base64
                      "data:text/html;Base64," + url.decode()
              )
 
-        await self.Call("Page.navigate", {"url": _url_})
-        if wait_for_load:
-            await self.WaitForLoad(ignore_loading_state=wait_for_complete)
-
-    async def WaitForLoad(
-        self,
-        desired_state:         str = "complete",
-        interval:            float = .1,
-        ignore_loading_state: bool = False
-    ) -> None:
-        """
-        Дожидается указанного состояния загрузки документа.
-            Если включены уведомления домена Page — дожидается, пока основной фрейм
-            страницы не перестанет загружаться.
-        :param desired_state:           (optional) Желаемое состояние загрузки. По умолчанию == полное.
-        :param interval:                (optional) Таймаут ожидания.
-        :param ignore_loading_state:    (optional) Ожидать только состояния загрузки страницы?
-        :return:        None
-        """
-
-        if self.page_domain_enabled and not ignore_loading_state:
-            while self.loading_state != "stopped":
-                await asyncio.sleep(.1)
-        else: await asyncio.sleep(1)
+        await self._connection.call("Page.navigate", {"url": _url_})
+        if wait_for_load or wait_for_network_idle:
+            await self.waitForLoad(wait_for_load, wait_for_network_idle)
+
+    async def waitForLoad(self, by_load_state: bool = False, by_network_idle: bool = True) -> None:
+        """ Дожидается указанного состояния.
+        :param by_load_state:       Ожидать завершения загрузки страницы.
+        :param by_network_idle:     Ожидать завершения активности сети.
+        """
+
+        if not by_load_state and not by_network_idle:
+            raise ValueError("'by_load_state' or 'by_network_idle' must be a True")
+
+        if not self.enabled:
+            await self.enable()
+
+        if by_load_state:
+            if not self.loading_state_watcher_enabled:
+                await self.enableLoadWatcher(True)
+                self.loading_state_watcher_enabled = True
+            await self.loading_state.wait()
+
+        if by_network_idle:
+            if not self.network_idle_state_watcher_enabled:
+                await self.enableNetworkIdleWatcher(True)
+            await self.network_idle_state.wait()
 
-        while (await self.Eval("document.readyState"))["value"] != desired_state:
-            await asyncio.sleep(interval)
-
-    async def WaitNavigate(
-            self,
-            url: Union[str, bytes] = "about:blank",
-            wait_for_load: bool    = True,
-            timeout: float         = 10.0
-    ) -> bool:
-        """
-        Дожидается совершения перехода на адрес за указанный интервал времени возвращая True, или False,
-            если дождаться не удалось.
-        :param url:                 Адрес, по которому происходит навигация.
-        :param wait_for_load:       (optional) Если 'True' - ожидает 'complete' у 'document.readyState'
-                                        страницы, на которую осуществляется переход.
-        :param timeout:             (optional) Кол-во секунд ожидания.
-        :return:
-        """
-        try: await asyncio.wait_for(self.Navigate(url, wait_for_load), timeout)
-        except asyncio.exceptions.TimeoutError: return False
-        else: return True
-
-    async def AddScriptOnLoad(self, src: str) -> str:
+    async def addScriptOnLoad(self, src: str) -> str:
         """
         Запускает полученный 'src' скрипта в каждом фрейме и перед загрузкой скриптов самого фрейма.
             Так же, такой скрипт будет запускаться автоматически в течении всей жизни инстанса,
             включая перезагрузку страницы.
-        Требует включения( PageEnable() ) уведомлений домена "Page".
+        Требует включения( Enable() ) уведомлений домена "Page".
         https://chromedevtools.github.io/devtools-protocol/tot/Page#method-addScriptToEvaluateOnNewDocument
         :param src:             Текст сценария.
         :return:                identifier -> Уникальный идентификатор скрипта.
         """
-        if not self.page_domain_enabled: await self.PageEnable()
-        return (await self.Call("Page.addScriptToEvaluateOnNewDocument", {"source": src}))["identifier"]
+        if not self.enabled: await self.enable()
+        return (await self._connection.call("Page.addScriptToEvaluateOnNewDocument", {"source": src}))["identifier"]
 
-    async def RemoveScriptOnLoad(self, identifier: str) -> None:
+    async def removeScriptOnLoad(self, identifier: str) -> None:
         """
         Удаляет данный скрипт из списка запускаемых при загрузке фрейма.
         https://chromedevtools.github.io/devtools-protocol/tot/Page#method-removeScriptToEvaluateOnNewDocument
         :param identifier:      Идентификатор сценария.
         :return:
         """
-        await self.Call("Page.removeScriptToEvaluateOnNewDocument", {"identifier": identifier})
+        await self._connection.call("Page.removeScriptToEvaluateOnNewDocument", {"identifier": identifier})
 
-    async def SetDocumentContent(self, html: str, frameId: str = None) -> None:
+    async def setDocumentContent(self, html: str, frameId: str = None) -> None:
         """
         Устанавливает полученную разметку как HTML-код документа.
             frameId — можно найти среди параметров события 'Runtime.executionContextCreated',
             а так же у корневого элемента документа root.children[1].frameId
         https://chromedevtools.github.io/devtools-protocol/tot/Page#method-setDocumentContent
         :param html:            HTML-разметка.
         :param frameId:         Идентификатор фрейма, которому предназначается html.
         :return:
         """
-        if frameId is None: frameId = self.page_id
-        await self.Call("Page.setDocumentContent", {"frameId": frameId, "html": html})
+        if frameId is None: frameId = self._connection.conn_id
+        await self._connection.call("Page.setDocumentContent", {"frameId": frameId, "html": html})
+
+    async def stopLoading(self) -> None:
+        """
+        Останавливает загрузку страницы.
+        https://chromedevtools.github.io/devtools-protocol/tot/Page#method-stopLoading
+        :return:
+        """
+        await self._connection.call("Page.stopLoading")
 
-    async def SetAdBlockingEnabled(self, enabled: bool) -> None:
+    async def setAdBlockingEnabled(self, enabled: bool) -> None:
         """
         (EXPERIMENTAL)
         Включите экспериментальный рекламный фильтр Chrome на всех сайтах.
         https://chromedevtools.github.io/devtools-protocol/tot/Page#method-setAdBlockingEnabled
         :param enabled:         Включить?
         :return:
         """
-        if not self.page_domain_enabled: await self.PageEnable()
-        await self.Call("Page.setAdBlockingEnabled", {"enabled": enabled})
+        if not self.enabled: await self.enable()
+        await self._connection.call("Page.setAdBlockingEnabled", {"enabled": enabled})
 
-    async def SetFontFamilies(self, fontFamilies: dict) -> None:
+    async def setFontFamilies(self, fontFamilies: dict) -> None:
         """
         (EXPERIMENTAL)
         Установить общие семейства шрифтов.
         https://chromedevtools.github.io/devtools-protocol/tot/Page#method-setFontFamilies
         :param fontFamilies:    Семейства шрифтов:
                                     {
                                         "standard":   str(), -> (optional)
@@ -248,32 +236,32 @@
                                         "sansSerif":  str(), -> (optional)
                                         "cursive":    str(), -> (optional)
                                         "fantasy":    str(), -> (optional)
                                         "pictograph": str(), -> (optional)
                                     }
         :return:
         """
-        await self.Call("Page.setFontFamilies", {"fontFamilies": fontFamilies})
+        await self._connection.call("Page.setFontFamilies", {"fontFamilies": fontFamilies})
 
-    async def SetFontSizes(self, fontSizes: dict) -> None:
+    async def setFontSizes(self, fontSizes: dict) -> None:
         """
         (EXPERIMENTAL)
         Установите размеры шрифта по умолчанию.
         https://chromedevtools.github.io/devtools-protocol/tot/Page#method-setFontSizes
         :param fontSizes:       Определяет размеры шрифта для установки. Если размер шрифта не
                                     указан, он не будет изменен:
                                     {
                                         "standard": int(), -> (optional)
                                         "fixed":    int(), -> (optional)
                                     }
         :return:
         """
-        await self.Call("Page.setFontSizes", {"fontSizes": fontSizes})
+        await self._connection.call("Page.setFontSizes", {"fontSizes": fontSizes})
 
-    async def CaptureScreenshot(
+    async def captureScreenshot(
         self,
         format_: str = "",
         quality: int = -1,
         clip: Optional[dict] = None,
         fromSurface: bool = True
     ) -> str:
         """
@@ -292,17 +280,17 @@
                                     Defaults to true.
         :return:                string => Base64-encoded image data.
         """
         args = {"fromSurface": fromSurface}
         if format_: args.update({"format": format_})
         if quality > -1 and format_ == "jpeg": args.update({"quality": quality})
         if clip: args.update({"clip": clip})
-        return (await self.Call("Page.captureScreenshot", args))["data"]
+        return (await self._connection.call("Page.captureScreenshot", args))["data"]
 
-    async def PrintToPDF(
+    async def printToPDF(
         self,
         landscape:               Optional[bool] = None,
         displayHeaderFooter:     Optional[bool] = None,
         printBackground:         Optional[bool] = None,
         scale:                  Optional[float] = None,
         paperWidth:             Optional[float] = None,
         paperHeight:            Optional[float] = None,
@@ -372,43 +360,47 @@
         if pageRanges is not None:              args.update({"pageRanges": pageRanges})
         if ignoreInvalidPageRanges is not None: args.update({"ignoreInvalidPageRanges": ignoreInvalidPageRanges})
         if headerTemplate is not None:          args.update({"headerTemplate": headerTemplate})
         if footerTemplate is not None:          args.update({"footerTemplate": footerTemplate})
         if preferCSSPageSize is not None:       args.update({"preferCSSPageSize": preferCSSPageSize})
         if transferMode is not None:            args.update({"transferMode": transferMode})
 
-        return await self.Call("Page.printToPDF", args)
+        return await self._connection.call("Page.printToPDF", args)
 
-    async def Reload(
-        self,
-        ignoreCache: bool = False,
-        scriptToEvaluateOnLoad: str = "",
-        wait_for_load: bool = True
+    async def reload(
+            self,
+            ignoreCache: bool = False,
+            scriptToEvaluateOnLoad: str = "",
+            wait_for_load: bool = False,
+            wait_for_network_idle: bool = True
     ) -> None:
         """
         Перезагружает страницу инстанса, при необходимости игнорируя кеш.
         https://chromedevtools.github.io/devtools-protocol/tot/Page#method-reload
         :param ignoreCache:             (optional) Игнорировать кеш?
         :param scriptToEvaluateOnLoad:  (optional) Если установлено, сценарий будет вставлен во все
                                             фреймы проверяемой страницы после перезагрузки. Аргумент
                                             будет игнорироваться при перезагрузке источника dataURL.
         :param wait_for_load:           (optional) По умолчанию — дожидается полного завершения
                                             загрузки страницы(document.readyState === "complete").
                                             Установите False, если это поведение не требуется.
         :return:
         """
-        if self.page_domain_enabled: self.loading_state = "do_reload"
+        if self.enabled:
+            self.loading_state.clear()
+        if self.lifecycle_events_enabled:
+            self.network_idle_state.clear()
         args = {}
         if ignoreCache:            args.update({"ignoreCache": ignoreCache})
         if scriptToEvaluateOnLoad: args.update({"scriptToEvaluateOnLoad": scriptToEvaluateOnLoad})
-        await self.Call("Page.reload", args)
-        if wait_for_load:
-            await self.WaitForLoad()
+        await self._connection.call("Page.reload", args)
+        if wait_for_load or wait_for_network_idle:
+            await self.waitForLoad(wait_for_load, wait_for_network_idle)
 
-    async def GetNavigationHistory(self) -> dict:
+    async def getNavigationHistory(self) -> dict:
         """
         Возвращает историю навигации для текущей страницы.
         https://chromedevtools.github.io/devtools-protocol/tot/Page#method-getNavigationHistory
         :return:            {
                                 "currentIndex": int(), -> Индекс текущей записи истории навигации.
                                 "entries": list({
                                     "id": int(),  -> Уникальный идентификатор записи истории навигации.
@@ -419,72 +411,98 @@
                                         link, typed, address_bar, auto_bookmark, auto_subframe,
                                         manual_subframe, generated, auto_toplevel, form_submit,
                                         reload, keyword, keyword_generated, other
                                     ) -> Тип перехода.
                                 }, ... ) -> Список записей истории навигации.
                             }
         """
-        return await self.Call("Page.getNavigationHistory")
+        return await self._connection.call("Page.getNavigationHistory")
 
-    async def NavigateToHistoryEntry(self, entryId: int) -> None:
+    async def navigateToHistoryEntry(self, entryId: int) -> None:
         """
         Навигация текущей страницы к выбранной записи в истории навгации.
         https://chromedevtools.github.io/devtools-protocol/tot/Page#method-navigateToHistoryEntry
         :param entryId:             Уникальный идентификатор записи для перехода.
         :return:
         """
-        if self.page_domain_enabled: self.loading_state = "do_navigate"
-        await self.Call("Page.navigateToHistoryEntry", {"entryId": entryId})
+        if self.enabled: self.loading_state = "do_navigate"
+        await self._connection.call("Page.navigateToHistoryEntry", {"entryId": entryId})
 
-    async def ResetNavigationHistory(self) -> None:
+    async def resetNavigationHistory(self) -> None:
         """
         Сбрасывает историю навигации для текущей страницы.
         https://chromedevtools.github.io/devtools-protocol/tot/Page#method-resetNavigationHistory
         :return:
         """
-        await self.Call("Page.resetNavigationHistory")
+        await self._connection.call("Page.resetNavigationHistory")
 
-    async def SetInterceptFileChooserDialog(self, enabled: bool) -> None:
+    async def setInterceptFileChooserDialog(self, enabled: bool) -> None:
         """
         Перехватывает запросы выбора файлов и передает управление клиентам протокола. Когда включен перехват
             файлов, диалоговое окно выбора файлов не отображается. Вместо этого генерируется событие
             протокола Page.fileChooserOpened.
         https://chromedevtools.github.io/devtools-protocol/tot/Page#method-setInterceptFileChooserDialog
         :param enabled:             Включить перехват?
         :return:
         """
-        await self.Call("Page.setInterceptFileChooserDialog", {"enabled": enabled})
+        await self._connection.call("Page.setInterceptFileChooserDialog", {"enabled": enabled})
 
-    @abstractmethod
-    async def AddListenerForEvent(
-            self, event: Union[str, DomainEvent], listener: Callable, *args: any) -> None:
-        raise NotImplementedError("async method AddListenerForEvent() — is not implemented")
-
-    @abstractmethod
-    def RemoveListenerForEvent(self, event: str, listener: Callable) -> None:
-        raise NotImplementedError("method RemoveListenerForEvent() — is not implemented")
-
-    @abstractmethod
-    async def Eval(
-            self, expression: str,
-            objectGroup:            str = "console",
-            includeCommandLineAPI: bool = True,
-            silent:                bool = False,
-            returnByValue:         bool = False,
-            userGesture:           bool = True,
-            awaitPromise:          bool = False
-    ) -> dict:
-        raise NotImplementedError("async method Eval() — is not implemented")
+    async def setLifecycleEventsEnabled(
+            self, enabled: bool,
+            handler: Optional[Callable[[LifecycleEventData], Awaitable[None]]] = None,
+    ) -> None:
+        """
+        Определяет, будет ли страница генерировать события жизненного цикла.
+        https://chromedevtools.github.io/devtools-protocol/tot/Page/#method-setLifecycleEventsEnabled
+        :param enabled:            Если true, начинает генерировать события жизненного цикла.
+        :param handler:            Awaitable объект, которому будут переданы данные события.
+        :return:
+        """
+        async def life_cycle_event_wrapper(params: dict) -> None:
+            await handler(LifecycleEventData(**params))
+
+        if self.lifecycle_events_enabled != enabled:
+            if enabled and handler is not None:
+                await self._connection.addListenerForEvent(
+                    PageEvent.lifecycleEvent, life_cycle_event_wrapper)
+            else:
+                self._connection.removeListenersForEvent(PageEvent.lifecycleEvent)
 
-    @abstractmethod
-    async def Call(
-            self, domain_and_method: str,
-            params: Optional[dict] = None,
-            wait_for_response: bool = True
-    ) -> Union[dict, None]: raise NotImplementedError("async method Call() — is not implemented")
+            await self._connection.call("Page.setLifecycleEventsEnabled", {"enabled": enabled})
+            self.lifecycle_events_enabled = enabled
+
+    async def enableNetworkIdleWatcher(self, state: bool) -> None:
+        """ [Вк/Вык]лючает наблюдение за событием жизненного цикла ресурса, когда
+        у него возникает состояние с именем `networkIdle`, говорящее о простое сети.
+
+        Этот метод активируется автоматически при совершении переходов по URL-адресам
+        """
+        async def idle_watcher_wrapper(params: dict) -> None:
+            if params["frameId"] == self._connection.conn_id:
+                if params["name"] == "networkIdle":
+                    self.network_idle_state.set()
+
+        if state:
+            if not self.lifecycle_events_enabled:
+                await self.setLifecycleEventsEnabled(True)
+            if not self.network_idle_state_watcher_enabled:
+                await self._connection.addListenerForEvent(
+                    PageEvent.lifecycleEvent, idle_watcher_wrapper)
+        elif not state and self.network_idle_state_watcher_enabled:
+            self._connection.removeListenerForEvent(
+                PageEvent.lifecycleEvent, idle_watcher_wrapper)
+        self.network_idle_state_watcher_enabled = state
+
+    async def bringToFront(self) -> None:
+        """
+        Выводит страницу на передний план (активирует вкладку).
+        https://chromedevtools.github.io/devtools-protocol/tot/Page#method-bringToFront
+        :return:
+        """
+        await self._connection.call("Page.bringToFront")
 
 
 class PageEvent(DomainEvent):
     domContentEventFired = "Page.domContentEventFired"
     fileChooserOpened = "Page.fileChooserOpened"
     frameAttached = "Page.frameAttached"
     frameDetached = "Page.frameDetached"
@@ -506,84 +524,7 @@
     frameStartedLoading = "Page.frameStartedLoading"                            # ! EXPERIMENTAL
     frameStoppedLoading = "Page.frameStoppedLoading"                            # ! EXPERIMENTAL
     navigatedWithinDocument = "Page.navigatedWithinDocument"                    # ! EXPERIMENTAL
     screencastFrame = "Page.screencastFrame"                                    # ! EXPERIMENTAL
     screencastVisibilityChanged = "Page.screencastVisibilityChanged"            # ! EXPERIMENTAL
     downloadProgress = "Page.downloadProgress"                                  # * EXPERIMENTAL DEPRECATED
     downloadWillBegin = "Page.downloadWillBegin"                                # * EXPERIMENTAL DEPRECATED
-
-
-@dataclass
-class AdFrameStatus:
-    """ Указывает, был ли frame идентифицирован как реклама и почему. """
-    adFrameType: Literal["none", "child", "root"]
-    explanations: Optional[List[Literal["ParentIsAd", "CreatedByAdScript", "MatchedBlockingRule"]]] = None
-
-
-@dataclass
-class Frame:
-    """ Информация о фрейме на странице """
-    id: str
-    loaderId: str                               # ? Network.LoaderId
-    url: str
-    domainAndRegistry: str
-    securityOrigin: str
-    mimeType: str
-    secureContextType: Literal["Secure", "SecureLocalhost", "InsecureScheme", "InsecureAncestor"]
-    crossOriginIsolatedContextType: Literal["Isolated", "NotIsolated", "NotIsolatedFeatureDisabled"]
-    gatedAPIFeatures: List[Literal[
-        "SharedArrayBuffers", "SharedArrayBuffersTransferAllowed", "PerformanceMeasureMemory", "PerformanceProfile"
-    ]]
-    adFrameStatus: Optional['AdFrameStatus']
-    parentId: Optional[str] = None
-    name: Optional[str] = None
-    urlFragment: Optional[str] = None
-    unreachableUrl: Optional[str] = None
-    _adFrameStatus: Optional['AdFrameStatus'] = field(init=False, repr=False, default=None)
-
-    @property
-    def adFrameStatus(self) -> Union['AdFrameStatus', None]:
-        return self._adFrameStatus
-
-    @adFrameStatus.setter
-    def adFrameStatus(self, data: dict) -> None:
-        self._adFrameStatus = AdFrameStatus(**data) if not isinstance(data, property) else None
-
-
-@dataclass
-class FrameTree:
-    """ Информация об иерархии фреймов """
-    frame: 'Frame'
-    childFrames: Optional[List['FrameTree']]
-    _childFrames: Optional[List['FrameTree']] = field(init=False, repr=False, default=None)
-
-    @property
-    def frame(self) -> 'Frame':
-        return self._frame
-
-    @frame.setter
-    def frame(self, data: dict) -> None:
-        self._frame = Frame(**data)
-
-    @property
-    def childFrames(self) -> Union[List['FrameTree'], None]:
-        return self._childFrames
-
-    @childFrames.setter
-    def childFrames(self, data: List[dict]) -> None:
-        if not isinstance(data, property):
-            self._childFrames = [FrameTree(**frame_data) for frame_data in data]
-        else:
-            self._childFrames = None
-
-    def GetFrameByUrl(self, value: str) -> Union['Frame', None]:
-        def search(tree: 'FrameTree', value: str) -> Union['Frame', None]:
-            print("tree.frame.url", tree.frame.url)
-            if value in tree.frame.url:
-                return tree.frame
-            else:
-                if tree.childFrames:
-                    for child in tree.childFrames:
-                        if result := search(child, value):
-                            return result
-            return None
-        return search(self, value)
```

### Comparing `aio_dt_protocol-0.9.5/aio_dt_protocol/domains/Target.py` & `aio_dt_protocol-1.0.0/aio_dt_protocol/domains/target/target.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-from abc import ABC, abstractmethod
-from typing import Optional, Union, List, Awaitable, Callable
-from ..Data import DomainEvent
-from dataclasses import dataclass
+from typing import Optional, List, Awaitable, Callable
+from ...data import DomainEvent
+from .types import TargetInfo
 
-class Target(ABC):
+
+class Target:
     """
     #   https://chromedevtools.github.io/devtools-protocol/tot/Target
     """
-    __slots__ = ()
+    __slots__ = ("_connection", "targets_discovered")
+
+    def __init__(self, conn) -> None:
+
+        from ...connection import Connection
 
-    def __init__(self):
+        self._connection: Connection = conn
         self.targets_discovered = False
 
-    @property
-    def connected(self) -> bool:
-        return False
-
-    @property
-    def verbose(self) -> bool:
-        return False
-
-    @property
-    def is_headless_mode(self) -> bool:
-        return False
-
-    @property
-    def page_id(self) -> str:
-        return ""
+    async def activateTarget(self, targetId: Optional[str] = None) -> None:
+        """
+        Активирует (создаёт фокус) "target".
+        https://chromedevtools.github.io/devtools-protocol/tot/Target#method-activateTarget
+        :param targetId:        Строка, представляющая идентификатор созданной страницы.
+        :return:
+        """
+        if targetId is None: targetId = self._connection.conn_id
+        await self._connection.call("Target.activateTarget", {"targetId": targetId})
 
-    async def CreateBrowserContext(
+    async def createBrowserContext(
         self,
         disposeOnDetach: Optional[bool] = None,
         proxyServer: Optional[str]      = None,
         proxyBypassList: Optional[str]  = None
     ) -> str:
         """
         Создает новый пустой BrowserContext. Аналогичен профилю в режиме инкогнито, но их может быть несколько.
@@ -42,34 +40,34 @@
         :param proxyBypassList:     Список обхода прокси, аналогичный тому, который передается в --proxy-bypass-list.
         :return:                Browser.BrowserContextID
         """
         args = {}
         if disposeOnDetach is not None: args.update(disposeOnDetach=disposeOnDetach)
         if proxyServer is not None: args.update(proxyServer=proxyServer)
         if proxyBypassList is not None: args.update(proxyBypassList=proxyBypassList)
-        return (await self.Call("Target.createBrowserContext", args))["browserContextId"]
+        return (await self._connection.call("Target.createBrowserContext", args))["browserContextId"]
 
-    async def GetBrowserContexts(self) -> List[str]:
+    async def getBrowserContexts(self) -> List[str]:
         """
         Возвращает все контексты браузера, созданные с помощью метода Target.createBrowserContext.
         https://chromedevtools.github.io/devtools-protocol/tot/Target/#method-getBrowserContexts
         :return:                [ Browser.BrowserContextID, Browser.BrowserContextID, ... ]
         """
-        return (await self.Call("Target.getBrowserContexts"))["browserContextIds"]
+        return (await self._connection.call("Target.getBrowserContexts"))["browserContextIds"]
 
-    async def DisposeBrowserContext(self, browserContextId: str) -> None:
+    async def disposeBrowserContext(self, browserContextId: str) -> None:
         """
         Удаляет BrowserContext. Все соответствующие страницы будут закрыты без вызова их хуков beforeunload.
         https://chromedevtools.github.io/devtools-protocol/tot/Target/#method-disposeBrowserContext
         :param browserContextId:    Идентификатор контекста браузера.
         :return:
         """
-        await self.Call("Target.disposeBrowserContext", {"browserContextId": browserContextId})
+        await self._connection.call("Target.disposeBrowserContext", {"browserContextId": browserContextId})
 
-    async def GetTargetInfo(self, targetId: Optional[str] = None) -> 'TargetType.TargetInfo':
+    async def getTargetInfo(self, targetId: Optional[str] = None) -> TargetInfo:
         """
         (EXPERIMENTAL)
         Возвращает информацию о "target", или о себе, если идентификатор не передан.
         https://chromedevtools.github.io/devtools-protocol/tot/Target#method-getTargetInfo
         :param targetId:            Идентификатор страницы/сервиса/воркера/...
         :return:                    targetInfo -> {
                                         "targetId":         str,
@@ -77,62 +75,63 @@
                                         "title":            str,
                                         "url":              str,
                                         "attached":         bool,
                                         "openerId":         str,
                                         "browserContextId": str,
                                     }
         """
-        if targetId is None: targetId = self.page_id
-        return TargetType.TargetInfo(**((await self.Call("Target.getTargetInfo", {"targetId": targetId}))["targetInfo"]))
+        if targetId is None: targetId = self._connection.conn_id
+        return TargetInfo(
+            **((await self._connection.call("Target.getTargetInfo", {"targetId": targetId}))["targetInfo"]))
 
-    async def GetTargets(self) -> List['TargetType.TargetInfo']:
+    async def getTargets(self) -> List[TargetInfo]:
         """
         Возвращает список 'targetInfo' о доступных 'targets'.
         https://chromedevtools.github.io/devtools-protocol/tot/Target#method-getTargets
         :return:                [ targetInfo, targetInfo, ... ]
         """
-        result = (await self.Call("Target.getTargets"))["targetInfos"]
-        return [TargetType.TargetInfo(**info) for i, info in enumerate(result)]
+        result = (await self._connection.call("Target.getTargets"))["targetInfos"]
+        return [TargetInfo(**info) for i, info in enumerate(result)]
 
-    async def AttachToBrowserTarget(self) -> str:
+    async def attachToBrowserTarget(self) -> str:
         """
         Присоединяется к target браузера, использует только режим flat sessionId.
         https://chromedevtools.github.io/devtools-protocol/tot/Target#method-attachToBrowserTarget
         :return:                    sessionId
         """
-        return (await self.Call("Target.attachToBrowserTarget"))["sessionId"]
+        return (await self._connection.call("Target.attachToBrowserTarget"))["sessionId"]
 
-    async def AttachToTarget(self, targetId: str, flatten: Optional[bool] = None) -> str:
+    async def attachToTarget(self, targetId: str, flatten: Optional[bool] = None) -> str:
         """
         Присоединяется к 'target' по указанному 'targetId'.
         https://chromedevtools.github.io/devtools-protocol/tot/Target#method-attachToTarget
         :param targetId:        Строка, представляющая идентификатор созданной страницы.
         :param flatten:         (optional) Разрешает "flat" доступ к сеансу с помощью указания атрибута
                                     sessionId в командах.
         :return:                sessionId -> Идентификатор, назначенный сеансу.
         """
         args = {"targetId": targetId}
         if flatten is not None: args.update({"flatten": flatten})
-        return (await self.Call("Target.attachToTarget", args))["sessionId"]
+        return (await self._connection.call("Target.attachToTarget", args))["sessionId"]
 
-    async def DetachFromTarget(self, sessionId: str = "", targetId: str = "") -> None:
+    async def detachFromTarget(self, sessionId: str = "", targetId: str = "") -> None:
         """
         Отключается от сессии переданного 'sessionId'.
         https://chromedevtools.github.io/devtools-protocol/tot/Target#method-detachFromTarget
         :param sessionId:       (optional) Строка, представляющая идентификатор сессии.
         :param targetId:        (optional) Строка, представляющая идентификатор созданной страницы.
         :return:
         """
         args = {}
         if sessionId: args.update({"sessionId": sessionId})
         elif targetId: args.update({"targetId": targetId})
         else: raise ValueError("At least one parameter must be specified 'sessionId' or 'targetId'")
-        await self.Call("Target.detachFromTarget", args)
+        await self._connection.call("Target.detachFromTarget", args)
 
-    async def SetAutoAttach(
+    async def setAutoAttach(
             self, autoAttach: bool, waitForDebuggerOnStart: bool, flatten: Optional[bool] = None) -> None:
         """
         Определяет, следует ли автоматически присоединяться к новым target, которые считаются связанными
             с этой. При включении также присоединяется ко всем существующим связанным целям. При
             выключении автоматически отсоединяется от всех присоединенных в данный момент целей. Это
             также удаляет все цели, добавленные autoAttachRelated из списка целей, чтобы отслеживать
             создание связанных целей.
@@ -141,17 +140,17 @@
         :param waitForDebuggerOnStart:      Приостанавливать ли новые targets при присоединении к ним.
                                                 Используйте Runtime.runIfWaitingForDebugger для запуска
                                                 приостановленных targets.
         :return:
         """
         args = {"autoAttach": autoAttach, "waitForDebuggerOnStart": waitForDebuggerOnStart}
         if flatten is not None: args.update(flatten=flatten)
-        await self.Call("Target.setAutoAttach", args)
+        await self._connection.call("Target.setAutoAttach", args)
 
-    async def CreateTarget(
+    async def createTarget(
         self,
         url: str                        = "about:blank",
         width: Optional[int]            = None,
         height: Optional[int]           = None,
         browserContextId: Optional[str] = None,
         enableBeginFrameControl: bool   = False,
         newWindow: bool                 = False,
@@ -172,123 +171,105 @@
                                                 умолчанию false).
         :param newWindow:                   Если 'True' — страница будет открыта в новом окне.
         :param background:                  Если 'True' — страница будет открыта в фоне.
         :return:                targetId -> строка, представляющая идентификатор созданной страницы.
         """
         args = {
             "url": url, "enableBeginFrameControl": enableBeginFrameControl,
-            "newWindow": False if self.is_headless_mode else newWindow,
-            "background": False if self.is_headless_mode else background
+            "newWindow": False if self._connection.is_headless_mode else newWindow,
+            "background": False if self._connection.is_headless_mode else background
         }
         if width is not None: args.update(width=width)
         if height is not None: args.update(height=height)
         if browserContextId is not None: args.update(browserContextId=browserContextId)
-        return (await self.Call("Target.createTarget", args))["targetId"]
+        return (await self._connection.call("Target.createTarget", args))["targetId"]
 
-    async def CloseTarget(self, targetId: Optional[str] = None) -> None:
+    async def closeTarget(self, targetId: Optional[str] = None) -> None:
         """
         Закрывает вкладку указанного идентификатора, или завершает собственный инстанс,
             если идентификатор не передан.
         https://chromedevtools.github.io/devtools-protocol/tot/Target#method-closeTarget
         :param targetId:        Строка, представляющая идентификатор созданной страницы.
         :return:                None
         """
-        if targetId is None: targetId = self.page_id
-        await self.Call("Target.closeTarget", {"targetId": targetId})
+        if targetId is None: targetId = self._connection.conn_id
+        await self._connection.call("Target.closeTarget", {"targetId": targetId})
 
-    async def Close(self) -> None:
+    async def close(self) -> None:
         """
         Закрывает вкладку.
         """
-        await self.CloseTarget()
+        await self.closeTarget()
 
-    async def SetDiscoverTargets(
+    async def setDiscoverTargets(
         self, discover: bool,
         message:   Optional[Callable[[str, str], Awaitable[None]]] = None,
-        created:   Optional[Callable[['TargetType.TargetInfo'], Awaitable[None]]] = None,
+        created:   Optional[Callable[['TargetInfo'], Awaitable[None]]] = None,
         crashed:   Optional[Callable[[str, str, int], Awaitable[None]]] = None,
-        changed:   Optional[Callable[['TargetType.TargetInfo'], Awaitable[None]]] = None,
+        changed:   Optional[Callable[['TargetInfo'], Awaitable[None]]] = None,
         destroyed: Optional[Callable[[str], Awaitable[None]]] = None
     ) -> None:
         """
         Управляет обнаружением доступных 'targets' уведомляя об их состоянии с помощью событий
             targetCreated / targetInfoChanged / targetDestroyed.
         https://chromedevtools.github.io/devtools-protocol/tot/Target#method-setDiscoverTargets
         :param discover:            'True' — включает эту надстройку, 'False' — выключает.
         :param message:             Корутина вызываемая для события 'Target.receivedMessageFromTarget'.
         :param created:             Корутина вызываемая для события 'Target.targetCreated'.
         :param crashed:             Корутина вызываемая для события 'Target.targetCrashed'.
         :param changed:             Корутина вызываемая для события 'Target.targetInfoChanged'.
         :param destroyed:           Корутина вызываемая для события 'Target.targetDestroyed'.
         :return:
         """
-        async def message_decor(params: dict, func: Callable[[str, str], Awaitable[None]]) -> None:
-            await func(params["sessionId"], params["message"])
+        async def on_message(params: dict) -> None:
+            await message(params["sessionId"], params["message"])
 
-        async def crash_decor(params: dict, func: Callable[[str, str, int], Awaitable[None]]) -> None:
-            await func(params["targetId"], params["status"], params["errorCode"])
+        async def on_crashed(params: dict) -> None:
+            await crashed(params["targetId"], params["status"], params["errorCode"])
 
-        async def decorator(params: dict, func: Callable[['TargetType.TargetInfo'], Awaitable[None]]) -> None:
-            await func(TargetType.TargetInfo(**params["targetInfo"]))
+        async def on_created(params: dict) -> None:
+            await created(TargetInfo(**params["targetInfo"]))
 
-        async def destroy_decor(params: dict, func: Callable[[str], Awaitable[None]]) -> None:
-            await func(params["targetId"])
-
-        if discover:
-            if message is not None: await self.AddListenerForEvent(TargetEvent.receivedMessageFromTarget, message_decor, message)
-            if created is not None: await self.AddListenerForEvent(TargetEvent.targetCreated, decorator, created)
-            if crashed is not None: await self.AddListenerForEvent(TargetEvent.targetCrashed, crash_decor, crashed)
-            if changed is not None: await self.AddListenerForEvent(TargetEvent.targetInfoChanged, decorator, changed)
-            if destroyed is not None: await self.AddListenerForEvent(TargetEvent.targetDestroyed, destroy_decor, destroyed)
-        else:
-            for event in [
-                'Target.receivedMessageFromTarget',
-                'Target.targetCreated',
-                'Target.targetCrashed',
-                'Target.targetInfoChanged',
-                'Target.targetDestroyed'
-            ]:
-                self.RemoveListenersForEvent(event)
-        self.targets_discovered = discover
-        await self.Call("Target.setDiscoverTargets", {"discover": discover})
-
-    @abstractmethod
-    async def Call(
-        self, domain_and_method: str,
-        params: Optional[dict]            = None,
-        wait_for_response: bool = True
-    ) -> Union[dict, None]: raise NotImplementedError("async method Call() — is not implemented")
-
-    @abstractmethod
-    async def AddListenerForEvent(
-            self, event: Union[str, DomainEvent], listener: Callable, *args: any) -> None:
-        raise NotImplementedError("async method AddListenerForEvent() — is not implemented")
-
-    @abstractmethod
-    def RemoveListenersForEvent(self, event: str) -> None:
-        raise NotImplementedError("method RemoveListenersForEvent() — is not implemented")
+        async def on_changed(params: dict) -> None:
+            await changed(TargetInfo(**params["targetInfo"]))
+
+        async def on_destroyed(params: dict) -> None:
+            await destroyed(params["targetId"])
+
+        if self.targets_discovered != discover:
+            if discover:
+                if message is not None:
+                    await self._connection.addListenerForEvent(
+                        TargetEvent.receivedMessageFromTarget, on_message)
+                if created is not None:
+                    await self._connection.addListenerForEvent(
+                        TargetEvent.targetCreated, on_created)
+                if crashed is not None:
+                    await self._connection.addListenerForEvent(
+                        TargetEvent.targetCrashed, on_crashed)
+                if changed is not None:
+                    await self._connection.addListenerForEvent(
+                        TargetEvent.targetInfoChanged, on_changed)
+                if destroyed is not None:
+                    await self._connection.addListenerForEvent(
+                        TargetEvent.targetDestroyed, on_destroyed)
+            else:
+                for event in [
+                    'Target.receivedMessageFromTarget',
+                    'Target.targetCreated',
+                    'Target.targetCrashed',
+                    'Target.targetInfoChanged',
+                    'Target.targetDestroyed'
+                ]:
+                    self._connection.removeListenersForEvent(event)
+            self.targets_discovered = discover
+            await self._connection.call("Target.setDiscoverTargets", {"discover": discover})
 
 
 class TargetEvent(DomainEvent):
     receivedMessageFromTarget = "Target.receivedMessageFromTarget"
     targetCrashed = "Target.targetCrashed"
     targetCreated = "Target.targetCreated"
     targetDestroyed = "Target.targetDestroyed"
     targetInfoChanged = "Target.targetInfoChanged"
     attachedToTarget = "Target.attachedToTarget"                        # ! EXPERIMENTAL
     detachedFromTarget = "Target.detachedFromTarget"                    # ! EXPERIMENTAL
-
-
-class TargetType:
-
-    @dataclass
-    class RemoteLocation:
-        host: str; port: int
-
-
-    @dataclass
-    class TargetInfo:
-        targetId: str; type: str; title: str; url: str; attached: bool
-        openerId:         Optional[str] = None
-        canAccessOpener: Optional[bool] = None
-        openerFrameId:    Optional[str] = None
-        browserContextId: Optional[str] = None
```

### Comparing `aio_dt_protocol-0.9.5/aio_dt_protocol/exceptions.py` & `aio_dt_protocol-1.0.0/aio_dt_protocol/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.5/aio_dt_protocol/utils.py` & `aio_dt_protocol-1.0.0/aio_dt_protocol/utils.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.5/aio_dt_protocol.egg-info/PKG-INFO` & `aio_dt_protocol-1.0.0/aio_dt_protocol.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-dt-protocol
-Version: 0.9.5
+Version: 1.0.0
 Summary: Asynchronous wrapper over Chromium browser debugger protocol.
 Home-page: https://github.com/PieceOfGood/aio_dt_protocol
 Author: PieceOfGood
 Author-email: 78sanchezz@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
@@ -30,17 +30,17 @@
 И так как всё общение через протокол основано на формате JSON, по желанию можно установить ujson:
 https://github.com/ultrajson/ultrajson
 
 ### Примеры:
 
 ```python
 import asyncio
-from aio_dt_protocol import BrowserEx as Browser
+from aio_dt_protocol import Browser
 from aio_dt_protocol import find_instances
-from aio_dt_protocol.Data import KeyEvents
+from aio_dt_protocol.data import KeyEvents
 
 DEBUG_PORT: int = 9222
 BROWSER_NAME: str = "chrome"
 
 
 async def main() -> None:
     # ? Если на указанном порту есть запущенный браузер, происходит подключение.
@@ -56,42 +56,42 @@
         msg = f"[- LAUNCH NEW BROWSER ON {DEBUG_PORT} PORT -]"
     print(msg)
 
     # ? Будет печатать в консоль всё, что приходит по соединению со страницей.
     # ? Полезно при разработке.
     # async def action_printer(data: dict) -> None:
     #     print(data)
-    # page = await browser.GetPage(callback=action_printer)
-    page = await browser.GetPage()
+    # conn = await browser.getPage(callback=action_printer)
+    conn = await browser.getPage()
 
     print("[- GO TO GOOGLE ... -]")
-    await page.Navigate("https://www.google.com")
+    await conn.Page.navigate("https://www.google.com")
 
-    input_node = await page.QuerySelector("input")
-    await input_node.Click()
+    input_node = await conn.DOM.querySelector("input")
+    await input_node.click()
     await asyncio.sleep(1)
-    await page.action.InsertText("github PieceOfGood")
+    await conn.extend.action.insertText("github PieceOfGood")
     await asyncio.sleep(1)
-    await page.action.SendKeyEvent(KeyEvents.enter)
+    await conn.extend.action.sendKeyEvent(KeyEvents.enter)
     await asyncio.sleep(1)
 
     submit_button_selector = "div:not([jsname])>center>[type=submit]:not([jsaction])"
 
-    submit_button = await page.QuerySelector(submit_button_selector)
-    await submit_button.Click()
+    submit_button = await conn.DOM.querySelector(submit_button_selector)
+    await submit_button.click()
 
     # ? Или выполнить клик используя JS
     # click_code = f"""\
     # document.querySelector("{submit_button_selector}").click();
     # """
-    # await page.InjectJS(click_code)
+    # await conn.extend.injectJS(click_code)
 
     print("[- WAIT FOR CLOSE PAGE ... -]")
     # ? Пока соединение существует, цикл выполняется.
-    await page.WaitForClose()
+    await conn.waitForClose()
     print("[- DONE -]")
 
 
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
@@ -114,55 +114,59 @@
                  func_name: "test_func",
                  args: [1, "test"]
             }))
         });
     </script>
     </html>"""
 
-    # ? number и text будут переданы из браузера, а bind_arg указан при регистрации
-    async def test_func(number: int, text: str, bind_arg: dict) -> None:
-        print(f"[- test_func -] Called with args:\n\tnumber: {number}\n\ttext: {text}\n\tbing_arg: {bind_arg}")
-
-    await page.AddListener(
-        test_func,                          # ! слушатель
-        {"name": "test", "value": True}     # ! bind_arg
-    )
 
-    # ? Если ожидается внушительный функционал прикрутить к странице, то это можно
-    # ? сделать за один раз.
-    # await page.AddListeners(
-    #     (test_func, [ {"name": "test", "value": True} ]),
-    #     # (any_awaitable1, [1, 2, 3])
-    #     # (any_awaitable2, [])
-    # )
+# ? number и text будут переданы из браузера, а bind_arg указан при регистрации
+async def test_func(number: int, text: str, bind_arg: dict) -> None:
+    print(f"[- test_func -] Called with args:\n\tnumber: {number}\n\ttext: {text}\n\tbing_arg: {bind_arg}")
+
+
+await conn.addListener(
+    test_func,  # ! слушатель
+    {"name": "test", "value": True}  # ! bind_arg
+)
+
+# ? Если ожидается внушительный функционал прикрутить к странице, то это можно
+# ? сделать за один раз.
+# await conn.addListeners(
+#     (test_func, [ {"name": "test", "value": True} ]),
+#     # (any_awaitable1, [1, 2, 3])
+#     # (any_awaitable2, [])
+# )
 
-    await page.Navigate(html)
+await conn.Page.navigate(html)
 ```
 ### Headless
 Чтобы запустить браузер в `безголовом` режиме, нужно передать аргументу принимающему путь к папке профиля пустую строку.
+
 ```python
 import asyncio
-from aio_dt_protocol import BrowserEx as Browser
+from aio_dt_protocol import Browser
 from aio_dt_protocol.utils import save_img_as, async_util_call
 
 
 async def main() -> None:
     print("[- HEADLESS RUN -]")
     browser = Browser(profile_path="")
     print("[- WAITING PAGE -]")
-    page = await browser.WaitFirstTab()
+    conn = await browser.waitFirstTab()
     print("[- GO TO GOOGLE -]")
-    await page.Navigate("https://www.google.com")
-    
+    await conn.Page.navigate("https://www.google.com")
+
     print("[- MAKE SCREENSHOT -]")
     await async_util_call(
-        save_img_as, "google.png", await page.MakeScreenshot()
+        save_img_as, "google.png", await conn.Page.makeScreenshot()
     )
-    
+
     print("[- CLOSE BROWSER -]")
-    await page.CloseBrowser()
+    await conn.Browser.close()
     print("[- DONE -]")
 
+
 if __name__ == '__main__':
     asyncio.run(main())
 
 ```
```

### Comparing `aio_dt_protocol-0.9.5/aio_dt_protocol.egg-info/SOURCES.txt` & `aio_dt_protocol-1.0.0/aio_dt_protocol.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,65 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-aio_dt_protocol/Actions.py
-aio_dt_protocol/Browser.py
-aio_dt_protocol/BrowserEx.py
-aio_dt_protocol/DOMElement.py
-aio_dt_protocol/Data.py
-aio_dt_protocol/Page.py
-aio_dt_protocol/PageEx.py
 aio_dt_protocol/__init__.py
+aio_dt_protocol/actions.py
+aio_dt_protocol/browser.py
+aio_dt_protocol/connection.py
+aio_dt_protocol/data.py
 aio_dt_protocol/exceptions.py
+aio_dt_protocol/extend_connection.py
 aio_dt_protocol/utils.py
 aio_dt_protocol.egg-info/PKG-INFO
 aio_dt_protocol.egg-info/SOURCES.txt
 aio_dt_protocol.egg-info/dependency_links.txt
 aio_dt_protocol.egg-info/requires.txt
 aio_dt_protocol.egg-info/top_level.txt
-aio_dt_protocol/domains/BackgroundService.py
-aio_dt_protocol/domains/Browser.py
-aio_dt_protocol/domains/CSS.py
-aio_dt_protocol/domains/Console.py
-aio_dt_protocol/domains/DOM.py
-aio_dt_protocol/domains/DeviceOrientation.py
-aio_dt_protocol/domains/Emulation.py
-aio_dt_protocol/domains/Fetch.py
-aio_dt_protocol/domains/Log.py
-aio_dt_protocol/domains/Network.py
-aio_dt_protocol/domains/Overlay.py
-aio_dt_protocol/domains/Page.py
-aio_dt_protocol/domains/Runtime.py
-aio_dt_protocol/domains/SystemInfo.py
-aio_dt_protocol/domains/Target.py
-aio_dt_protocol/domains/__init__.py
+aio_dt_protocol/domains/__init__.py
+aio_dt_protocol/domains/background_service/__init__.py
+aio_dt_protocol/domains/background_service/background_service.py
+aio_dt_protocol/domains/background_service/types.py
+aio_dt_protocol/domains/browser/__init__.py
+aio_dt_protocol/domains/browser/browser.py
+aio_dt_protocol/domains/browser/types.py
+aio_dt_protocol/domains/css/__init__.py
+aio_dt_protocol/domains/css/css.py
+aio_dt_protocol/domains/css/types.py
+aio_dt_protocol/domains/device_orientation/__init__.py
+aio_dt_protocol/domains/device_orientation/device_orientation.py
+aio_dt_protocol/domains/device_orientation/types.py
+aio_dt_protocol/domains/dom/__init__.py
+aio_dt_protocol/domains/dom/dom.py
+aio_dt_protocol/domains/dom/dom_element.py
+aio_dt_protocol/domains/dom/types.py
+aio_dt_protocol/domains/emulation/__init__.py
+aio_dt_protocol/domains/emulation/emulation.py
+aio_dt_protocol/domains/emulation/types.py
+aio_dt_protocol/domains/fetch/__init__.py
+aio_dt_protocol/domains/fetch/fetch.py
+aio_dt_protocol/domains/fetch/types.py
+aio_dt_protocol/domains/input/__init__.py
+aio_dt_protocol/domains/input/input.py
+aio_dt_protocol/domains/input/types.py
+aio_dt_protocol/domains/log/__init__.py
+aio_dt_protocol/domains/log/log.py
+aio_dt_protocol/domains/log/types.py
+aio_dt_protocol/domains/network/__init__.py
+aio_dt_protocol/domains/network/network.py
+aio_dt_protocol/domains/network/types.py
+aio_dt_protocol/domains/overlay/__init__.py
+aio_dt_protocol/domains/overlay/overlay.py
+aio_dt_protocol/domains/overlay/types.py
+aio_dt_protocol/domains/page/__init__.py
+aio_dt_protocol/domains/page/page.py
+aio_dt_protocol/domains/page/types.py
+aio_dt_protocol/domains/runtime/__init__.py
+aio_dt_protocol/domains/runtime/runtime.py
+aio_dt_protocol/domains/runtime/types.py
+aio_dt_protocol/domains/system_info/__init__.py
+aio_dt_protocol/domains/system_info/system_info.py
+aio_dt_protocol/domains/system_info/types.py
+aio_dt_protocol/domains/target/__init__.py
+aio_dt_protocol/domains/target/target.py
+aio_dt_protocol/domains/target/types.py
```

### Comparing `aio_dt_protocol-0.9.5/setup.py` & `aio_dt_protocol-1.0.0/setup.py`

 * *Files identical despite different names*

