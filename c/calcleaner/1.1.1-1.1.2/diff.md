# Comparing `tmp/calcleaner-1.1.1.tar.gz` & `tmp/calcleaner-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calcleaner-1.1.1.tar", last modified: Thu Oct 27 11:27:32 2022, max compression
+gzip compressed data, was "calcleaner-1.1.2.tar", last modified: Wed May 24 11:56:48 2023, max compression
```

## Comparing `calcleaner-1.1.1.tar` & `calcleaner-1.1.2.tar`

### file list

```diff
@@ -1,57 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 11:27:32.235439 calcleaner-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-10-27 11:27:20.000000 calcleaner-1.1.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-10-27 11:27:20.000000 calcleaner-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7462 2022-10-27 11:27:32.235439 calcleaner-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7154 2022-10-27 11:27:20.000000 calcleaner-1.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 11:27:32.235439 calcleaner-1.1.1/calcleaner/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      981 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/about_dialog.py
--rw-r--r--   0 runner    (1001) docker     (121)     2409 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/account_edit_dialog.py
--rw-r--r--   0 runner    (1001) docker     (121)     2484 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/accounts.py
--rw-r--r--   0 runner    (1001) docker     (121)     2784 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/accounts_manage_dialog.py
--rw-r--r--   0 runner    (1001) docker     (121)    12014 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/application.py
--rw-r--r--   0 runner    (1001) docker     (121)     3089 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/caldav_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5467 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/calendar_store.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 11:27:32.231439 calcleaner-1.1.1/calcleaner/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 11:27:32.235439 calcleaner-1.1.1/calcleaner/data/images/
--rw-r--r--   0 runner    (1001) docker     (121)     2611 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/data/images/calcleaner.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3480 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/data/images/calcleaner_128.png
--rw-r--r--   0 runner    (1001) docker     (121)     7009 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/data/images/calcleaner_256.png
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/data/images/calcleaner_32.png
--rw-r--r--   0 runner    (1001) docker     (121)     1826 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/data/images/calcleaner_64.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 11:27:32.231439 calcleaner-1.1.1/calcleaner/data/locales/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 11:27:32.231439 calcleaner-1.1.1/calcleaner/data/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 11:27:32.235439 calcleaner-1.1.1/calcleaner/data/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     4354 2022-10-27 11:27:31.000000 calcleaner-1.1.1/calcleaner/data/locales/de/LC_MESSAGES/org.flozz.calcleaner.mo
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 11:27:32.231439 calcleaner-1.1.1/calcleaner/data/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 11:27:32.235439 calcleaner-1.1.1/calcleaner/data/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     4158 2022-10-27 11:27:31.000000 calcleaner-1.1.1/calcleaner/data/locales/fr/LC_MESSAGES/org.flozz.calcleaner.mo
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 11:27:32.231439 calcleaner-1.1.1/calcleaner/data/locales/it/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 11:27:32.235439 calcleaner-1.1.1/calcleaner/data/locales/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     4064 2022-10-27 11:27:31.000000 calcleaner-1.1.1/calcleaner/data/locales/it/LC_MESSAGES/org.flozz.calcleaner.mo
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 11:27:32.231439 calcleaner-1.1.1/calcleaner/data/locales/nl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 11:27:32.235439 calcleaner-1.1.1/calcleaner/data/locales/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     4006 2022-10-27 11:27:31.000000 calcleaner-1.1.1/calcleaner/data/locales/nl/LC_MESSAGES/org.flozz.calcleaner.mo
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 11:27:32.231439 calcleaner-1.1.1/calcleaner/data/locales/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 11:27:32.235439 calcleaner-1.1.1/calcleaner/data/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      941 2022-10-27 11:27:31.000000 calcleaner-1.1.1/calcleaner/data/locales/pt_BR/LC_MESSAGES/org.flozz.calcleaner.mo
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 11:27:32.235439 calcleaner-1.1.1/calcleaner/data/style/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/data/style/calcleaner.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 11:27:32.235439 calcleaner-1.1.1/calcleaner/data/ui/
--rw-r--r--   0 runner    (1001) docker     (121)     8132 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/data/ui/account-edit-dialog.glade
--rw-r--r--   0 runner    (1001) docker     (121)     9089 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/data/ui/accounts-manage-dialog.glade
--rw-r--r--   0 runner    (1001) docker     (121)    23542 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/data/ui/main-window.glade
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/data_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     7035 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/main_window.py
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-10-27 11:27:20.000000 calcleaner-1.1.1/calcleaner/translation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 11:27:32.235439 calcleaner-1.1.1/calcleaner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7462 2022-10-27 11:27:32.000000 calcleaner-1.1.1/calcleaner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-10-27 11:27:32.000000 calcleaner-1.1.1/calcleaner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 11:27:32.000000 calcleaner-1.1.1/calcleaner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-10-27 11:27:32.000000 calcleaner-1.1.1/calcleaner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-10-27 11:27:32.000000 calcleaner-1.1.1/calcleaner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-27 11:27:32.000000 calcleaner-1.1.1/calcleaner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-27 11:27:32.235439 calcleaner-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      958 2022-10-27 11:27:20.000000 calcleaner-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.052017 calcleaner-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-24 11:56:33.000000 calcleaner-1.1.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-24 11:56:33.000000 calcleaner-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-05-24 11:56:48.052017 calcleaner-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-24 11:56:33.000000 calcleaner-1.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.036017 calcleaner-1.1.2/calcleaner/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/about_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/account_edit_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/accounts_manage_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/caldav_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/calendar_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.028017 calcleaner-1.1.2/calcleaner/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.044017 calcleaner-1.1.2/calcleaner/data/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/data/images/calcleaner.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/data/images/calcleaner_128.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/data/images/calcleaner_256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/data/images/calcleaner_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/data/images/calcleaner_64.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.024017 calcleaner-1.1.2/calcleaner/data/locales/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.024017 calcleaner-1.1.2/calcleaner/data/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.044017 calcleaner-1.1.2/calcleaner/data/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-05-24 11:56:45.000000 calcleaner-1.1.2/calcleaner/data/locales/de/LC_MESSAGES/org.flozz.calcleaner.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.024017 calcleaner-1.1.2/calcleaner/data/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.048017 calcleaner-1.1.2/calcleaner/data/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-24 11:56:45.000000 calcleaner-1.1.2/calcleaner/data/locales/fr/LC_MESSAGES/org.flozz.calcleaner.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.024017 calcleaner-1.1.2/calcleaner/data/locales/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.048017 calcleaner-1.1.2/calcleaner/data/locales/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-24 11:56:45.000000 calcleaner-1.1.2/calcleaner/data/locales/hr/LC_MESSAGES/org.flozz.calcleaner.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.024017 calcleaner-1.1.2/calcleaner/data/locales/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.048017 calcleaner-1.1.2/calcleaner/data/locales/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-24 11:56:45.000000 calcleaner-1.1.2/calcleaner/data/locales/it/LC_MESSAGES/org.flozz.calcleaner.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.024017 calcleaner-1.1.2/calcleaner/data/locales/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.048017 calcleaner-1.1.2/calcleaner/data/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-24 11:56:45.000000 calcleaner-1.1.2/calcleaner/data/locales/nl/LC_MESSAGES/org.flozz.calcleaner.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.024017 calcleaner-1.1.2/calcleaner/data/locales/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.048017 calcleaner-1.1.2/calcleaner/data/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-24 11:56:45.000000 calcleaner-1.1.2/calcleaner/data/locales/pt_BR/LC_MESSAGES/org.flozz.calcleaner.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.048017 calcleaner-1.1.2/calcleaner/data/style/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/data/style/calcleaner.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.048017 calcleaner-1.1.2/calcleaner/data/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/data/ui/account-edit-dialog.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/data/ui/accounts-manage-dialog.glade
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/data/ui/main-window.glade
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/data_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.044017 calcleaner-1.1.2/calcleaner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-05-24 11:56:47.000000 calcleaner-1.1.2/calcleaner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-24 11:56:48.000000 calcleaner-1.1.2/calcleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:56:47.000000 calcleaner-1.1.2/calcleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-24 11:56:47.000000 calcleaner-1.1.2/calcleaner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-24 11:56:47.000000 calcleaner-1.1.2/calcleaner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-24 11:56:47.000000 calcleaner-1.1.2/calcleaner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 11:56:48.052017 calcleaner-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-24 11:56:33.000000 calcleaner-1.1.2/setup.py
```

### Comparing `calcleaner-1.1.1/COPYING` & `calcleaner-1.1.2/COPYING`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.1/PKG-INFO` & `calcleaner-1.1.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: calcleaner
-Version: 1.1.1
-Summary: A simple graphical tool to purge old events from CalDAV calendars
-Home-page: https://github.com/flozz/calcleaner
-Author: Fabien LOISON
-License: GPLv3
-Keywords: calendar caldav event cleaner purge prune
-Provides-Extra: dev
-License-File: COPYING
-
 CalCleaner
 ==========
 
 |Github| |Discord| |Github Actions| |Black| |License|
 
     A simple graphical tool to purge old events from CalDAV calendars
 
@@ -151,20 +140,20 @@
     pip install -e ".[dev]"
 
 Then run::
 
     python -m calcleaner
 
 
-Codding Style / Lint
-~~~~~~~~~~~~~~~~~~~~
+Coding Style / Lint
+~~~~~~~~~~~~~~~~~~~
 
-This project follows `Black's <https://black.readthedocs.io/en/stable/>`_ codding style.
+This project follows `Black's <https://black.readthedocs.io/en/stable/>`_ coding style.
 
-To check codding style, you will first have to install `nox <https://nox.thea.codes/>`_::
+To check coding style, you will first have to install `nox <https://nox.thea.codes/>`_::
 
     pip3 install nox
 
 Then you can check for lint error (Flake8 and Black)::
 
     nox --session lint
 
@@ -236,15 +225,20 @@
 
 
 Changelog
 ---------
 
 * **[NEXT]** (changes on ``master`` but not released yet):
 
-  * Nothing yet :)
+  * Nothing yet ;)
+
+* **v1.1.2:**
+
+  * Added Croatian translation (@milotype, #7)
+  * Added Python 3.11 support
 
 * **v1.1.1:**
 
   * Added German translation (Jürgen Benvenuti)
 
 * **v1.1.0:**
```

### Comparing `calcleaner-1.1.1/README.rst` & `calcleaner-1.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: calcleaner
+Version: 1.1.2
+Summary: A simple graphical tool to purge old events from CalDAV calendars
+Home-page: https://calcleaner.flozz.org/
+Author: Fabien LOISON
+License: GPLv3
+Project-URL: Source Code, https://github.com/flozz/calcleaner
+Project-URL: Changelog, https://github.com/flozz/calcleaner#changelog
+Project-URL: Issues, https://github.com/flozz/calcleaner/issues
+Project-URL: Chat, https://discord.gg/P77sWhuSs4
+Project-URL: Donate, https://github.com/flozz/calcleaner#supporting-this-project
+Keywords: calendar caldav event cleaner purge prune
+Provides-Extra: dev
+License-File: COPYING
+
 CalCleaner
 ==========
 
 |Github| |Discord| |Github Actions| |Black| |License|
 
     A simple graphical tool to purge old events from CalDAV calendars
 
@@ -140,20 +156,20 @@
     pip install -e ".[dev]"
 
 Then run::
 
     python -m calcleaner
 
 
-Codding Style / Lint
-~~~~~~~~~~~~~~~~~~~~
+Coding Style / Lint
+~~~~~~~~~~~~~~~~~~~
 
-This project follows `Black's <https://black.readthedocs.io/en/stable/>`_ codding style.
+This project follows `Black's <https://black.readthedocs.io/en/stable/>`_ coding style.
 
-To check codding style, you will first have to install `nox <https://nox.thea.codes/>`_::
+To check coding style, you will first have to install `nox <https://nox.thea.codes/>`_::
 
     pip3 install nox
 
 Then you can check for lint error (Flake8 and Black)::
 
     nox --session lint
 
@@ -225,15 +241,20 @@
 
 
 Changelog
 ---------
 
 * **[NEXT]** (changes on ``master`` but not released yet):
 
-  * Nothing yet :)
+  * Nothing yet ;)
+
+* **v1.1.2:**
+
+  * Added Croatian translation (@milotype, #7)
+  * Added Python 3.11 support
 
 * **v1.1.1:**
 
   * Added German translation (Jürgen Benvenuti)
 
 * **v1.1.0:**
```

### Comparing `calcleaner-1.1.1/calcleaner/about_dialog.py` & `calcleaner-1.1.2/calcleaner/about_dialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             self,
             parent=parent,
             program_name=APPLICATION_NAME,
             comments=_(
                 "A simple graphical tool to purge old events from CalDAV calendars"
             ),
             version=VERSION,
-            copyright="Copyright (c) 2022 Fabien LOISON",
+            copyright="Copyright (c) 2022-2023 Fabien LOISON",
             website_label="github.com/flozz/calcleaner",
             website="https://github.com/flozz/calcleaner",
             license_type=Gtk.License.GPL_3_0,
         )
 
         logo = GdkPixbuf.Pixbuf.new_from_file(
             data_helpers.find_data_path("images/calcleaner_128.png")
```

### Comparing `calcleaner-1.1.1/calcleaner/account_edit_dialog.py` & `calcleaner-1.1.2/calcleaner/account_edit_dialog.py`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.1/calcleaner/accounts.py` & `calcleaner-1.1.2/calcleaner/accounts.py`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.1/calcleaner/accounts_manage_dialog.py` & `calcleaner-1.1.2/calcleaner/accounts_manage_dialog.py`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.1/calcleaner/application.py` & `calcleaner-1.1.2/calcleaner/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from .accounts import Accounts
 from .translation import gettext as _
 from .helpers import load_gtk_custom_css
 from .data_helpers import find_data_path
 
 
 class CalcleanerApplication(Gtk.Application):
-
     accounts = None
     calendar_store = None
 
     def __init__(self):
         Gtk.Application.__init__(
             self,
             application_id=APPLICATION_ID,
```

### Comparing `calcleaner-1.1.1/calcleaner/caldav_helpers.py` & `calcleaner-1.1.2/calcleaner/caldav_helpers.py`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.1/calcleaner/calendar_store.py` & `calcleaner-1.1.2/calcleaner/calendar_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from gi.repository import Gtk
 
 
 class CalendarStore(object):
-
     # fmt: off
     FIELDS = {
         "account_name":        {"id": 0, "type": str,  "default": ""},
         "calendar_url":        {"id": 1, "type": str,  "default": ""},
         "calendar_name":       {"id": 2, "type": str,  "default": ""},
         "calendar_color":      {"id": 3, "type": str,  "default": "#888888"},
         "event_count":         {"id": 4, "type": int,  "default": 0},
```

### Comparing `calcleaner-1.1.1/calcleaner/data/images/calcleaner.svg` & `calcleaner-1.1.2/calcleaner/data/images/calcleaner.svg`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.1/calcleaner/data/images/calcleaner_128.png` & `calcleaner-1.1.2/calcleaner/data/images/calcleaner_128.png`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.1/calcleaner/data/images/calcleaner_256.png` & `calcleaner-1.1.2/calcleaner/data/images/calcleaner_256.png`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.1/calcleaner/data/images/calcleaner_32.png` & `calcleaner-1.1.2/calcleaner/data/images/calcleaner_32.png`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.1/calcleaner/data/images/calcleaner_64.png` & `calcleaner-1.1.2/calcleaner/data/images/calcleaner_64.png`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.1/calcleaner/data/locales/de/LC_MESSAGES/org.flozz.calcleaner.mo` & `calcleaner-1.1.2/calcleaner/data/locales/de/LC_MESSAGES/org.flozz.calcleaner.mo`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.1/calcleaner/data/locales/fr/LC_MESSAGES/org.flozz.calcleaner.mo` & `calcleaner-1.1.2/calcleaner/data/locales/fr/LC_MESSAGES/org.flozz.calcleaner.mo`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.1/calcleaner/data/locales/it/LC_MESSAGES/org.flozz.calcleaner.mo` & `calcleaner-1.1.2/calcleaner/data/locales/it/LC_MESSAGES/org.flozz.calcleaner.mo`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.1/calcleaner/data/locales/nl/LC_MESSAGES/org.flozz.calcleaner.mo` & `calcleaner-1.1.2/calcleaner/data/locales/nl/LC_MESSAGES/org.flozz.calcleaner.mo`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.1/calcleaner/data/locales/pt_BR/LC_MESSAGES/org.flozz.calcleaner.mo` & `calcleaner-1.1.2/calcleaner/data/locales/pt_BR/LC_MESSAGES/org.flozz.calcleaner.mo`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.1/calcleaner/data/ui/account-edit-dialog.glade` & `calcleaner-1.1.2/calcleaner/data/ui/account-edit-dialog.glade`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.1/calcleaner/data/ui/accounts-manage-dialog.glade` & `calcleaner-1.1.2/calcleaner/data/ui/accounts-manage-dialog.glade`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.1/calcleaner/data/ui/main-window.glade` & `calcleaner-1.1.2/calcleaner/data/ui/main-window.glade`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.1/calcleaner/main_window.py` & `calcleaner-1.1.2/calcleaner/main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from . import APPLICATION_NAME, APPLICATION_ID
 from . import data_helpers
 from .translation import gettext as _
 
 
 class MainWindow(Gtk.ApplicationWindow):
-
     STATE_INITIAL = "state-initial"
     STATE_UPDATING = "state-updating"
     STATE_ERROR = "state-error"
     STATE_CALENDAR_LIST = "state-calendar-list"
     STATE_CLEANING = "state-cleaning"
 
     def __init__(self, app):
```

### Comparing `calcleaner-1.1.1/calcleaner/translation.py` & `calcleaner-1.1.2/calcleaner/translation.py`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.1/calcleaner.egg-info/PKG-INFO` & `calcleaner-1.1.2/calcleaner.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Metadata-Version: 2.1
 Name: calcleaner
-Version: 1.1.1
+Version: 1.1.2
 Summary: A simple graphical tool to purge old events from CalDAV calendars
-Home-page: https://github.com/flozz/calcleaner
+Home-page: https://calcleaner.flozz.org/
 Author: Fabien LOISON
 License: GPLv3
+Project-URL: Source Code, https://github.com/flozz/calcleaner
+Project-URL: Changelog, https://github.com/flozz/calcleaner#changelog
+Project-URL: Issues, https://github.com/flozz/calcleaner/issues
+Project-URL: Chat, https://discord.gg/P77sWhuSs4
+Project-URL: Donate, https://github.com/flozz/calcleaner#supporting-this-project
 Keywords: calendar caldav event cleaner purge prune
 Provides-Extra: dev
 License-File: COPYING
 
 CalCleaner
 ==========
 
@@ -151,20 +156,20 @@
     pip install -e ".[dev]"
 
 Then run::
 
     python -m calcleaner
 
 
-Codding Style / Lint
-~~~~~~~~~~~~~~~~~~~~
+Coding Style / Lint
+~~~~~~~~~~~~~~~~~~~
 
-This project follows `Black's <https://black.readthedocs.io/en/stable/>`_ codding style.
+This project follows `Black's <https://black.readthedocs.io/en/stable/>`_ coding style.
 
-To check codding style, you will first have to install `nox <https://nox.thea.codes/>`_::
+To check coding style, you will first have to install `nox <https://nox.thea.codes/>`_::
 
     pip3 install nox
 
 Then you can check for lint error (Flake8 and Black)::
 
     nox --session lint
 
@@ -236,15 +241,20 @@
 
 
 Changelog
 ---------
 
 * **[NEXT]** (changes on ``master`` but not released yet):
 
-  * Nothing yet :)
+  * Nothing yet ;)
+
+* **v1.1.2:**
+
+  * Added Croatian translation (@milotype, #7)
+  * Added Python 3.11 support
 
 * **v1.1.1:**
 
   * Added German translation (Jürgen Benvenuti)
 
 * **v1.1.0:**
```

### Comparing `calcleaner-1.1.1/calcleaner.egg-info/SOURCES.txt` & `calcleaner-1.1.2/calcleaner.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 calcleaner/data/images/calcleaner.svg
 calcleaner/data/images/calcleaner_128.png
 calcleaner/data/images/calcleaner_256.png
 calcleaner/data/images/calcleaner_32.png
 calcleaner/data/images/calcleaner_64.png
 calcleaner/data/locales/de/LC_MESSAGES/org.flozz.calcleaner.mo
 calcleaner/data/locales/fr/LC_MESSAGES/org.flozz.calcleaner.mo
+calcleaner/data/locales/hr/LC_MESSAGES/org.flozz.calcleaner.mo
 calcleaner/data/locales/it/LC_MESSAGES/org.flozz.calcleaner.mo
 calcleaner/data/locales/nl/LC_MESSAGES/org.flozz.calcleaner.mo
 calcleaner/data/locales/pt_BR/LC_MESSAGES/org.flozz.calcleaner.mo
 calcleaner/data/style/calcleaner.css
 calcleaner/data/ui/account-edit-dialog.glade
 calcleaner/data/ui/accounts-manage-dialog.glade
 calcleaner/data/ui/main-window.glade
```

