# Comparing `tmp/ZipDAS-0.1.0.tar.gz` & `tmp/ZipDAS-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ZipDAS-0.1.0.tar", last modified: Mon May 22 07:23:20 2023, max compression
+gzip compressed data, was "ZipDAS-0.1.1.tar", last modified: Wed May 24 00:00:54 2023, max compression
```

## Comparing `ZipDAS-0.1.0.tar` & `ZipDAS-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,15 @@
-drwxr-xr-x   0 weiqiang   (501) staff       (20)        0 2023-05-22 07:23:20.245207 ZipDAS-0.1.0/
--rw-r--r--   0 weiqiang   (501) staff       (20)      112 2023-05-22 07:23:20.244866 ZipDAS-0.1.0/PKG-INFO
-drwxr-xr-x   0 weiqiang   (501) staff       (20)        0 2023-05-22 07:23:20.244466 ZipDAS-0.1.0/ZipDAS.egg-info/
--rw-r--r--   0 weiqiang   (501) staff       (20)      112 2023-05-22 07:23:20.000000 ZipDAS-0.1.0/ZipDAS.egg-info/PKG-INFO
--rw-r--r--   0 weiqiang   (501) staff       (20)      157 2023-05-22 07:23:20.000000 ZipDAS-0.1.0/ZipDAS.egg-info/SOURCES.txt
--rw-r--r--   0 weiqiang   (501) staff       (20)        1 2023-05-22 07:23:20.000000 ZipDAS-0.1.0/ZipDAS.egg-info/dependency_links.txt
--rw-r--r--   0 weiqiang   (501) staff       (20)       29 2023-05-22 07:23:20.000000 ZipDAS-0.1.0/ZipDAS.egg-info/requires.txt
--rw-r--r--   0 weiqiang   (501) staff       (20)        7 2023-05-22 07:23:20.000000 ZipDAS-0.1.0/ZipDAS.egg-info/top_level.txt
--rw-r--r--   0 weiqiang   (501) staff       (20)       38 2023-05-22 07:23:20.245310 ZipDAS-0.1.0/setup.cfg
--rw-r--r--   0 weiqiang   (501) staff       (20)      265 2023-05-22 07:22:09.000000 ZipDAS-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:00:54.841277 ZipDAS-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-24 00:00:46.000000 ZipDAS-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-24 00:00:54.841277 ZipDAS-0.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:00:54.841277 ZipDAS-0.1.1/ZipDAS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-24 00:00:54.000000 ZipDAS-0.1.1/ZipDAS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-24 00:00:54.000000 ZipDAS-0.1.1/ZipDAS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 00:00:54.000000 ZipDAS-0.1.1/ZipDAS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-24 00:00:54.000000 ZipDAS-0.1.1/ZipDAS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 00:00:54.000000 ZipDAS-0.1.1/ZipDAS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 00:00:54.841277 ZipDAS-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-24 00:00:46.000000 ZipDAS-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:00:54.841277 ZipDAS-0.1.1/zipdas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 00:00:46.000000 ZipDAS-0.1.1/zipdas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14364 2023-05-24 00:00:46.000000 ZipDAS-0.1.1/zipdas/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19837 2023-05-24 00:00:46.000000 ZipDAS-0.1.1/zipdas/model.py
```

