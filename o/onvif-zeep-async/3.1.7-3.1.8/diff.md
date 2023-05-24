# Comparing `tmp/onvif-zeep-async-3.1.7.tar.gz` & `tmp/onvif-zeep-async-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-zeep-async-3.1.7.tar", last modified: Sun May 14 17:33:03 2023, max compression
+gzip compressed data, was "onvif-zeep-async-3.1.8.tar", last modified: Wed May 24 14:19:34 2023, max compression
```

## Comparing `onvif-zeep-async-3.1.7.tar` & `onvif-zeep-async-3.1.8.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 17:33:03.109942 onvif-zeep-async-3.1.7/
--rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/.pre-commit-config.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.7/CHANGES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.7/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/MANIFEST.in
--rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/Makefile
--rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-14 17:33:03.109992 onvif-zeep-async-3.1.7/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/README.rst
--rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/bandit.yaml
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 17:33:03.101055 onvif-zeep-async-3.1.7/examples/
--rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/examples/events.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/examples/rotate_image.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/examples/streaming.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 17:33:03.102269 onvif-zeep-async-3.1.7/onvif/
--rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-05-14 16:23:24.000000 onvif-zeep-async-3.1.7/onvif/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    24998 2023-05-14 17:17:16.000000 onvif-zeep-async-3.1.7/onvif/client.py
--rw-r--r--   0 bdraco     (501) staff       (20)      104 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.7/onvif/const.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/definition.py
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)    12024 2023-05-14 17:32:05.000000 onvif-zeep-async-3.1.7/onvif/managers.py
--rw-r--r--   0 bdraco     (501) staff       (20)      157 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.7/onvif/settings.py
--rw-r--r--   0 bdraco     (501) staff       (20)      563 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.7/onvif/transport.py
--rw-r--r--   0 bdraco     (501) staff       (20)      764 2023-05-14 17:17:16.000000 onvif-zeep-async-3.1.7/onvif/types.py
--rw-r--r--   0 bdraco     (501) staff       (20)     3613 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.7/onvif/util.py
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-14 17:32:45.000000 onvif-zeep-async-3.1.7/onvif/version.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     2331 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.7/onvif/wrappers.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 17:33:03.108841 onvif-zeep-async-3.1.7/onvif/wsdl/
--rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/accesscontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/actionengine.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/addressing
--rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/advancedsecurity.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/analytics.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/analyticsdevice.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/b-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/bf-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/bw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/deviceio.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/devicemgmt.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/display.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/doorcontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/envelope
--rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/events.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/imaging.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/include
--rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/media.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/onvif.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/ptz.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/r-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/receiver.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/recording.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/remotediscovery.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/replay.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/rw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/search.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/t-1.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/types.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/ws-addr.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/ws-discovery.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/xml.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/onvif/wsdl/xmlmime
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 17:33:03.109634 onvif-zeep-async-3.1.7/onvif_zeep_async.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-14 17:33:03.000000 onvif-zeep-async-3.1.7/onvif_zeep_async.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     1553 2023-05-14 17:33:03.000000 onvif-zeep-async-3.1.7/onvif_zeep_async.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-14 17:33:03.000000 onvif-zeep-async-3.1.7/onvif_zeep_async.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-14 17:33:03.000000 onvif-zeep-async-3.1.7/onvif_zeep_async.egg-info/entry_points.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-3.1.7/onvif_zeep_async.egg-info/not-zip-safe
--rw-r--r--   0 bdraco     (501) staff       (20)       63 2023-05-14 17:33:03.000000 onvif-zeep-async-3.1.7/onvif_zeep_async.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-14 17:33:03.000000 onvif-zeep-async-3.1.7/onvif_zeep_async.egg-info/top_level.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/pyproject.toml
--rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-14 17:33:03.110220 onvif-zeep-async-3.1.7/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1836 2023-05-14 17:17:16.000000 onvif-zeep-async-3.1.7/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-14 17:33:03.109843 onvif-zeep-async-3.1.7/tests/
--rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.7/tests/test.py
--rw-r--r--   0 bdraco     (501) staff       (20)      291 2023-05-07 02:28:47.000000 onvif-zeep-async-3.1.7/tests/test_util.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-24 14:19:34.160561 onvif-zeep-async-3.1.8/
+-rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.8/CHANGES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.8/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/MANIFEST.in
+-rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/Makefile
+-rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-24 14:19:34.160641 onvif-zeep-async-3.1.8/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/README.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/bandit.yaml
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-24 14:19:34.150068 onvif-zeep-async-3.1.8/examples/
+-rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/examples/events.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/examples/rotate_image.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/examples/streaming.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-24 14:19:34.152464 onvif-zeep-async-3.1.8/onvif/
+-rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-05-14 16:23:24.000000 onvif-zeep-async-3.1.8/onvif/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    25053 2023-05-24 14:16:33.000000 onvif-zeep-async-3.1.8/onvif/client.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      104 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.8/onvif/const.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/definition.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    12024 2023-05-24 14:18:59.000000 onvif-zeep-async-3.1.8/onvif/managers.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      157 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.8/onvif/settings.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      563 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.8/onvif/transport.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      764 2023-05-14 17:17:16.000000 onvif-zeep-async-3.1.8/onvif/types.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     3947 2023-05-24 14:19:06.000000 onvif-zeep-async-3.1.8/onvif/util.py
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-24 14:19:11.000000 onvif-zeep-async-3.1.8/onvif/version.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     2331 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.8/onvif/wrappers.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-24 14:19:34.159251 onvif-zeep-async-3.1.8/onvif/wsdl/
+-rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/accesscontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/actionengine.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/addressing
+-rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/advancedsecurity.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/analytics.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/analyticsdevice.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/b-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/bf-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/bw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/deviceio.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/devicemgmt.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/display.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/doorcontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/envelope
+-rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/events.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/imaging.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/include
+-rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/media.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/onvif.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/ptz.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/r-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/receiver.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/recording.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/remotediscovery.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/replay.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/rw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/search.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/t-1.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/types.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/ws-addr.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/ws-discovery.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/xml.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/xmlmime
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-24 14:19:34.160135 onvif-zeep-async-3.1.8/onvif_zeep_async.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-24 14:19:34.000000 onvif-zeep-async-3.1.8/onvif_zeep_async.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     1553 2023-05-24 14:19:34.000000 onvif-zeep-async-3.1.8/onvif_zeep_async.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-24 14:19:34.000000 onvif-zeep-async-3.1.8/onvif_zeep_async.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-24 14:19:34.000000 onvif-zeep-async-3.1.8/onvif_zeep_async.egg-info/entry_points.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-3.1.8/onvif_zeep_async.egg-info/not-zip-safe
+-rw-r--r--   0 bdraco     (501) staff       (20)       63 2023-05-24 14:19:34.000000 onvif-zeep-async-3.1.8/onvif_zeep_async.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-24 14:19:34.000000 onvif-zeep-async-3.1.8/onvif_zeep_async.egg-info/top_level.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/pyproject.toml
+-rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-24 14:19:34.160873 onvif-zeep-async-3.1.8/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1836 2023-05-14 17:17:16.000000 onvif-zeep-async-3.1.8/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-24 14:19:34.160350 onvif-zeep-async-3.1.8/tests/
+-rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/tests/test.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     3533 2023-05-24 14:16:33.000000 onvif-zeep-async-3.1.8/tests/test_util.py
```

### Comparing `onvif-zeep-async-3.1.7/.gitignore` & `onvif-zeep-async-3.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/.pre-commit-config.yaml` & `onvif-zeep-async-3.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/LICENSE` & `onvif-zeep-async-3.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/Makefile` & `onvif-zeep-async-3.1.8/Makefile`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/PKG-INFO` & `onvif-zeep-async-3.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 3.1.7
+Version: 3.1.8
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-3.1.7/README.rst` & `onvif-zeep-async-3.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/examples/events.py` & `onvif-zeep-async-3.1.8/examples/events.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/examples/rotate_image.py` & `onvif-zeep-async-3.1.8/examples/rotate_image.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/examples/streaming.py` & `onvif-zeep-async-3.1.8/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/__init__.py` & `onvif-zeep-async-3.1.8/onvif/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/client.py` & `onvif-zeep-async-3.1.8/onvif/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -569,15 +569,17 @@
                 self.port,
             )
             return xaddr, wsdlpath, binding_name
 
         # Get other XAddr
         xaddr = self.xaddrs.get(namespace)
         if not xaddr:
-            raise ONVIFError("Device doesn`t support service: %s" % name)
+            raise ONVIFError(
+                f"Device doesn`t support service: {name} with namespace {namespace}"
+            )
 
         return xaddr, wsdlpath, binding_name
 
     async def create_onvif_service(
         self,
         name: str,
         port_type: str | None = None,
```

### Comparing `onvif-zeep-async-3.1.7/onvif/definition.py` & `onvif-zeep-async-3.1.8/onvif/definition.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/exceptions.py` & `onvif-zeep-async-3.1.8/onvif/exceptions.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/managers.py` & `onvif-zeep-async-3.1.8/onvif/managers.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/transport.py` & `onvif-zeep-async-3.1.8/onvif/transport.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/types.py` & `onvif-zeep-async-3.1.8/onvif/types.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/util.py` & `onvif-zeep-async-3.1.8/onvif/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,32 +3,37 @@
 
 import contextlib
 import datetime as dt
 from functools import lru_cache, partial
 import os
 import ssl
 from typing import Any
-from urllib.parse import urlparse, urlunparse
+from urllib.parse import urlparse, urlunparse, ParseResultBytes
 
 from zeep.exceptions import Fault
 
 utcnow: partial[dt.datetime] = partial(dt.datetime.now, dt.timezone.utc)
 
 # This does blocking I/O (stat) so we cache the result
 # to minimize the impact of the blocking I/O.
 path_isfile = lru_cache(maxsize=128)(os.path.isfile)
 
 
-def normalize_url(url: str) -> str:
+def normalize_url(url: bytes | str | None) -> str | None:
     """Normalize URL.
 
     Some cameras respond with <wsa5:Address>http://192.168.1.106:8106:8106/onvif/Subscription?Idx=43</wsa5:Address>
     https://github.com/home-assistant/core/issues/92603#issuecomment-1537213126
     """
+    if url is None:
+        return None
     parsed = urlparse(url)
+    # If the URL is not a string, return None
+    if isinstance(parsed, ParseResultBytes):
+        return None
     if "[" not in parsed.netloc and parsed.netloc.count(":") > 1:
         net_location = parsed.netloc.split(":", 3)
         net_location.pop()
         return urlunparse(parsed._replace(netloc=":".join(net_location)))
     return url
 
 
@@ -92,8 +97,10 @@
     sslcontext.verify_mode = ssl.CERT_NONE
     # Allow all ciphers rather than only Python 3.10 default
     sslcontext.set_ciphers("DEFAULT")
     with contextlib.suppress(AttributeError):
         # This only works for OpenSSL >= 1.0.0
         sslcontext.options |= ssl.OP_NO_COMPRESSION
     sslcontext.set_default_verify_paths()
+    # ssl.OP_LEGACY_SERVER_CONNECT is only available in Python 3.12a4+
+    sslcontext.options |= getattr(ssl, "OP_LEGACY_SERVER_CONNECT", 0x4)
     return sslcontext
```

### Comparing `onvif-zeep-async-3.1.7/onvif/wrappers.py` & `onvif-zeep-async-3.1.8/onvif/wrappers.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/accesscontrol.wsdl` & `onvif-zeep-async-3.1.8/onvif/wsdl/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/actionengine.wsdl` & `onvif-zeep-async-3.1.8/onvif/wsdl/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/addressing` & `onvif-zeep-async-3.1.8/onvif/wsdl/addressing`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/advancedsecurity.wsdl` & `onvif-zeep-async-3.1.8/onvif/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/analytics.wsdl` & `onvif-zeep-async-3.1.8/onvif/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/analyticsdevice.wsdl` & `onvif-zeep-async-3.1.8/onvif/wsdl/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/b-2.xsd` & `onvif-zeep-async-3.1.8/onvif/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/bf-2.xsd` & `onvif-zeep-async-3.1.8/onvif/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/bw-2.wsdl` & `onvif-zeep-async-3.1.8/onvif/wsdl/bw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/deviceio.wsdl` & `onvif-zeep-async-3.1.8/onvif/wsdl/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/devicemgmt.wsdl` & `onvif-zeep-async-3.1.8/onvif/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/display.wsdl` & `onvif-zeep-async-3.1.8/onvif/wsdl/display.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/doorcontrol.wsdl` & `onvif-zeep-async-3.1.8/onvif/wsdl/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/envelope` & `onvif-zeep-async-3.1.8/onvif/wsdl/envelope`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/events.wsdl` & `onvif-zeep-async-3.1.8/onvif/wsdl/events.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/imaging.wsdl` & `onvif-zeep-async-3.1.8/onvif/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/media.wsdl` & `onvif-zeep-async-3.1.8/onvif/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/onvif.xsd` & `onvif-zeep-async-3.1.8/onvif/wsdl/onvif.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/ptz.wsdl` & `onvif-zeep-async-3.1.8/onvif/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/r-2.xsd` & `onvif-zeep-async-3.1.8/onvif/wsdl/r-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/receiver.wsdl` & `onvif-zeep-async-3.1.8/onvif/wsdl/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/recording.wsdl` & `onvif-zeep-async-3.1.8/onvif/wsdl/recording.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/remotediscovery.wsdl` & `onvif-zeep-async-3.1.8/onvif/wsdl/remotediscovery.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/replay.wsdl` & `onvif-zeep-async-3.1.8/onvif/wsdl/replay.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/rw-2.wsdl` & `onvif-zeep-async-3.1.8/onvif/wsdl/rw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/search.wsdl` & `onvif-zeep-async-3.1.8/onvif/wsdl/search.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/t-1.xsd` & `onvif-zeep-async-3.1.8/onvif/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/types.xsd` & `onvif-zeep-async-3.1.8/onvif/wsdl/types.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/ws-addr.xsd` & `onvif-zeep-async-3.1.8/onvif/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/ws-discovery.xsd` & `onvif-zeep-async-3.1.8/onvif/wsdl/ws-discovery.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/xml.xsd` & `onvif-zeep-async-3.1.8/onvif/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif/wsdl/xmlmime` & `onvif-zeep-async-3.1.8/onvif/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/onvif_zeep_async.egg-info/PKG-INFO` & `onvif-zeep-async-3.1.8/onvif_zeep_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 3.1.7
+Version: 3.1.8
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-3.1.7/onvif_zeep_async.egg-info/SOURCES.txt` & `onvif-zeep-async-3.1.8/onvif_zeep_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/pylintrc` & `onvif-zeep-async-3.1.8/pylintrc`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/setup.py` & `onvif-zeep-async-3.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.7/tests/test.py` & `onvif-zeep-async-3.1.8/tests/test.py`

 * *Files identical despite different names*

