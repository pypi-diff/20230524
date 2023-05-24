# Comparing `tmp/py-Ayiin-0.3.3.tar.gz` & `tmp/py-Ayiin-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.3.3.tar", last modified: Tue May 23 10:54:34 2023, max compression
+gzip compressed data, was "py-Ayiin-0.3.4.tar", last modified: Wed May 24 09:48:10 2023, max compression
```

## Comparing `py-Ayiin-0.3.3.tar` & `py-Ayiin-0.3.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:34.265192 py-Ayiin-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-23 10:54:34.265192 py-Ayiin-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:34.257192 py-Ayiin-0.3.3/pyAyiin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:34.257192 py-Ayiin-0.3.3/pyAyiin/Clients/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/Clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/Clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/Clients/pytgcalls.py
--rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/Clients/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:34.261192 py-Ayiin-0.3.3/pyAyiin/dB/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/absen.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/blacklistfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/blacklistgcast.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/blacklistuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/gban.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/logdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/pmpermit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/videocalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/dB/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:34.261192 py-Ayiin-0.3.3/pyAyiin/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/changer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/funcb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/inlinebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:34.265192 py-Ayiin-0.3.3/pyAyiin/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/pyrogram/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/pyrogram/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/pyrogram/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/pyrogram/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/pyrogram/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/pyrogram/toolbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/pyrogram/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:34.265192 py-Ayiin-0.3.3/pyAyiin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:34.265192 py-Ayiin-0.3.3/pyAyiin/telethon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/telethon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:34.265192 py-Ayiin-0.3.3/pyAyiin/telethon/ayiin/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/telethon/ayiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/telethon/ayiin/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/telethon/ayiin/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/telethon/ayiin/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/pyAyiin/xd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:54:34.265192 py-Ayiin-0.3.3/py_Ayiin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-23 10:54:34.000000 py-Ayiin-0.3.3/py_Ayiin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-23 10:54:34.000000 py-Ayiin-0.3.3/py_Ayiin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 10:54:34.000000 py-Ayiin-0.3.3/py_Ayiin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-23 10:54:34.000000 py-Ayiin-0.3.3/py_Ayiin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 10:54:34.000000 py-Ayiin-0.3.3/py_Ayiin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 10:54:34.265192 py-Ayiin-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-23 10:54:21.000000 py-Ayiin-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:48:10.514754 py-Ayiin-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-24 09:48:10.514754 py-Ayiin-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:48:10.502754 py-Ayiin-0.3.4/pyAyiin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:48:10.506754 py-Ayiin-0.3.4/pyAyiin/Clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/Clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/Clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/Clients/pytgcalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/Clients/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:48:10.506754 py-Ayiin-0.3.4/pyAyiin/dB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/absen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/blacklistfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/blacklistgcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/blacklistuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/gban.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/logdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/pmpermit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/videocalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:48:10.510754 py-Ayiin-0.3.4/pyAyiin/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/changer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/funcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/inlinebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:48:10.510754 py-Ayiin-0.3.4/pyAyiin/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/pyrogram/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/pyrogram/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/pyrogram/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/pyrogram/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/pyrogram/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/pyrogram/toolbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/pyrogram/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:48:10.510754 py-Ayiin-0.3.4/pyAyiin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:48:10.510754 py-Ayiin-0.3.4/pyAyiin/telethon/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/telethon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:48:10.510754 py-Ayiin-0.3.4/pyAyiin/telethon/ayiin/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/telethon/ayiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/telethon/ayiin/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/telethon/ayiin/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/telethon/ayiin/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/xd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:48:10.510754 py-Ayiin-0.3.4/py_Ayiin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-24 09:48:10.000000 py-Ayiin-0.3.4/py_Ayiin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-24 09:48:10.000000 py-Ayiin-0.3.4/py_Ayiin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:48:10.000000 py-Ayiin-0.3.4/py_Ayiin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 09:48:10.000000 py-Ayiin-0.3.4/py_Ayiin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 09:48:10.000000 py-Ayiin-0.3.4/py_Ayiin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:48:10.514754 py-Ayiin-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/setup.py
```

### Comparing `py-Ayiin-0.3.3/LICENSE` & `py-Ayiin-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/NOTICE` & `py-Ayiin-0.3.4/NOTICE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/PKG-INFO` & `py-Ayiin-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.3.3/README.md` & `py-Ayiin-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/Clients/__init__.py` & `py-Ayiin-0.3.4/pyAyiin/Clients/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/Clients/client.py` & `py-Ayiin-0.3.4/pyAyiin/Clients/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,39 +10,21 @@
 
 Var = Variable()
 
 
 hndlr = f"{Var.HNDLR[0]} {Var.HNDLR[1]} {Var.HNDLR[2]} {Var.HNDLR[3]} {Var.HNDLR[4]} {Var.HNDLR[5]}"
 
 
-try:
-    from pytgcalls import PyTgCalls
-except ImportError:
-    pytgcalls = None
-
 
 TeleBot = TelegramClient(
     MemorySession(), 
     Var.API_ID, 
     Var.API_HASH
 )
 
-
-assist = PyroClient(
-    api_id=Var.API_ID, 
-    api_hash=Var.API_HASH, 
-    session_name=str(Var.ASS_STRING),
-)
-assistant = PyTgCalls(
-    assist,
-    cache_duration=100,
-    overload_quiet_mode=True,
-)
-
-
 tgbot = (
     Client(
         name="tgbot",
         api_id=Var.API_ID,
         api_hash=Var.API_HASH,
         bot_token=Var.BOT_TOKEN,
     )
```

### Comparing `py-Ayiin-0.3.3/pyAyiin/Clients/startup.py` & `py-Ayiin-0.3.4/pyAyiin/Clients/startup.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/__init__.py` & `py-Ayiin-0.3.4/pyAyiin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,25 +42,25 @@
 
 
 logs = logging.getLogger(__name__)
 
 
 __copyright__ = "Copyright (C) 2022-present AyiinXd <https://github.com/AyiinXd>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "0.3.3"
+__version__ = "0.3.4"
 ayiin_ver = "0.1.1"
 
 
 DEVS = [
     607067484, # Ayiin
     997461844, #Ayang_Ayiin
     2130526178, # Alfa
 ]
 
-API_AI = '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'
+API_AI = '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'
 
 GCAST_BLACKLIST = [
     -1001675396283,  # AyiinXdSupport
     -1001473548283,  # SharingUserbot
     -1001433238829,  # TedeSupport
     -1001476936696,  # AnosSupport
     -1001327032795,  # UltroidSupport
```

### Comparing `py-Ayiin-0.3.3/pyAyiin/__main__.py` & `py-Ayiin-0.3.4/pyAyiin/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/assistant.py` & `py-Ayiin-0.3.4/pyAyiin/assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/config.py` & `py-Ayiin-0.3.4/pyAyiin/config.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/dB/__init__.py` & `py-Ayiin-0.3.4/pyAyiin/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/dB/absen.py` & `py-Ayiin-0.3.4/pyAyiin/dB/absen.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/dB/admins.py` & `py-Ayiin-0.3.4/pyAyiin/dB/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/dB/auth.py` & `py-Ayiin-0.3.4/pyAyiin/dB/auth.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/dB/blacklistfilter.py` & `py-Ayiin-0.3.4/pyAyiin/dB/blacklistfilter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/dB/blacklistgcast.py` & `py-Ayiin-0.3.4/pyAyiin/dB/blacklistgcast.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/dB/blacklistuser.py` & `py-Ayiin-0.3.4/pyAyiin/dB/blacklistuser.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/dB/gban.py` & `py-Ayiin-0.3.4/pyAyiin/dB/gban.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/dB/langs.py` & `py-Ayiin-0.3.4/pyAyiin/dB/langs.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/dB/logdb.py` & `py-Ayiin-0.3.4/pyAyiin/dB/logdb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/dB/pmpermit.py` & `py-Ayiin-0.3.4/pyAyiin/dB/pmpermit.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/dB/premium.py` & `py-Ayiin-0.3.4/pyAyiin/dB/premium.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/dB/start.py` & `py-Ayiin-0.3.4/pyAyiin/dB/start.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/dB/sudo.py` & `py-Ayiin-0.3.4/pyAyiin/dB/sudo.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/dB/variable.py` & `py-Ayiin-0.3.4/pyAyiin/dB/variable.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/dB/videocalls.py` & `py-Ayiin-0.3.4/pyAyiin/dB/videocalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/dB/welcome.py` & `py-Ayiin-0.3.4/pyAyiin/dB/welcome.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/decorator.py` & `py-Ayiin-0.3.4/pyAyiin/decorator.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/exceptions.py` & `py-Ayiin-0.3.4/pyAyiin/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/methods/__init__.py` & `py-Ayiin-0.3.4/pyAyiin/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/methods/_misc.py` & `py-Ayiin-0.3.4/pyAyiin/methods/_misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/methods/changer.py` & `py-Ayiin-0.3.4/pyAyiin/methods/changer.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/methods/converter.py` & `py-Ayiin-0.3.4/pyAyiin/methods/converter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/methods/func.py` & `py-Ayiin-0.3.4/pyAyiin/methods/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/methods/funcb.py` & `py-Ayiin-0.3.4/pyAyiin/methods/funcb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/methods/helpers.py` & `py-Ayiin-0.3.4/pyAyiin/methods/helpers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/methods/hosting.py` & `py-Ayiin-0.3.4/pyAyiin/methods/hosting.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/methods/inlinebot.py` & `py-Ayiin-0.3.4/pyAyiin/methods/inlinebot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/methods/queue.py` & `py-Ayiin-0.3.4/pyAyiin/methods/queue.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/methods/thumbnail.py` & `py-Ayiin-0.3.4/pyAyiin/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/pyrogram/__init__.py` & `py-Ayiin-0.3.4/pyAyiin/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/pyrogram/_wrappers.py` & `py-Ayiin-0.3.4/pyAyiin/pyrogram/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/pyrogram/func.py` & `py-Ayiin-0.3.4/pyAyiin/pyrogram/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/pyrogram/misc.py` & `py-Ayiin-0.3.4/pyAyiin/pyrogram/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/pyrogram/pastebin.py` & `py-Ayiin-0.3.4/pyAyiin/pyrogram/pastebin.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/pyrogram/sections.py` & `py-Ayiin-0.3.4/pyAyiin/pyrogram/sections.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/pyrogram/toolbot.py` & `py-Ayiin-0.3.4/pyAyiin/pyrogram/toolbot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/pyrogram/tools.py` & `py-Ayiin-0.3.4/pyAyiin/pyrogram/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/telethon/ayiin/_wrappers.py` & `py-Ayiin-0.3.4/pyAyiin/telethon/ayiin/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/telethon/ayiin/events.py` & `py-Ayiin-0.3.4/pyAyiin/telethon/ayiin/events.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/telethon/ayiin/misc.py` & `py-Ayiin-0.3.4/pyAyiin/telethon/ayiin/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/pyAyiin/xd.py` & `py-Ayiin-0.3.4/pyAyiin/xd.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 try:
     import pybase64
 except ImportError:
     logs.info("'pybase64' not found\nInstall pybase64 or Add pybase64 in requirements.txt")
     pybase64 = None
 
 try:
-    from pyrogram import Client
-    from pyrogram.errors import (
+    from pyro import Client
+    from pyro.errors import (
         ApiIdInvalid,
         PhoneNumberInvalid,
         PhoneCodeInvalid,
         PhoneCodeExpired,
         SessionPasswordNeeded,
         PasswordHashInvalid
     )
@@ -50,15 +50,15 @@
     Client = None
     ApiIdInvalid = None
     PhoneNumberInvalid = None
     PhoneCodeInvalid = None
     PhoneCodeExpired = None
     SessionPasswordNeeded = None
     PasswordHashInvalid = None
-    logs.info(f"'pyrogram' not found\nUse pip install pyrogram==1.4.16 or Add pyrogram==1.4.16 in requirements.txt")
+    logs.info(f"'py-Pyro' not found\nUse pip install py-Pyro or Add py-Pyro in requirements.txt")
 
 ERROR_MESSAGE = "Maaf Terjadi Kesalahan ! \n\n<b>Kesalahan:</b> \n{} \n\nSilakan Teruskan Ini Ke @AyiinChat"
 
 
 class GenSession(object):
     async def cancelled(self, msg):
         if "/cancel" in msg.text:
```

### Comparing `py-Ayiin-0.3.3/py_Ayiin.egg-info/PKG-INFO` & `py-Ayiin-0.3.4/py_Ayiin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.3.3/py_Ayiin.egg-info/SOURCES.txt` & `py-Ayiin-0.3.4/py_Ayiin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.3/setup.py` & `py-Ayiin-0.3.4/setup.py`

 * *Files identical despite different names*

