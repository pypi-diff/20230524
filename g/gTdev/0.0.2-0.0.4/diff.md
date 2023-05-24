# Comparing `tmp/gTdev-0.0.2.tar.gz` & `tmp/gTdev-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "gTdev-0.0.4.tar", last modified: Wed May 24 03:08:20 2023, max compression
```

## Comparing `gTdev-0.0.2.tar` & `gTdev-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,19 @@
--rw-r--r--   0        0        0     7816 2020-02-02 00:00:00.000000 gtdev-0.0.2/LICENSE
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 gtdev-0.0.2/README.md
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 gtdev-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 gtdev-0.0.2/dist/gTdev-0.0.1-py3-none-any.whl
--rw-r--r--   0        0        0    23122 2020-02-02 00:00:00.000000 gtdev-0.0.2/dist/gTdev-0.0.1.tar.gz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtdev-0.0.2/src/gTdev/Vth.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtdev-0.0.2/src/gTdev/__init__.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 gtdev-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-24 03:08:20.111321 gTdev-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2022-12-02 07:39:30.000000 gTdev-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      123 2023-04-19 01:59:01.000000 gTdev-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    30681 2023-05-24 03:08:20.110319 gTdev-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    30256 2023-05-11 05:41:21.000000 gTdev-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 03:08:20.083758 gTdev-0.0.4/gTdev/
+-rw-rw-rw-   0        0        0      129 2023-05-22 03:09:44.000000 gTdev-0.0.4/gTdev/__init__.py
+-rw-rw-rw-   0        0        0     2548 2023-05-22 02:15:58.000000 gTdev-0.0.4/gTdev/gtInv.py
+-rw-rw-rw-   0        0        0     2975 2023-05-16 06:31:45.000000 gTdev-0.0.4/gTdev/gtcurve.py
+-rw-rw-rw-   0        0        0      187 2023-05-16 06:36:50.000000 gTdev-0.0.4/gTdev/gtdevCommon.py
+-rw-rw-rw-   0        0        0     1561 2023-05-24 00:29:00.000000 gTdev-0.0.4/gTdev/gtfile.py
+-rw-rw-rw-   0        0        0     3756 2023-05-24 02:30:33.000000 gTdev-0.0.4/gTdev/gtmos.py
+drwxrwxrwx   0        0        0        0 2023-05-24 03:08:20.107309 gTdev-0.0.4/gTdev.egg-info/
+-rw-rw-rw-   0        0        0    30681 2023-05-24 03:08:19.000000 gTdev-0.0.4/gTdev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-05-24 03:08:19.000000 gTdev-0.0.4/gTdev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 03:08:19.000000 gTdev-0.0.4/gTdev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-24 03:08:19.000000 gTdev-0.0.4/gTdev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 03:08:20.111321 gTdev-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      689 2023-05-24 02:53:37.000000 gTdev-0.0.4/setup.py
```

