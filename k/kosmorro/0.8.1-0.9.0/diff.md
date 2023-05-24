# Comparing `tmp/kosmorro-0.8.1.tar.gz` & `tmp/kosmorro-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kosmorro-0.8.1.tar", last modified: Sun Jun  7 09:19:33 2020, max compression
+gzip compressed data, was "dist/kosmorro-0.9.0.tar", last modified: Sun Jan 31 09:20:21 2021, max compression
```

## Comparing `kosmorro-0.8.1.tar` & `kosmorro-0.9.0.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 09:19:33.000000 kosmorro-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (116)       79 2020-06-07 09:18:22.000000 kosmorro-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     5193 2020-06-07 09:19:33.000000 kosmorro-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3969 2020-06-07 09:18:22.000000 kosmorro-0.8.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (116)     1032 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorro
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5193 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2277 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       80 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorrolib/
--rw-r--r--   0 runner    (1001) docker     (116)      823 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorrolib/assets/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/png/
--rw-r--r--   0 runner    (1001) docker     (116)    37047 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/png/first-quarter.png
--rw-r--r--   0 runner    (1001) docker     (116)    48608 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/png/full-moon.png
--rw-r--r--   0 runner    (1001) docker     (116)    35968 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/png/last-quarter.png
--rw-r--r--   0 runner    (1001) docker     (116)    23877 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/png/new-moon.png
--rw-r--r--   0 runner    (1001) docker     (116)    26900 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/png/unknown.png
--rw-r--r--   0 runner    (1001) docker     (116)    30960 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/png/waning-crescent.png
--rw-r--r--   0 runner    (1001) docker     (116)    44583 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/png/waning-gibbous.png
--rw-r--r--   0 runner    (1001) docker     (116)    30326 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/png/waxing-crescent.png
--rw-r--r--   0 runner    (1001) docker     (116)    45284 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/png/waxing-gibbous.png
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/svg/
--rw-r--r--   0 runner    (1001) docker     (116)     4521 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/svg/first-quarter.svg
--rw-r--r--   0 runner    (1001) docker     (116)     4295 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/svg/full-moon.svg
--rw-r--r--   0 runner    (1001) docker     (116)     4280 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/svg/last-quarter.svg
--rw-r--r--   0 runner    (1001) docker     (116)     4590 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/svg/new-moon.svg
--rw-r--r--   0 runner    (1001) docker     (116)     4546 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/svg/unknown.svg
--rw-r--r--   0 runner    (1001) docker     (116)     4608 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/svg/waning-crescent.svg
--rw-r--r--   0 runner    (1001) docker     (116)     4535 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/svg/waning-gibbous.svg
--rw-r--r--   0 runner    (1001) docker     (116)     4611 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/svg/waxing-crescent.svg
--rw-r--r--   0 runner    (1001) docker     (116)     4539 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/moonphases/svg/waxing-gibbous.svg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorrolib/assets/pdf/
--rw-r--r--   0 runner    (1001) docker     (116)     2770 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/pdf/kosmorro.sty
--rw-r--r--   0 runner    (1001) docker     (116)     1902 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/pdf/template.tex
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorrolib/assets/png/
--rw-r--r--   0 runner    (1001) docker     (116)    49644 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/png/kosmorro-icon-white.png
--rw-r--r--   0 runner    (1001) docker     (116)    46617 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/png/kosmorro-icon.png
--rw-r--r--   0 runner    (1001) docker     (116)    19533 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/png/kosmorro-logo-white.png
--rw-r--r--   0 runner    (1001) docker     (116)    17451 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/png/kosmorro-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorrolib/assets/svg/
--rw-r--r--   0 runner    (1001) docker     (116)     5666 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/svg/kosmorro-icon-white.svg
--rw-r--r--   0 runner    (1001) docker     (116)     5659 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/svg/kosmorro-icon.svg
--rw-r--r--   0 runner    (1001) docker     (116)    12940 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/svg/kosmorro-logo-white.svg
--rw-r--r--   0 runner    (1001) docker     (116)    13055 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/assets/svg/kosmorro-logo.svg
--rw-r--r--   0 runner    (1001) docker     (116)     3469 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/core.py
--rw-r--r--   0 runner    (1001) docker     (116)    10079 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/data.py
--rw-r--r--   0 runner    (1001) docker     (116)     1170 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/dateutil.py
--rw-r--r--   0 runner    (1001) docker     (116)    15477 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/dumper.py
--rw-r--r--   0 runner    (1001) docker     (116)     5455 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/ephemerides.py
--rw-r--r--   0 runner    (1001) docker     (116)     6307 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/events.py
--rw-r--r--   0 runner    (1001) docker     (116)     1533 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     1835 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorrolib/locales/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorrolib/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorrolib/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     7989 2020-06-07 09:19:32.000000 kosmorro-0.8.1/kosmorrolib/locales/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (116)     9870 2020-06-07 09:19:32.000000 kosmorro-0.8.1/kosmorrolib/locales/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorrolib/locales/en/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorrolib/locales/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     7497 2020-06-07 09:19:32.000000 kosmorro-0.8.1/kosmorrolib/locales/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (116)     9382 2020-06-07 09:19:30.000000 kosmorro-0.8.1/kosmorrolib/locales/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorrolib/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 09:19:33.000000 kosmorro-0.8.1/kosmorrolib/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     8110 2020-06-07 09:19:32.000000 kosmorro-0.8.1/kosmorrolib/locales/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (116)     9992 2020-06-07 09:19:31.000000 kosmorro-0.8.1/kosmorrolib/locales/fr/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (116)     7001 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/locales/messages.pot
--rw-r--r--   0 runner    (1001) docker     (116)     8493 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/main.py
--rw-r--r--   0 runner    (1001) docker     (116)      842 2020-06-07 09:18:22.000000 kosmorro-0.8.1/kosmorrolib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 09:19:33.000000 kosmorro-0.8.1/manpage/
--rw-r--r--   0 runner    (1001) docker     (116)     3202 2020-06-07 09:19:27.000000 kosmorro-0.8.1/manpage/kosmorro.1
--rw-r--r--   0 runner    (1001) docker     (116)     2879 2020-06-07 09:19:28.000000 kosmorro-0.8.1/manpage/kosmorro.7
--rw-r--r--   0 runner    (1001) docker     (116)      315 2020-06-07 09:19:33.000000 kosmorro-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1982 2020-06-07 09:18:22.000000 kosmorro-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-07 09:19:33.000000 kosmorro-0.8.1/test/
--rw-r--r--   0 runner    (1001) docker     (116)      160 2020-06-07 09:18:22.000000 kosmorro-0.8.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1409 2020-06-07 09:18:22.000000 kosmorro-0.8.1/test/core.py
--rw-r--r--   0 runner    (1001) docker     (116)      495 2020-06-07 09:18:22.000000 kosmorro-0.8.1/test/data.py
--rw-r--r--   0 runner    (1001) docker     (116)      757 2020-06-07 09:18:22.000000 kosmorro-0.8.1/test/dateutil.py
--rw-r--r--   0 runner    (1001) docker     (116)    16819 2020-06-07 09:18:22.000000 kosmorro-0.8.1/test/dumper.py
--rw-r--r--   0 runner    (1001) docker     (116)     5827 2020-06-07 09:18:22.000000 kosmorro-0.8.1/test/ephemerides.py
--rw-r--r--   0 runner    (1001) docker     (116)     3371 2020-06-07 09:18:22.000000 kosmorro-0.8.1/test/events.py
--rw-r--r--   0 runner    (1001) docker     (116)     1778 2020-06-07 09:18:22.000000 kosmorro-0.8.1/test/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-31 09:20:21.000000 kosmorro-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (117)       79 2021-01-31 09:19:30.000000 kosmorro-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (117)     4978 2021-01-31 09:20:21.000000 kosmorro-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (117)     3826 2021-01-31 09:19:30.000000 kosmorro-0.9.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (117)     1032 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorro
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (117)     4978 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (117)     2297 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (117)        1 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (117)       80 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (117)       17 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorrolib/
+-rw-r--r--   0 runner    (1001) docker     (117)      823 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorrolib/assets/
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/png/
+-rw-r--r--   0 runner    (1001) docker     (117)    37047 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/png/first-quarter.png
+-rw-r--r--   0 runner    (1001) docker     (117)    48608 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/png/full-moon.png
+-rw-r--r--   0 runner    (1001) docker     (117)    35968 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/png/last-quarter.png
+-rw-r--r--   0 runner    (1001) docker     (117)    23877 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/png/new-moon.png
+-rw-r--r--   0 runner    (1001) docker     (117)    26900 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/png/unknown.png
+-rw-r--r--   0 runner    (1001) docker     (117)    30960 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/png/waning-crescent.png
+-rw-r--r--   0 runner    (1001) docker     (117)    44583 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/png/waning-gibbous.png
+-rw-r--r--   0 runner    (1001) docker     (117)    30326 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/png/waxing-crescent.png
+-rw-r--r--   0 runner    (1001) docker     (117)    45284 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/png/waxing-gibbous.png
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/svg/
+-rw-r--r--   0 runner    (1001) docker     (117)     4521 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/svg/first-quarter.svg
+-rw-r--r--   0 runner    (1001) docker     (117)     4295 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/svg/full-moon.svg
+-rw-r--r--   0 runner    (1001) docker     (117)     4280 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/svg/last-quarter.svg
+-rw-r--r--   0 runner    (1001) docker     (117)     4590 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/svg/new-moon.svg
+-rw-r--r--   0 runner    (1001) docker     (117)     4546 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/svg/unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (117)     4608 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/svg/waning-crescent.svg
+-rw-r--r--   0 runner    (1001) docker     (117)     4535 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/svg/waning-gibbous.svg
+-rw-r--r--   0 runner    (1001) docker     (117)     4611 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/svg/waxing-crescent.svg
+-rw-r--r--   0 runner    (1001) docker     (117)     4539 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/moonphases/svg/waxing-gibbous.svg
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorrolib/assets/pdf/
+-rw-r--r--   0 runner    (1001) docker     (117)     2770 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/pdf/kosmorro.sty
+-rw-r--r--   0 runner    (1001) docker     (117)     1902 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/pdf/template.tex
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorrolib/assets/png/
+-rw-r--r--   0 runner    (1001) docker     (117)    49644 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/png/kosmorro-icon-white.png
+-rw-r--r--   0 runner    (1001) docker     (117)    46617 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/png/kosmorro-icon.png
+-rw-r--r--   0 runner    (1001) docker     (117)    19533 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/png/kosmorro-logo-white.png
+-rw-r--r--   0 runner    (1001) docker     (117)    17451 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/png/kosmorro-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorrolib/assets/svg/
+-rw-r--r--   0 runner    (1001) docker     (117)     5666 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/svg/kosmorro-icon-white.svg
+-rw-r--r--   0 runner    (1001) docker     (117)     5659 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/svg/kosmorro-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (117)    12940 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/svg/kosmorro-logo-white.svg
+-rw-r--r--   0 runner    (1001) docker     (117)    13055 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/assets/svg/kosmorro-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (117)     3559 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/core.py
+-rw-r--r--   0 runner    (1001) docker     (117)     7904 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/data.py
+-rw-r--r--   0 runner    (1001) docker     (117)     1170 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/dateutil.py
+-rw-r--r--   0 runner    (1001) docker     (117)    16601 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (117)     1497 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/enum.py
+-rw-r--r--   0 runner    (1001) docker     (117)     6782 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/ephemerides.py
+-rw-r--r--   0 runner    (1001) docker     (117)     7664 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/events.py
+-rw-r--r--   0 runner    (1001) docker     (117)     1594 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (117)     1835 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorrolib/locales/
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorrolib/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorrolib/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (117)     8521 2021-01-31 09:20:20.000000 kosmorro-0.9.0/kosmorrolib/locales/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (117)    10498 2021-01-31 09:20:20.000000 kosmorro-0.9.0/kosmorrolib/locales/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorrolib/locales/en/
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorrolib/locales/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (117)     7991 2021-01-31 09:20:20.000000 kosmorro-0.9.0/kosmorrolib/locales/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (117)     9972 2021-01-31 09:20:18.000000 kosmorro-0.9.0/kosmorrolib/locales/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorrolib/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-31 09:20:21.000000 kosmorro-0.9.0/kosmorrolib/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (117)     8635 2021-01-31 09:20:20.000000 kosmorro-0.9.0/kosmorrolib/locales/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (117)    10613 2021-01-31 09:20:19.000000 kosmorro-0.9.0/kosmorrolib/locales/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (117)     7367 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/locales/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (117)     8679 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/main.py
+-rw-r--r--   0 runner    (1001) docker     (117)      842 2021-01-31 09:19:30.000000 kosmorro-0.9.0/kosmorrolib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-31 09:20:21.000000 kosmorro-0.9.0/manpage/
+-rw-r--r--   0 runner    (1001) docker     (117)     3205 2021-01-31 09:20:20.000000 kosmorro-0.9.0/manpage/kosmorro.1
+-rw-r--r--   0 runner    (1001) docker     (117)     3086 2021-01-31 09:20:20.000000 kosmorro-0.9.0/manpage/kosmorro.7
+-rw-r--r--   0 runner    (1001) docker     (117)      315 2021-01-31 09:20:21.000000 kosmorro-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (117)     1982 2021-01-31 09:19:30.000000 kosmorro-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-01-31 09:20:21.000000 kosmorro-0.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (117)      160 2021-01-31 09:19:30.000000 kosmorro-0.9.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (117)     1409 2021-01-31 09:19:30.000000 kosmorro-0.9.0/test/core.py
+-rw-r--r--   0 runner    (1001) docker     (117)      495 2021-01-31 09:19:30.000000 kosmorro-0.9.0/test/data.py
+-rw-r--r--   0 runner    (1001) docker     (117)      757 2021-01-31 09:19:30.000000 kosmorro-0.9.0/test/dateutil.py
+-rw-r--r--   0 runner    (1001) docker     (117)    16901 2021-01-31 09:19:30.000000 kosmorro-0.9.0/test/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (117)     6168 2021-01-31 09:19:30.000000 kosmorro-0.9.0/test/ephemerides.py
+-rw-r--r--   0 runner    (1001) docker     (117)     4038 2021-01-31 09:19:30.000000 kosmorro-0.9.0/test/events.py
+-rw-r--r--   0 runner    (1001) docker     (117)     1778 2021-01-31 09:19:30.000000 kosmorro-0.9.0/test/testutils.py
```

### Comparing `kosmorro-0.8.1/PKG-INFO` & `kosmorro-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 Metadata-Version: 2.1
 Name: kosmorro
-Version: 0.8.1
+Version: 0.9.0
 Summary: A program that computes the ephemerides.
 Home-page: http://kosmorro.space
 Author: Jérôme Deuchnord
 Author-email: jerome@deuchnord.fr
 License: AGPL-3.0
 Description: # ![Kosmorro](kosmorrolib/assets/png/kosmorro-logo.png)
-        [![Coverage Status](https://coveralls.io/repos/github/Deuchnord/kosmorro/badge.svg)](https://coveralls.io/github/Deuchnord/kosmorro) [![Version on PyPI](https://img.shields.io/pypi/v/kosmorro)](https://pypi.org/project/kosmorro) [![Discord](https://img.shields.io/discord/650237632533757965?logo=discord&label=%23kosmorro)](https://discord.gg/nyemBqE)
+        [![Coverage Status](https://coveralls.io/repos/github/Kosmorro/kosmorro/badge.svg?branch=master)](https://coveralls.io/github/Kosmorro/kosmorro?branch=master) [![Version on PyPI](https://img.shields.io/pypi/v/kosmorro)](https://pypi.org/project/kosmorro) [![Discord](https://img.shields.io/discord/650237632533757965?logo=discord&label=%23kosmorro)](https://discord.gg/TVX4MSKGaa)
         
-        ## About the project
-        
-        Kosmorro is a software that allows you to compute the ephemeris for a date, a month or a year.
+        A program that calculates your astronomical ephemerides!
         
         ## Installation
         
-        ### Requirements
-        
-        Kosmorro requires the following software to work:
-        
-        - Python ≥ 3.5.0
-        - PIP
-        
         ### Production environment
         
         Keep in mind that Kosmorro is still in alpha development stage and is not considered as stable.
         
         #### Linux
         
         ##### Arch Linux, Manjaro…
@@ -36,26 +27,30 @@
         
         Kosmorro is available [on PyPI](https://pypi.org/project/kosmorro/), a repository dedicated to Python.
         First, install `python-pip` on your system and invoke the following command: `pip install kosmorro`.
         
         #### macOS
         
         Currently, macOS does not provide Python 3, so you will first have to install it.
-        If you don't have it, first install [HomeBrew](https://formulae.brew.sh), then install Python 3: `brew install python`.
+        If you don't have it, install [HomeBrew](https://formulae.brew.sh), then install Python 3: `brew install python`.
         
         This will install Python 3 and its PIP on your system. Note that their executables are called `python3` and `pip3`.
         Now, you can install Kosmorro with your PIP: `pip3 install kosmorro`.
         
         #### Windows
         
         Kosmorro being at an early-stage development, Windows is not supported officially for now.
         
         ### Development environment
         
-        First, install [Pipenv](https://pypi.org/project/pipenv/).
+        Before you run Kosmorro in your development environment, check you have installed these programs on your system:
+        
+        - Python ≥ 3.7.0 (needed run Kosmorro)
+        - PIP3 (needed for package management, usually installed among with Python 3)
+        - [Pipenv](https://pypi.org/project/pipenv/) (needed to manage the virtual environment)
         
         Clone this repository and run `pipenv sync` to install all the dependencies.
         Then, run Kosmorro by invoking `pipenv run python kosmorro`.
         
         For comfort, you may want to invoke `pipenv shell` first and then just `python kosmoro`.
         
         ## Using Kosmorro
@@ -67,28 +62,24 @@
         
         Kosmorro has a lot of available options. To get a list of them, run `kosmorro --help`, or read its manual with `man kosmorro`.
         
         Note: the first time it runs, Kosmorro will download some important files needed to make the computations. They are stored in a cache folder named `.kosmorro-cache` located in your home directory (`/home/<username>` on Linux, `/Users/<username>` on macOS).
         
         ### Exporting to PDF
         
-        Kosmorro can export the computation results to PDF files, but this feature requires first that you install some additional dependencies. Before you use this feature, please check these packages are installed:
+        Kosmorro can export the computation results to PDF files, but this feature requires first that you install some additional dependencies.
+        Before you use this feature, make sure you have installed a LaTeX distribution:
         
-        - **A LaTeX distribution:**
-            - Linux: install TeXLive through your packages manager. Kosmorro just needs the minimal installation, you don't need any extension.
-            - macOS: install [MacTeX](https://www.tug.org/mactex/), the basic version will suffice:
-                - from the official website, choose the _smaller download_
-                - with Brew: `brew install basictex`
-        - **The `latex` Python library:**
-            - Arch Linux: the library is available [on the AUR](https://aur.archlinux.org/packages/python-latex)
-            - Any other systems: install it through PyPI: `pip install latex`
+        - **Linux:** install TeXLive through your packages manager. Kosmorro just needs the minimal installation, you don't need any extension.  
+          Note: **on Ubuntu 20.04+**, you will also need the `texlive-latex-extra` package.
+        - **macOS**: install basic version of [MacTeX](https://www.tug.org/mactex/):
+            - from the official website, choose the _smaller download_
+            - with Brew: `brew install basictex`
         
         These dependencies are not installed by default, because they take a lot of place and are not necessary if you are not interested in generating PDF files.
-        The first time you ask Kosmorro to create a PDF, it may be a little verbose. You can ignore its blahblah.
-        
         
 Keywords: kosmorro astronomy ephemerides ephemeris
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Environment :: Console
```

### Comparing `kosmorro-0.8.1/README.md` & `kosmorro-0.9.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,14 @@
 # ![Kosmorro](kosmorrolib/assets/png/kosmorro-logo.png)
-[![Coverage Status](https://coveralls.io/repos/github/Deuchnord/kosmorro/badge.svg)](https://coveralls.io/github/Deuchnord/kosmorro) [![Version on PyPI](https://img.shields.io/pypi/v/kosmorro)](https://pypi.org/project/kosmorro) [![Discord](https://img.shields.io/discord/650237632533757965?logo=discord&label=%23kosmorro)](https://discord.gg/nyemBqE)
+[![Coverage Status](https://coveralls.io/repos/github/Kosmorro/kosmorro/badge.svg?branch=master)](https://coveralls.io/github/Kosmorro/kosmorro?branch=master) [![Version on PyPI](https://img.shields.io/pypi/v/kosmorro)](https://pypi.org/project/kosmorro) [![Discord](https://img.shields.io/discord/650237632533757965?logo=discord&label=%23kosmorro)](https://discord.gg/TVX4MSKGaa)
 
-## About the project
-
-Kosmorro is a software that allows you to compute the ephemeris for a date, a month or a year.
+A program that calculates your astronomical ephemerides!
 
 ## Installation
 
-### Requirements
-
-Kosmorro requires the following software to work:
-
-- Python ≥ 3.5.0
-- PIP
-
 ### Production environment
 
 Keep in mind that Kosmorro is still in alpha development stage and is not considered as stable.
 
 #### Linux
 
 ##### Arch Linux, Manjaro…
@@ -28,26 +19,30 @@
 
 Kosmorro is available [on PyPI](https://pypi.org/project/kosmorro/), a repository dedicated to Python.
 First, install `python-pip` on your system and invoke the following command: `pip install kosmorro`.
 
 #### macOS
 
 Currently, macOS does not provide Python 3, so you will first have to install it.
-If you don't have it, first install [HomeBrew](https://formulae.brew.sh), then install Python 3: `brew install python`.
+If you don't have it, install [HomeBrew](https://formulae.brew.sh), then install Python 3: `brew install python`.
 
 This will install Python 3 and its PIP on your system. Note that their executables are called `python3` and `pip3`.
 Now, you can install Kosmorro with your PIP: `pip3 install kosmorro`.
 
 #### Windows
 
 Kosmorro being at an early-stage development, Windows is not supported officially for now.
 
 ### Development environment
 
-First, install [Pipenv](https://pypi.org/project/pipenv/).
+Before you run Kosmorro in your development environment, check you have installed these programs on your system:
+
+- Python ≥ 3.7.0 (needed run Kosmorro)
+- PIP3 (needed for package management, usually installed among with Python 3)
+- [Pipenv](https://pypi.org/project/pipenv/) (needed to manage the virtual environment)
 
 Clone this repository and run `pipenv sync` to install all the dependencies.
 Then, run Kosmorro by invoking `pipenv run python kosmorro`.
 
 For comfort, you may want to invoke `pipenv shell` first and then just `python kosmoro`.
 
 ## Using Kosmorro
@@ -59,21 +54,17 @@
 
 Kosmorro has a lot of available options. To get a list of them, run `kosmorro --help`, or read its manual with `man kosmorro`.
 
 Note: the first time it runs, Kosmorro will download some important files needed to make the computations. They are stored in a cache folder named `.kosmorro-cache` located in your home directory (`/home/<username>` on Linux, `/Users/<username>` on macOS).
 
 ### Exporting to PDF
 
-Kosmorro can export the computation results to PDF files, but this feature requires first that you install some additional dependencies. Before you use this feature, please check these packages are installed:
+Kosmorro can export the computation results to PDF files, but this feature requires first that you install some additional dependencies.
+Before you use this feature, make sure you have installed a LaTeX distribution:
 
-- **A LaTeX distribution:**
-    - Linux: install TeXLive through your packages manager. Kosmorro just needs the minimal installation, you don't need any extension.
-    - macOS: install [MacTeX](https://www.tug.org/mactex/), the basic version will suffice:
-        - from the official website, choose the _smaller download_
-        - with Brew: `brew install basictex`
-- **The `latex` Python library:**
-    - Arch Linux: the library is available [on the AUR](https://aur.archlinux.org/packages/python-latex)
-    - Any other systems: install it through PyPI: `pip install latex`
+- **Linux:** install TeXLive through your packages manager. Kosmorro just needs the minimal installation, you don't need any extension.  
+  Note: **on Ubuntu 20.04+**, you will also need the `texlive-latex-extra` package.
+- **macOS**: install basic version of [MacTeX](https://www.tug.org/mactex/):
+    - from the official website, choose the _smaller download_
+    - with Brew: `brew install basictex`
 
 These dependencies are not installed by default, because they take a lot of place and are not necessary if you are not interested in generating PDF files.
-The first time you ask Kosmorro to create a PDF, it may be a little verbose. You can ignore its blahblah.
-
```

### Comparing `kosmorro-0.8.1/kosmorro` & `kosmorro-0.9.0/kosmorro`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorro.egg-info/PKG-INFO` & `kosmorro-0.9.0/kosmorro.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 Metadata-Version: 2.1
 Name: kosmorro
-Version: 0.8.1
+Version: 0.9.0
 Summary: A program that computes the ephemerides.
 Home-page: http://kosmorro.space
 Author: Jérôme Deuchnord
 Author-email: jerome@deuchnord.fr
 License: AGPL-3.0
 Description: # ![Kosmorro](kosmorrolib/assets/png/kosmorro-logo.png)
-        [![Coverage Status](https://coveralls.io/repos/github/Deuchnord/kosmorro/badge.svg)](https://coveralls.io/github/Deuchnord/kosmorro) [![Version on PyPI](https://img.shields.io/pypi/v/kosmorro)](https://pypi.org/project/kosmorro) [![Discord](https://img.shields.io/discord/650237632533757965?logo=discord&label=%23kosmorro)](https://discord.gg/nyemBqE)
+        [![Coverage Status](https://coveralls.io/repos/github/Kosmorro/kosmorro/badge.svg?branch=master)](https://coveralls.io/github/Kosmorro/kosmorro?branch=master) [![Version on PyPI](https://img.shields.io/pypi/v/kosmorro)](https://pypi.org/project/kosmorro) [![Discord](https://img.shields.io/discord/650237632533757965?logo=discord&label=%23kosmorro)](https://discord.gg/TVX4MSKGaa)
         
-        ## About the project
-        
-        Kosmorro is a software that allows you to compute the ephemeris for a date, a month or a year.
+        A program that calculates your astronomical ephemerides!
         
         ## Installation
         
-        ### Requirements
-        
-        Kosmorro requires the following software to work:
-        
-        - Python ≥ 3.5.0
-        - PIP
-        
         ### Production environment
         
         Keep in mind that Kosmorro is still in alpha development stage and is not considered as stable.
         
         #### Linux
         
         ##### Arch Linux, Manjaro…
@@ -36,26 +27,30 @@
         
         Kosmorro is available [on PyPI](https://pypi.org/project/kosmorro/), a repository dedicated to Python.
         First, install `python-pip` on your system and invoke the following command: `pip install kosmorro`.
         
         #### macOS
         
         Currently, macOS does not provide Python 3, so you will first have to install it.
-        If you don't have it, first install [HomeBrew](https://formulae.brew.sh), then install Python 3: `brew install python`.
+        If you don't have it, install [HomeBrew](https://formulae.brew.sh), then install Python 3: `brew install python`.
         
         This will install Python 3 and its PIP on your system. Note that their executables are called `python3` and `pip3`.
         Now, you can install Kosmorro with your PIP: `pip3 install kosmorro`.
         
         #### Windows
         
         Kosmorro being at an early-stage development, Windows is not supported officially for now.
         
         ### Development environment
         
-        First, install [Pipenv](https://pypi.org/project/pipenv/).
+        Before you run Kosmorro in your development environment, check you have installed these programs on your system:
+        
+        - Python ≥ 3.7.0 (needed run Kosmorro)
+        - PIP3 (needed for package management, usually installed among with Python 3)
+        - [Pipenv](https://pypi.org/project/pipenv/) (needed to manage the virtual environment)
         
         Clone this repository and run `pipenv sync` to install all the dependencies.
         Then, run Kosmorro by invoking `pipenv run python kosmorro`.
         
         For comfort, you may want to invoke `pipenv shell` first and then just `python kosmoro`.
         
         ## Using Kosmorro
@@ -67,28 +62,24 @@
         
         Kosmorro has a lot of available options. To get a list of them, run `kosmorro --help`, or read its manual with `man kosmorro`.
         
         Note: the first time it runs, Kosmorro will download some important files needed to make the computations. They are stored in a cache folder named `.kosmorro-cache` located in your home directory (`/home/<username>` on Linux, `/Users/<username>` on macOS).
         
         ### Exporting to PDF
         
-        Kosmorro can export the computation results to PDF files, but this feature requires first that you install some additional dependencies. Before you use this feature, please check these packages are installed:
+        Kosmorro can export the computation results to PDF files, but this feature requires first that you install some additional dependencies.
+        Before you use this feature, make sure you have installed a LaTeX distribution:
         
-        - **A LaTeX distribution:**
-            - Linux: install TeXLive through your packages manager. Kosmorro just needs the minimal installation, you don't need any extension.
-            - macOS: install [MacTeX](https://www.tug.org/mactex/), the basic version will suffice:
-                - from the official website, choose the _smaller download_
-                - with Brew: `brew install basictex`
-        - **The `latex` Python library:**
-            - Arch Linux: the library is available [on the AUR](https://aur.archlinux.org/packages/python-latex)
-            - Any other systems: install it through PyPI: `pip install latex`
+        - **Linux:** install TeXLive through your packages manager. Kosmorro just needs the minimal installation, you don't need any extension.  
+          Note: **on Ubuntu 20.04+**, you will also need the `texlive-latex-extra` package.
+        - **macOS**: install basic version of [MacTeX](https://www.tug.org/mactex/):
+            - from the official website, choose the _smaller download_
+            - with Brew: `brew install basictex`
         
         These dependencies are not installed by default, because they take a lot of place and are not necessary if you are not interested in generating PDF files.
-        The first time you ask Kosmorro to create a PDF, it may be a little verbose. You can ignore its blahblah.
-        
         
 Keywords: kosmorro astronomy ephemerides ephemeris
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Environment :: Console
```

### Comparing `kosmorro-0.8.1/kosmorro.egg-info/SOURCES.txt` & `kosmorro-0.9.0/kosmorro.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 kosmorro.egg-info/requires.txt
 kosmorro.egg-info/top_level.txt
 kosmorrolib/__init__.py
 kosmorrolib/core.py
 kosmorrolib/data.py
 kosmorrolib/dateutil.py
 kosmorrolib/dumper.py
+kosmorrolib/enum.py
 kosmorrolib/ephemerides.py
 kosmorrolib/events.py
 kosmorrolib/exceptions.py
 kosmorrolib/i18n.py
 kosmorrolib/main.py
 kosmorrolib/version.py
 kosmorrolib/assets/moonphases/png/first-quarter.png
```

### Comparing `kosmorro-0.8.1/kosmorrolib/__init__.py` & `kosmorro-0.9.0/kosmorrolib/__init__.py`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/moonphases/png/first-quarter.png` & `kosmorro-0.9.0/kosmorrolib/assets/moonphases/png/first-quarter.png`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/moonphases/png/full-moon.png` & `kosmorro-0.9.0/kosmorrolib/assets/moonphases/png/full-moon.png`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/moonphases/png/last-quarter.png` & `kosmorro-0.9.0/kosmorrolib/assets/moonphases/png/last-quarter.png`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/moonphases/png/new-moon.png` & `kosmorro-0.9.0/kosmorrolib/assets/moonphases/png/new-moon.png`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/moonphases/png/unknown.png` & `kosmorro-0.9.0/kosmorrolib/assets/moonphases/png/unknown.png`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/moonphases/png/waning-crescent.png` & `kosmorro-0.9.0/kosmorrolib/assets/moonphases/png/waning-crescent.png`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/moonphases/png/waning-gibbous.png` & `kosmorro-0.9.0/kosmorrolib/assets/moonphases/png/waning-gibbous.png`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/moonphases/png/waxing-crescent.png` & `kosmorro-0.9.0/kosmorrolib/assets/moonphases/png/waxing-crescent.png`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/moonphases/png/waxing-gibbous.png` & `kosmorro-0.9.0/kosmorrolib/assets/moonphases/png/waxing-gibbous.png`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/moonphases/svg/first-quarter.svg` & `kosmorro-0.9.0/kosmorrolib/assets/moonphases/svg/first-quarter.svg`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/moonphases/svg/full-moon.svg` & `kosmorro-0.9.0/kosmorrolib/assets/moonphases/svg/full-moon.svg`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/moonphases/svg/last-quarter.svg` & `kosmorro-0.9.0/kosmorrolib/assets/moonphases/svg/last-quarter.svg`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/moonphases/svg/new-moon.svg` & `kosmorro-0.9.0/kosmorrolib/assets/moonphases/svg/new-moon.svg`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/moonphases/svg/unknown.svg` & `kosmorro-0.9.0/kosmorrolib/assets/moonphases/svg/unknown.svg`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/moonphases/svg/waning-crescent.svg` & `kosmorro-0.9.0/kosmorrolib/assets/moonphases/svg/waning-crescent.svg`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/moonphases/svg/waning-gibbous.svg` & `kosmorro-0.9.0/kosmorrolib/assets/moonphases/svg/waning-gibbous.svg`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/moonphases/svg/waxing-crescent.svg` & `kosmorro-0.9.0/kosmorrolib/assets/moonphases/svg/waxing-crescent.svg`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/moonphases/svg/waxing-gibbous.svg` & `kosmorro-0.9.0/kosmorrolib/assets/moonphases/svg/waxing-gibbous.svg`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/pdf/kosmorro.sty` & `kosmorro-0.9.0/kosmorrolib/assets/pdf/kosmorro.sty`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/pdf/template.tex` & `kosmorro-0.9.0/kosmorrolib/assets/pdf/template.tex`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/png/kosmorro-icon-white.png` & `kosmorro-0.9.0/kosmorrolib/assets/png/kosmorro-icon-white.png`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/png/kosmorro-icon.png` & `kosmorro-0.9.0/kosmorrolib/assets/png/kosmorro-icon.png`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/png/kosmorro-logo-white.png` & `kosmorro-0.9.0/kosmorrolib/assets/png/kosmorro-logo-white.png`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/png/kosmorro-logo.png` & `kosmorro-0.9.0/kosmorrolib/assets/png/kosmorro-logo.png`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/svg/kosmorro-icon-white.svg` & `kosmorro-0.9.0/kosmorrolib/assets/svg/kosmorro-icon-white.svg`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/svg/kosmorro-icon.svg` & `kosmorro-0.9.0/kosmorrolib/assets/svg/kosmorro-icon.svg`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/svg/kosmorro-logo-white.svg` & `kosmorro-0.9.0/kosmorrolib/assets/svg/kosmorro-logo-white.svg`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/assets/svg/kosmorro-logo.svg` & `kosmorro-0.9.0/kosmorrolib/assets/svg/kosmorro-logo.svg`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/core.py` & `kosmorro-0.9.0/kosmorrolib/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,15 +94,16 @@
 
 
 def get_date(date_arg: str) -> date:
     if re.match(r'^\d{4}-\d{2}-\d{2}$', date_arg):
         try:
             return date.fromisoformat(date_arg)
         except ValueError as error:
-            raise ValueError(_('The date {date} is not valid: {error}').format(date=date_arg, error=error.args[0]))
+            raise ValueError(_('The date {date} is not valid: {error}').format(date=date_arg,
+                                                                               error=error.args[0])) from error
     elif re.match(r'^([+-])(([0-9]+)y)?[ ]?(([0-9]+)m)?[ ]?(([0-9]+)d)?$', date_arg):
         def get_offset(date_arg: str, signifier: str):
             if re.search(r'([0-9]+)' + signifier, date_arg):
                 return abs(int(re.search(r'[+-]?([0-9]+)' + signifier, date_arg).group(0)[:-1]))
             return 0
 
         days = get_offset(date_arg, 'd')
```

### Comparing `kosmorro-0.8.1/kosmorrolib/data.py` & `kosmorro-0.9.0/kosmorrolib/data.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,78 +21,47 @@
 from datetime import datetime
 
 from numpy import pi, arcsin
 
 from skyfield.api import Topos, Time
 from skyfield.vectorlib import VectorSum as SkfPlanet
 
-from .core import get_skf_objects, get_timescale
+from .core import get_skf_objects
+from .enum import MoonPhaseType, EventType
 from .i18n import _
 
-MOON_PHASES = {
-    'NEW_MOON': _('New Moon'),
-    'WAXING_CRESCENT': _('Waxing crescent'),
-    'FIRST_QUARTER': _('First Quarter'),
-    'WAXING_GIBBOUS': _('Waxing gibbous'),
-    'FULL_MOON': _('Full Moon'),
-    'WANING_GIBBOUS': _('Waning gibbous'),
-    'LAST_QUARTER': _('Last Quarter'),
-    'WANING_CRESCENT': _('Waning crescent'),
-    'UNKNOWN': _('Unavailable')
-}
-
-EVENTS = {
-    'OPPOSITION': {'message': _('%s is in opposition')},
-    'CONJUNCTION': {'message': _('%s and %s are in conjunction')},
-    'OCCULTATION': {'message': _('%s occults %s')},
-    'MAXIMAL_ELONGATION': {'message': _("%s's largest elongation")}
-}
-
 
 class Serializable(ABC):
     @abstractmethod
     def serialize(self) -> dict:
         pass
 
 
 class MoonPhase(Serializable):
-    def __init__(self, identifier: str, time: datetime = None, next_phase_date: datetime = None):
-        if identifier not in MOON_PHASES.keys():
-            raise ValueError('identifier parameter must be one of %s (got %s)' % (', '.join(MOON_PHASES.keys()),
-                                                                                  identifier))
-
-        self.identifier = identifier
+    def __init__(self, phase_type: MoonPhaseType, time: datetime = None, next_phase_date: datetime = None):
+        self.phase_type = phase_type
         self.time = time
         self.next_phase_date = next_phase_date
 
-    def get_phase(self):
-        return MOON_PHASES[self.identifier]
-
-    def get_next_phase_name(self):
-        next_identifier = self.get_next_phase()
-
-        return MOON_PHASES[next_identifier]
-
     def get_next_phase(self):
-        if self.identifier == 'NEW_MOON' or self.identifier == 'WAXING_CRESCENT':
-            next_identifier = 'FIRST_QUARTER'
-        elif self.identifier == 'FIRST_QUARTER' or self.identifier == 'WAXING_GIBBOUS':
-            next_identifier = 'FULL_MOON'
-        elif self.identifier == 'FULL_MOON' or self.identifier == 'WANING_GIBBOUS':
-            next_identifier = 'LAST_QUARTER'
-        else:
-            next_identifier = 'NEW_MOON'
-        return next_identifier
+        if self.phase_type in [MoonPhaseType.NEW_MOON, MoonPhaseType.WAXING_CRESCENT]:
+            return MoonPhaseType.FIRST_QUARTER
+        if self.phase_type in [MoonPhaseType.FIRST_QUARTER, MoonPhaseType.WAXING_GIBBOUS]:
+            return MoonPhaseType.FULL_MOON
+        if self.phase_type in [MoonPhaseType.FULL_MOON, MoonPhaseType.WANING_GIBBOUS]:
+            return MoonPhaseType.LAST_QUARTER
+
+        return MoonPhaseType.NEW_MOON
 
     def serialize(self) -> dict:
         return {
-            'phase': self.identifier,
+            'phase': self.phase_type.name,
             'time': self.time.isoformat() if self.time is not None else None,
             'next': {
-                'phase': self.get_next_phase(),
+                'phase': self.get_next_phase().name,
                 'time': self.next_phase_date.isoformat()
             }
         }
 
 
 class Object(Serializable):
     """
@@ -111,14 +80,17 @@
         :param float radius: the radius (in km) of the object
         :param AsterEphemerides ephemerides: the ephemerides associated to the object
         """
         self.name = name
         self.skyfield_name = skyfield_name
         self.radius = radius
 
+    def __repr__(self):
+        return '<Object type=%s name=%s />' % (self.get_type(), self.name)
+
     def get_skyfield_object(self) -> SkfPlanet:
         return get_skf_objects()[self.skyfield_name]
 
     @abstractmethod
     def get_type(self) -> str:
         pass
 
@@ -159,86 +131,51 @@
 
 class Satellite(Object):
     def get_type(self) -> str:
         return 'satellite'
 
 
 class Event(Serializable):
-    def __init__(self, event_type: str, objects: [Object], start_time: datetime,
+    def __init__(self, event_type: EventType, objects: [Object], start_time: datetime,
                  end_time: Union[datetime, None] = None, details: str = None):
-        if event_type not in EVENTS.keys():
-            accepted_types = ', '.join(EVENTS.keys())
-            raise ValueError('event_type parameter must be one of the following: %s (got %s)' % (accepted_types,
-                                                                                                 event_type))
-
         self.event_type = event_type
         self.objects = objects
         self.start_time = start_time
         self.end_time = end_time
         self.details = details
 
+    def __repr__(self):
+        return '<Event type=%s objects=[%s] start=%s end=%s details=%s>' % (self.event_type,
+                                                                            self.objects,
+                                                                            self.start_time,
+                                                                            self.end_time,
+                                                                            self.details)
+
     def get_description(self, show_details: bool = True) -> str:
-        description = EVENTS[self.event_type]['message'] % self._get_objects_name()
+        description = self.event_type.value % self._get_objects_name()
         if show_details and self.details is not None:
             description += ' ({:s})'.format(self.details)
         return description
 
     def _get_objects_name(self):
         if len(self.objects) == 1:
             return self.objects[0].name
 
         return tuple(object.name for object in self.objects)
 
     def serialize(self) -> dict:
         return {
             'objects': [object.serialize() for object in self.objects],
-            'event': self.event_type,
+            'event': self.event_type.name,
             'starts_at': self.start_time.isoformat(),
             'ends_at': self.end_time.isoformat() if self.end_time is not None else None,
             'details': self.details
         }
 
 
-def skyfield_to_moon_phase(times: [Time], vals: [int], now: Time) -> Union[MoonPhase, None]:
-    tomorrow = get_timescale().utc(now.utc_datetime().year, now.utc_datetime().month, now.utc_datetime().day + 1)
-
-    phases = list(MOON_PHASES.keys())
-    current_phase = None
-    current_phase_time = None
-    next_phase_time = None
-    i = 0
-
-    if len(times) == 0:
-        return None
-
-    for i, time in enumerate(times):
-        if now.utc_iso() <= time.utc_iso():
-            if vals[i] in [0, 2, 4, 6]:
-                if time.utc_datetime() < tomorrow.utc_datetime():
-                    current_phase_time = time
-                    current_phase = phases[vals[i]]
-                else:
-                    i -= 1
-                    current_phase_time = None
-                    current_phase = phases[vals[i]]
-            else:
-                current_phase = phases[vals[i]]
-
-            break
-
-    for j in range(i + 1, len(times)):
-        if vals[j] in [0, 2, 4, 6]:
-            next_phase_time = times[j]
-            break
-
-    return MoonPhase(current_phase,
-                     current_phase_time.utc_datetime() if current_phase_time is not None else None,
-                     next_phase_time.utc_datetime() if next_phase_time is not None else None)
-
-
 class AsterEphemerides(Serializable):
     def __init__(self,
                  rise_time: Union[datetime, None],
                  culmination_time: Union[datetime, None],
                  set_time: Union[datetime, None],
                  aster: Object):
         self.rise_time = rise_time
@@ -251,16 +188,14 @@
             'object': self.object.serialize(),
             'rise_time': self.rise_time.isoformat() if self.rise_time is not None else None,
             'culmination_time': self.culmination_time.isoformat() if self.culmination_time is not None else None,
             'set_time': self.set_time.isoformat() if self.set_time is not None else None
         }
 
 
-MONTHS = ['JAN', 'FEB', 'MAR', 'APR', 'MAY', 'JUN', 'JUL', 'AUG', 'SEP', 'OCT', 'NOV', 'DEC']
-
 EARTH = Planet('Earth', 'EARTH')
 
 ASTERS = [Star(_('Sun'), 'SUN', radius=696342),
           Satellite(_('Moon'), 'MOON', radius=1737.4),
           Planet(_('Mercury'), 'MERCURY', radius=2439.7),
           Planet(_('Venus'), 'VENUS', radius=6051.8),
           Planet(_('Mars'), 'MARS', radius=3396.2),
```

### Comparing `kosmorro-0.8.1/kosmorrolib/dateutil.py` & `kosmorro-0.9.0/kosmorrolib/dateutil.py`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/dumper.py` & `kosmorro-0.9.0/kosmorrolib/dumper.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 #    You should have received a copy of the GNU Affero General Public License
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
 import datetime
 import json
 import os
+import tempfile
+import subprocess
+import shutil
 from pathlib import Path
 from tabulate import tabulate
 from termcolor import colored
+
 from .data import ASTERS, AsterEphemerides, MoonPhase, Event
 from .i18n import _, FULL_DATE_FORMAT, SHORT_DATETIME_FORMAT, TIME_FORMAT
 from .version import VERSION
-from .exceptions import UnavailableFeatureError
-try:
-    from latex import build_pdf
-except ImportError:
-    build_pdf = None
+from .exceptions import UnavailableFeatureError, CompileError
 
 
 class Dumper(ABC):
     def __init__(self, ephemerides: [AsterEphemerides] = None, moon_phase: MoonPhase = None, events: [Event] = None,
                  date: datetime.date = datetime.date.today(), timezone: int = 0, with_colors: bool = True,
                  show_graph: bool = False):
         self.ephemerides = ephemerides
@@ -155,17 +155,17 @@
 
         return tabulate(data, tablefmt='plain', stralign='left')
 
     def get_moon(self, moon_phase: MoonPhase) -> str:
         if moon_phase is None:
             return _('Moon phase is unavailable for this date.')
 
-        current_moon_phase = ' '.join([self.style(_('Moon phase:'), 'strong'), moon_phase.get_phase()])
+        current_moon_phase = ' '.join([self.style(_('Moon phase:'), 'strong'), moon_phase.phase_type.value])
         new_moon_phase = _('{next_moon_phase} on {next_moon_phase_date} at {next_moon_phase_time}').format(
-            next_moon_phase=moon_phase.get_next_phase_name(),
+            next_moon_phase=moon_phase.get_next_phase().value,
             next_moon_phase_date=moon_phase.next_phase_date.strftime(FULL_DATE_FORMAT),
             next_moon_phase_time=moon_phase.next_phase_date.strftime(TIME_FORMAT)
         )
 
         return '\n'.join([current_moon_phase, new_moon_phase])
 
 
@@ -179,20 +179,17 @@
 
         return self._make_document(template)
 
     def _make_document(self, template: str) -> str:
         kosmorro_logo_path = os.path.join(os.path.abspath(os.path.dirname(__file__)),
                                           'assets', 'png', 'kosmorro-logo.png')
 
-        if self.moon_phase is None:
-            self.moon_phase = MoonPhase('UNKNOWN')
-
         moon_phase_graphics = os.path.join(os.path.abspath(os.path.dirname(__file__)),
                                            'assets', 'moonphases', 'png',
-                                           '.'.join([self.moon_phase.identifier.lower().replace('_', '-'),
+                                           '.'.join([self.moon_phase.phase_type.name.lower().replace('_', '-'),
                                                      'png']))
 
         document = template
 
         if self.ephemerides is None:
             document = self._remove_section(document, 'ephemerides')
 
@@ -230,15 +227,15 @@
             .replace('+++EPHEMERIDES-RISE-TIME+++', _('Rise time')) \
             .replace('+++EPHEMERIDES-CULMINATION-TIME+++', _('Culmination time')) \
             .replace('+++EPHEMERIDES-SET-TIME+++', _('Set time')) \
             .replace('+++EPHEMERIDES+++', self._make_ephemerides()) \
             .replace('+++GRAPH_LABEL_HOURS+++', _('hours')) \
             .replace('+++MOON-PHASE-GRAPHICS+++', moon_phase_graphics) \
             .replace('+++CURRENT-MOON-PHASE-TITLE+++', _('Moon phase:')) \
-            .replace('+++CURRENT-MOON-PHASE+++', self.moon_phase.get_phase()) \
+            .replace('+++CURRENT-MOON-PHASE+++', self.moon_phase.phase_type.value) \
             .replace('+++SECTION-EVENTS+++', _('Expected events')) \
             .replace('+++EVENTS+++', self._make_events())
 
         for aster in ASTERS:
             document = document.replace('+++ASTER_%s+++' % aster.skyfield_name.upper().split(' ')[0],
                                         aster.name)
 
@@ -344,24 +341,45 @@
 class PdfDumper(Dumper):
     def to_string(self):
         try:
             latex_dumper = _LatexDumper(self.ephemerides, self.moon_phase, self.events,
                                         date=self.date, timezone=self.timezone, with_colors=self.with_colors,
                                         show_graph=self.show_graph)
             return self._compile(latex_dumper.to_string())
-        except RuntimeError:
+        except CompileError as error:
+            raise UnavailableFeatureError from error
+        except RuntimeError as error:
             raise UnavailableFeatureError(_("Building PDFs was not possible, because some dependencies are not"
                                             " installed.\nPlease look at the documentation at http://kosmorro.space "
-                                            "for more information."))
+                                            "for more information.")) from error
 
     @staticmethod
     def is_file_output_needed() -> bool:
         return True
 
     @staticmethod
     def _compile(latex_input) -> bytes:
-        if build_pdf is None:
-            raise RuntimeError('Python latex module not found')
+        package = str(Path(__file__).parent.absolute()) + '/assets/pdf/kosmorro.sty'
 
-        package = str(Path(__file__).parent.absolute()) + '/assets/pdf/'
+        with tempfile.TemporaryDirectory() as tempdir:
+            timestamp = datetime.datetime.now().strftime('%Y%m%d%H%M%S')
+            shutil.copy(package, tempdir)
+
+            with open('%s/%s.tex' % (tempdir, timestamp), 'w') as texfile:
+                texfile.write(latex_input)
+
+            os.chdir(tempdir)
+            try:
+                subprocess.run(['pdflatex', '-interaction', 'nonstopmode', '%s.tex' % timestamp],
+                               capture_output=True, check=True)
+            except FileNotFoundError as error:
+                raise RuntimeError('pdflatex is not installed.') from error
+            except subprocess.CalledProcessError as error:
+                with open('/tmp/kosmorro-%s.log' % timestamp, 'wb') as file:
+                    file.write(error.stdout)
+
+                raise CompileError(_('An error occured during the compilation of the PDF.\n'
+                                     'Please open an issue at https://github.com/Kosmorro/kosmorro/issues and share '
+                                     'the content of the log file at /tmp/kosmorro-%s.log' % timestamp)) from error
 
-        return bytes(build_pdf(latex_input, [package]))
+            with open('%s.pdf' % timestamp, 'rb') as pdffile:
+                return bytes(pdffile.read())
```

### Comparing `kosmorro-0.8.1/kosmorrolib/ephemerides.py` & `kosmorro-0.9.0/kosmorrolib/ephemerides.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,28 +13,67 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU Affero General Public License for more details.
 #
 #    You should have received a copy of the GNU Affero General Public License
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import datetime
+from typing import Union
 
 from skyfield.searchlib import find_discrete, find_maxima
 from skyfield.timelib import Time
 from skyfield.constants import tau
 from skyfield.errors import EphemerisRangeError
 
-from .data import Position, AsterEphemerides, MoonPhase, Object, ASTERS, skyfield_to_moon_phase
+from .data import Position, AsterEphemerides, MoonPhase, Object, ASTERS
 from .dateutil import translate_to_timezone
 from .core import get_skf_objects, get_timescale, get_iau2000b
+from .enum import MoonPhaseType
 from .exceptions import OutOfRangeDateError
 
 RISEN_ANGLE = -0.8333
 
 
+def _get_skyfield_to_moon_phase(times: [Time], vals: [int], now: Time) -> Union[MoonPhase, None]:
+    tomorrow = get_timescale().utc(now.utc_datetime().year, now.utc_datetime().month, now.utc_datetime().day + 1)
+
+    phases = list(MoonPhaseType)
+    current_phase = None
+    current_phase_time = None
+    next_phase_time = None
+    i = 0
+
+    if len(times) == 0:
+        return None
+
+    for i, time in enumerate(times):
+        if now.utc_iso() <= time.utc_iso():
+            if vals[i] in [0, 2, 4, 6]:
+                if time.utc_datetime() < tomorrow.utc_datetime():
+                    current_phase_time = time
+                    current_phase = phases[vals[i]]
+                else:
+                    i -= 1
+                    current_phase_time = None
+                    current_phase = phases[vals[i]]
+            else:
+                current_phase = phases[vals[i]]
+
+            break
+
+    for j in range(i + 1, len(times)):
+        if vals[j] in [0, 2, 4, 6]:
+            next_phase_time = times[j]
+            break
+
+    return MoonPhase(current_phase,
+                     current_phase_time.utc_datetime() if current_phase_time is not None else None,
+                     next_phase_time.utc_datetime() if next_phase_time is not None else None)
+
+
 def get_moon_phase(compute_date: datetime.date, timezone: int = 0) -> MoonPhase:
     earth = get_skf_objects()['earth']
     moon = get_skf_objects()['moon']
     sun = get_skf_objects()['sun']
 
     def moon_phase_at(time: Time):
         time._nutation_angles = get_iau2000b(time)
@@ -54,17 +93,17 @@
     except EphemerisRangeError as error:
         start = translate_to_timezone(error.start_time.utc_datetime(), timezone)
         end = translate_to_timezone(error.end_time.utc_datetime(), timezone)
 
         start = datetime.date(start.year, start.month, start.day) + datetime.timedelta(days=12)
         end = datetime.date(end.year, end.month, end.day) - datetime.timedelta(days=12)
 
-        raise OutOfRangeDateError(start, end)
+        raise OutOfRangeDateError(start, end) from error
 
-    return skyfield_to_moon_phase(times, phase, today)
+    return _get_skyfield_to_moon_phase(times, phase, today)
 
 
 def get_ephemerides(date: datetime.date, position: Position, timezone: int = 0) -> [AsterEphemerides]:
     ephemerides = []
 
     def get_angle(for_aster: Object):
         def fun(time: Time) -> float:
@@ -115,10 +154,10 @@
     except EphemerisRangeError as error:
         start = translate_to_timezone(error.start_time.utc_datetime(), timezone)
         end = translate_to_timezone(error.end_time.utc_datetime(), timezone)
 
         start = datetime.date(start.year, start.month, start.day + 1)
         end = datetime.date(end.year, end.month, end.day - 1)
 
-        raise OutOfRangeDateError(start, end)
+        raise OutOfRangeDateError(start, end) from error
 
     return ephemerides
```

### Comparing `kosmorro-0.8.1/kosmorrolib/events.py` & `kosmorro-0.9.0/kosmorrolib/events.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 #    You should have received a copy of the GNU Affero General Public License
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from datetime import date as date_type
 
 from skyfield.errors import EphemerisRangeError
 from skyfield.timelib import Time
-from skyfield.searchlib import find_discrete, find_maxima
+from skyfield.searchlib import find_discrete, find_maxima, find_minima
 from numpy import pi
 
 from .data import Event, Star, Planet, ASTERS
 from .dateutil import translate_to_timezone
+from .enum import EventType
 from .exceptions import OutOfRangeDateError
 from .core import get_timescale, get_skf_objects, flatten_list
 
 
 def _search_conjunction(start_time: Time, end_time: Time, timezone: int) -> [Event]:
     earth = get_skf_objects()['earth']
     aster1 = None
@@ -64,18 +65,18 @@
                     distance = aster1_pos.separation_from(aster2_pos).degrees
 
                     if distance - aster2.get_apparent_radius(time, earth) < aster1.get_apparent_radius(time, earth):
                         occulting_aster = [aster1,
                                            aster2] if aster1_pos.distance().km < aster2_pos.distance().km else [aster2,
                                                                                                                 aster1]
 
-                        conjunctions.append(Event('OCCULTATION', occulting_aster,
+                        conjunctions.append(Event(EventType.OCCULTATION, occulting_aster,
                                                   translate_to_timezone(time.utc_datetime(), timezone)))
                     else:
-                        conjunctions.append(Event('CONJUNCTION', [aster1, aster2],
+                        conjunctions.append(Event(EventType.CONJUNCTION, [aster1, aster2],
                                                   translate_to_timezone(time.utc_datetime(), timezone)))
 
         computed.append(aster1)
 
     return conjunctions
 
 
@@ -97,15 +98,15 @@
 
     for aster in ASTERS:
         if not isinstance(aster, Planet) or aster.skyfield_name in ['MERCURY', 'VENUS']:
             continue
 
         times, _ = find_discrete(start_time, end_time, is_oppositing)
         for time in times:
-            events.append(Event('OPPOSITION', [aster], translate_to_timezone(time.utc_datetime(), timezone)))
+            events.append(Event(EventType.OPPOSITION, [aster], translate_to_timezone(time.utc_datetime(), timezone)))
 
     return events
 
 
 def _search_maximal_elongations(start_time: Time, end_time: Time, timezone: int) -> [Event]:
     earth = get_skf_objects()['earth']
     sun = get_skf_objects()['sun']
@@ -125,31 +126,74 @@
         if aster.skyfield_name not in ['MERCURY', 'VENUS']:
             continue
 
         times, elongations = find_maxima(start_time, end_time, f=get_elongation, epsilon=1./24/3600, num=12)
 
         for i, time in enumerate(times):
             elongation = elongations[i]
-            events.append(Event('MAXIMAL_ELONGATION', [aster], translate_to_timezone(time.utc_datetime(), timezone),
+            events.append(Event(EventType.MAXIMAL_ELONGATION,
+                                [aster],
+                                translate_to_timezone(time.utc_datetime(), timezone),
                                 details='{:.3n}°'.format(elongation)))
 
     return events
 
 
+def _get_moon_distance():
+    earth = get_skf_objects()['earth']
+    moon = get_skf_objects()['moon']
+
+    def get_distance(time: Time):
+        earth_pos = earth.at(time)
+        moon_pos = earth_pos.observe(moon).apparent()
+
+        return moon_pos.distance().au
+
+    get_distance.rough_period = 1.0
+
+    return get_distance
+
+
+def _search_moon_apogee(start_time: Time, end_time: Time, timezone: int) -> [Event]:
+    moon = ASTERS[1]
+    events = []
+
+    times, _ = find_maxima(start_time, end_time, f=_get_moon_distance(), epsilon=1./24/60)
+
+    for time in times:
+        events.append(Event(EventType.MOON_APOGEE, [moon], translate_to_timezone(time.utc_datetime(), timezone)))
+
+    return events
+
+
+def _search_moon_perigee(start_time: Time, end_time: Time, timezone: int) -> [Event]:
+    moon = ASTERS[1]
+    events = []
+
+    times, _ = find_minima(start_time, end_time, f=_get_moon_distance(), epsilon=1./24/60)
+
+    for time in times:
+        events.append(Event(EventType.MOON_PERIGEE, [moon], translate_to_timezone(time.utc_datetime(), timezone)))
+
+    return events
+
+
 def search_events(date: date_type, timezone: int = 0) -> [Event]:
     start_time = get_timescale().utc(date.year, date.month, date.day, -timezone)
     end_time = get_timescale().utc(date.year, date.month, date.day + 1, -timezone)
 
     try:
         return sorted(flatten_list([
             _search_oppositions(start_time, end_time, timezone),
             _search_conjunction(start_time, end_time, timezone),
-            _search_maximal_elongations(start_time, end_time, timezone)
+            _search_maximal_elongations(start_time, end_time, timezone),
+            _search_moon_apogee(start_time, end_time, timezone),
+            _search_moon_perigee(start_time, end_time, timezone),
         ]), key=lambda event: event.start_time)
     except EphemerisRangeError as error:
         start_date = translate_to_timezone(error.start_time.utc_datetime(), timezone)
         end_date = translate_to_timezone(error.end_time.utc_datetime(), timezone)
 
         start_date = date_type(start_date.year, start_date.month, start_date.day)
         end_date = date_type(end_date.year, end_date.month, end_date.day)
 
-        raise OutOfRangeDateError(start_date, end_date)
+        raise OutOfRangeDateError(start_date, end_date) from error
```

### Comparing `kosmorro-0.8.1/kosmorrolib/exceptions.py` & `kosmorro-0.9.0/kosmorrolib/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,19 +18,25 @@
 
 from datetime import date
 from .i18n import _, SHORT_DATE_FORMAT
 
 
 class UnavailableFeatureError(RuntimeError):
     def __init__(self, msg: str):
-        super(UnavailableFeatureError, self).__init__()
+        super().__init__()
         self.msg = msg
 
 
 class OutOfRangeDateError(RuntimeError):
     def __init__(self, min_date: date, max_date: date):
-        super(OutOfRangeDateError, self).__init__()
+        super().__init__()
         self.min_date = min_date
         self.max_date = max_date
         self.msg = _('The date must be between {minimum_date}'
                      ' and {maximum_date}').format(minimum_date=min_date.strftime(SHORT_DATE_FORMAT),
                                                    maximum_date=max_date.strftime(SHORT_DATE_FORMAT))
+
+
+class CompileError(RuntimeError):
+    def __init__(self, msg):
+        super().__init__()
+        self.msg = msg
```

### Comparing `kosmorro-0.8.1/kosmorrolib/i18n.py` & `kosmorro-0.9.0/kosmorrolib/i18n.py`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/kosmorrolib/locales/de/LC_MESSAGES/messages.mo` & `kosmorro-0.9.0/kosmorrolib/locales/de/LC_MESSAGES/messages.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,25 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  Kosmorro\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2020-06-07 09:19+0000\n"
+"POT-Creation-Date: 2021-01-31 09:20+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.8.0\n"
+"Generated-By: Babel 2.9.0\n"
 
 msgid "%s and %s are in conjunction"
 msgstr "Konjunktion zwischen %s und %s"
 
+msgid "%s is at its apogee"
+msgstr "%s steht auf seinem Apogäum"
+
+msgid "%s is at its perigee"
+msgstr "%s befindet sich am Perigäum"
+
 msgid "%s is in opposition"
 msgstr "%s steht in Opposition"
 
 msgid "%s occults %s"
 msgstr "%s bedeckt %s"
 
 msgid "%s's largest elongation"
@@ -32,14 +38,23 @@
 "A file to export the output to. If not given, the standard output is used. "
 "This argument is needed for PDF format."
 msgstr ""
 "Eine Datei, in die die Ausgabe exportiert wird. Wenn nicht angegeben, wird "
 "die Standardausgabe verwendet. Dieses Argument wird für das PDF-Format "
 "benötigt."
 
+msgid ""
+"An error occured during the compilation of the PDF.\n"
+"Please open an issue at https://github.com/Kosmorro/kosmorro/issues and "
+"share the content of the log file at /tmp/kosmorro-%s.log"
+msgstr ""
+"Bei der Kompilierung der PDF ist ein Fehler aufgetreten.\n"
+"Bitte öffnen Sie ein Issue unter https://github.com/Kosmorro/kosmorro/issues "
+"und teilen Sie den Inhalt der Log-Datei unter /tmp/kosmorro-%s.log"
+
 msgid "Answer did not match expected options, cache not cleared."
 msgstr ""
 "Die Antwort passte nicht zu erwartete Wahlen. Der Cache wurde nicht gelöscht."
 
 msgid ""
 "Building PDFs was not possible, because some dependencies are not "
 "installed.\n"
```

### Comparing `kosmorro-0.8.1/kosmorrolib/locales/de/LC_MESSAGES/messages.po` & `kosmorro-0.9.0/kosmorrolib/locales/de/LC_MESSAGES/messages.po`

 * *Files 10% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 "Project-Id-Version: Kosmorro\n"
 "Language: de\n"
 
 #: kosmorrolib/dumper.py:87
 msgid "Expected events:"
 msgstr "Erwartete Ereignisse"
 
-#: kosmorrolib/dumper.py:142 kosmorrolib/dumper.py:229
+#: kosmorrolib/dumper.py:142 kosmorrolib/dumper.py:226
 msgid "Object"
 msgstr "Gestirn"
 
-#: kosmorrolib/dumper.py:143 kosmorrolib/dumper.py:230
+#: kosmorrolib/dumper.py:143 kosmorrolib/dumper.py:227
 msgid "Rise time"
 msgstr "Aufgangszeit"
 
-#: kosmorrolib/dumper.py:144 kosmorrolib/dumper.py:231
+#: kosmorrolib/dumper.py:144 kosmorrolib/dumper.py:228
 msgid "Culmination time"
 msgstr "Höhepunkt"
 
-#: kosmorrolib/dumper.py:145 kosmorrolib/dumper.py:232
+#: kosmorrolib/dumper.py:145 kosmorrolib/dumper.py:229
 msgid "Set time"
 msgstr "Untergangszeit"
 
 #: kosmorrolib/dumper.py:91
 msgid "Note: All the hours are given in UTC."
 msgstr "Hinweis: alle Stunden werden in UTC angegeben."
 
@@ -39,148 +39,148 @@
 msgid "{hours}:{minutes}"
 msgstr "{hours}:{minutes}"
 
 #: kosmorrolib/dumper.py:163
 msgid "{next_moon_phase} on {next_moon_phase_date} at {next_moon_phase_time}"
 msgstr "{next_moon_phase} am {next_moon_phase_date} um {next_moon_phase_time}"
 
-#: kosmorrolib/data.py:262
+#: kosmorrolib/data.py:197
 msgid "Sun"
 msgstr "Sohne"
 
-#: kosmorrolib/data.py:263
+#: kosmorrolib/data.py:198
 msgid "Moon"
 msgstr "Mond"
 
-#: kosmorrolib/data.py:264
+#: kosmorrolib/data.py:199
 msgid "Mercury"
 msgstr "Merkur"
 
-#: kosmorrolib/data.py:265
+#: kosmorrolib/data.py:200
 msgid "Venus"
 msgstr "Venus"
 
-#: kosmorrolib/data.py:266
+#: kosmorrolib/data.py:201
 msgid "Mars"
 msgstr "Mars"
 
-#: kosmorrolib/data.py:267
+#: kosmorrolib/data.py:202
 msgid "Jupiter"
 msgstr "Jupiter"
 
-#: kosmorrolib/data.py:268
+#: kosmorrolib/data.py:203
 msgid "Saturn"
 msgstr "Saturn"
 
-#: kosmorrolib/data.py:269
+#: kosmorrolib/data.py:204
 msgid "Uranus"
 msgstr "Uranus"
 
-#: kosmorrolib/data.py:270
+#: kosmorrolib/data.py:205
 msgid "Neptune"
 msgstr "Neptun"
 
-#: kosmorrolib/data.py:271
+#: kosmorrolib/data.py:206
 msgid "Pluto"
 msgstr "Pluto"
 
-#: kosmorrolib/data.py:32
+#: kosmorrolib/enum.py:24
 msgid "New Moon"
 msgstr "Neumond"
 
-#: kosmorrolib/data.py:33
+#: kosmorrolib/enum.py:25
 msgid "Waxing crescent"
 msgstr "Zunehmender Sichelmond"
 
-#: kosmorrolib/data.py:34
+#: kosmorrolib/enum.py:26
 msgid "First Quarter"
 msgstr "Erstes Viertel"
 
-#: kosmorrolib/data.py:35
+#: kosmorrolib/enum.py:27
 msgid "Waxing gibbous"
 msgstr "Zunehmender Dreiviertelmond"
 
-#: kosmorrolib/data.py:36
+#: kosmorrolib/enum.py:28
 msgid "Full Moon"
 msgstr "Vollmond"
 
-#: kosmorrolib/data.py:37
+#: kosmorrolib/enum.py:29
 msgid "Waning gibbous"
 msgstr "Abnehmender Sichelmond"
 
-#: kosmorrolib/data.py:38
+#: kosmorrolib/enum.py:30
 msgid "Last Quarter"
 msgstr "Letztes Viertel"
 
-#: kosmorrolib/data.py:39
+#: kosmorrolib/enum.py:31
 msgid "Waning crescent"
 msgstr "Abnehmender Dreiviertelmond"
 
-#: kosmorrolib/data.py:44
+#: kosmorrolib/enum.py:35
 msgid "%s is in opposition"
 msgstr "%s steht in Opposition"
 
-#: kosmorrolib/data.py:45
+#: kosmorrolib/enum.py:36
 msgid "%s and %s are in conjunction"
 msgstr "Konjunktion zwischen %s und %s"
 
-#: kosmorrolib/main.py:134
+#: kosmorrolib/main.py:139
 msgid "Running on Python {python_version}"
 msgstr "Mit Python {python_version} ausführt"
 
-#: kosmorrolib/main.py:140
+#: kosmorrolib/main.py:145
 msgid "Do you really want to clear Kosmorro's cache? [yN] "
 msgstr "Wollen Sie wirklich Kosmorros Cache löschen?"
 
-#: kosmorrolib/main.py:147
+#: kosmorrolib/main.py:152
 msgid "Answer did not match expected options, cache not cleared."
 msgstr "Die Antwort passte nicht zu erwartete Wahlen. Der Cache wurde nicht gelöscht."
 
-#: kosmorrolib/main.py:156
+#: kosmorrolib/main.py:161
 msgid "Compute the ephemerides and the events for a given date, at a given position on Earth."
 msgstr "Berechnet die Ephemeriden und die Ereignisse für das gegeben Datum und für das gegeben Standort auf der Erde."
 
-#: kosmorrolib/main.py:158
+#: kosmorrolib/main.py:163
 msgid "By default, only the events will be computed for today ({date}).\n"
 "To compute also the ephemerides, latitude and longitude arguments are needed."
 msgstr "Nur werden standardmäßig die Ereignisse für den heutigen Tag ({date}) berechnet. Um auch die Ephemeriden zu berechnen, werden die Breiten- und Längengrad benötigt."
 
-#: kosmorrolib/main.py:163
+#: kosmorrolib/main.py:168
 msgid "Show the program version"
 msgstr "Stellt die Version des Programms aus"
 
-#: kosmorrolib/main.py:165
+#: kosmorrolib/main.py:170
 msgid "Delete all the files Kosmorro stored in the cache."
 msgstr "Löscht alle die Dateien, die von Kosmorro im Cache gelagert wurden."
 
-#: kosmorrolib/main.py:167
+#: kosmorrolib/main.py:172
 msgid "The format under which the information have to be output"
 msgstr "Die Datenstruktur für die Ausgabe."
 
-#: kosmorrolib/dumper.py:162 kosmorrolib/dumper.py:236
+#: kosmorrolib/dumper.py:162 kosmorrolib/dumper.py:233
 msgid "Moon phase:"
 msgstr "Mondphase:"
 
-#: kosmorrolib/main.py:183
+#: kosmorrolib/main.py:188
 msgid "Disable the colors in the console."
 msgstr "Deaktiviert die Farben in der Konsole."
 
-#: kosmorrolib/dumper.py:216
+#: kosmorrolib/dumper.py:213
 msgid "A Summary of your Sky"
 msgstr "Übersicht über Ihren Himmel"
 
-#: kosmorrolib/dumper.py:228
+#: kosmorrolib/dumper.py:225
 msgid "Ephemerides of the day"
 msgstr "Ephemeriden des Tages"
 
-#: kosmorrolib/dumper.py:238
+#: kosmorrolib/dumper.py:235
 msgid "Expected events"
 msgstr "Erwartete Ereignisse"
 
-#: kosmorrolib/dumper.py:352
+#: kosmorrolib/dumper.py:351
 msgid "Building PDFs was not possible, because some dependencies are not installed.\n"
 "Please look at the documentation at http://kosmorro.space for more information."
 msgstr "Konnte nicht das PDF-Dokument herstellen, weil Abhängigkeiten nicht installiert werden.\n"
 "Bitte die Dokumentation auf http://kosmorro.space für mehr Informationen lesen."
 
 #: kosmorrolib/main.py:61
 msgid "Save the planet and paper!\n"
@@ -188,79 +188,79 @@
 msgstr "Bring der Planet in Sicherheit, spare Papier!\n"
 "Drucken Sie das PDF-Dokument, nur wenn Sie wirklich brauchen aus, und nutzen Sie das Verso!"
 
 #: kosmorrolib/main.py:65
 msgid "PDF output will not contain the ephemerides, because you didn't provide the observation coordinate."
 msgstr "Die PDF-Ausgabe wird die Ephemeriden nicht enthalten, weil Sie die Beobachtungskoordinate nicht angegeben haben."
 
-#: kosmorrolib/main.py:90
+#: kosmorrolib/main.py:93
 msgid "Could not save the output in \"{path}\": {error}"
 msgstr "Die Ausgabe in \"{path}\" konnte nicht gespeichert werden: {error}"
 
-#: kosmorrolib/main.py:95
+#: kosmorrolib/main.py:100
 msgid "Selected output format needs an output file (--output)."
 msgstr "Ausgewähltes Ausgabeformat benötigt eine Ausgabedatei (--output)."
 
-#: kosmorrolib/main.py:185
+#: kosmorrolib/main.py:190
 msgid "A file to export the output to. If not given, the standard output is used. This argument is needed for PDF format."
 msgstr "Eine Datei, in die die Ausgabe exportiert wird. Wenn nicht angegeben, wird die Standardausgabe verwendet. Dieses Argument wird für das PDF-Format benötigt."
 
 #: kosmorrolib/i18n.py:29
 msgid "{month} {day_number}, {hours}:{minutes}"
 msgstr "{day_number}. {month}, {hours}:{minutes}"
 
 #: kosmorrolib/dumper.py:96
 msgid "Note: All the hours are given in the UTC{offset} timezone."
 msgstr "Hinweis: Alle Stunden werden in der UTC{offset}-Zeitzone angegeben."
 
-#: kosmorrolib/dumper.py:220
+#: kosmorrolib/dumper.py:217
 msgid "This document summarizes the ephemerides and the events of {date}. It aims to help you to prepare your observation session. All the hours are given in {timezone}."
 msgstr "Dieses Dokument fasst die Ephemeriden und die Ereignisse von {date} zusammen. Es soll Ihnen bei der Vorbereitung Ihrer Beobachtungssitzung helfen. Alle Stunden sind in der Zeitzone {timezone} angegeben."
 
-#: kosmorrolib/data.py:47
+#: kosmorrolib/enum.py:38
 msgid "%s's largest elongation"
 msgstr "Höchste Elongation von %s"
 
-#: kosmorrolib/data.py:46
+#: kosmorrolib/enum.py:37
 msgid "%s occults %s"
 msgstr "%s bedeckt %s"
 
 #: kosmorrolib/core.py:101
 msgid "The date {date} is not valid: {error}"
 msgstr "Das Datum {date} ist nicht gültig: {error}"
 
-#: kosmorrolib/main.py:169
+#: kosmorrolib/main.py:174
 msgid "The observer's latitude on Earth. Can also be set in the KOSMORRO_LATITUDE environment variable."
 msgstr "Der Breitengrad des Beobachters auf der Erde. Kann auch in der Umgebungsvariablen KOSMORRO_LATITUDE gesetzt werden."
 
-#: kosmorrolib/main.py:172
+#: kosmorrolib/main.py:177
 msgid "The observer's longitude on Earth. Can also be set in the KOSMORRO_LONGITUDE environment variable."
 msgstr "Der Längengrad des Beobachters auf der Erde. Kann auch in der Umgebungsvariablen KOSMORRO_LONGITUDE gesetzt werden."
 
-#: kosmorrolib/main.py:180
+#: kosmorrolib/main.py:185
 msgid "The timezone to display the hours in (e.g. 2 for UTC+2 or -3 for UTC-3). Can also be set in the KOSMORRO_TIMEZONE environment variable."
 msgstr "Die Zeitzone, in der die Stunden angezeigt werden sollen (z.B. 2 für UTC+2 oder -3 für UTC-3). Kann auch in der Umgebungsvariablen KOSMORRO_TIMEZONE gesetzt werden."
 
-#: kosmorrolib/dumper.py:226
+#: kosmorrolib/dumper.py:223
 msgid "Don't forget to check the weather forecast before you go out with your equipment."
 msgstr "Vergessen Sie nicht, die Wettervorhersage zu prüfen, bevor Sie mit Ihrer Ausrüstung hinausfahren."
 
-#: kosmorrolib/core.py:117
+#: kosmorrolib/core.py:118
 msgid "The date {date} does not match the required YYYY-MM-DD format or the offset format."
 msgstr "Das Datum {date} entspricht nicht dem erforderlichen Format JJJJ-MM-TT oder dem Offset-Format."
 
-#: kosmorrolib/dumper.py:234
+#: kosmorrolib/dumper.py:231
 msgid "hours"
 msgstr "Uhr"
 
-#: kosmorrolib/main.py:175
+#: kosmorrolib/main.py:180
 msgid "The date for which the ephemerides must be computed (in the YYYY-MM-DD format), or as an interval in the \"[+-]YyMmDd\" format (with Y, M, and D numbers). Defaults to the current date ({default_date})"
 msgstr "Das Datum, für das die Ephemeriden berechnet werden müssen (im Format JJJJ-MM-TT), oder als Intervall im Format \"[+-]JyMmTd\" (wo J, M und T Zahlen sind). Standardwert ist das aktuelle Datum ({default_date})"
 
-#: kosmorrolib/main.py:188
+#: kosmorrolib/main.py:193
 msgid "Do not generate a graph to represent the rise and set times in the PDF format."
 msgstr "Keine Grafik zur Darstellung der Anstiegs- und Abfallzeiten im PDF-Format generieren"
 
 #: kosmorrolib/data.py:40
 msgid "Unavailable"
 msgstr "Nicht verfügbar"
 
@@ -272,11 +272,25 @@
 msgid "The date must be between {minimum_date} and {maximum_date}"
 msgstr "Das Datum muss zwischen dem {minimum_date} und dem {maximum_date} liegen"
 
 #: kosmorrolib/i18n.py:31
 msgid "{month} {day_number}, {year}"
 msgstr "{day_number}. {month} {year}"
 
-#: kosmorrolib/main.py:112
+#: kosmorrolib/main.py:117
 msgid "Moon phase can only be displayed between {min_date} and {max_date}"
 msgstr "Die Mondphase kann nur zwischen dem {min_date} und dem {max_date} angezeigt werden"
 
+#: kosmorrolib/dumper.py:380
+msgid "An error occured during the compilation of the PDF.\n"
+"Please open an issue at https://github.com/Kosmorro/kosmorro/issues and share the content of the log file at /tmp/kosmorro-%s.log"
+msgstr "Bei der Kompilierung der PDF ist ein Fehler aufgetreten.\n"
+"Bitte öffnen Sie ein Issue unter https://github.com/Kosmorro/kosmorro/issues und teilen Sie den Inhalt der Log-Datei unter /tmp/kosmorro-%s.log"
+
+#: kosmorrolib/enum.py:39
+msgid "%s is at its perigee"
+msgstr "%s befindet sich am Perigäum"
+
+#: kosmorrolib/enum.py:40
+msgid "%s is at its apogee"
+msgstr "%s steht auf seinem Apogäum"
+
```

### Comparing `kosmorro-0.8.1/kosmorrolib/locales/en/LC_MESSAGES/messages.mo` & `kosmorro-0.9.0/kosmorrolib/locales/en/LC_MESSAGES/messages.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,25 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  Kosmorro\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2020-06-07 09:19+0000\n"
+"POT-Creation-Date: 2021-01-31 09:20+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: en\n"
 "Language-Team: en <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.8.0\n"
+"Generated-By: Babel 2.9.0\n"
 
 msgid "%s and %s are in conjunction"
 msgstr "%s and %s are in conjunction"
 
+msgid "%s is at its apogee"
+msgstr "%s is at its apogee"
+
+msgid "%s is at its perigee"
+msgstr "%s is at its perigee"
+
 msgid "%s is in opposition"
 msgstr "%s is in opposition"
 
 msgid "%s occults %s"
 msgstr "%s occults %s"
 
 msgid "%s's largest elongation"
@@ -31,14 +37,23 @@
 msgid ""
 "A file to export the output to. If not given, the standard output is used. "
 "This argument is needed for PDF format."
 msgstr ""
 "A file to export the output to. If not given, the standard output is used. "
 "This argument is needed for PDF format."
 
+msgid ""
+"An error occured during the compilation of the PDF.\n"
+"Please open an issue at https://github.com/Kosmorro/kosmorro/issues and "
+"share the content of the log file at /tmp/kosmorro-%s.log"
+msgstr ""
+"An error occured during the compilation of the PDF.\n"
+"Please open an issue at https://github.com/Kosmorro/kosmorro/issues and "
+"share the content of the log file at /tmp/kosmorro-%s.log"
+
 msgid "Answer did not match expected options, cache not cleared."
 msgstr "Answer did not match expected options, cache not cleared."
 
 msgid ""
 "Building PDFs was not possible, because some dependencies are not "
 "installed.\n"
 "Please look at the documentation at http://kosmorro.space for more "
```

### Comparing `kosmorro-0.8.1/kosmorrolib/locales/en/LC_MESSAGES/messages.po` & `kosmorro-0.9.0/kosmorrolib/locales/en/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 "Project-Id-Version: Kosmorro\n"
 "Language: en\n"
 
 #: kosmorrolib/dumper.py:87
 msgid "Expected events:"
 msgstr "Expected events:"
 
-#: kosmorrolib/dumper.py:142 kosmorrolib/dumper.py:229
+#: kosmorrolib/dumper.py:142 kosmorrolib/dumper.py:226
 msgid "Object"
 msgstr "Object"
 
-#: kosmorrolib/dumper.py:143 kosmorrolib/dumper.py:230
+#: kosmorrolib/dumper.py:143 kosmorrolib/dumper.py:227
 msgid "Rise time"
 msgstr "Rise time"
 
-#: kosmorrolib/dumper.py:144 kosmorrolib/dumper.py:231
+#: kosmorrolib/dumper.py:144 kosmorrolib/dumper.py:228
 msgid "Culmination time"
 msgstr "Culmination time"
 
-#: kosmorrolib/dumper.py:145 kosmorrolib/dumper.py:232
+#: kosmorrolib/dumper.py:145 kosmorrolib/dumper.py:229
 msgid "Set time"
 msgstr "Set time"
 
 #: kosmorrolib/dumper.py:91
 msgid "Note: All the hours are given in UTC."
 msgstr "Note: All the hours are given in UTC."
 
@@ -39,149 +39,149 @@
 msgid "{hours}:{minutes}"
 msgstr "{hours}:{minutes}"
 
 #: kosmorrolib/dumper.py:163
 msgid "{next_moon_phase} on {next_moon_phase_date} at {next_moon_phase_time}"
 msgstr "{next_moon_phase} on {next_moon_phase_date} at {next_moon_phase_time}"
 
-#: kosmorrolib/data.py:262
+#: kosmorrolib/data.py:197
 msgid "Sun"
 msgstr "Sun"
 
-#: kosmorrolib/data.py:263
+#: kosmorrolib/data.py:198
 msgid "Moon"
 msgstr "Moon"
 
-#: kosmorrolib/data.py:264
+#: kosmorrolib/data.py:199
 msgid "Mercury"
 msgstr "Mercury"
 
-#: kosmorrolib/data.py:265
+#: kosmorrolib/data.py:200
 msgid "Venus"
 msgstr "Venus"
 
-#: kosmorrolib/data.py:266
+#: kosmorrolib/data.py:201
 msgid "Mars"
 msgstr "Mars"
 
-#: kosmorrolib/data.py:267
+#: kosmorrolib/data.py:202
 msgid "Jupiter"
 msgstr "Jupiter"
 
-#: kosmorrolib/data.py:268
+#: kosmorrolib/data.py:203
 msgid "Saturn"
 msgstr "Saturn"
 
-#: kosmorrolib/data.py:269
+#: kosmorrolib/data.py:204
 msgid "Uranus"
 msgstr "Uranus"
 
-#: kosmorrolib/data.py:270
+#: kosmorrolib/data.py:205
 msgid "Neptune"
 msgstr "Neptune"
 
-#: kosmorrolib/data.py:271
+#: kosmorrolib/data.py:206
 msgid "Pluto"
 msgstr "Pluto"
 
-#: kosmorrolib/data.py:32
+#: kosmorrolib/enum.py:24
 msgid "New Moon"
 msgstr "New Moon"
 
-#: kosmorrolib/data.py:33
+#: kosmorrolib/enum.py:25
 msgid "Waxing crescent"
 msgstr "Waxing crescent"
 
-#: kosmorrolib/data.py:34
+#: kosmorrolib/enum.py:26
 msgid "First Quarter"
 msgstr "First Quarter"
 
-#: kosmorrolib/data.py:35
+#: kosmorrolib/enum.py:27
 msgid "Waxing gibbous"
 msgstr "Waxing gibbous"
 
-#: kosmorrolib/data.py:36
+#: kosmorrolib/enum.py:28
 msgid "Full Moon"
 msgstr "Full Moon"
 
-#: kosmorrolib/data.py:37
+#: kosmorrolib/enum.py:29
 msgid "Waning gibbous"
 msgstr "Waning gibbous"
 
-#: kosmorrolib/data.py:38
+#: kosmorrolib/enum.py:30
 msgid "Last Quarter"
 msgstr "Last Quarter"
 
-#: kosmorrolib/data.py:39
+#: kosmorrolib/enum.py:31
 msgid "Waning crescent"
 msgstr "Waning crescent"
 
-#: kosmorrolib/data.py:44
+#: kosmorrolib/enum.py:35
 msgid "%s is in opposition"
 msgstr "%s is in opposition"
 
-#: kosmorrolib/data.py:45
+#: kosmorrolib/enum.py:36
 msgid "%s and %s are in conjunction"
 msgstr "%s and %s are in conjunction"
 
-#: kosmorrolib/main.py:134
+#: kosmorrolib/main.py:139
 msgid "Running on Python {python_version}"
 msgstr "Running on Python {python_version}"
 
-#: kosmorrolib/main.py:140
+#: kosmorrolib/main.py:145
 msgid "Do you really want to clear Kosmorro's cache? [yN] "
 msgstr "Do you really want to clear Kosmorro's cache? [yN] "
 
-#: kosmorrolib/main.py:147
+#: kosmorrolib/main.py:152
 msgid "Answer did not match expected options, cache not cleared."
 msgstr "Answer did not match expected options, cache not cleared."
 
-#: kosmorrolib/main.py:156
+#: kosmorrolib/main.py:161
 msgid "Compute the ephemerides and the events for a given date, at a given position on Earth."
 msgstr "Compute the ephemerides and the events for a given date, at a given position on Earth."
 
-#: kosmorrolib/main.py:158
+#: kosmorrolib/main.py:163
 msgid "By default, only the events will be computed for today ({date}).\n"
 "To compute also the ephemerides, latitude and longitude arguments are needed."
 msgstr "By default, only the events will be computed for today ({date}).\n"
 "To compute also the ephemerides, latitude and longitude arguments are needed."
 
-#: kosmorrolib/main.py:163
+#: kosmorrolib/main.py:168
 msgid "Show the program version"
 msgstr "Show the program version"
 
-#: kosmorrolib/main.py:165
+#: kosmorrolib/main.py:170
 msgid "Delete all the files Kosmorro stored in the cache."
 msgstr "Delete all the files Kosmorro stored in the cache."
 
-#: kosmorrolib/main.py:167
+#: kosmorrolib/main.py:172
 msgid "The format under which the information have to be output"
 msgstr "The format under which the information have to be output"
 
-#: kosmorrolib/dumper.py:162 kosmorrolib/dumper.py:236
+#: kosmorrolib/dumper.py:162 kosmorrolib/dumper.py:233
 msgid "Moon phase:"
 msgstr "Moon phase:"
 
-#: kosmorrolib/main.py:183
+#: kosmorrolib/main.py:188
 msgid "Disable the colors in the console."
 msgstr "Disable the colors in the console."
 
-#: kosmorrolib/dumper.py:216
+#: kosmorrolib/dumper.py:213
 msgid "A Summary of your Sky"
 msgstr "A Summary of your Sky"
 
-#: kosmorrolib/dumper.py:228
+#: kosmorrolib/dumper.py:225
 msgid "Ephemerides of the day"
 msgstr "Ephemerides of the day"
 
-#: kosmorrolib/dumper.py:238
+#: kosmorrolib/dumper.py:235
 msgid "Expected events"
 msgstr "Expected events"
 
-#: kosmorrolib/dumper.py:352
+#: kosmorrolib/dumper.py:351
 msgid "Building PDFs was not possible, because some dependencies are not installed.\n"
 "Please look at the documentation at http://kosmorro.space for more information."
 msgstr "Building PDFs was not possible, because some dependencies are not installed.\n"
 "Please look at the documentation at http://kosmorro.space for more information."
 
 #: kosmorrolib/main.py:61
 msgid "Save the planet and paper!\n"
@@ -189,79 +189,79 @@
 msgstr "Save the planet and paper!\n"
 "Consider printing you PDF document only if really necessary, and use the other side of the sheet."
 
 #: kosmorrolib/main.py:65
 msgid "PDF output will not contain the ephemerides, because you didn't provide the observation coordinate."
 msgstr "PDF output will not contain the ephemerides, because you didn't provide the observation coordinate."
 
-#: kosmorrolib/main.py:90
+#: kosmorrolib/main.py:93
 msgid "Could not save the output in \"{path}\": {error}"
 msgstr "Could not save the output in \"{path}\": {error}"
 
-#: kosmorrolib/main.py:95
+#: kosmorrolib/main.py:100
 msgid "Selected output format needs an output file (--output)."
 msgstr "Selected output format needs an output file (--output)."
 
-#: kosmorrolib/main.py:185
+#: kosmorrolib/main.py:190
 msgid "A file to export the output to. If not given, the standard output is used. This argument is needed for PDF format."
 msgstr "A file to export the output to. If not given, the standard output is used. This argument is needed for PDF format."
 
 #: kosmorrolib/i18n.py:29
 msgid "{month} {day_number}, {hours}:{minutes}"
 msgstr "{month} {day_number}, {hours}:{minutes}"
 
 #: kosmorrolib/dumper.py:96
 msgid "Note: All the hours are given in the UTC{offset} timezone."
 msgstr "Note: All the hours are given in the UTC{offset} timezone."
 
-#: kosmorrolib/dumper.py:220
+#: kosmorrolib/dumper.py:217
 msgid "This document summarizes the ephemerides and the events of {date}. It aims to help you to prepare your observation session. All the hours are given in {timezone}."
 msgstr "This document summarizes the ephemerides and the events of {date}. It aims to help you to prepare your observation session. All the hours are given in {timezone}."
 
-#: kosmorrolib/data.py:47
+#: kosmorrolib/enum.py:38
 msgid "%s's largest elongation"
 msgstr "%s's largest elongation"
 
-#: kosmorrolib/data.py:46
+#: kosmorrolib/enum.py:37
 msgid "%s occults %s"
 msgstr "%s occults %s"
 
 #: kosmorrolib/core.py:101
 msgid "The date {date} is not valid: {error}"
 msgstr "The date {date} is not valid: {error}"
 
-#: kosmorrolib/main.py:169
+#: kosmorrolib/main.py:174
 msgid "The observer's latitude on Earth. Can also be set in the KOSMORRO_LATITUDE environment variable."
 msgstr "The observer's latitude on Earth. Can also be set in the KOSMORRO_LATITUDE environment variable."
 
-#: kosmorrolib/main.py:172
+#: kosmorrolib/main.py:177
 msgid "The observer's longitude on Earth. Can also be set in the KOSMORRO_LONGITUDE environment variable."
 msgstr "The observer's longitude on Earth. Can also be set in the KOSMORRO_LONGITUDE environment variable."
 
-#: kosmorrolib/main.py:180
+#: kosmorrolib/main.py:185
 msgid "The timezone to display the hours in (e.g. 2 for UTC+2 or -3 for UTC-3). Can also be set in the KOSMORRO_TIMEZONE environment variable."
 msgstr "The timezone to display the hours in (e.g. 2 for UTC+2 or -3 for UTC-3). Can also be set in the KOSMORRO_TIMEZONE environment variable."
 
-#: kosmorrolib/dumper.py:226
+#: kosmorrolib/dumper.py:223
 msgid "Don't forget to check the weather forecast before you go out with your equipment."
 msgstr "Don't forget to check the weather forecast before you go out with your equipment."
 
-#: kosmorrolib/core.py:117
+#: kosmorrolib/core.py:118
 msgid "The date {date} does not match the required YYYY-MM-DD format or the offset format."
 msgstr "The date {date} does not match the required YYYY-MM-DD format or the offset format."
 
-#: kosmorrolib/dumper.py:234
+#: kosmorrolib/dumper.py:231
 msgid "hours"
 msgstr "hours"
 
-#: kosmorrolib/main.py:175
+#: kosmorrolib/main.py:180
 msgid "The date for which the ephemerides must be computed (in the YYYY-MM-DD format), or as an interval in the \"[+-]YyMmDd\" format (with Y, M, and D numbers). Defaults to the current date ({default_date})"
 msgstr "The date for which the ephemerides must be computed (in the YYYY-MM-DD format), or as an interval in the \"[+-]YyMmDd\" format (with Y, M, and D numbers). Defaults to the current date ({default_date})"
 
-#: kosmorrolib/main.py:188
+#: kosmorrolib/main.py:193
 msgid "Do not generate a graph to represent the rise and set times in the PDF format."
 msgstr "Do not generate a graph to represent the rise and set times in the PDF format."
 
 #: kosmorrolib/data.py:40
 msgid "Unavailable"
 msgstr "Unavailable"
 
@@ -273,11 +273,25 @@
 msgid "The date must be between {minimum_date} and {maximum_date}"
 msgstr "The date must be between {minimum_date} and {maximum_date}"
 
 #: kosmorrolib/i18n.py:31
 msgid "{month} {day_number}, {year}"
 msgstr "{month} {day_number}, {year}"
 
-#: kosmorrolib/main.py:112
+#: kosmorrolib/main.py:117
 msgid "Moon phase can only be displayed between {min_date} and {max_date}"
 msgstr "Moon phase can only be displayed between {min_date} and {max_date}"
 
+#: kosmorrolib/dumper.py:380
+msgid "An error occured during the compilation of the PDF.\n"
+"Please open an issue at https://github.com/Kosmorro/kosmorro/issues and share the content of the log file at /tmp/kosmorro-%s.log"
+msgstr "An error occured during the compilation of the PDF.\n"
+"Please open an issue at https://github.com/Kosmorro/kosmorro/issues and share the content of the log file at /tmp/kosmorro-%s.log"
+
+#: kosmorrolib/enum.py:39
+msgid "%s is at its perigee"
+msgstr "%s is at its perigee"
+
+#: kosmorrolib/enum.py:40
+msgid "%s is at its apogee"
+msgstr "%s is at its apogee"
+
```

### Comparing `kosmorro-0.8.1/kosmorrolib/locales/fr/LC_MESSAGES/messages.mo` & `kosmorro-0.9.0/kosmorrolib/locales/fr/LC_MESSAGES/messages.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,25 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  Kosmorro\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2020-06-07 09:19+0000\n"
+"POT-Creation-Date: 2021-01-31 09:20+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.8.0\n"
+"Generated-By: Babel 2.9.0\n"
 
 msgid "%s and %s are in conjunction"
 msgstr "%s et %s sont en conjonction"
 
+msgid "%s is at its apogee"
+msgstr "%s est à son apogée"
+
+msgid "%s is at its perigee"
+msgstr "%s est à son périgée"
+
 msgid "%s is in opposition"
 msgstr "%s est à l'opposition"
 
 msgid "%s occults %s"
 msgstr "%s occulte %s"
 
 msgid "%s's largest elongation"
@@ -32,14 +38,23 @@
 "A file to export the output to. If not given, the standard output is used. "
 "This argument is needed for PDF format."
 msgstr ""
 "Un fichier dans lequel la sortie doit être enregistré. S'il n'est pas donné, "
 "la sortie standard de la console est utilisée. Cet argument est nécessaire "
 "pour le format de sortie PDF."
 
+msgid ""
+"An error occured during the compilation of the PDF.\n"
+"Please open an issue at https://github.com/Kosmorro/kosmorro/issues and "
+"share the content of the log file at /tmp/kosmorro-%s.log"
+msgstr ""
+"Une erreur s'est produite pendant la compilation du PDF.\n"
+"Merci d'ouvrir un ticket sur https://github.com/Kosmorro/kosmorro/issues et "
+"de partager le contenu du fichier journal situé dans /tmp/kosmorro-%s.log"
+
 msgid "Answer did not match expected options, cache not cleared."
 msgstr "Réponse erronée, le cache n'a pas été effacé."
 
 msgid ""
 "Building PDFs was not possible, because some dependencies are not "
 "installed.\n"
 "Please look at the documentation at http://kosmorro.space for more "
```

### Comparing `kosmorro-0.8.1/kosmorrolib/locales/fr/LC_MESSAGES/messages.po` & `kosmorro-0.9.0/kosmorrolib/locales/fr/LC_MESSAGES/messages.po`

 * *Files 5% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 "Project-Id-Version: Kosmorro\n"
 "Language: fr\n"
 
 #: kosmorrolib/dumper.py:87
 msgid "Expected events:"
 msgstr "Événements prévus :"
 
-#: kosmorrolib/dumper.py:142 kosmorrolib/dumper.py:229
+#: kosmorrolib/dumper.py:142 kosmorrolib/dumper.py:226
 msgid "Object"
 msgstr "Objet"
 
-#: kosmorrolib/dumper.py:143 kosmorrolib/dumper.py:230
+#: kosmorrolib/dumper.py:143 kosmorrolib/dumper.py:227
 msgid "Rise time"
 msgstr "Heure de lever"
 
-#: kosmorrolib/dumper.py:144 kosmorrolib/dumper.py:231
+#: kosmorrolib/dumper.py:144 kosmorrolib/dumper.py:228
 msgid "Culmination time"
 msgstr "Heure de culmination"
 
-#: kosmorrolib/dumper.py:145 kosmorrolib/dumper.py:232
+#: kosmorrolib/dumper.py:145 kosmorrolib/dumper.py:229
 msgid "Set time"
 msgstr "Heure de coucher"
 
 #: kosmorrolib/dumper.py:91
 msgid "Note: All the hours are given in UTC."
 msgstr "Note : toutes les heures sont en temps universel (UTC)."
 
@@ -39,148 +39,148 @@
 msgid "{hours}:{minutes}"
 msgstr "{hours}h{minutes}"
 
 #: kosmorrolib/dumper.py:163
 msgid "{next_moon_phase} on {next_moon_phase_date} at {next_moon_phase_time}"
 msgstr "{next_moon_phase} le {next_moon_phase_date} à {next_moon_phase_time}"
 
-#: kosmorrolib/data.py:262
+#: kosmorrolib/data.py:197
 msgid "Sun"
 msgstr "Soleil"
 
-#: kosmorrolib/data.py:263
+#: kosmorrolib/data.py:198
 msgid "Moon"
 msgstr "Lune"
 
-#: kosmorrolib/data.py:264
+#: kosmorrolib/data.py:199
 msgid "Mercury"
 msgstr "Mercure"
 
-#: kosmorrolib/data.py:265
+#: kosmorrolib/data.py:200
 msgid "Venus"
 msgstr "Vénus"
 
-#: kosmorrolib/data.py:266
+#: kosmorrolib/data.py:201
 msgid "Mars"
 msgstr "Mars"
 
-#: kosmorrolib/data.py:267
+#: kosmorrolib/data.py:202
 msgid "Jupiter"
 msgstr "Jupiter"
 
-#: kosmorrolib/data.py:268
+#: kosmorrolib/data.py:203
 msgid "Saturn"
 msgstr "Saturne"
 
-#: kosmorrolib/data.py:269
+#: kosmorrolib/data.py:204
 msgid "Uranus"
 msgstr "Uranus"
 
-#: kosmorrolib/data.py:270
+#: kosmorrolib/data.py:205
 msgid "Neptune"
 msgstr "Neptune"
 
-#: kosmorrolib/data.py:271
+#: kosmorrolib/data.py:206
 msgid "Pluto"
 msgstr "Pluton"
 
-#: kosmorrolib/data.py:32
+#: kosmorrolib/enum.py:24
 msgid "New Moon"
 msgstr "Nouvelle lune"
 
-#: kosmorrolib/data.py:33
+#: kosmorrolib/enum.py:25
 msgid "Waxing crescent"
 msgstr "Premier croissant"
 
-#: kosmorrolib/data.py:34
+#: kosmorrolib/enum.py:26
 msgid "First Quarter"
 msgstr "Premier quartier"
 
-#: kosmorrolib/data.py:35
+#: kosmorrolib/enum.py:27
 msgid "Waxing gibbous"
 msgstr "Gibbeuse croissante"
 
-#: kosmorrolib/data.py:36
+#: kosmorrolib/enum.py:28
 msgid "Full Moon"
 msgstr "Pleine lune"
 
-#: kosmorrolib/data.py:37
+#: kosmorrolib/enum.py:29
 msgid "Waning gibbous"
 msgstr "Gibbeuse décroissante"
 
-#: kosmorrolib/data.py:38
+#: kosmorrolib/enum.py:30
 msgid "Last Quarter"
 msgstr "Dernier quartier"
 
-#: kosmorrolib/data.py:39
+#: kosmorrolib/enum.py:31
 msgid "Waning crescent"
 msgstr "Dernier croissant"
 
-#: kosmorrolib/data.py:44
+#: kosmorrolib/enum.py:35
 msgid "%s is in opposition"
 msgstr "%s est à l'opposition"
 
-#: kosmorrolib/data.py:45
+#: kosmorrolib/enum.py:36
 msgid "%s and %s are in conjunction"
 msgstr "%s et %s sont en conjonction"
 
-#: kosmorrolib/main.py:134
+#: kosmorrolib/main.py:139
 msgid "Running on Python {python_version}"
 msgstr "Exécuté à l'aide de Python {python_version}"
 
-#: kosmorrolib/main.py:140
+#: kosmorrolib/main.py:145
 msgid "Do you really want to clear Kosmorro's cache? [yN] "
 msgstr "Voulez-vous vraiment effacer le cache de Kosmorro ? [oN]"
 
-#: kosmorrolib/main.py:147
+#: kosmorrolib/main.py:152
 msgid "Answer did not match expected options, cache not cleared."
 msgstr "Réponse erronée, le cache n'a pas été effacé."
 
-#: kosmorrolib/main.py:156
+#: kosmorrolib/main.py:161
 msgid "Compute the ephemerides and the events for a given date, at a given position on Earth."
 msgstr "Calcule les éphémérides et les événements pour une date et une position sur Terre données."
 
-#: kosmorrolib/main.py:158
+#: kosmorrolib/main.py:163
 msgid "By default, only the events will be computed for today ({date}).\n"
 "To compute also the ephemerides, latitude and longitude arguments are needed."
 msgstr "Par défaut, seuls les événements sont calculés pour la date actuelle ({date}). Pour calculer les éphémérides, la latitude et la longitude sont requis."
 
-#: kosmorrolib/main.py:163
+#: kosmorrolib/main.py:168
 msgid "Show the program version"
 msgstr "Affiche la version du programme"
 
-#: kosmorrolib/main.py:165
+#: kosmorrolib/main.py:170
 msgid "Delete all the files Kosmorro stored in the cache."
 msgstr "Efface tous les fichiers du cache de Kosmorro"
 
-#: kosmorrolib/main.py:167
+#: kosmorrolib/main.py:172
 msgid "The format under which the information have to be output"
 msgstr "Le format de sortie des informations"
 
-#: kosmorrolib/dumper.py:162 kosmorrolib/dumper.py:236
+#: kosmorrolib/dumper.py:162 kosmorrolib/dumper.py:233
 msgid "Moon phase:"
 msgstr "Phase de la Lune :"
 
-#: kosmorrolib/main.py:183
+#: kosmorrolib/main.py:188
 msgid "Disable the colors in the console."
 msgstr "Désactive les couleurs dans la console."
 
-#: kosmorrolib/dumper.py:216
+#: kosmorrolib/dumper.py:213
 msgid "A Summary of your Sky"
 msgstr "Synthèse de votre ciel"
 
-#: kosmorrolib/dumper.py:228
+#: kosmorrolib/dumper.py:225
 msgid "Ephemerides of the day"
 msgstr "Éphémérides du jour"
 
-#: kosmorrolib/dumper.py:238
+#: kosmorrolib/dumper.py:235
 msgid "Expected events"
 msgstr "Événements prévus"
 
-#: kosmorrolib/dumper.py:352
+#: kosmorrolib/dumper.py:351
 msgid "Building PDFs was not possible, because some dependencies are not installed.\n"
 "Please look at the documentation at http://kosmorro.space for more information."
 msgstr "La génération du document PDF n'est pas possible, car certaines dépendances ne sont pas installées.\n"
 "Veuillez vous référer à la documentation sur http://kosmorro.space pour de plus amples informations."
 
 #: kosmorrolib/main.py:61
 msgid "Save the planet and paper!\n"
@@ -188,79 +188,79 @@
 msgstr "Sauvez la planète, économisez du papier !\n"
 "N'imprimez le document PDF uniquement si nécessaire, et pensez à utiliser le verso de la feuille."
 
 #: kosmorrolib/main.py:65
 msgid "PDF output will not contain the ephemerides, because you didn't provide the observation coordinate."
 msgstr "Le document PDF ne contiendra pas les éphémérides, car les coordonnées du lieu d'observation sont manquantes."
 
-#: kosmorrolib/main.py:90
+#: kosmorrolib/main.py:93
 msgid "Could not save the output in \"{path}\": {error}"
 msgstr "Impossible d'enregistrer le fichier \"{path}\" : {error}"
 
-#: kosmorrolib/main.py:95
+#: kosmorrolib/main.py:100
 msgid "Selected output format needs an output file (--output)."
 msgstr "Le format de sortie choisi requiert un fichier de sortie (--output)."
 
-#: kosmorrolib/main.py:185
+#: kosmorrolib/main.py:190
 msgid "A file to export the output to. If not given, the standard output is used. This argument is needed for PDF format."
 msgstr "Un fichier dans lequel la sortie doit être enregistré. S'il n'est pas donné, la sortie standard de la console est utilisée. Cet argument est nécessaire pour le format de sortie PDF."
 
 #: kosmorrolib/i18n.py:29
 msgid "{month} {day_number}, {hours}:{minutes}"
 msgstr "{day_number} {month}, {hours}:{minutes}"
 
 #: kosmorrolib/dumper.py:96
 msgid "Note: All the hours are given in the UTC{offset} timezone."
 msgstr "Note : toutes les heures sont données dans le fuseau horaire UTC{offset}."
 
-#: kosmorrolib/dumper.py:220
+#: kosmorrolib/dumper.py:217
 msgid "This document summarizes the ephemerides and the events of {date}. It aims to help you to prepare your observation session. All the hours are given in {timezone}."
 msgstr "Ce document synthétise les éphémérides et les événements prévus pour le {date}. Son but est de vous aider à préparer votre soirée d'observation. Toutes les heures sont données en {timezone}."
 
-#: kosmorrolib/data.py:47
+#: kosmorrolib/enum.py:38
 msgid "%s's largest elongation"
 msgstr "L'élongation de %s est à son maximum"
 
-#: kosmorrolib/data.py:46
+#: kosmorrolib/enum.py:37
 msgid "%s occults %s"
 msgstr "%s occulte %s"
 
 #: kosmorrolib/core.py:101
 msgid "The date {date} is not valid: {error}"
 msgstr "La date {date} n'est pas valide : {error}"
 
-#: kosmorrolib/main.py:169
+#: kosmorrolib/main.py:174
 msgid "The observer's latitude on Earth. Can also be set in the KOSMORRO_LATITUDE environment variable."
 msgstr "La latitude de l'observateur. Peut également être renseignée dans la variable d'environnement KOSMORRO_LATITUDE."
 
-#: kosmorrolib/main.py:172
+#: kosmorrolib/main.py:177
 msgid "The observer's longitude on Earth. Can also be set in the KOSMORRO_LONGITUDE environment variable."
 msgstr "La longitude de l'observateur. Peut également être renseignée dans la variable d'environnement KOSMORRO_LONGITUDE."
 
-#: kosmorrolib/main.py:180
+#: kosmorrolib/main.py:185
 msgid "The timezone to display the hours in (e.g. 2 for UTC+2 or -3 for UTC-3). Can also be set in the KOSMORRO_TIMEZONE environment variable."
 msgstr "Le fuseau horaire dans lequel les heures doivent être données (par exemple 2 pour UTC+2 ou -3 pour UTC-3). Peut également être renseigné dans la variable d'environnement KOSMORRO_TIMEZONE."
 
-#: kosmorrolib/dumper.py:226
+#: kosmorrolib/dumper.py:223
 msgid "Don't forget to check the weather forecast before you go out with your equipment."
 msgstr "N’oubliez pas de vous assurer que les conditions météo sont favorables avant de sortir votre matériel d’observation."
 
-#: kosmorrolib/core.py:117
+#: kosmorrolib/core.py:118
 msgid "The date {date} does not match the required YYYY-MM-DD format or the offset format."
 msgstr "La date {date} ne répond pas au format YYYY-MM-DD ou au format relatif."
 
-#: kosmorrolib/dumper.py:234
+#: kosmorrolib/dumper.py:231
 msgid "hours"
 msgstr "heures"
 
-#: kosmorrolib/main.py:175
+#: kosmorrolib/main.py:180
 msgid "The date for which the ephemerides must be computed (in the YYYY-MM-DD format), or as an interval in the \"[+-]YyMmDd\" format (with Y, M, and D numbers). Defaults to the current date ({default_date})"
 msgstr "La date pour laquelle les éphémérides doivent être calculées (au format AAAA-MM-JJ), ou comme un intervalle au format \"[+-]Ay-Mm-Jd\" (où A, M, et J sont des nombres). Par défaut, la date du jour ({default_date}) est utilisée."
 
-#: kosmorrolib/main.py:188
+#: kosmorrolib/main.py:193
 msgid "Do not generate a graph to represent the rise and set times in the PDF format."
 msgstr "Désactive la génération du graphique des levers et couchers des astres dans le format PDF."
 
 #: kosmorrolib/data.py:40
 msgid "Unavailable"
 msgstr "Information non disponible"
 
@@ -272,11 +272,25 @@
 msgid "The date must be between {minimum_date} and {maximum_date}"
 msgstr "La date doit être entre le {minimum_date} et le {maximum_date}"
 
 #: kosmorrolib/i18n.py:31
 msgid "{month} {day_number}, {year}"
 msgstr "{day_number} {month} {year}"
 
-#: kosmorrolib/main.py:112
+#: kosmorrolib/main.py:117
 msgid "Moon phase can only be displayed between {min_date} and {max_date}"
 msgstr "La phase de la Lune ne peut être affichée qu'entre le {min_date} et le {max_date}"
 
+#: kosmorrolib/dumper.py:380
+msgid "An error occured during the compilation of the PDF.\n"
+"Please open an issue at https://github.com/Kosmorro/kosmorro/issues and share the content of the log file at /tmp/kosmorro-%s.log"
+msgstr "Une erreur s'est produite pendant la compilation du PDF.\n"
+"Merci d'ouvrir un ticket sur https://github.com/Kosmorro/kosmorro/issues et de partager le contenu du fichier journal situé dans /tmp/kosmorro-%s.log"
+
+#: kosmorrolib/enum.py:39
+msgid "%s is at its perigee"
+msgstr "%s est à son périgée"
+
+#: kosmorrolib/enum.py:40
+msgid "%s is at its apogee"
+msgstr "%s est à son apogée"
+
```

### Comparing `kosmorro-0.8.1/kosmorrolib/locales/messages.pot` & `kosmorro-0.9.0/kosmorrolib/locales/messages.pot`

 * *Files 8% similar despite different names*

```diff
@@ -1,129 +1,73 @@
 # Translations template for kosmorro.
-# Copyright (C) 2020 ORGANIZATION
+# Copyright (C) 2021 ORGANIZATION
 # This file is distributed under the same license as the kosmorro project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2020.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2021.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: kosmorro 0.8.1\n"
+"Project-Id-Version: kosmorro 0.9.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2020-06-07 11:13+0200\n"
+"POT-Creation-Date: 2021-01-31 10:15+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.8.0\n"
+"Generated-By: Babel 2.9.0\n"
 
 #: kosmorrolib/core.py:101
 msgid "The date {date} is not valid: {error}"
 msgstr ""
 
-#: kosmorrolib/core.py:117
+#: kosmorrolib/core.py:118
 msgid ""
 "The date {date} does not match the required YYYY-MM-DD format or the "
 "offset format."
 msgstr ""
 
-#: kosmorrolib/data.py:32
-msgid "New Moon"
-msgstr ""
-
-#: kosmorrolib/data.py:33
-msgid "Waxing crescent"
-msgstr ""
-
-#: kosmorrolib/data.py:34
-msgid "First Quarter"
-msgstr ""
-
-#: kosmorrolib/data.py:35
-msgid "Waxing gibbous"
-msgstr ""
-
-#: kosmorrolib/data.py:36
-msgid "Full Moon"
-msgstr ""
-
-#: kosmorrolib/data.py:37
-msgid "Waning gibbous"
-msgstr ""
-
-#: kosmorrolib/data.py:38
-msgid "Last Quarter"
-msgstr ""
-
-#: kosmorrolib/data.py:39
-msgid "Waning crescent"
-msgstr ""
-
-#: kosmorrolib/data.py:40
-msgid "Unavailable"
-msgstr ""
-
-#: kosmorrolib/data.py:44
-#, python-format
-msgid "%s is in opposition"
-msgstr ""
-
-#: kosmorrolib/data.py:45
-#, python-format
-msgid "%s and %s are in conjunction"
-msgstr ""
-
-#: kosmorrolib/data.py:46
-#, python-format
-msgid "%s occults %s"
-msgstr ""
-
-#: kosmorrolib/data.py:47
-#, python-format
-msgid "%s's largest elongation"
-msgstr ""
-
-#: kosmorrolib/data.py:262
+#: kosmorrolib/data.py:197
 msgid "Sun"
 msgstr ""
 
-#: kosmorrolib/data.py:263
+#: kosmorrolib/data.py:198
 msgid "Moon"
 msgstr ""
 
-#: kosmorrolib/data.py:264
+#: kosmorrolib/data.py:199
 msgid "Mercury"
 msgstr ""
 
-#: kosmorrolib/data.py:265
+#: kosmorrolib/data.py:200
 msgid "Venus"
 msgstr ""
 
-#: kosmorrolib/data.py:266
+#: kosmorrolib/data.py:201
 msgid "Mars"
 msgstr ""
 
-#: kosmorrolib/data.py:267
+#: kosmorrolib/data.py:202
 msgid "Jupiter"
 msgstr ""
 
-#: kosmorrolib/data.py:268
+#: kosmorrolib/data.py:203
 msgid "Saturn"
 msgstr ""
 
-#: kosmorrolib/data.py:269
+#: kosmorrolib/data.py:204
 msgid "Uranus"
 msgstr ""
 
-#: kosmorrolib/data.py:270
+#: kosmorrolib/data.py:205
 msgid "Neptune"
 msgstr ""
 
-#: kosmorrolib/data.py:271
+#: kosmorrolib/data.py:206
 msgid "Pluto"
 msgstr ""
 
 #: kosmorrolib/dumper.py:87
 msgid "Expected events:"
 msgstr ""
 
@@ -131,79 +75,149 @@
 msgid "Note: All the hours are given in UTC."
 msgstr ""
 
 #: kosmorrolib/dumper.py:96
 msgid "Note: All the hours are given in the UTC{offset} timezone."
 msgstr ""
 
-#: kosmorrolib/dumper.py:142 kosmorrolib/dumper.py:229
+#: kosmorrolib/dumper.py:142 kosmorrolib/dumper.py:226
 msgid "Object"
 msgstr ""
 
-#: kosmorrolib/dumper.py:143 kosmorrolib/dumper.py:230
+#: kosmorrolib/dumper.py:143 kosmorrolib/dumper.py:227
 msgid "Rise time"
 msgstr ""
 
-#: kosmorrolib/dumper.py:144 kosmorrolib/dumper.py:231
+#: kosmorrolib/dumper.py:144 kosmorrolib/dumper.py:228
 msgid "Culmination time"
 msgstr ""
 
-#: kosmorrolib/dumper.py:145 kosmorrolib/dumper.py:232
+#: kosmorrolib/dumper.py:145 kosmorrolib/dumper.py:229
 msgid "Set time"
 msgstr ""
 
 #: kosmorrolib/dumper.py:160
 msgid "Moon phase is unavailable for this date."
 msgstr ""
 
-#: kosmorrolib/dumper.py:162 kosmorrolib/dumper.py:236
+#: kosmorrolib/dumper.py:162 kosmorrolib/dumper.py:233
 msgid "Moon phase:"
 msgstr ""
 
 #: kosmorrolib/dumper.py:163
 msgid "{next_moon_phase} on {next_moon_phase_date} at {next_moon_phase_time}"
 msgstr ""
 
-#: kosmorrolib/dumper.py:216
+#: kosmorrolib/dumper.py:213
 msgid "A Summary of your Sky"
 msgstr ""
 
-#: kosmorrolib/dumper.py:220
+#: kosmorrolib/dumper.py:217
 msgid ""
 "This document summarizes the ephemerides and the events of {date}. It "
 "aims to help you to prepare your observation session. All the hours are "
 "given in {timezone}."
 msgstr ""
 
-#: kosmorrolib/dumper.py:226
+#: kosmorrolib/dumper.py:223
 msgid ""
 "Don't forget to check the weather forecast before you go out with your "
 "equipment."
 msgstr ""
 
-#: kosmorrolib/dumper.py:228
+#: kosmorrolib/dumper.py:225
 msgid "Ephemerides of the day"
 msgstr ""
 
-#: kosmorrolib/dumper.py:234
+#: kosmorrolib/dumper.py:231
 msgid "hours"
 msgstr ""
 
-#: kosmorrolib/dumper.py:238
+#: kosmorrolib/dumper.py:235
 msgid "Expected events"
 msgstr ""
 
-#: kosmorrolib/dumper.py:352
+#: kosmorrolib/dumper.py:351
 msgid ""
 "Building PDFs was not possible, because some dependencies are not "
 "installed.\n"
 "Please look at the documentation at http://kosmorro.space for more "
 "information."
 msgstr ""
 
+#: kosmorrolib/dumper.py:380
+#, python-format
+msgid ""
+"An error occured during the compilation of the PDF.\n"
+"Please open an issue at https://github.com/Kosmorro/kosmorro/issues and "
+"share the content of the log file at /tmp/kosmorro-%s.log"
+msgstr ""
+
+#: kosmorrolib/enum.py:24
+msgid "New Moon"
+msgstr ""
+
+#: kosmorrolib/enum.py:25
+msgid "Waxing crescent"
+msgstr ""
+
+#: kosmorrolib/enum.py:26
+msgid "First Quarter"
+msgstr ""
+
+#: kosmorrolib/enum.py:27
+msgid "Waxing gibbous"
+msgstr ""
+
+#: kosmorrolib/enum.py:28
+msgid "Full Moon"
+msgstr ""
+
+#: kosmorrolib/enum.py:29
+msgid "Waning gibbous"
+msgstr ""
+
+#: kosmorrolib/enum.py:30
+msgid "Last Quarter"
+msgstr ""
+
+#: kosmorrolib/enum.py:31
+msgid "Waning crescent"
+msgstr ""
+
+#: kosmorrolib/enum.py:35
+#, python-format
+msgid "%s is in opposition"
+msgstr ""
+
+#: kosmorrolib/enum.py:36
+#, python-format
+msgid "%s and %s are in conjunction"
+msgstr ""
+
+#: kosmorrolib/enum.py:37
+#, python-format
+msgid "%s occults %s"
+msgstr ""
+
+#: kosmorrolib/enum.py:38
+#, python-format
+msgid "%s's largest elongation"
+msgstr ""
+
+#: kosmorrolib/enum.py:39
+#, python-format
+msgid "%s is at its perigee"
+msgstr ""
+
+#: kosmorrolib/enum.py:40
+#, python-format
+msgid "%s is at its apogee"
+msgstr ""
+
 #: kosmorrolib/exceptions.py:34
 msgid "The date must be between {minimum_date} and {maximum_date}"
 msgstr ""
 
 #: kosmorrolib/i18n.py:27
 msgid "{day_of_week} {month} {day_number}, {year}"
 msgstr ""
@@ -229,97 +243,97 @@
 
 #: kosmorrolib/main.py:65
 msgid ""
 "PDF output will not contain the ephemerides, because you didn't provide "
 "the observation coordinate."
 msgstr ""
 
-#: kosmorrolib/main.py:90
+#: kosmorrolib/main.py:93
 msgid "Could not save the output in \"{path}\": {error}"
 msgstr ""
 
-#: kosmorrolib/main.py:95
+#: kosmorrolib/main.py:100
 msgid "Selected output format needs an output file (--output)."
 msgstr ""
 
-#: kosmorrolib/main.py:112
+#: kosmorrolib/main.py:117
 msgid "Moon phase can only be displayed between {min_date} and {max_date}"
 msgstr ""
 
-#: kosmorrolib/main.py:134
+#: kosmorrolib/main.py:139
 msgid "Running on Python {python_version}"
 msgstr ""
 
-#: kosmorrolib/main.py:140
+#: kosmorrolib/main.py:145
 msgid "Do you really want to clear Kosmorro's cache? [yN] "
 msgstr ""
 
-#: kosmorrolib/main.py:147
+#: kosmorrolib/main.py:152
 msgid "Answer did not match expected options, cache not cleared."
 msgstr ""
 
-#: kosmorrolib/main.py:156
+#: kosmorrolib/main.py:161
 msgid ""
 "Compute the ephemerides and the events for a given date, at a given "
 "position on Earth."
 msgstr ""
 
-#: kosmorrolib/main.py:158
+#: kosmorrolib/main.py:163
 msgid ""
 "By default, only the events will be computed for today ({date}).\n"
 "To compute also the ephemerides, latitude and longitude arguments are "
 "needed."
 msgstr ""
 
-#: kosmorrolib/main.py:163
+#: kosmorrolib/main.py:168
 msgid "Show the program version"
 msgstr ""
 
-#: kosmorrolib/main.py:165
+#: kosmorrolib/main.py:170
 msgid "Delete all the files Kosmorro stored in the cache."
 msgstr ""
 
-#: kosmorrolib/main.py:167
+#: kosmorrolib/main.py:172
 msgid "The format under which the information have to be output"
 msgstr ""
 
-#: kosmorrolib/main.py:169
+#: kosmorrolib/main.py:174
 msgid ""
 "The observer's latitude on Earth. Can also be set in the "
 "KOSMORRO_LATITUDE environment variable."
 msgstr ""
 
-#: kosmorrolib/main.py:172
+#: kosmorrolib/main.py:177
 msgid ""
 "The observer's longitude on Earth. Can also be set in the "
 "KOSMORRO_LONGITUDE environment variable."
 msgstr ""
 
-#: kosmorrolib/main.py:175
+#: kosmorrolib/main.py:180
 msgid ""
 "The date for which the ephemerides must be computed (in the YYYY-MM-DD "
 "format), or as an interval in the \"[+-]YyMmDd\" format (with Y, M, and D"
 " numbers). Defaults to the current date ({default_date})"
 msgstr ""
 
-#: kosmorrolib/main.py:180
+#: kosmorrolib/main.py:185
 msgid ""
 "The timezone to display the hours in (e.g. 2 for UTC+2 or -3 for UTC-3). "
 "Can also be set in the KOSMORRO_TIMEZONE environment variable."
 msgstr ""
 
-#: kosmorrolib/main.py:183
+#: kosmorrolib/main.py:188
 msgid "Disable the colors in the console."
 msgstr ""
 
-#: kosmorrolib/main.py:185
+#: kosmorrolib/main.py:190
 msgid ""
 "A file to export the output to. If not given, the standard output is "
 "used. This argument is needed for PDF format."
 msgstr ""
 
-#: kosmorrolib/main.py:188
+#: kosmorrolib/main.py:193
 msgid ""
 "Do not generate a graph to represent the rise and set times in the PDF "
 "format."
 msgstr ""
```

### Comparing `kosmorro-0.8.1/kosmorrolib/main.py` & `kosmorro-0.9.0/kosmorrolib/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,17 +82,22 @@
         print(colored(error.msg, 'red'))
         return 1
 
     if args.output is not None:
         try:
             with open(args.output, 'wb') as output_file:
                 output_file.write(output.to_string())
+        except UnavailableFeatureError as error:
+            print(colored(error.msg, 'red'))
+            return 2
         except OSError as error:
-            print(_('Could not save the output in "{path}": {error}').format(path=args.output,
-                                                                             error=error.strerror))
+            print(colored(_('Could not save the output in "{path}": {error}').format(path=args.output,
+                                                                                     error=error.strerror),
+                          'red'))
+            return 3
     elif not output.is_file_output_needed():
         print(output)
     else:
         print(colored(_('Selected output format needs an output file (--output).'), color='red'))
         return 1
 
     return 0
```

### Comparing `kosmorro-0.8.1/kosmorrolib/version.py` & `kosmorro-0.9.0/kosmorrolib/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU Affero General Public License for more details.
 #
 #    You should have received a copy of the GNU Affero General Public License
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-VERSION = '0.8.1'
+VERSION = '0.9.0'
```

### Comparing `kosmorro-0.8.1/manpage/kosmorro.1` & `kosmorro-0.9.0/manpage/kosmorro.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .\" generated with Ronn/v0.7.3
 .\" http://github.com/rtomayko/ronn/tree/0.7.3
 .
-.TH "KOSMORRO" "1" "June 2020" "" ""
+.TH "KOSMORRO" "1" "January 2021" "" ""
 .
 .SH "NAME"
 \fBkosmorro\fR \- a program that computes the ephemerides
 .
 .SH "SYNOPSIS"
 \fBkosmorro\fR
 .
```

### Comparing `kosmorro-0.8.1/manpage/kosmorro.7` & `kosmorro-0.9.0/manpage/kosmorro.7`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 .\" generated with Ronn/v0.7.3
 .\" http://github.com/rtomayko/ronn/tree/0.7.3
 .
-.TH "KOSMORRO" "7" "June 2020" "" ""
+.TH "KOSMORRO" "7" "January 2021" "" ""
 .
 .SH "NAME"
 \fBkosmorro\fR \- a program that computes the ephemerides
 .
 .SH "DESCRIPTION"
 This manual explains the different terms that one can find when using \fBkosmorro\fR(1)\. The terms are given in an alphabetically order\.
 .
 .SH "TERMS"
 .
+.SS "Apogee"
+The Moon is told being at its apogee when it is at its furthest point from the Earth\.
+.
 .SS "Conjunction"
 From the point of view of the Earth, two asters are said in conjunction when they are close together\. It is, of course, an illusion caused by the position of the Earth combined with the two other objects\' ones\.
 .
 .SS "Elongation"
 The elongation is the angle of visual separation between a planet and the Sun, as seen from the point of view of the Earth\. For the inferior planets, the time when the elongation is maximal is propice to their observation, because it is the moment when they are the most visible\.
 .
 .SS "Occultation"
@@ -22,14 +25,17 @@
 .
 .SS "Opposition"
 An aster is said in opposition when it is positionned at the exact opposite of the Sun, from the point of view of the Earth, i\.e\. when their angle is equal to 180 degrees\. For all the superior planets, it is the best moment to observe them, because they will be at the smallest distance to the Earth\. Plus, they will appear full\.
 .
 .br
 For instance, Mars is in opposition when the angle Mars\-Earth\-Sun is equal to 180 degrees\.
 .
+.SS "Perigee"
+The Moon is told being at its apogee when it is at its nearest point from the Earth\.
+.
 .SS "Planet"
 A planet is an aster that orbits around a star, is not a star itself, is massive enough to maintain it nearly round, and has cleaned its orbit from other massive objects\.
 .
 .P
 \fBInferior planet\fR
 .
 .P
```

### Comparing `kosmorro-0.8.1/setup.py` & `kosmorro-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/test/core.py` & `kosmorro-0.9.0/test/core.py`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/test/dateutil.py` & `kosmorro-0.9.0/test/dateutil.py`

 * *Files identical despite different names*

### Comparing `kosmorro-0.8.1/test/dumper.py` & `kosmorro-0.9.0/test/dumper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
 from datetime import date, datetime
 
 from kosmorrolib.data import AsterEphemerides, Planet, MoonPhase, Event
 from kosmorrolib.dumper import JsonDumper, TextDumper, _LatexDumper
+from kosmorrolib.enum import MoonPhaseType, EventType
 
 
 class DumperTestCase(unittest.TestCase):
     def setUp(self) -> None:
         self.maxDiff = None
 
     def test_json_dumper_returns_correct_json(self):
@@ -279,22 +280,22 @@
         culmination_time = datetime(2019, 10, 14, 13) if aster_rise_set else None
         set_time = datetime(2019, 10, 14, 23) if aster_rise_set else None
 
         return [AsterEphemerides(rise_time, culmination_time, set_time, Planet('Mars', 'MARS'))]
 
     @staticmethod
     def _get_moon_phase():
-        return MoonPhase('FULL_MOON', datetime(2019, 10, 14), datetime(2019, 10, 21))
+        return MoonPhase(MoonPhaseType.FULL_MOON, datetime(2019, 10, 14), datetime(2019, 10, 21))
 
     @staticmethod
     def _get_events():
-        return [Event('OPPOSITION',
+        return [Event(EventType.OPPOSITION,
                       [Planet('Mars', 'MARS')],
                       datetime(2019, 10, 14, 23, 00)),
-                Event('MAXIMAL_ELONGATION',
+                Event(EventType.MAXIMAL_ELONGATION,
                       [Planet('Venus', 'VENUS')],
                       datetime(2019, 10, 14, 12, 00), details='42.0°'),
                 ]
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kosmorro-0.8.1/test/ephemerides.py` & `kosmorro-0.9.0/test/ephemerides.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import unittest
+
 from .testutils import expect_assertions
 from kosmorrolib import ephemerides
 from kosmorrolib.data import EARTH, Position, MoonPhase
+from kosmorrolib.enum import MoonPhaseType
+
 from datetime import date
 from kosmorrolib.exceptions import OutOfRangeDateError
 
 
 class EphemeridesTestCase(unittest.TestCase):
     def test_get_ephemerides_for_aster_returns_correct_hours(self):
         position = Position(0, 0, EARTH)
@@ -25,92 +28,92 @@
 
     ###################################################################################################################
     ###                                             MOON PHASE TESTS                                                ###
     ###################################################################################################################
 
     def test_moon_phase_new_moon(self):
         phase = ephemerides.get_moon_phase(date(2019, 11, 25))
-        self.assertEqual('WANING_CRESCENT', phase.identifier)
+        self.assertEqual(MoonPhaseType.WANING_CRESCENT, phase.phase_type)
         self.assertIsNone(phase.time)
         self.assertRegexpMatches(phase.next_phase_date.isoformat(), '^2019-11-26T')
 
         phase = ephemerides.get_moon_phase(date(2019, 11, 26))
-        self.assertEqual('NEW_MOON', phase.identifier)
+        self.assertEqual(MoonPhaseType.NEW_MOON, phase.phase_type)
         self.assertRegexpMatches(phase.next_phase_date.isoformat(), '^2019-12-04T')
 
         phase = ephemerides.get_moon_phase(date(2019, 11, 27))
-        self.assertEqual('WAXING_CRESCENT', phase.identifier)
+        self.assertEqual(MoonPhaseType.WAXING_CRESCENT, phase.phase_type)
         self.assertIsNone(phase.time)
         self.assertRegexpMatches(phase.next_phase_date.isoformat(), '^2019-12-04T')
 
     def test_moon_phase_first_crescent(self):
         phase = ephemerides.get_moon_phase(date(2019, 11, 3))
-        self.assertEqual('WAXING_CRESCENT', phase.identifier)
+        self.assertEqual(MoonPhaseType.WAXING_CRESCENT, phase.phase_type)
         self.assertIsNone(phase.time)
         self.assertRegexpMatches(phase.next_phase_date.isoformat(), '^2019-11-04T')
 
         phase = ephemerides.get_moon_phase(date(2019, 11, 4))
-        self.assertEqual('FIRST_QUARTER', phase.identifier)
+        self.assertEqual(MoonPhaseType.FIRST_QUARTER, phase.phase_type)
         self.assertRegexpMatches(phase.next_phase_date.isoformat(), '^2019-11-12T')
 
         phase = ephemerides.get_moon_phase(date(2019, 11, 5))
-        self.assertEqual('WAXING_GIBBOUS', phase.identifier)
+        self.assertEqual(MoonPhaseType.WAXING_GIBBOUS, phase.phase_type)
         self.assertIsNone(phase.time)
         self.assertRegexpMatches(phase.next_phase_date.isoformat(), '^2019-11-12T')
 
     def test_moon_phase_full_moon(self):
         phase = ephemerides.get_moon_phase(date(2019, 11, 11))
-        self.assertEqual('WAXING_GIBBOUS', phase.identifier)
+        self.assertEqual(MoonPhaseType.WAXING_GIBBOUS, phase.phase_type)
         self.assertIsNone(phase.time)
         self.assertRegexpMatches(phase.next_phase_date.isoformat(), '^2019-11-12T')
 
         phase = ephemerides.get_moon_phase(date(2019, 11, 12))
-        self.assertEqual('FULL_MOON', phase.identifier)
+        self.assertEqual(MoonPhaseType.FULL_MOON, phase.phase_type)
         self.assertRegexpMatches(phase.next_phase_date.isoformat(), '^2019-11-19T')
 
         phase = ephemerides.get_moon_phase(date(2019, 11, 13))
-        self.assertEqual('WANING_GIBBOUS', phase.identifier)
+        self.assertEqual(MoonPhaseType.WANING_GIBBOUS, phase.phase_type)
         self.assertIsNone(phase.time)
         self.assertRegexpMatches(phase.next_phase_date.isoformat(), '^2019-11-19T')
 
     def test_moon_phase_last_quarter(self):
         phase = ephemerides.get_moon_phase(date(2019, 11, 18))
-        self.assertEqual('WANING_GIBBOUS', phase.identifier)
+        self.assertEqual(MoonPhaseType.WANING_GIBBOUS, phase.phase_type)
         self.assertIsNone(phase.time)
         self.assertRegexpMatches(phase.next_phase_date.isoformat(), '^2019-11-19T')
 
         phase = ephemerides.get_moon_phase(date(2019, 11, 19))
-        self.assertEqual('LAST_QUARTER', phase.identifier)
+        self.assertEqual(MoonPhaseType.LAST_QUARTER, phase.phase_type)
         self.assertRegexpMatches(phase.next_phase_date.isoformat(), '^2019-11-26T')
 
         phase = ephemerides.get_moon_phase(date(2019, 11, 20))
-        self.assertEqual('WANING_CRESCENT', phase.identifier)
+        self.assertEqual(MoonPhaseType.WANING_CRESCENT, phase.phase_type)
         self.assertIsNone(phase.time)
         self.assertRegexpMatches(phase.next_phase_date.isoformat(), '^2019-11-26T')
 
     def test_moon_phase_prediction(self):
-        phase = MoonPhase('NEW_MOON', None, None)
-        self.assertEqual('First Quarter', phase.get_next_phase_name())
-        phase = MoonPhase('WAXING_CRESCENT', None, None)
-        self.assertEqual('First Quarter', phase.get_next_phase_name())
-
-        phase = MoonPhase('FIRST_QUARTER', None, None)
-        self.assertEqual('Full Moon', phase.get_next_phase_name())
-        phase = MoonPhase('WAXING_GIBBOUS', None, None)
-        self.assertEqual('Full Moon', phase.get_next_phase_name())
-
-        phase = MoonPhase('FULL_MOON', None, None)
-        self.assertEqual('Last Quarter', phase.get_next_phase_name())
-        phase = MoonPhase('WANING_GIBBOUS', None, None)
-        self.assertEqual('Last Quarter', phase.get_next_phase_name())
-
-        phase = MoonPhase('LAST_QUARTER', None, None)
-        self.assertEqual('New Moon', phase.get_next_phase_name())
-        phase = MoonPhase('WANING_CRESCENT', None, None)
-        self.assertEqual('New Moon', phase.get_next_phase_name())
+        phase = MoonPhase(MoonPhaseType.NEW_MOON, None, None)
+        self.assertEqual(MoonPhaseType.FIRST_QUARTER, phase.get_next_phase())
+        phase = MoonPhase(MoonPhaseType.WAXING_CRESCENT, None, None)
+        self.assertEqual(MoonPhaseType.FIRST_QUARTER, phase.get_next_phase())
+
+        phase = MoonPhase(MoonPhaseType.FIRST_QUARTER, None, None)
+        self.assertEqual(MoonPhaseType.FULL_MOON, phase.get_next_phase())
+        phase = MoonPhase(MoonPhaseType.WAXING_GIBBOUS, None, None)
+        self.assertEqual(MoonPhaseType.FULL_MOON, phase.get_next_phase())
+
+        phase = MoonPhase(MoonPhaseType.FULL_MOON, None, None)
+        self.assertEqual(MoonPhaseType.LAST_QUARTER, phase.get_next_phase())
+        phase = MoonPhase(MoonPhaseType.WANING_GIBBOUS, None, None)
+        self.assertEqual(MoonPhaseType.LAST_QUARTER, phase.get_next_phase())
+
+        phase = MoonPhase(MoonPhaseType.LAST_QUARTER, None, None)
+        self.assertEqual(MoonPhaseType.NEW_MOON, phase.get_next_phase())
+        phase = MoonPhase(MoonPhaseType.WANING_CRESCENT, None, None)
+        self.assertEqual(MoonPhaseType.NEW_MOON, phase.get_next_phase())
 
     def test_get_ephemerides_raises_exception_on_out_of_date_range(self):
         with self.assertRaises(OutOfRangeDateError):
             ephemerides.get_ephemerides(date(1789, 5, 5), Position(0, 0, EARTH))
 
     def test_get_moon_phase_raises_exception_on_out_of_date_range(self):
         with self.assertRaises(OutOfRangeDateError):
```

### Comparing `kosmorro-0.8.1/test/testutils.py` & `kosmorro-0.9.0/test/testutils.py`

 * *Files identical despite different names*

