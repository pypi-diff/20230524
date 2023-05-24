# Comparing `tmp/py-Ayiin-0.3.4.tar.gz` & `tmp/py-Ayiin-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.3.4.tar", last modified: Wed May 24 09:48:10 2023, max compression
+gzip compressed data, was "py-Ayiin-0.3.5.tar", last modified: Wed May 24 09:52:42 2023, max compression
```

## Comparing `py-Ayiin-0.3.4.tar` & `py-Ayiin-0.3.5.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:48:10.514754 py-Ayiin-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-24 09:48:10.514754 py-Ayiin-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:48:10.502754 py-Ayiin-0.3.4/pyAyiin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:48:10.506754 py-Ayiin-0.3.4/pyAyiin/Clients/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/Clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/Clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/Clients/pytgcalls.py
--rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/Clients/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:48:10.506754 py-Ayiin-0.3.4/pyAyiin/dB/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/absen.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/blacklistfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/blacklistgcast.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/blacklistuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/gban.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/logdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/pmpermit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/videocalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/dB/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:48:10.510754 py-Ayiin-0.3.4/pyAyiin/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/changer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/funcb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/inlinebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:48:10.510754 py-Ayiin-0.3.4/pyAyiin/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/pyrogram/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/pyrogram/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/pyrogram/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/pyrogram/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/pyrogram/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/pyrogram/toolbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/pyrogram/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:48:10.510754 py-Ayiin-0.3.4/pyAyiin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:48:10.510754 py-Ayiin-0.3.4/pyAyiin/telethon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/telethon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:48:10.510754 py-Ayiin-0.3.4/pyAyiin/telethon/ayiin/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/telethon/ayiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/telethon/ayiin/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/telethon/ayiin/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/telethon/ayiin/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/pyAyiin/xd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:48:10.510754 py-Ayiin-0.3.4/py_Ayiin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-24 09:48:10.000000 py-Ayiin-0.3.4/py_Ayiin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-24 09:48:10.000000 py-Ayiin-0.3.4/py_Ayiin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:48:10.000000 py-Ayiin-0.3.4/py_Ayiin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 09:48:10.000000 py-Ayiin-0.3.4/py_Ayiin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 09:48:10.000000 py-Ayiin-0.3.4/py_Ayiin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:48:10.514754 py-Ayiin-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-24 09:47:57.000000 py-Ayiin-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:52:42.407622 py-Ayiin-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-24 09:52:42.407622 py-Ayiin-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:52:42.399622 py-Ayiin-0.3.5/pyAyiin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:52:42.399622 py-Ayiin-0.3.5/pyAyiin/Clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/Clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/Clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/Clients/pytgcalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/Clients/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:52:42.399622 py-Ayiin-0.3.5/pyAyiin/dB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/dB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/dB/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/dB/absen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/dB/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/dB/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/dB/blacklistfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/dB/blacklistgcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/dB/blacklistuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/dB/gban.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/dB/langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/dB/logdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/dB/pmpermit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/dB/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/dB/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/dB/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/dB/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/dB/videocalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/dB/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:52:42.403622 py-Ayiin-0.3.5/pyAyiin/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/methods/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/methods/changer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/methods/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/methods/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/methods/funcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/methods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/methods/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/methods/inlinebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/methods/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:52:42.403622 py-Ayiin-0.3.5/pyAyiin/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/pyrogram/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/pyrogram/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/pyrogram/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/pyrogram/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/pyrogram/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/pyrogram/toolbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/pyrogram/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:52:42.403622 py-Ayiin-0.3.5/pyAyiin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:52:42.403622 py-Ayiin-0.3.5/pyAyiin/telethon/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/telethon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:52:42.403622 py-Ayiin-0.3.5/pyAyiin/telethon/ayiin/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/telethon/ayiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/telethon/ayiin/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/telethon/ayiin/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/telethon/ayiin/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/pyAyiin/xd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:52:42.403622 py-Ayiin-0.3.5/py_Ayiin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-24 09:52:42.000000 py-Ayiin-0.3.5/py_Ayiin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-24 09:52:42.000000 py-Ayiin-0.3.5/py_Ayiin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:52:42.000000 py-Ayiin-0.3.5/py_Ayiin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 09:52:42.000000 py-Ayiin-0.3.5/py_Ayiin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 09:52:42.000000 py-Ayiin-0.3.5/py_Ayiin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:52:42.407622 py-Ayiin-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-24 09:52:29.000000 py-Ayiin-0.3.5/setup.py
```

### Comparing `py-Ayiin-0.3.4/LICENSE` & `py-Ayiin-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/NOTICE` & `py-Ayiin-0.3.5/NOTICE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/PKG-INFO` & `py-Ayiin-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.3.4/README.md` & `py-Ayiin-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/Clients/__init__.py` & `py-Ayiin-0.3.5/pyAyiin/Clients/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/Clients/client.py` & `py-Ayiin-0.3.5/pyAyiin/Clients/client.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/Clients/pytgcalls.py` & `py-Ayiin-0.3.5/pyAyiin/Clients/pytgcalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/Clients/startup.py` & `py-Ayiin-0.3.5/pyAyiin/Clients/startup.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/__init__.py` & `py-Ayiin-0.3.5/pyAyiin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 
 logs = logging.getLogger(__name__)
 
 
 __copyright__ = "Copyright (C) 2022-present AyiinXd <https://github.com/AyiinXd>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "0.3.4"
+__version__ = "0.3.5"
 ayiin_ver = "0.1.1"
 
 
 DEVS = [
     607067484, # Ayiin
     997461844, #Ayang_Ayiin
     2130526178, # Alfa
```

### Comparing `py-Ayiin-0.3.4/pyAyiin/__main__.py` & `py-Ayiin-0.3.5/pyAyiin/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from fipper import idle
 
 from pyAyiin import __version__
 
 from . import *
 
 from .config import Var
-from .Clients.client import assistant
 from .Clients.startup import StartPyrogram
 from .exceptions import DependencyMissingError
 
 yinsxd = Var()
 xd = PyrogramXd()
 
 
@@ -44,24 +43,14 @@
                 HOSTED_ON,
                 ayiin_ver, 
                 len(CMD_HELP),
             )
         )
     except BaseException as s:
         print(s)
-    if yinsxd.ASS_STRING:
-        try:
-            await assistant.start()
-            await Yins.stream_call(
-                Var.LOG_CHAT,
-                "http://docs.evostream.com/sample_content/assets/sintel1m720p.mp4"
-            )
-        except BaseException as e:
-            logs.info(e)
-        await Yins.decorators()
     print(f"AyiinUbot Version - {ayiin_ver}\n[🔥 BERHASIL DIAKTIFKAN! 🔥]")
     await idle()
     await aiosession.close()
 
 if __name__ == "__main__":
     install()
     xd.heroku()
```

### Comparing `py-Ayiin-0.3.4/pyAyiin/assistant.py` & `py-Ayiin-0.3.5/pyAyiin/assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/config.py` & `py-Ayiin-0.3.5/pyAyiin/config.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/dB/__init__.py` & `py-Ayiin-0.3.5/pyAyiin/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/dB/absen.py` & `py-Ayiin-0.3.5/pyAyiin/dB/absen.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/dB/admins.py` & `py-Ayiin-0.3.5/pyAyiin/dB/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/dB/auth.py` & `py-Ayiin-0.3.5/pyAyiin/dB/auth.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/dB/blacklistfilter.py` & `py-Ayiin-0.3.5/pyAyiin/dB/blacklistfilter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/dB/blacklistgcast.py` & `py-Ayiin-0.3.5/pyAyiin/dB/blacklistgcast.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/dB/blacklistuser.py` & `py-Ayiin-0.3.5/pyAyiin/dB/blacklistuser.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/dB/gban.py` & `py-Ayiin-0.3.5/pyAyiin/dB/gban.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/dB/langs.py` & `py-Ayiin-0.3.5/pyAyiin/dB/langs.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/dB/logdb.py` & `py-Ayiin-0.3.5/pyAyiin/dB/logdb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/dB/pmpermit.py` & `py-Ayiin-0.3.5/pyAyiin/dB/pmpermit.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/dB/premium.py` & `py-Ayiin-0.3.5/pyAyiin/dB/premium.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/dB/start.py` & `py-Ayiin-0.3.5/pyAyiin/dB/start.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/dB/sudo.py` & `py-Ayiin-0.3.5/pyAyiin/dB/sudo.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/dB/variable.py` & `py-Ayiin-0.3.5/pyAyiin/dB/variable.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/dB/videocalls.py` & `py-Ayiin-0.3.5/pyAyiin/dB/videocalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/dB/welcome.py` & `py-Ayiin-0.3.5/pyAyiin/dB/welcome.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/decorator.py` & `py-Ayiin-0.3.5/pyAyiin/decorator.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/exceptions.py` & `py-Ayiin-0.3.5/pyAyiin/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/methods/__init__.py` & `py-Ayiin-0.3.5/pyAyiin/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/methods/_misc.py` & `py-Ayiin-0.3.5/pyAyiin/methods/_misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/methods/changer.py` & `py-Ayiin-0.3.5/pyAyiin/methods/changer.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/methods/converter.py` & `py-Ayiin-0.3.5/pyAyiin/methods/converter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/methods/func.py` & `py-Ayiin-0.3.5/pyAyiin/methods/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/methods/funcb.py` & `py-Ayiin-0.3.5/pyAyiin/methods/funcb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/methods/helpers.py` & `py-Ayiin-0.3.5/pyAyiin/methods/helpers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/methods/hosting.py` & `py-Ayiin-0.3.5/pyAyiin/methods/hosting.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/methods/inlinebot.py` & `py-Ayiin-0.3.5/pyAyiin/methods/inlinebot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/methods/queue.py` & `py-Ayiin-0.3.5/pyAyiin/methods/queue.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/methods/thumbnail.py` & `py-Ayiin-0.3.5/pyAyiin/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/pyrogram/__init__.py` & `py-Ayiin-0.3.5/pyAyiin/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/pyrogram/_wrappers.py` & `py-Ayiin-0.3.5/pyAyiin/pyrogram/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/pyrogram/func.py` & `py-Ayiin-0.3.5/pyAyiin/pyrogram/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/pyrogram/misc.py` & `py-Ayiin-0.3.5/pyAyiin/pyrogram/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/pyrogram/pastebin.py` & `py-Ayiin-0.3.5/pyAyiin/pyrogram/pastebin.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/pyrogram/sections.py` & `py-Ayiin-0.3.5/pyAyiin/pyrogram/sections.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/pyrogram/toolbot.py` & `py-Ayiin-0.3.5/pyAyiin/pyrogram/toolbot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/pyrogram/tools.py` & `py-Ayiin-0.3.5/pyAyiin/pyrogram/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/telethon/ayiin/_wrappers.py` & `py-Ayiin-0.3.5/pyAyiin/telethon/ayiin/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/telethon/ayiin/events.py` & `py-Ayiin-0.3.5/pyAyiin/telethon/ayiin/events.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/telethon/ayiin/misc.py` & `py-Ayiin-0.3.5/pyAyiin/telethon/ayiin/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/pyAyiin/xd.py` & `py-Ayiin-0.3.5/pyAyiin/xd.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/py_Ayiin.egg-info/PKG-INFO` & `py-Ayiin-0.3.5/py_Ayiin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.3.4/py_Ayiin.egg-info/SOURCES.txt` & `py-Ayiin-0.3.5/py_Ayiin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.4/setup.py` & `py-Ayiin-0.3.5/setup.py`

 * *Files identical despite different names*

