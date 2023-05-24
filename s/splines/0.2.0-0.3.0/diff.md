# Comparing `tmp/splines-0.2.0.tar.gz` & `tmp/splines-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splines-0.2.0.tar", last modified: Fri Mar  4 18:59:20 2022, max compression
+gzip compressed data, was "splines-0.3.0.tar", last modified: Wed May 24 21:07:44 2023, max compression
```

## Comparing `splines-0.2.0.tar` & `splines-0.3.0.tar`

### file list

```diff
@@ -1,95 +1,87 @@
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2022-03-04 18:59:20.493077 splines-0.2.0/
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2022-03-04 18:59:20.473077 splines-0.2.0/.binder/
--rw-r--r--   0 mg        (1000) mg        (1000)      328 2021-08-22 13:40:33.000000 splines-0.2.0/.binder/README
--rw-r--r--   0 mg        (1000) mg        (1000)        0 2021-08-22 13:40:33.000000 splines-0.2.0/.binder/apt.txt
--rwxr-xr-x   0 mg        (1000) mg        (1000)       44 2021-08-22 13:40:33.000000 splines-0.2.0/.binder/postBuild
--rw-r--r--   0 mg        (1000) mg        (1000)       31 2021-08-22 13:52:06.000000 splines-0.2.0/.binder/requirements.txt
--rw-r--r--   0 mg        (1000) mg        (1000)      304 2018-07-09 18:17:30.000000 splines-0.2.0/.editorconfig
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2022-03-04 18:59:20.473077 splines-0.2.0/.github/
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2022-03-04 18:59:20.473077 splines-0.2.0/.github/workflows/
--rw-r--r--   0 mg        (1000) mg        (1000)     1749 2021-11-22 17:48:37.000000 splines-0.2.0/.github/workflows/docs.yml
--rw-r--r--   0 mg        (1000) mg        (1000)      772 2021-11-22 17:48:37.000000 splines-0.2.0/.github/workflows/tests.yml
--rw-r--r--   0 mg        (1000) mg        (1000)      100 2021-08-22 13:40:33.000000 splines-0.2.0/.gitignore
--rw-r--r--   0 mg        (1000) mg        (1000)      195 2022-01-28 19:59:43.000000 splines-0.2.0/.readthedocs.yml
--rw-r--r--   0 mg        (1000) mg        (1000)     1063 2022-03-04 18:58:04.000000 splines-0.2.0/LICENSE
--rw-r--r--   0 mg        (1000) mg        (1000)      163 2018-07-09 19:06:29.000000 splines-0.2.0/MANIFEST.in
--rw-r--r--   0 mg        (1000) mg        (1000)     1449 2022-03-04 18:59:20.493077 splines-0.2.0/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)      631 2021-08-22 13:40:33.000000 splines-0.2.0/README.rst
--rwxr-xr-x   0 mg        (1000) mg        (1000)      281 2021-12-23 13:54:01.000000 splines-0.2.0/autobuild.sh
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2022-03-04 18:59:20.477077 splines-0.2.0/doc/
--rw-r--r--   0 mg        (1000) mg        (1000)     5264 2022-01-28 19:59:43.000000 splines-0.2.0/doc/conf.py
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2022-03-04 18:59:20.485077 splines-0.2.0/doc/euclidean/
--rw-r--r--   0 mg        (1000) mg        (1000)     2362 2021-10-23 07:33:41.000000 splines-0.2.0/doc/euclidean/barry_goldman.py
--rw-r--r--   0 mg        (1000) mg        (1000)    27860 2021-12-23 13:51:01.000000 splines-0.2.0/doc/euclidean/bezier-de-casteljau.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     6436 2021-09-25 18:28:29.000000 splines-0.2.0/doc/euclidean/bezier-non-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     4154 2021-09-25 18:28:29.000000 splines-0.2.0/doc/euclidean/bezier-properties.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     1936 2021-09-25 18:28:29.000000 splines-0.2.0/doc/euclidean/bezier.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     1715 2021-09-29 20:01:14.000000 splines-0.2.0/doc/euclidean/casteljau.py
--rw-r--r--   0 mg        (1000) mg        (1000)    30701 2021-12-23 14:11:29.000000 splines-0.2.0/doc/euclidean/catmull-rom-barry-goldman.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    19264 2022-01-13 16:58:04.000000 splines-0.2.0/doc/euclidean/catmull-rom-non-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    17978 2022-01-13 16:58:04.000000 splines-0.2.0/doc/euclidean/catmull-rom-properties.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    23367 2022-01-13 16:56:46.000000 splines-0.2.0/doc/euclidean/catmull-rom-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     2300 2021-08-22 13:40:33.000000 splines-0.2.0/doc/euclidean/catmull-rom.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     3735 2021-10-23 07:33:41.000000 splines-0.2.0/doc/euclidean/catmull_rom.py
--rw-r--r--   0 mg        (1000) mg        (1000)    17059 2022-01-13 16:58:04.000000 splines-0.2.0/doc/euclidean/end-conditions-natural.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     1004 2021-08-22 13:40:33.000000 splines-0.2.0/doc/euclidean/end-conditions.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     5316 2022-01-13 16:58:04.000000 splines-0.2.0/doc/euclidean/helper.py
--rw-r--r--   0 mg        (1000) mg        (1000)    16988 2021-09-25 18:28:29.000000 splines-0.2.0/doc/euclidean/hermite-non-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     8831 2021-08-22 13:40:33.000000 splines-0.2.0/doc/euclidean/hermite-properties.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    20316 2021-09-25 18:28:29.000000 splines-0.2.0/doc/euclidean/hermite-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     1721 2021-08-22 13:40:33.000000 splines-0.2.0/doc/euclidean/hermite.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     1437 2021-08-27 14:01:24.000000 splines-0.2.0/doc/euclidean/index.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)      125 2021-09-25 18:28:29.000000 splines-0.2.0/doc/euclidean/ipython_kernel_config.py
--rw-r--r--   0 mg        (1000) mg        (1000)    13986 2022-01-13 16:58:04.000000 splines-0.2.0/doc/euclidean/kochanek-bartels-non-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     7455 2021-09-25 18:28:29.000000 splines-0.2.0/doc/euclidean/kochanek-bartels-properties.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    15071 2021-09-25 18:28:29.000000 splines-0.2.0/doc/euclidean/kochanek-bartels-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     1703 2021-09-25 18:28:29.000000 splines-0.2.0/doc/euclidean/kochanek-bartels.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    16522 2021-09-25 18:28:29.000000 splines-0.2.0/doc/euclidean/lagrange.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     7549 2021-09-25 18:28:29.000000 splines-0.2.0/doc/euclidean/natural-non-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     4235 2021-09-25 18:28:29.000000 splines-0.2.0/doc/euclidean/natural-properties.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    14381 2022-01-28 19:36:21.000000 splines-0.2.0/doc/euclidean/natural-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     1776 2021-09-25 18:28:29.000000 splines-0.2.0/doc/euclidean/natural.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    30468 2021-09-26 20:16:30.000000 splines-0.2.0/doc/euclidean/piecewise-monotone.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     8217 2021-09-25 18:28:29.000000 splines-0.2.0/doc/euclidean/polynomials.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     6818 2021-11-22 17:48:37.000000 splines-0.2.0/doc/euclidean/utility.py
--rw-r--r--   0 mg        (1000) mg        (1000)     1818 2021-08-22 13:40:33.000000 splines-0.2.0/doc/favicon.svg
--rw-r--r--   0 mg        (1000) mg        (1000)     1958 2021-08-22 14:32:07.000000 splines-0.2.0/doc/index.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)      125 2021-09-25 18:28:29.000000 splines-0.2.0/doc/ipython_kernel_config.py
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2022-03-04 18:59:20.485077 splines-0.2.0/doc/python-module/
--rw-r--r--   0 mg        (1000) mg        (1000)      405 2021-12-04 14:15:22.000000 splines-0.2.0/doc/python-module/splines.quaternion.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      351 2021-09-04 18:22:07.000000 splines-0.2.0/doc/python-module/splines.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      110 2021-08-22 13:40:33.000000 splines-0.2.0/doc/python-module.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     4957 2021-11-22 21:59:43.000000 splines-0.2.0/doc/references.bib
--rw-r--r--   0 mg        (1000) mg        (1000)      231 2021-08-22 13:40:33.000000 splines-0.2.0/doc/references.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      152 2022-01-28 19:59:43.000000 splines-0.2.0/doc/requirements.txt
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2022-03-04 18:59:20.489077 splines-0.2.0/doc/rotation/
--rw-r--r--   0 mg        (1000) mg        (1000)    10844 2022-01-13 16:58:04.000000 splines-0.2.0/doc/rotation/barry-goldman.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    13523 2022-01-13 16:58:04.000000 splines-0.2.0/doc/rotation/catmull-rom-non-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    25642 2022-01-13 16:58:04.000000 splines-0.2.0/doc/rotation/catmull-rom-uniform.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    14073 2022-01-03 19:56:46.000000 splines-0.2.0/doc/rotation/cumulative-form.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     8507 2022-01-13 16:58:04.000000 splines-0.2.0/doc/rotation/de-casteljau.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     5692 2022-01-13 16:58:04.000000 splines-0.2.0/doc/rotation/end-conditions-natural.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     9371 2022-01-03 19:56:46.000000 splines-0.2.0/doc/rotation/helper.py
--rw-r--r--   0 mg        (1000) mg        (1000)     1742 2022-01-13 16:58:04.000000 splines-0.2.0/doc/rotation/index.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)      125 2021-09-25 18:28:29.000000 splines-0.2.0/doc/rotation/ipython_kernel_config.py
--rw-r--r--   0 mg        (1000) mg        (1000)    11327 2022-01-13 16:58:04.000000 splines-0.2.0/doc/rotation/kochanek-bartels.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    10769 2022-01-03 19:56:46.000000 splines-0.2.0/doc/rotation/naive-4d-interpolation.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)     4506 2022-01-03 19:56:46.000000 splines-0.2.0/doc/rotation/naive-euler-angles-interpolation.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    18868 2022-01-03 19:56:46.000000 splines-0.2.0/doc/rotation/quaternions.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)    17104 2022-01-03 19:56:46.000000 splines-0.2.0/doc/rotation/slerp.ipynb
--rw-r--r--   0 mg        (1000) mg        (1000)       73 2022-03-04 18:59:20.493077 splines-0.2.0/setup.cfg
--rw-r--r--   0 mg        (1000) mg        (1000)     1226 2021-08-22 13:40:33.000000 splines-0.2.0/setup.py
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2022-03-04 18:59:20.473077 splines-0.2.0/src/
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2022-03-04 18:59:20.489077 splines-0.2.0/src/splines/
--rw-r--r--   0 mg        (1000) mg        (1000)    30889 2022-03-04 18:58:04.000000 splines-0.2.0/src/splines/__init__.py
--rw-r--r--   0 mg        (1000) mg        (1000)    22610 2022-01-13 16:58:04.000000 splines-0.2.0/src/splines/quaternion.py
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2022-03-04 18:59:20.493077 splines-0.2.0/src/splines.egg-info/
--rw-r--r--   0 mg        (1000) mg        (1000)     1449 2022-03-04 18:59:20.000000 splines-0.2.0/src/splines.egg-info/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)     2449 2022-03-04 18:59:20.000000 splines-0.2.0/src/splines.egg-info/SOURCES.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2022-03-04 18:59:20.000000 splines-0.2.0/src/splines.egg-info/dependency_links.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        6 2022-03-04 18:59:20.000000 splines-0.2.0/src/splines.egg-info/requires.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        8 2022-03-04 18:59:20.000000 splines-0.2.0/src/splines.egg-info/top_level.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2020-06-17 15:26:29.000000 splines-0.2.0/src/splines.egg-info/zip-safe
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2022-03-04 18:59:20.493077 splines-0.2.0/tests/
--rw-r--r--   0 mg        (1000) mg        (1000)        7 2018-09-15 15:50:44.000000 splines-0.2.0/tests/requirements.txt
--rw-r--r--   0 mg        (1000) mg        (1000)      250 2018-09-15 15:50:44.000000 splines-0.2.0/tests/test_catmullrom.py
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 21:07:44.620894 splines-0.3.0/
+-rw-r--r--   0 mg        (1000) mg        (1000)     1063 2023-03-12 19:44:03.000000 splines-0.3.0/LICENSE
+-rw-r--r--   0 mg        (1000) mg        (1000)      163 2018-09-20 14:33:18.000000 splines-0.3.0/MANIFEST.in
+-rw-r--r--   0 mg        (1000) mg        (1000)     1469 2023-05-24 21:07:44.620894 splines-0.3.0/PKG-INFO
+-rw-r--r--   0 mg        (1000) mg        (1000)      629 2023-03-12 19:44:03.000000 splines-0.3.0/README.rst
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 21:07:44.596893 splines-0.3.0/doc/
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 21:07:44.588894 splines-0.3.0/doc/_templates/
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 21:07:44.596893 splines-0.3.0/doc/_templates/autosummary/
+-rw-r--r--   0 mg        (1000) mg        (1000)     1249 2023-05-24 20:38:03.000000 splines-0.3.0/doc/_templates/autosummary/module.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)     5619 2023-05-24 20:38:03.000000 splines-0.3.0/doc/conf.py
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 21:07:44.608893 splines-0.3.0/doc/euclidean/
+-rw-r--r--   0 mg        (1000) mg        (1000)     2362 2022-01-09 19:33:11.000000 splines-0.3.0/doc/euclidean/barry_goldman.py
+-rw-r--r--   0 mg        (1000) mg        (1000)    28201 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/bezier-de-casteljau.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     6458 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/bezier-non-uniform.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     4297 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/bezier-properties.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     2076 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/bezier.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     1715 2023-04-18 14:00:08.000000 splines-0.3.0/doc/euclidean/casteljau.py
+-rw-r--r--   0 mg        (1000) mg        (1000)    29812 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/catmull-rom-barry-goldman.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    23169 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/catmull-rom-non-uniform.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    25084 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/catmull-rom-properties.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    25543 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/catmull-rom-uniform.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     2113 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/catmull-rom.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     3735 2022-01-09 19:33:11.000000 splines-0.3.0/doc/euclidean/catmull_rom.py
+-rw-r--r--   0 mg        (1000) mg        (1000)    17191 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/end-conditions-natural.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     1977 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/end-conditions.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)     5734 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/helper.py
+-rw-r--r--   0 mg        (1000) mg        (1000)    17242 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/hermite-non-uniform.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     8746 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/hermite-properties.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    21419 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/hermite-uniform.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     1721 2023-03-19 17:15:42.000000 splines-0.3.0/doc/euclidean/hermite.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     2397 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/index.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    13944 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/kochanek-bartels-non-uniform.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     6292 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/kochanek-bartels-properties.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    15000 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/kochanek-bartels-uniform.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     1568 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/kochanek-bartels.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     1335 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/kochanek_bartels.py
+-rw-r--r--   0 mg        (1000) mg        (1000)    20703 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/lagrange.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     7526 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/natural-non-uniform.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     5008 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/natural-properties.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    14601 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/natural-uniform.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     1776 2023-03-19 19:45:40.000000 splines-0.3.0/doc/euclidean/natural.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    32062 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/piecewise-monotone.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     8414 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/polynomials.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    11467 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/quadrangle.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    10260 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/re-parameterization.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    11703 2023-05-24 20:38:03.000000 splines-0.3.0/doc/euclidean/splines.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)     7149 2022-12-23 22:22:43.000000 splines-0.3.0/doc/euclidean/utility.py
+-rw-r--r--   0 mg        (1000) mg        (1000)     1288 2023-03-12 19:44:03.000000 splines-0.3.0/doc/how-to-navigate.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)     1951 2023-05-07 18:14:33.000000 splines-0.3.0/doc/index.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     3526 2023-05-24 20:38:03.000000 splines-0.3.0/doc/intro.rst
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 21:07:44.608893 splines-0.3.0/doc/python-module/
+-rw-r--r--   0 mg        (1000) mg        (1000)      505 2023-05-20 17:07:27.000000 splines-0.3.0/doc/python-module/splines.quaternion.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)      406 2023-05-20 19:32:46.000000 splines-0.3.0/doc/python-module/splines.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)      110 2023-05-20 18:14:02.000000 splines-0.3.0/doc/python-module.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)      229 2023-03-12 19:44:03.000000 splines-0.3.0/doc/references.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)      415 2023-05-07 21:32:11.000000 splines-0.3.0/doc/requirements.txt
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 21:07:44.616894 splines-0.3.0/doc/rotation/
+-rw-r--r--   0 mg        (1000) mg        (1000)    10830 2023-05-24 20:38:03.000000 splines-0.3.0/doc/rotation/barry-goldman.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    13521 2023-05-24 20:38:03.000000 splines-0.3.0/doc/rotation/catmull-rom-non-uniform.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    25668 2023-05-24 20:38:03.000000 splines-0.3.0/doc/rotation/catmull-rom-uniform.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    14119 2023-05-24 20:38:03.000000 splines-0.3.0/doc/rotation/cumulative-form.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     9181 2023-05-24 20:38:03.000000 splines-0.3.0/doc/rotation/de-casteljau.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     5683 2023-05-24 20:38:03.000000 splines-0.3.0/doc/rotation/end-conditions-natural.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     9613 2023-01-08 17:55:49.000000 splines-0.3.0/doc/rotation/helper.py
+-rw-r--r--   0 mg        (1000) mg        (1000)     2611 2023-05-24 20:38:03.000000 splines-0.3.0/doc/rotation/index.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    11334 2023-05-24 20:38:03.000000 splines-0.3.0/doc/rotation/kochanek-bartels.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    10747 2023-05-24 20:38:03.000000 splines-0.3.0/doc/rotation/naive-4d-interpolation.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)     4503 2023-05-24 20:38:03.000000 splines-0.3.0/doc/rotation/naive-euler-angles-interpolation.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    20730 2023-05-24 20:38:03.000000 splines-0.3.0/doc/rotation/quaternions.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    17234 2023-05-24 20:38:03.000000 splines-0.3.0/doc/rotation/slerp.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)    13947 2023-05-24 20:38:03.000000 splines-0.3.0/doc/rotation/squad.ipynb
+-rw-r--r--   0 mg        (1000) mg        (1000)      100 2023-02-15 20:49:49.000000 splines-0.3.0/pyproject.toml
+-rw-r--r--   0 mg        (1000) mg        (1000)       38 2023-05-24 21:07:44.620894 splines-0.3.0/setup.cfg
+-rw-r--r--   0 mg        (1000) mg        (1000)     1336 2023-02-15 20:49:49.000000 splines-0.3.0/setup.py
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 21:07:44.588894 splines-0.3.0/src/
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 21:07:44.616894 splines-0.3.0/src/splines/
+-rw-r--r--   0 mg        (1000) mg        (1000)    33233 2023-05-24 21:03:31.000000 splines-0.3.0/src/splines/__init__.py
+-rw-r--r--   0 mg        (1000) mg        (1000)    25771 2023-05-24 20:38:03.000000 splines-0.3.0/src/splines/quaternion.py
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 21:07:44.616894 splines-0.3.0/src/splines.egg-info/
+-rw-r--r--   0 mg        (1000) mg        (1000)     1469 2023-05-24 21:07:44.000000 splines-0.3.0/src/splines.egg-info/PKG-INFO
+-rw-r--r--   0 mg        (1000) mg        (1000)     2336 2023-05-24 21:07:44.000000 splines-0.3.0/src/splines.egg-info/SOURCES.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2023-05-24 21:07:44.000000 splines-0.3.0/src/splines.egg-info/dependency_links.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        6 2023-05-24 21:07:44.000000 splines-0.3.0/src/splines.egg-info/requires.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        8 2023-05-24 21:07:44.000000 splines-0.3.0/src/splines.egg-info/top_level.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2023-05-20 17:04:43.000000 splines-0.3.0/src/splines.egg-info/zip-safe
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-05-24 21:07:44.620894 splines-0.3.0/tests/
+-rw-r--r--   0 mg        (1000) mg        (1000)      250 2018-09-20 14:33:18.000000 splines-0.3.0/tests/test_catmullrom.py
```

### Comparing `splines-0.2.0/LICENSE` & `splines-0.3.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2020-2022 Matthias Geier
+Copyright (c) 2020-2023 Matthias Geier
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `splines-0.2.0/PKG-INFO` & `splines-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 Metadata-Version: 2.1
 Name: splines
-Version: 0.2.0
+Version: 0.3.0
 Summary: Splines in Euclidean Space and Beyond
-Home-page: UNKNOWN
+Home-page: https://splines.readthedocs.io/
 Author: Matthias Geier
 Author-email: Matthias.Geier@gmail.com
 License: MIT
 Project-URL: Documentation, https://splines.readthedocs.io/
 Project-URL: Source Code, https://github.com/AudioSceneDescriptionFormat/splines/
 Project-URL: Bug Tracker, https://github.com/AudioSceneDescriptionFormat/splines/issues/
 Keywords: splines,curves,interpolation,quaternions
 Platform: any
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE
 
 Splines in Euclidean Space and Beyond
 =====================================
 
 ... with focus on univariate, non-uniform piecewise cubic polynomial curves
 in one, two and three spatial dimensions, as well as rotation splines.
 
 Installation
-    ``python3 -m pip install splines``
+    ``python -m pip install splines``
 
 Online documentation
     https://splines.readthedocs.io/
 
 Documentation notebooks on Binder
-    https://mybinder.org/v2/gh/AudioSceneDescriptionFormat/splines/master?filepath=doc/index.ipynb
+    https://mybinder.org/v2/gh/AudioSceneDescriptionFormat/splines/master?labpath=doc/index.ipynb
 
 Source code repository (and issue tracker)
     https://github.com/AudioSceneDescriptionFormat/splines
 
 License
     MIT -- see the file ``LICENSE`` for details.
 
-
-
```

### Comparing `splines-0.2.0/README.rst` & `splines-0.3.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Splines in Euclidean Space and Beyond
 =====================================
 
 ... with focus on univariate, non-uniform piecewise cubic polynomial curves
 in one, two and three spatial dimensions, as well as rotation splines.
 
 Installation
-    ``python3 -m pip install splines``
+    ``python -m pip install splines``
 
 Online documentation
     https://splines.readthedocs.io/
 
 Documentation notebooks on Binder
-    https://mybinder.org/v2/gh/AudioSceneDescriptionFormat/splines/master?filepath=doc/index.ipynb
+    https://mybinder.org/v2/gh/AudioSceneDescriptionFormat/splines/master?labpath=doc/index.ipynb
 
 Source code repository (and issue tracker)
     https://github.com/AudioSceneDescriptionFormat/splines
 
 License
     MIT -- see the file ``LICENSE`` for details.
```

### Comparing `splines-0.2.0/doc/conf.py` & `splines-0.3.0/doc/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,17 +31,25 @@
     'members': True,
     'undoc-members': True,
     'show-inheritance': True,
 }
 
 default_role = 'any'
 
+exclude_patterns = ['how-to-navigate.rst']
+
 linkcheck_ignore = [
     # Anchors with line numbers don't seem to work with linkcheck builder
     'https://github.com/scipy/scipy/blob/',
+    # The idea of DOIs is that they are kept valid, so why check them at all?
+    'https://doi.org/',
+]
+
+nbsphinx_execute_arguments = [
+    "--InlineBackend.figure_formats={'svg', 'pdf'}",
 ]
 
 
 def if_docname(text):
     return r"""
 {% if not env.docname.endswith('index') and env.docname not in [
     'euclidean/hermite',
@@ -69,15 +77,15 @@
 nbsphinx_prolog = if_docname(r"""
 .. raw:: html
 
     <div class="admonition note">
       This page was generated from
       <a class="reference external" href="https://github.com/AudioSceneDescriptionFormat/splines/blob/{{ env.config.release|e }}/{{ docname|e }}">{{ docname|e }}</a>.
       Interactive online version:
-      <span style="white-space: nowrap;"><a href="https://mybinder.org/v2/gh/AudioSceneDescriptionFormat/splines/{{ env.config.release|e }}?filepath={{ docname|e }}"><img alt="Binder badge" src="https://mybinder.org/badge_logo.svg" style="vertical-align:text-bottom"></a>.</span>
+      <span style="white-space: nowrap;"><a href="https://mybinder.org/v2/gh/AudioSceneDescriptionFormat/splines/{{ env.config.release|e }}?labpath={{ docname|e }}"><img alt="Binder badge" src="https://mybinder.org/badge_logo.svg" style="vertical-align:text-bottom"></a>.</span>
     </div>
 
 .. raw:: latex
 
     \nbsphinxstartnotebook{\scriptsize\noindent\strut
     \textcolor{gray}{The following section was generated from {{ latex_href }}
     \dotfill}}
@@ -90,29 +98,28 @@
     \textcolor{gray}{\dotfill\ {{ latex_href }} ends here.}}
 """)
 
 # Import Matplotlib to avoid this message in notebooks:
 # "Matplotlib is building the font cache; this may take a moment."
 import matplotlib.pyplot
 
+templates_path = ['_templates']
+
 # -- Work-around to get LaTeX References at the same place as HTML --------
 
 # See https://github.com/mcmtroffaes/sphinxcontrib-bibtex/issues/156
 
-import docutils
-import sphinx.builders.latex
-
-class DummyTransform(docutils.transforms.Transform):
+import sphinx.builders.latex.transforms
 
-    default_priority = 0
+class DummyTransform(sphinx.builders.latex.transforms.BibliographyTransform):
 
-    def apply(self):
+    def run(self, **kwargs):
         pass
 
-sphinx.builders.latex.BibliographyTransform = DummyTransform
+sphinx.builders.latex.transforms.BibliographyTransform = DummyTransform
 
 # -- Get version information and date from Git ----------------------------
 
 try:
     from subprocess import check_output
     release = check_output(['git', 'describe', '--tags', '--always'])
     release = release.decode().strip()
@@ -125,48 +132,54 @@
 # -- Options for HTML output -------------------------------------------------
 
 html_title = 'splines, version ' + release
 html_theme = 'insipid'
 html_domain_indices = False
 html_favicon = 'favicon.svg'
 html_copy_source = False
-html_permalinks_icon = '§'
+html_permalinks_icon = '#'
 html_show_copyright = False
 
 mathjax3_config = {
     'tex': {'tags': 'ams', 'useLabelIds': True},
 }
 
 # -- Options for LaTeX output ------------------------------------------------
 
 latex_elements = {
     'papersize': 'a4paper',
     'printindex': '',
     'sphinxsetup': r"""
-        VerbatimColor={HTML}{F5F5F5},
-        VerbatimBorderColor={HTML}{E0E0E0},
-        noteBorderColor={HTML}{E0E0E0},
-        noteborder=1.5pt,
-        warningBorderColor={HTML}{E0E0E0},
-        warningborder=1.5pt,
-        warningBgColor={HTML}{FBFBFB},
-    """,
-    'preamble': r"""
-\usepackage[sc,osf]{mathpazo}
+HeaderFamily=\rmfamily\bfseries,
+noteBorderColor={HTML}{E0E0E0},
+noteborder=0.5pt,
+warningBorderColor={HTML}{E0E0E0},
+warningborder=1.5pt,
+warningBgColor={HTML}{FBFBFB},
+div.topic_box-shadow=none,
+div.topic_border-TeXcolor={HTML}{E0E0E0},
+div.topic_border-width=0.5pt,
+""",
+    'fontpkg': r"""
+\usepackage{mathpazo}
 \linespread{1.05}  % see http://www.tug.dk/FontCatalogue/urwpalladio/
-\renewcommand{\sfdefault}{pplj}  % Palatino instead of sans serif
-\IfFileExists{zlmtt.sty}{
-    \usepackage[light,scaled=1.05]{zlmtt}  % light typewriter font from lmodern
-}{
-    \renewcommand{\ttdefault}{lmtt}  % typewriter font from lmodern
-}
+\setmainfont{TeX Gyre Pagella}[Numbers=OldStyle]
+\setmonofont{Latin Modern Mono Light}[Numbers=Lining]
 \usepackage{mathrsfs}  % for \mathscr{}
 """,
+    'preamble': r"""
+\urlstyle{tt}
+\renewenvironment{sphinxnote}[1]
+  {\begin{sphinxheavybox}\sphinxstrong{#1} }{\end{sphinxheavybox}}
+""",
 }
 
+latex_engine = 'lualatex'
+latex_use_xindy = False
+latex_table_style = ['booktabs']
 latex_show_urls = 'footnote'
 latex_show_pagerefs = True
 latex_domain_indices = False
 
 latex_documents = [
     ('index', 'splines.tex', project, author, 'howto'),
 ]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `splines-0.2.0/doc/euclidean/barry_goldman.py` & `splines-0.3.0/doc/euclidean/barry_goldman.py`

 * *Files identical despite different names*

### Comparing `splines-0.2.0/doc/euclidean/bezier-de-casteljau.ipynb` & `splines-0.3.0/doc/euclidean/bezier-de-casteljau.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9894085576259489%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'There are several ways that lead to Bézier "*

 * *            "curves,\\n'), (3, 'one (but only for cubic curves) was already shown in\\n'), (4, "*

 * *            "'[the notebook about Hermite "*

 * *            "curves](hermite-uniform.ipynb#Relation-to-Bézier-Splines).\\n')], delete: [4, 3, "*

 * *            "2]}}, 2: {'source': ['### Preparations']}, 11: {'source': {delete: [1]}}, 14: "*

 * *            "{'source': {insert: [(0, 'Another way to write the same thing is like this:\\n'), […]*

```diff
@@ -13,29 +13,27 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# De Casteljau's Algorithm\n",
                 "\n",
-                "There are several ways that lead to B\u00e9zier curves, one was already shown in\n",
-                "[the notebook about Hermite curves](hermite-uniform.ipynb#Relation-to-B\u00e9zier-Splines)\n",
-                "(but only for cubic curves).\n",
+                "There are several ways that lead to B\u00e9zier curves,\n",
+                "one (but only for cubic curves) was already shown in\n",
+                "[the notebook about Hermite curves](hermite-uniform.ipynb#Relation-to-B\u00e9zier-Splines).\n",
                 "In this notebook,\n",
                 "we will derive B\u00e9zier curves of arbitrary polynomial degree utilizing\n",
                 "[De Casteljau's algorithm](https://en.wikipedia.org/wiki/De_Casteljau's_algorithm)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Preparations\n",
-                "\n",
-                "Before we continue, here are are few preparations for the following calculations:"
+                "### Preparations"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -124,15 +122,14 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from casteljau import create_animation\n",
-                "from IPython.display import display, HTML\n",
                 "\n",
                 "def show_casteljau_animation(points, frames=30, interval=200):\n",
                 "    ani = create_animation(points, frames=frames, interval=interval)\n",
                 "    display({\n",
                 "        'text/html': ani.to_jshtml(default_mode='reflect'),\n",
                 "        'text/plain': 'Animations can only be shown in HTML output, sorry!',\n",
                 "    }, raw=True)\n",
@@ -164,20 +161,21 @@
                 "\\end{equation*}"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Another way to write the same thing it like this:\n",
+                "Another way to write the same thing is like this:\n",
                 "\n",
                 "\\begin{equation*}\n",
                 "\\boldsymbol{p}_{0,1}(t) = (1 - t) \\boldsymbol{x}_0 + t \\boldsymbol{x}_1,\n",
                 "\\end{equation*}\n",
-                "where in both cases $t \\in [0, 1]$.\n",
+                "where in both cases $0 \\le t \\le 1$.\n",
+                "These linear interpolations are sometimes also called *affine combinations*.\n",
                 "Since we will be needing quite a few of those linear interpolations,\n",
                 "let's create a helper function:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -559,15 +557,15 @@
                 "The length of the tangent vectors is twice the length of those lines."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "You might have already seen that coming, but it turns out that the last line in de Casteljau's algorithm ($\\boldsymbol{p}_{1,2}(t) - \\boldsymbol{p}_{0,1}(t)$ in our case) is exactly half of the tangent vector (at any given $t \\in [0, 1]$)."
+                "You might have already seen that coming, but it turns out that the last line in De Casteljau's algorithm ($\\boldsymbol{p}_{1,2}(t) - \\boldsymbol{p}_{0,1}(t)$ in our case) is exactly half of the tangent vector (at any given $t \\in [0, 1]$)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -816,15 +814,15 @@
                 "[construct uniform Catmull--Rom splines using B\u00e9zier segments](catmull-rom-uniform.ipynb#Using-B\u00e9zier-Segments)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We can now also see that the last linear segment in de Casteljau's algorithm\n",
+                "We can now also see that the last linear segment in De Casteljau's algorithm\n",
                 "($\\boldsymbol{p}_{1,3}(t) - \\boldsymbol{p}_{0,2}(t)$ in this case)\n",
                 "is exactly a third of the tangent vector (at any given $t \\in [0, 1]$):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -922,15 +920,15 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Degree 4 (Quartic)\n",
                 "\n",
                 "By now you know the drill,\n",
-                "we consider five control points,\n",
+                "let's consider five control points,\n",
                 "$\\boldsymbol{x}_0$,\n",
                 "$\\boldsymbol{x}_1$,\n",
                 "$\\boldsymbol{x}_2$,\n",
                 "$\\boldsymbol{x}_3$ and $\\boldsymbol{x}_4$,\n",
                 "which lead to more linear interpolations:"
             ]
         },
@@ -939,23 +937,42 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "p34 = NamedExpression('pbm_3,4', lerp(x3, x4))\n",
                 "p24 = NamedExpression('pbm_2,4', lerp(p23.expr, p34.expr))\n",
                 "p14 = NamedExpression('pbm_1,4', lerp(p13.expr, p24.expr))\n",
-                "p04 = NamedExpression('pbm_0,4', lerp(p03.expr, p14.expr))\n",
-                "p04"
+                "p04 = NamedExpression('pbm_0,4', lerp(p03.expr, p14.expr))"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The resulting expression for $\\boldsymbol{p}_{0,4}(t)$\n",
+                "is quite long and unwieldy (and frankly, quite boring as well),\n",
+                "so we are not showing it here."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "#p04"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Kinda long, but anyway, let's try to extract the Bernstein bases:"
+                "Instead, we are using it immediately to extract the Bernstein bases:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -1087,15 +1104,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "By now it shouldn't be surprising that the tangent vector at the beginning and end of the curve is parallel to the line\n",
                 "from $\\boldsymbol{x}_0$ to $\\boldsymbol{x}_1$ and\n",
                 "from $\\boldsymbol{x}_3$ to $\\boldsymbol{x}_4$, respectively.\n",
                 "The length of the tangent vectors is four times the length of those lines.\n",
-                "The last line in de Casteljau's algorithm ($\\boldsymbol{p}_{1,4}(t) - \\boldsymbol{p}_{0,3}(t)$ in this case) is exactly a fourth of the tangent vector (at any given $t \\in [0, 1]$):"
+                "The last line in De Casteljau's algorithm ($\\boldsymbol{p}_{1,4}(t) - \\boldsymbol{p}_{0,3}(t)$ in this case) is exactly a fourth of the tangent vector (at any given $t \\in [0, 1]$):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -1155,27 +1172,27 @@
                 "    (1, -0.5),\n",
                 "])"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.2"
+            "version": "3.11.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/euclidean/bezier-non-uniform.ipynb` & `splines-0.3.0/doc/euclidean/bezier-non-uniform.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921066252587991%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, '# Non-Uniform (Cubic) Bézier Splines\\n')], delete: "*

 * *            "[0]}}, 21: {'source': {insert: [(3, '-- i.e. when a non-uniform [Hermite "*

 * *            "spline](hermite.ipynb) is given,\\n')], delete: [3]}}}",*

 * * "'metadata'": "{'kernelspec': {'display_name': 'Python 3 (ipykernel)'}, 'language_info': "*

 * *               "{'version': '3.11.2'}}"}*

```diff
@@ -11,15 +11,15 @@
                 "[back to overview](bezier.ipynb)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Non-Uniform B\u00e9zier Splines\n",
+                "# Non-Uniform (Cubic) B\u00e9zier Splines\n",
                 "\n",
                 "Very commonly,\n",
                 "B\u00e9zier splines are used with a parameter range of $0 \\le t \\le 1$,\n",
                 "which has also been used to derive the basis polynomials and basis matrices in\n",
                 "[the notebook about De Casteljau's algorithm](bezier-de-casteljau.ipynb).\n",
                 "\n",
                 "The parameter range can be re-scaled to any desired parameter range,\n",
@@ -224,15 +224,15 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Control Points From Tangent Vectors\n",
                 "\n",
                 "If the tangent vectors are given in the first place\n",
-                "(i.e. when a non-uniform [Hermite spline](hermite.ipynb) is given),\n",
+                "-- i.e. when a non-uniform [Hermite spline](hermite.ipynb) is given,\n",
                 "the cubic B\u00e9zier control points can be calculated like this:"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -243,27 +243,27 @@
                 "\\boldsymbol{x}_i - \\frac{\\Delta_{i-1} \\boldsymbol{\\dot{x}}_i^{(-)}}{3}\n",
                 "\\end{align*}"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.2"
+            "version": "3.11.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/euclidean/bezier-properties.ipynb` & `splines-0.3.0/doc/euclidean/bezier-properties.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9896765271765272%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'are sometimes used interchangeably for two slightly "*

 * *            "different things:\\n'), (8, '   lie on the curve (at its start and end, "*

 * *            "respectively),\\n')], delete: [8, 3]}}, 2: {'source': {insert: [(0, 'We use the term "*

 * *            "*Bézier curve* for the former\\n'), (1, 'and *Bézier spline* for the latter.\\n')]}}, "*

 * *            "6: {'source': {insert: [(3, '    [(4, 4), (6, 4), (5, 2), (7, 2)],\\n'), (4, '    "*

 * *            "[(7, 2), (8, 0),  […]*

```diff
@@ -14,20 +14,20 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Properties of B\u00e9zier Splines\n",
                 "\n",
                 "The terms *B\u00e9zier spline* and *B\u00e9zier curve*\n",
-                "can mean two slightly different things:\n",
+                "are sometimes used interchangeably for two slightly different things:\n",
                 "\n",
                 "1. A curve constructed from a single Bernstein polynomial of degree $d$,\n",
                 "   given a *control polygon* consisting of a sequence of $d + 1$ vertices.\n",
                 "   The first and last vertex\n",
-                "   lies on the curve (at its start and end, respectively),\n",
+                "   lie on the curve (at its start and end, respectively),\n",
                 "   while the other vertices in general don't\n",
                 "   (the curve *approximates* them).\n",
                 "\n",
                 "2. A piecewise polynomial curve consisting of multiple segments,\n",
                 "   each of them constructed from a separate Bernstein polynomial.\n",
                 "   The start and end points of neighboring control polygons typically coincide,\n",
                 "   leading to $C^0$ continuity.\n",
@@ -35,14 +35,16 @@
                 "   $G^1$ or $C^1$ (or even higher) continuity."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "We use the term *B\u00e9zier curve* for the former\n",
+                "and *B\u00e9zier spline* for the latter.\n",
                 "B\u00e9zier splines in the latter sense are well known\n",
                 "from their common use in 2D vector graphics software,\n",
                 "where cubic (i.e. degree 3) curve segments are typically used.\n",
                 "Each segment has four control points:\n",
                 "The start and end point of the segment\n",
                 "(shared with the end and start of the previous and next segment, respectively)\n",
                 "as well as two additional points that control the shape of the curve segment."
@@ -82,26 +84,26 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "control_points = [\n",
                 "    [(0, 0), (1, 4)],\n",
                 "    [(1, 4), (2, 2), (4, 4)],\n",
-                "    [(4, 4), (6, 4), (5, 2), (6, 2)],\n",
-                "    [(6, 2), (6, 0), (4, 0), (5, 1), (3, 1)],\n",
+                "    [(4, 4), (6, 4), (5, 2), (7, 2)],\n",
+                "    [(7, 2), (8, 0), (4, 0), (5, 1), (3, 1)],\n",
                 "]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We are using the\n",
+                "We are using the class\n",
                 "[splines.Bernstein](../python-module/splines.rst#splines.Bernstein)\n",
-                "class to construct a B\u00e9zier splines from these control points."
+                "to construct a B\u00e9zier spline from these control points."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -132,27 +134,27 @@
                 "ax.plot(*s.evaluate(times).T, 'k.')\n",
                 "ax.axis('equal');"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.2"
+            "version": "3.11.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/euclidean/bezier.ipynb` & `splines-0.3.0/doc/euclidean/bezier.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9876405423280423%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'Named after [Pierre "*

 * *            "Bézier](https://en.wikipedia.org/wiki/Pierre_Bézier),\\n'), (3, 'Bézier curves are "*

 * *            'defined by means of\\n\'), (5, \'<cite data-cite="farouki2012bernstein">(Farouki, '*

 * *            "2012)</cite>,\\n'), (6, 'which are named after\\n'), (7, '[Sergei "*

 * *            "Bernstein](https://en.wikipedia.org/wiki/Sergei_Bernstein).\\n'), (8, 'A popular "*

 * *            'method to evaluate Bézier curves at given parameter values\\n\ […]*

```diff
@@ -13,23 +13,26 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# B\u00e9zier Splines\n",
                 "\n",
-                "Named after [Pierre B\u00e9zier](https://en.wikipedia.org/wiki/Pierre_B%C3%A9zier),\n",
-                "B\u00e9zier splines are defined by means of\n",
+                "Named after [Pierre B\u00e9zier](https://en.wikipedia.org/wiki/Pierre_B\u00e9zier),\n",
+                "B\u00e9zier curves are defined by means of\n",
                 "[Bernstein polynomials](https://en.wikipedia.org/wiki/Bernstein_polynomial)\n",
-                "(which are named after\n",
-                "[Sergei Bernstein](https://en.wikipedia.org/wiki/Sergei_Bernstein)).\n",
-                "A popular method to evaluate B\u00e9zier splines at given parameter values\n",
-                "is [de Casteljau's algorithm](bezier-de-casteljau.ipynb).\n",
+                "<cite data-cite=\"farouki2012bernstein\">(Farouki, 2012)</cite>,\n",
+                "which are named after\n",
+                "[Sergei Bernstein](https://en.wikipedia.org/wiki/Sergei_Bernstein).\n",
+                "A popular method to evaluate B\u00e9zier curves at given parameter values\n",
+                "is [De Casteljau's algorithm](bezier-de-casteljau.ipynb).\n",
                 "A very good online resource with many interactive examples is\n",
-                "*A Primer on B\u00e9zier Curves*: https://pomax.github.io/bezierinfo/.\n",
+                "the website https://pomax.github.io/bezierinfo/.\n",
+                "\n",
+                "B\u00e9zier *splines* are composed of B\u00e9zier *curve* segments.\n",
                 "\n",
                 "A Python implementation is available in the class\n",
                 "[splines.Bernstein](../python-module/splines.rst#splines.Bernstein)."
             ]
         },
         {
             "cell_type": "markdown",
@@ -43,27 +46,27 @@
                 "* [De Casteljau's Algorithm](bezier-de-casteljau.ipynb)\n",
                 "* [Non-Uniform (Cubic) B\u00e9zier Splines](bezier-non-uniform.ipynb)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.2"
+            "version": "3.11.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/euclidean/casteljau.py` & `splines-0.3.0/doc/euclidean/casteljau.py`

 * *Files identical despite different names*

### Comparing `splines-0.2.0/doc/euclidean/catmull-rom-barry-goldman.ipynb` & `splines-0.3.0/doc/euclidean/catmull-rom-barry-goldman.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9829902078940057%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, '-- named after\\n'), (4, '<cite "*

 * *            'data-cite-t="barry1988recursive">Barry and Goldman (1988)</cite> --\\n\')], delete: '*

 * *            '[3]}}, 2: {\'source\': {insert: [(0, \'<cite data-cite-t="catmull1974splines">Catmull '*

 * *            "and Rom (1974)</cite> describe\\n'), (2, '<cite "*

 * *            'data-cite-t="barry1988recursive">Barry and Goldman (1988)</cite> describe\\n\')], '*

 * *            "delete: [2, 0]}}, 3: {'source': {insert: [(12, '> ---<cite "*

 * *  […]*

```diff
@@ -14,28 +14,29 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Barry--Goldman Algorithm\n",
                 "\n",
                 "The *Barry--Goldman algorithm*\n",
-                "(named after *Phillip Barry* and *Ronald Goldman*)\n",
+                "-- named after\n",
+                "<cite data-cite-t=\"barry1988recursive\">Barry and Goldman (1988)</cite> --\n",
                 "can be used to calculate values of\n",
                 "[non-uniform Catmull--Rom splines](catmull-rom-non-uniform.ipynb).\n",
                 "We have also applied this algorithm to\n",
                 "[rotation splines](../rotation/barry-goldman.ipynb)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "<cite data-cite=\"catmull1974splines\">(Catmull and Rom, 1974)</cite> describes\n",
+                "<cite data-cite-t=\"catmull1974splines\">Catmull and Rom (1974)</cite> describe\n",
                 "\"a class of local interpolating splines\" and\n",
-                "<cite data-cite=\"barry1988recursive\">(Barry and Goldman, 1988)</cite> describes\n",
+                "<cite data-cite-t=\"barry1988recursive\">Barry and Goldman (1988)</cite> describe\n",
                 "\"a recursive evaluation algorithm for a class of Catmull\u2013Rom splines\",\n",
                 "by which they mean a sub-class of the original class,\n",
                 "which only contains splines generated from a combination of\n",
                 "[Lagrange interpolation](lagrange.ipynb) and B-spline blending:"
             ]
         },
         {
@@ -50,15 +51,15 @@
                 "interpolating polynomials.\n",
                 "> [...]\n",
                 "> They are\n",
                 "piecewise polynomial, have local support, are invariant under affine\n",
                 "transformations, and have certain differentiability and interpolatory\n",
                 "properties.\n",
                 ">\n",
-                "> ---<cite data-cite=\"barry1988recursive\">Barry and Goldman (1988)</cite>, section 1: \"Introduction\""
+                "> ---<cite data-cite-t=\"barry1988recursive\">Barry and Goldman (1988)</cite>, section 1: \"Introduction\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The algorithm can be set up to construct curves of arbitrary degree\n",
@@ -73,15 +74,15 @@
             "metadata": {},
             "source": [
                 "The algorithm is a combination of two sub-algorithms:\n",
                 "\n",
                 "> The Catmull--Rom evaluation algorithm is constructed by combining the de Boor algorithm for evaluating B-spline curves with Neville's algorithm for evaluating Lagrange\n",
                 "polynomials.\n",
                 ">\n",
-                "> ---<cite data-cite=\"barry1988recursive\">Barry and Goldman (1988)</cite>, abstract"
+                "> ---<cite data-cite-t=\"barry1988recursive\">Barry and Goldman (1988)</cite>, abstract"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Combining the two will lead to a multi-stage algorithm,\n",
@@ -100,16 +101,16 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Triangular Schemes\n",
                 "\n",
-                "In <cite data-cite=\"barry1988recursive\">(Barry and Goldman, 1988)</cite>,\n",
-                "the presented algorithms are illustrated\n",
+                "<cite data-cite-t=\"barry1988recursive\">Barry and Goldman (1988)</cite>\n",
+                "illustrate the presented algorithms\n",
                 "using triangular evaluation patterns,\n",
                 "which we will use here in a very similar form.\n",
                 "\n",
                 "As an example, let's look at the most basic building block:\n",
                 "linear interpolation between two given points\n",
                 "(in this case $\\boldsymbol{x}_4$ and $\\boldsymbol{x}_5$\n",
                 "with corresponding parameter values $t_4$ and $t_5$, respectively):\n",
@@ -178,21 +179,19 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Neville's Algorithm\n",
                 "\n",
                 "We have already seen this algorithm in our\n",
-                "[notebook about Lagrange interpolation](lagrange.ipynb)."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "[notebook about Lagrange interpolation](lagrange.ipynb#Neville's-Algorithm),\n",
+                "where we have shown the triangular scheme for the *cubic* case\n",
+                "-- which is also shown by\n",
+                "<cite data-cite-t=\"barry1988recursive\">Barry and Goldman (1988)</cite>\n",
+                "in figure 2.\n",
                 "In the *quadratic* case, it looks like this:\n",
                 "\n",
                 "\\begin{equation*}\n",
                 "\\begin{array}{ccccccccc}\n",
                 "&&&&\n",
                 "\\boldsymbol{p}_{3,4,5}\n",
                 "&&&&\n",
@@ -210,22 +209,14 @@
                 "\\\\\n",
                 "\\boldsymbol{x}_{3} &&&& \\boldsymbol{x}_{4} &&&& \\boldsymbol{x}_{5}\n",
                 "\\end{array}\n",
                 "\\end{equation*}"
             ]
         },
         {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "The *cubic* case is shown in figure 2 of\n",
-                "<cite data-cite=\"barry1988recursive\">(Barry and Goldman, 1988)</cite>."
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np"
@@ -297,16 +288,15 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## De Boor's Algorithm\n",
                 "\n",
                 "This algorithm\n",
-                "(named after [Carl de Boor](https://en.wikipedia.org/wiki/Carl_R._de_Boor),\n",
-                "see <cite data-cite=\"de_boor1972calculating\">(de Boor, 1972)</cite>)\n",
+                "<cite data-cite=\"de_boor1972calculating\">(de Boor 1972)</cite>\n",
                 "can be used to calculate B-spline basis functions.\n",
                 "\n",
                 "The quadratic case looks like this:\n",
                 "\n",
                 "\\begin{equation*}\n",
                 "\\begin{array}{ccccccccc}\n",
                 "&&&&\n",
@@ -329,16 +319,17 @@
                 "\\end{equation*}"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The *cubic* case shown in figure 1 of\n",
-                "<cite data-cite=\"barry1988recursive\">(Barry and Goldman, 1988)</cite>."
+                "The *cubic* case is shown by\n",
+                "<cite data-cite-t=\"barry1988recursive\">Barry and Goldman (1988)</cite>\n",
+                "in figure 1."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -354,16 +345,16 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Combining Both Algorithms\n",
                 "\n",
-                "Figure 5 of <cite data-cite=\"catmull1974splines\">(Catmull and Rom, 1974)</cite>\n",
-                "shows an example where linear interpolation is followed by\n",
+                "<cite data-cite-t=\"catmull1974splines\">Catmull and Rom (1974)</cite>\n",
+                "show (in figure 5) an example where linear interpolation is followed by\n",
                 "quadratic B-spline blending to create a cubic curve.\n",
                 "\n",
                 "We can re-create this example with the building blocks from above:\n",
                 "\n",
                 "* At the base of the triangle, we put four known vertices.\n",
                 "* Consecutive pairs of these vertices form three linear interpolations\n",
                 "  (and *extra*polations),\n",
@@ -435,36 +426,37 @@
                 "$t_3$ and $t_6$, respectively."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This same triangular scheme is also shown in figure 3 of\n",
-                "<cite data-cite=\"yuksel2011parameterization\">(Yuksel et al., 2011)</cite>,\n",
+                "This same triangular scheme is also shown by\n",
+                "<cite data-cite-t=\"yuksel2011parameterization\">Yuksel et al. (2011)</cite>\n",
+                "in figure 3,\n",
                 "except that here we shifted the indices by $+3$."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Another way to construct a cubic curve with this algorithm\n",
-                "would be to flip the degrees of interpolation and blending,\n",
+                "would be to swap the degrees of interpolation and blending,\n",
                 "in other words:\n",
                 "\n",
                 "* Instead of three linear interpolations (and extrapolations),\n",
                 "  apply two overlapping quadratic Lagrange interpolations\n",
                 "  using Neville's algorithm (as shown above) to\n",
                 "  $\\boldsymbol{x}_3$, $\\boldsymbol{x}_4$, $\\boldsymbol{x}_5$ and\n",
                 "  $\\boldsymbol{x}_4$, $\\boldsymbol{x}_5$, $\\boldsymbol{x}_6$, respectively.\n",
                 "  Note that the interpolation of $\\boldsymbol{x}_4$ and $\\boldsymbol{x}_5$\n",
                 "  appears in both triangles but has to be calculated only once\n",
-                "  (see also figures 3 and 4 in\n",
-                "  <cite data-cite=\"barry1988recursive\">(Barry and Goldman, 1988)</cite>).\n",
+                "  -- see also figures 3 and 4 by\n",
+                "  <cite data-cite-t=\"barry1988recursive\">Barry and Goldman (1988)</cite>.\n",
                 "* This will occupy the lower two stages of the triangle,\n",
                 "  yielding two interpolated values.\n",
                 "* Those two values are then linearly blended in the final stage."
             ]
         },
         {
             "cell_type": "markdown",
@@ -478,30 +470,31 @@
                 "and therefore they are equivalent!"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The same scheme, but only for the *uniform* case, is also shown in figure 7 of\n",
-                "<cite data-cite=\"barry1988recursive\">(Barry and Goldman, 1988)</cite>,\n",
+                "The same scheme, but only for the *uniform* case, is also shown by\n",
+                "<cite data-cite-t=\"barry1988recursive\">Barry and Goldman (1988)</cite>\n",
+                "in figure 7,\n",
                 "which casually mentions the equivalent cases\n",
                 "(with $m$ being the degree of Lagrange interpolation\n",
                 "and $n$ being the degree of the B-spline basis functions):"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "> Note too from Figure 7 that the case\n",
                 "$n=1$, $m=2$ [...] is identical to the case\n",
                 "$n=2$, $m=1$ [...]\n",
                 ">\n",
-                "> ---<cite data-cite=\"barry1988recursive\">Barry and Goldman (1988)</cite>, section 3: \"Examples\""
+                "> ---<cite data-cite-t=\"barry1988recursive\">Barry and Goldman (1988)</cite>, section 3: \"Examples\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "<div class=\"alert alert-warning\">\n",
@@ -509,20 +502,20 @@
                 "Not an Overhauser Spline\n",
                 "\n",
                 "Equally casually, they mention:\n",
                 "\n",
                 "> Finally, the particular case here is also an Overhauser spline\n",
                 "> <cite data-cite=\"overhauser1968parabolic\">(Overhauser, 1968)</cite>.\n",
                 ">\n",
-                "> ---<cite data-cite=\"barry1988recursive\">Barry and Goldman (1988)</cite>, section 3: \"Examples\"\n",
+                "> ---<cite data-cite-t=\"barry1988recursive\">Barry and Goldman (1988)</cite>, section 3: \"Examples\"\n",
                 "\n",
                 "This is not true.\n",
                 "Overhauser splines\n",
-                "-- as described in\n",
-                "<cite data-cite=\"overhauser1968parabolic\">(Overhauser, 1968)</cite> --\n",
+                "-- as described by\n",
+                "<cite data-cite-t=\"overhauser1968parabolic\">Overhauser (1968)</cite> --\n",
                 "don't provide a choice of parameter values.\n",
                 "The parameter values are determined\n",
                 "by the Euclidean distances between control points,\n",
                 "similar, but not quite identical to\n",
                 "[chordal parameterization](catmull-rom-properties.ipynb#Chordal-Parameterization).\n",
                 "Calculating a value of a Catmull--Rom spline doesn't involve calculating any distances.\n",
                 "\n",
@@ -535,36 +528,38 @@
             "source": [
                 "For completeness' sake,\n",
                 "there are two more combinations that lead to cubic splines,\n",
                 "but they have their limitations:\n",
                 "\n",
                 "* Cubic Lagrange interpolation, followed by no blending at all,\n",
                 "  which leads to a cubic spline that's not $C^1$ continuous (only $C^0$),\n",
-                "  as shown in figure 8 of\n",
-                "  <cite data-cite=\"barry1988recursive\">(Barry and Goldman, 1988)</cite>.\n",
+                "  as shown by\n",
+                "  <cite data-cite-t=\"barry1988recursive\">Barry and Goldman (1988)</cite>\n",
+                "  in figure 8.\n",
                 "* No interpolation at all, followed by cubic B-spline blending,\n",
                 "  which leads to an approximating spline (instead of an interpolating spline),\n",
-                "  as shown in figure 5 of\n",
-                "  <cite data-cite=\"barry1988recursive\">(Barry and Goldman, 1988)</cite>."
+                "  as shown by\n",
+                "  <cite data-cite-t=\"barry1988recursive\">Barry and Goldman (1988)</cite>\n",
+                "  in figure 5."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "<div class=\"alert alert-info\">\n",
                 "\n",
                 "Note\n",
                 "\n",
                 "Here we are using the time instances of the Lagrange interpolation\n",
                 "also as B-spline knots.\n",
-                "Equation (9) of\n",
-                "<cite data-cite=\"barry1988recursive\">(Barry and Goldman, 1988)</cite>\n",
-                "shows a more generic formulation of the algorithm\n",
-                "with separate parameters $s_i$ and $t_i$.\n",
+                "<cite data-cite-t=\"barry1988recursive\">Barry and Goldman (1988)</cite>\n",
+                "show a more generic formulation of the algorithm\n",
+                "with separate parameters $s_i$ and $t_i$\n",
+                "in equation (9).\n",
                 "\n",
                 "</div>"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -879,72 +874,49 @@
                 "p3456"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This time, the interpolation interval is exactly the one we care about.\n",
+                "This time, the interpolation interval is exactly the one we are interested in.\n",
                 "\n",
                 "To get the final result, we just have to combine all the above expressions:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "p3456 = p3456.subs_symbols(p345, p456, p34, p45, p56).simplify()\n",
-                "p3456"
+                "p3456 = p3456.subs_symbols(p345, p456, p34, p45, p56).simplify()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We can make this marginally shorter\n",
-                "if we rewrite the segment durations as\n",
-                "$\\Delta_i = t_{i+1} - t_i$:"
+                "This expression is quite unwieldy, so let's not even look at it."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "delta3, delta4, delta5 = sp.symbols('Delta3:6')\n",
-                "deltas = {\n",
-                "    t4 - t3: delta3,\n",
-                "    t5 - t4: delta4,\n",
-                "    t6 - t5: delta5,\n",
-                "    t5 - t3: delta3 + delta4,\n",
-                "    t6 - t4: delta4 + delta5,\n",
-                "    t6 - t3: delta3 + delta4 + delta5,\n",
-                "    # A few special cases that SymPy has a hard time resolving:\n",
-                "    t4 + t4 - t3: t4 + delta3,\n",
-                "    t6 + t6 - t3: t6 + delta3 + delta4 + delta5,\n",
-                "}"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "p3456.subs(deltas)"
+                "#p3456"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Apart from checking if it's really cubic ..."
+                "Apart from checking whether it's really cubic ..."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -952,15 +924,15 @@
                 "sp.degree(p3456.expr, t)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "... and if it's really interpolating ..."
+                "... and whether it's really interpolating ..."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -1041,34 +1013,27 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Animation\n",
                 "\n",
                 "The linear interpolations (and *extra*polations) of this algorithm\n",
                 "can be shown graphically.\n",
-                "By means of the file [barry_goldman.py](barry_goldman.py),\n",
-                "we can generate an animation of the algorithm:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from barry_goldman import animation"
+                "By means of the file [barry_goldman.py](barry_goldman.py)\n",
+                "-- and with the help of [helper.py](helper.py) --\n",
+                "we can show an animation of the algorithm:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from IPython.display import HTML"
+                "from barry_goldman import animation\n",
+                "from helper import show_animation"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -1097,24 +1062,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ani = animation(vertices, times)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "HTML(ani.to_jshtml(default_mode='reflect'))"
+                "show_animation(animation(vertices, times))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "If this doesn't look very intuitive to you,\n",
@@ -1123,27 +1079,27 @@
                 "have a look at the\n",
                 "[notebook about non-uniform Catmull--Rom splines](catmull-rom-non-uniform.ipynb#Animation)."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.2"
+            "version": "3.11.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/euclidean/catmull-rom-non-uniform.ipynb` & `splines-0.3.0/doc/euclidean/catmull-rom-non-uniform.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9629093950857344%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(2, \'<cite data-cite-t="catmull1974splines">Catmull and '*

 * *            "Rom (1974)</cite>\\n'), (3, 'describe only the [uniform "*

 * *            "case](catmull-rom-uniform.ipynb),\\n'), (4, 'but it is straightforward to extend "*

 * *            "their method to non-uniform splines.\\n')], delete: [4, 3, 2]}}, 2: {'source': "*

 * *            "{insert: [(4, 'the respective degrees can be swapped.\\n')], delete: [4]}}, 3: "*

 * *            "{'source': {insert: [(0, 'Since the latter is […]*

```diff
@@ -13,17 +13,17 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Non-Uniform Catmull--Rom Splines\n",
                 "\n",
-                "<cite data-cite=\"catmull1974splines\">Catmull and Rom (1974)</cite>\n",
-                "describes only the [uniform case](catmull-rom-uniform.ipynb),\n",
-                "but it is straightforward to extend the method to non-uniform splines.\n",
+                "<cite data-cite-t=\"catmull1974splines\">Catmull and Rom (1974)</cite>\n",
+                "describe only the [uniform case](catmull-rom-uniform.ipynb),\n",
+                "but it is straightforward to extend their method to non-uniform splines.\n",
                 "\n",
                 "The method creates three linear interpolations\n",
                 "(and *extra*polations)\n",
                 "between neighboring pairs of the four relevant control points\n",
                 "and then blends the three resulting points\n",
                 "with a quadratic B-spline basis function."
             ]
@@ -32,40 +32,37 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "As we have seen in the\n",
                 "[notebook about uniform Catmull--Rom splines](catmull-rom-uniform.ipynb#Cardinal-Functions)\n",
                 "and as we will again see in the\n",
                 "[notebook about the Barry--Goldman algorithm](catmull-rom-barry-goldman.ipynb#Combining-Both-Algorithms),\n",
-                "the respective degrees can be reversed.\n",
+                "the respective degrees can be swapped.\n",
                 "This means that equivalently,\n",
                 "two (overlapping) quadratic Lagrange interpolations can be used,\n",
                 "followed by linearly blending the two resulting points."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Since latter is both easier to implement\n",
+                "Since the latter is both easier to implement\n",
                 "and easier to wrap one's head around,\n",
-                "we use it in the following derivations."
+                "we'll use it in the following derivations."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We will derive\n",
-                "the [tangent vectors](#Tangent-Vectors) at the segment boundaries\n",
-                "(which will serve as basis for deriving\n",
-                "[non-uniform Kochanek--Bartels splines](kochanek-bartels-non-uniform.ipynb)\n",
-                "later)\n",
-                "and\n",
-                "the [basis matrix](#Basis-Matrix).\n",
+                "the [tangent vectors](#Tangent-Vectors) at the segment boundaries,\n",
+                "which will later serve as a starting point for deriving\n",
+                "[non-uniform Kochanek--Bartels splines](kochanek-bartels-non-uniform.ipynb).\n",
                 "See the\n",
                 "[notebook about the Barry--Goldman algorithm](catmull-rom-barry-goldman.ipynb)\n",
                 "for an alternative (but closely related) derivation."
             ]
         },
         {
             "cell_type": "code",
@@ -74,14 +71,22 @@
             "outputs": [],
             "source": [
                 "import sympy as sp\n",
                 "sp.init_printing()"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "As usual, we look at the fifth polynomial segment $\\boldsymbol{p}_4(t)$\n",
+                "from $\\boldsymbol{x}_4$ to $\\boldsymbol{x}_5$, where $t_4 \\le t \\le t_5$.\n"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "x3, x4, x5, x6 = sp.symbols('xbm3:7')"
             ]
@@ -146,15 +151,16 @@
                 "def neville(xs, ts, t):\n",
                 "    \"\"\"Lagrange interpolation using Neville's algorithm.\n",
                 "    \n",
                 "    Returns the interpolated value at time *t*,\n",
                 "    given the values *xs* at times *ts*.\n",
                 "    \n",
                 "    \"\"\"\n",
-                "    assert len(xs) == len(ts)\n",
+                "    if len(xs) != len(ts):\n",
+                "        raise ValueError('xs and ts must have the same length')\n",
                 "    while len(xs) > 1:\n",
                 "        step = len(ts) - len(xs) + 1\n",
                 "        xs = [\n",
                 "            lerp(*args, t)\n",
                 "            for args in zip(zip(xs, xs[1:]), zip(ts, ts[step:]))]\n",
                 "    return xs[0]"
             ]
@@ -212,23 +218,14 @@
                 "this doesn't really matter\n",
                 "because the redundant expressions should be simplified away by SymPy.\n",
                 "\n",
                 "</div>"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "p4.simplify()"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The following expressions can be simplified\n",
                 "by introducing a few new symbols $\\Delta_i$:"
             ]
         },
@@ -430,15 +427,15 @@
                 "$\\boldsymbol{v}_i = \\frac{\\boldsymbol{x}_{i+1} - \\boldsymbol{x}_i}{\\Delta_i}$."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "<cite data-cite=\"de_boor1978splines\">(de Boor 1978)</cite>\n",
+                "<cite data-cite-t=\"de_boor1978splines\">Boor (1978)</cite>\n",
                 "calls this *piecewise cubic Bessel interpolation*,\n",
                 "and it has also been called\n",
                 "*Bessel tangent method*,\n",
                 "*Overhauser method* and\n",
                 "*Bessel--Overhauser splines*."
             ]
         },
@@ -448,17 +445,17 @@
             "source": [
                 "<div class=\"alert alert-info\">\n",
                 "\n",
                 "Note\n",
                 "\n",
                 "Even though this formula\n",
                 "is commonly associated with the name *Overhauser*,\n",
-                "it is *not* describing the tangents of *Overhauser splines*\n",
-                "(as presented in\n",
-                "<cite data-cite=\"overhauser1968parabolic\">Overhauser (1968)</cite>).\n",
+                "it does *not* describe the tangents of *Overhauser splines*\n",
+                "as presented by\n",
+                "<cite data-cite-t=\"overhauser1968parabolic\">Overhauser (1968)</cite>.\n",
                 "\n",
                 "</div>"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -502,15 +499,15 @@
                 "assert sp.simplify(_ - end_tangent.expr) == 0"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "You might encounter another way\n",
+                "You might encounter yet another way\n",
                 "to write the equation for $\\boldsymbol{\\dot{x}}_4$\n",
                 "(e.g. at https://stackoverflow.com/a/23980479/) ..."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -604,34 +601,202 @@
             "metadata": {},
             "source": [
                 "This is again using $\\Delta_i = t_{i+1} - t_i$ and\n",
                 "$\\boldsymbol{v}_i = \\frac{\\boldsymbol{x}_{i+1} - \\boldsymbol{x}_i}{\\Delta_i}$."
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "x4tilde = x4 + (t5 - t4) * start_tangent.expr / 3"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "x5tilde = x5 - (t5 - t4) * end_tangent.expr / 3"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "## Using Non-Uniform Quadrangle Interpolation\n",
+                "\n",
+                "Just like in [the uniform case](catmull-rom-uniform.ipynb#Using-Quadrangle-Interpolation),\n",
+                "we calculate the quadrangle points\n",
+                "from the B\u00e9zier control points,\n",
+                "as shown in the\n",
+                "[notebook about quadrangle interpolation](quadrangle.ipynb):\n",
+                "\n",
+                "\\begin{align*}\n",
+                "\\boldsymbol{\\bar{x}}_i^{(+)} &=\n",
+                "\\frac{3}{2} \\boldsymbol{\\tilde{x}}_i^{(+)} -\n",
+                "\\frac{1}{2} \\boldsymbol{x}_{i+1}\\\\\n",
+                "\\boldsymbol{\\bar{x}}_i^{(-)} &=\n",
+                "\\frac{3}{2} \\boldsymbol{\\tilde{x}}_i^{(-)} -\n",
+                "\\frac{1}{2} \\boldsymbol{x}_{i-1}\n",
+                "\\end{align*}"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "x4bar = 3 * x4tilde / 2 - x5 / 2"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "terms4 = sp.collect(x4bar.expand(), [x3, x4, x5], evaluate=False)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Some manual rewriting leads to this expression:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "sp.factor(terms4[x4] + terms4[x5] + terms4[x3]) * x4 - (\n",
+                "    sp.factor(-terms4[x5]) * (x5 - x4) +\n",
+                "    sp.factor(-terms4[x3]) * (x3 - x4))"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "We should make sure that our re-written expression\n",
+                "is actually the same as the one we started from:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "assert sp.simplify(_ - x4bar) == 0"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Now the same for the incoming quadrangle point:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "x5bar = 3 * x5tilde / 2 - x4 / 2"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "terms5 = sp.collect(x5bar.expand(), [x4, x5, x6], evaluate=False)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "sp.factor(terms5[x5] + terms5[x6] + terms5[x4]) * x5 - (\n",
+                "    sp.factor(-terms5[x6]) * (x6 - x5) +\n",
+                "    sp.factor(-terms5[x4]) * (x4 - x5))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "assert sp.simplify(_ - x5bar) == 0"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The above expressions can be generalized to\n",
+                "(as always with $\\Delta_i = t_{i+1} - t_i$):\n",
+                "\n",
+                "\\begin{align*}\n",
+                "\\boldsymbol{\\bar{x}}_i^{(+)} &=\n",
+                "\\boldsymbol{x}_i -\n",
+                "\\frac{\\Delta_i}{2 (\\Delta_{i-1} + \\Delta_i)}\n",
+                "\\left(\n",
+                "(\\boldsymbol{x}_{i+1} - \\boldsymbol{x}_i)\n",
+                "+\n",
+                "\\frac{\\Delta_i}{\\Delta_{i-1}} (\\boldsymbol{x}_{i-1} - \\boldsymbol{x}_i)\n",
+                "\\right)\\\\\n",
+                "\\boldsymbol{\\bar{x}}_i^{(-)} &=\n",
+                "\\boldsymbol{x}_i -\n",
+                "\\frac{\\Delta_{i-1}}{2 (\\Delta_{i-1} + \\Delta_i)}\n",
+                "\\left(\n",
+                "\\frac{\\Delta_{i-1}}{\\Delta_i} (\\boldsymbol{x}_{i+1} - \\boldsymbol{x}_i)\n",
+                "+\n",
+                "(\\boldsymbol{x}_{i-1} - \\boldsymbol{x}_i)\n",
+                "\\right)\n",
+                "\\end{align*}"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "tags": []
+            },
+            "source": [
                 "## Animation\n",
                 "\n",
-                "To illustrate how two quadratic Lagrange interpolations\n",
+                "To illustrate what two quadratic Lagrange interpolations\n",
                 "followed by linear blending\n",
                 "might look like,\n",
                 "we can generate an animation\n",
-                "by means of the file [catmull_rom.py](catmull_rom.py):"
+                "by means of the file [catmull_rom.py](catmull_rom.py),\n",
+                "with some help from [helper.py](helper.py):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from catmull_rom import animation_2_1, animation_1_2\n",
-                "from IPython.display import HTML"
+                "from helper import show_animation"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -660,54 +825,36 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ani_2_1 = animation_2_1(vertices, times)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "HTML(ani_2_1.to_jshtml(default_mode='reflect'))"
+                "show_animation(animation_2_1(vertices, times))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "In the beginning of this notebook\n",
+                "In the beginning of this notebook,\n",
                 "we claimed that two quadratic interpolations\n",
                 "followed by linear blending are easier to understand.\n",
-                "To prove this, let's have a look at how\n",
+                "To prove this, let's have a look at what\n",
                 "three linear interpolations (and *extra*polations)\n",
                 "followed by quadratic B-spline blending would look like:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ani_1_2 = animation_1_2(vertices, times)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "HTML(ani_1_2.to_jshtml(default_mode='reflect'))"
+                "show_animation(animation_1_2(vertices, times))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Would you agree that this is less straightforward?\n",
@@ -717,27 +864,27 @@
                 "take a look at\n",
                 "[the notebook about the Barry--Goldman algorithm](catmull-rom-barry-goldman.ipynb#Animation)."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.11.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/euclidean/catmull-rom-properties.ipynb` & `splines-0.3.0/doc/euclidean/catmull-rom-properties.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9595754927825635%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(2, \'<cite data-cite-t="catmull1974splines">Catmull and '*

 * *            "Rom (1974)</cite>\\n'), (3, 'present a whole class of splines with a whole range of "*

 * *            "properties.\\n'), (9, 'This type of spline is very popular because they are very easy "*

 * *            "to use.\\n'), (10, 'Only a sequence of control points has to be specified, the "*

 * *            "corresponding tangents are calculated automatically from the given points.\\n')], "*

 * *            "delete: [ […]*

```diff
@@ -13,23 +13,23 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Properties of Catmull--Rom Splines\n",
                 "\n",
-                "<cite data-cite=\"catmull1974splines\">Catmull and Rom (1974)</cite>\n",
-                "presents a whole class of splines with a whole range of properties.\n",
+                "<cite data-cite-t=\"catmull1974splines\">Catmull and Rom (1974)</cite>\n",
+                "present a whole class of splines with a whole range of properties.\n",
                 "Here we only consider one member of this class which is\n",
                 "a cubic polynomial interpolating spline with $C^1$ continuity and local support.\n",
                 "Nowadays, this specific case is typically simply referred to as\n",
                 "*Catmull--Rom spline*.\n",
                 "\n",
-                "This type of splines is very popular because they are very easy to use.\n",
-                "Only a sequence of control points has to be specified, the tangents are calculated automatically from the given points.\n",
+                "This type of spline is very popular because they are very easy to use.\n",
+                "Only a sequence of control points has to be specified, the corresponding tangents are calculated automatically from the given points.\n",
                 "Using those tangents, the spline can be implemented using\n",
                 "cubic [Hermite splines](hermite.ipynb).\n",
                 "Alternatively, spline values can be directly calculated\n",
                 "with the [Barry--Goldman algorithm](catmull-rom-barry-goldman.ipynb).\n",
                 "\n",
                 "To calculate the spline values between two control points,\n",
                 "the preceding and the following control points are needed as well.\n",
@@ -293,14 +293,21 @@
                 "\\end{equation*}"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "## Wrong Tangent Vectors"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "Some sources provide a simpler equation\n",
                 "which is different from the tangent vector of a Catmull--Rom spline\n",
                 "(except in the uniform case):\n",
                 "\n",
                 "\\begin{equation*}\n",
                 "\\boldsymbol{\\dot{x}}_i\n",
                 "\\overset{?}{=}\n",
@@ -310,29 +317,247 @@
                 "\\frac{\\boldsymbol{x}_i - \\boldsymbol{x}_{i-1}}{t_i - t_{i-1}} +\n",
                 "\\frac{\\boldsymbol{x}_{i + 1} - \\boldsymbol{x}_i}{t_{i + 1} - t_i}\n",
                 "\\right)\n",
                 "\\end{equation*}"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "class MeanVelocity(splines.CatmullRom):\n",
+                "    \n",
+                "    @staticmethod\n",
+                "    def _calculate_tangent(points, times):\n",
+                "        x_1, x0, x1 = np.asarray(points)\n",
+                "        t_1, t0, t1 = times\n",
+                "        v_1 = (x0 - x_1) / (t0 - t_1)\n",
+                "        v0 = (x1 - x0) / (t1 - t0)\n",
+                "        return (v_1 + v0) / 2"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "There are even sources\n",
-                "(e.g. [Wikipedia](https://en.wikipedia.org/wiki/Cubic_Hermite_spline#Catmull%E2%80%93Rom_spline))\n",
-                "which show yet a simpler equation,\n",
-                "which has even less to do with Catmull--Rom splines\n",
-                "(except in the uniform case):\n",
+                "[Wikipedia](https://en.wikipedia.org/wiki/Cubic_Hermite_spline#Catmull\u2013Rom_spline)\n",
+                "shows yet a simpler equation.\n",
+                "They mention that \"this assumes uniform parameter spacing\",\n",
+                "but since $t_{i - 1}$ and $t_{i + 1}$ appear in the equation,\n",
+                "it might be tempting to use it\n",
+                "for the non-uniform case as well.\n",
+                "We'll see below how that turns out.\n",
+                "\n",
+                "The authors of the page don't seem to be quite sure about this equation,\n",
+                "because it has changed over time.\n",
+                "This was\n",
+                "[shown until mid-2021](https://web.archive.org/web/20210420082245/https://en.wikipedia.org/wiki/Cubic_Hermite_spline#Catmull\u2013Rom_spline):\n",
                 "\n",
                 "\\begin{equation*}\n",
                 "\\boldsymbol{\\dot{x}}_i \\overset{?}{=} \\frac{\\boldsymbol{x}_{i + 1} - \\boldsymbol{x}_{i - 1}}{t_{i + 1} - t_{i - 1}}\n",
                 "\\end{equation*}"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "class Wikipedia1(splines.CatmullRom):\n",
+                "    \n",
+                "    @staticmethod\n",
+                "    def _calculate_tangent(points, times):\n",
+                "        x_1, _, x1 = np.asarray(points)\n",
+                "        t_1, _, t1 = times\n",
+                "        return (x1 - x_1) / (t1 - t_1)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "And this slight variation was [shown since then](https://web.archive.org/web/20210727071020/https://en.wikipedia.org/wiki/Cubic_Hermite_spline#Catmull\u2013Rom_spline):\n",
+                "\n",
+                "\\begin{equation*}\n",
+                "\\boldsymbol{\\dot{x}}_i \\overset{?}{=} \\frac{1}{2}\\frac{\\boldsymbol{x}_{i + 1} - \\boldsymbol{x}_{i - 1}}{t_{i + 1} - t_{i - 1}}\n",
+                "\\end{equation*}"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "class Wikipedia2(splines.CatmullRom):\n",
+                "    \n",
+                "    @staticmethod\n",
+                "    def _calculate_tangent(points, times):\n",
+                "        x_1, _, x1 = np.asarray(points)\n",
+                "        t_1, _, t1 = times\n",
+                "        return (1/2) * (x1 - x_1) / (t1 - t_1)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The first one is correct in the uniform case\n",
+                "(which the Wikipedia page assumes),\n",
+                "but not in the general non-uniform case, as we'll see in a moment."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The second one is obviously wrong in the case where all intervals are\n",
+                "of length $1$ (i.e. $t_{i+1} - t_i = t_i - t_{i-1} = 1$):\n",
+                "\n",
+                "\\begin{equation*}\n",
+                "\\frac{\\boldsymbol{x}_{i + 1} - \\boldsymbol{x}_{i - 1}}{4}\n",
+                "\\ne\n",
+                "\\frac{\\boldsymbol{x}_{i + 1} - \\boldsymbol{x}_{i - 1}}{2}\n",
+                "= \\boldsymbol{\\dot{x}}_i\n",
+                "\\end{equation*}"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The\n",
+                "[X3D standard (version 3.3)](https://www.web3d.org/documents/specifications/19775-1/V3.3/Part01/components/interp.html#HermiteSplineInterpolation)\n",
+                "even suggests to use different incoming and outgoing tangents,\n",
+                "which destroys $C^1$ continuity!"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "\\begin{align*}\n",
+                "\\boldsymbol{\\dot{x}}_i^{(+)} &\\overset{?}{=} \\frac{\n",
+                "(t_i - t_{i-1}) (\\boldsymbol{x}_{i+1} - \\boldsymbol{x}_{i-1})\n",
+                "}{\n",
+                "t_{i+1} - t_{i-1}\n",
+                "}\\\\\n",
+                "\\boldsymbol{\\dot{x}}_i^{(-)} &\\overset{?}{=} \\frac{\n",
+                "(t_{i+1} - t_i) (\\boldsymbol{x}_{i+1} - \\boldsymbol{x}_{i-1})\n",
+                "}{\n",
+                "t_{i+1} - t_{i-1}\n",
+                "}\n",
+                "\\end{align*}"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "class X3D(splines.KochanekBartels):\n",
+                "    # We derive from KochanekBartels because the\n",
+                "    # incoming and outgoing tangents are different:\n",
+                "    @staticmethod\n",
+                "    def _calculate_tangents(points, times, _ignored):\n",
+                "        x_1, _, x1 = np.asarray(points)\n",
+                "        t_1, t0, t1 = times\n",
+                "        incoming = (t1 - t0) * (x1 - x_1) / (t1 - t_1)\n",
+                "        outgoing = (t0 - t_1) * (x1 - x_1) / (t1 - t_1)\n",
+                "        return incoming, outgoing"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "To illustrate the different choices of tangent vectors,\n",
+                "we use the vertex data from\n",
+                "<cite data-cite-t=\"lee1989choosing\">Lee (1989)</cite>, figure 6:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "points3 = [\n",
+                "    (0, 0),\n",
+                "    (10, 25),\n",
+                "    (10, 24),\n",
+                "    (11, 24.5),\n",
+                "    (33, 25),\n",
+                "]"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Deciding between \"right\" and \"wrong\" tangent vectors is surprisingly hard,\n",
+                "because most of the options look somewhat reasonable in most cases.\n",
+                "However, we can try to use quite extreme vertex positions\n",
+                "and we can use *centripetal parameterization* (see below)\n",
+                "and check if its guaranteed properties hold\n",
+                "for different choices of tangent vectors."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "def plot_spline(cls, linestyle='-', **args):\n",
+                "    # alpha=0.5 => centripetal parameterization\n",
+                "    spline = cls(points3, alpha=0.5)\n",
+                "    plot_spline_2d(\n",
+                "        spline, label=cls.__name__, chords=False,\n",
+                "        marker=None, linestyle=linestyle, **args)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "plot_spline(MeanVelocity, linestyle=':')\n",
+                "plot_spline(X3D, linestyle='-.')\n",
+                "plot_spline(Wikipedia1)\n",
+                "plot_spline(Wikipedia2, linestyle='--')\n",
+                "plot_spline(splines.CatmullRom, linewidth=3)\n",
+                "plt.axis([9, 13, 23.9, 25.6])\n",
+                "plt.legend();"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "As we can immediately see,\n",
+                "the tangents from X3D are utterly wrong\n",
+                "and the first one from Wikipedia is also quite obviously broken.\n",
+                "The other two don't look too bad,\n",
+                "but they slightly overshoot,\n",
+                "and according to\n",
+                "<cite data-cite-t=\"yuksel2011parameterization\">Yuksel et al. (2011)</cite>\n",
+                "that is something that centripetal Catmull--Rom splines are guaranteed not to do.\n",
+                "\n",
+                "Again, to be fair to the Wikipedia article's authors,\n",
+                "they mention that uniform parameter spacing is assumed,\n",
+                "so their equation is not supposed to be used in this non-uniform context."
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Cusps and Self-Intersections\n",
                 "\n",
                 "Uniform parametrization typically works very well\n",
                 "if the (Euclidean) distances between consecutive vertices are all similar.\n",
@@ -355,15 +580,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "points3 = [\n",
+                "points4 = [\n",
                 "    (0, 0),\n",
                 "    (0, 0.5),\n",
                 "    (1.5, 1.5),\n",
                 "    (1.6, 1.5),\n",
                 "    (3, 0.2),\n",
                 "    (3, 0),\n",
                 "]"
@@ -371,15 +596,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plot_catmull_rom(points3)"
+                "plot_catmull_rom(points4)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We can try to compensate this\n",
@@ -388,24 +613,24 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "times3 = 0, 0.2, 0.9, 1, 3, 3.3, 4.5"
+                "times4 = 0, 0.2, 0.9, 1, 3, 3.3, 4.5"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plot_catmull_rom(points3, times3)"
+                "plot_catmull_rom(points4, times4)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Time values can be chosen by trial and error,\n",
@@ -416,45 +641,45 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Chordal Parameterization\n",
                 "\n",
                 "One way to go about this is to measure the (Euclidean) distances\n",
-                "between consecutive vertices (i.e. the \"chordal lengths\")\n",
+                "between consecutive vertices (i.e. the *chordal lengths*)\n",
                 "and simply use those distances as time intervals:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "distances = np.linalg.norm(np.diff(points3 + points3[:1], axis=0), axis=1)\n",
+                "distances = np.linalg.norm(np.diff(points4 + points4[:1], axis=0), axis=1)\n",
                 "distances"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "times4 = np.concatenate([[0], np.cumsum(distances)])\n",
-                "times4"
+                "times5 = np.concatenate([[0], np.cumsum(distances)])\n",
+                "times5"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plot_catmull_rom(points3, times4)"
+                "plot_catmull_rom(points4, times5)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This makes the speed along the spline nearly constant,\n",
@@ -466,59 +691,60 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Centripetal Parameterization\n",
                 "\n",
                 "As a variation of the previous method,\n",
                 "the square roots of the chordal lengths\n",
-                "can be used to define the time intervals."
+                "can be used to define the time intervals\n",
+                "<cite data-cite=\"lee1989choosing\">(Lee 1989)</cite>."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "times5 = np.concatenate([[0], np.cumsum(np.sqrt(distances))])\n",
-                "times5"
+                "times6 = np.concatenate([[0], np.cumsum(np.sqrt(distances))])\n",
+                "times6"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plot_catmull_rom(points3, times5)"
+                "plot_catmull_rom(points4, times6)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The curve takes its course much closer to the chords,\n",
                 "but its speed is obviously far from constant.\n",
                 "\n",
                 "Centripetal parameterization has the very nice property that\n",
                 "it guarantees no cusps and no self-intersections,\n",
                 "as shown by \n",
-                "<cite data-cite=\"yuksel2011parameterization\">Yuksel et al. (2011)</cite>.\n",
+                "<cite data-cite-t=\"yuksel2011parameterization\">Yuksel et al. (2011)</cite>.\n",
                 "The curve is also guaranteed to never \"move away\" from the successive vertex:"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "> When centripetal parameterization is used with Catmull--Rom splines to\n",
                 "define a path curve, the direction of motion for the object following this path\n",
                 "will always be towards the next key-frame position.\n",
                 ">\n",
-                "> ---<cite data-cite=\"yuksel2011parameterization\">Yuksel et al. (2011)</cite>, Section 7.2: \"Path Curves\""
+                "> ---<cite data-cite-t=\"yuksel2011parameterization\">Yuksel et al. (2011)</cite>, Section 7.2: \"Path Curves\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Parameterized Parameterization\n",
@@ -540,15 +766,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def plot_alpha(alpha, label):\n",
-                "    s = splines.CatmullRom(points3, alpha=alpha, endconditions='closed')\n",
+                "    s = splines.CatmullRom(points4, alpha=alpha, endconditions='closed')\n",
                 "    plot_spline_2d(s, label=label)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -561,17 +787,17 @@
                 "plt.legend(loc='center', numpoints=3);"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "As can be seen here (and as\n",
-                "<cite data-cite=\"yuksel2011parameterization\">Yuksel et al. (2011)</cite>\n",
-                "shows to be generally true),\n",
+                "As can be seen here -- and as\n",
+                "<cite data-cite-t=\"yuksel2011parameterization\">Yuksel et al. (2011)</cite>\n",
+                "demonstrate to be generally true --\n",
                 "the uniform curve is farthest away from short chords\n",
                 "and closest to long chords.\n",
                 "The chordal curve behaves contrarily:\n",
                 "closest to short chords and awkwardly far from long chords.\n",
                 "The centripetal curve is closer to the uniform curve for long chords\n",
                 "and closer to the chordal curve for short chords,\n",
                 "providing a very good compromise.\n",
@@ -587,59 +813,59 @@
             "metadata": {},
             "source": [
                 "> In this paper\n",
                 "we prove that, for cubic Catmull--Rom curves, centripetal parameterization\n",
                 "is the only parameterization in this family that guarantees that the curves\n",
                 "do not form cusps or self-intersections within curve segments.\n",
                 ">\n",
-                "> ---<cite data-cite=\"yuksel2011parameterization\">Yuksel et al. (2011)</cite>, abstract"
+                "> ---<cite data-cite-t=\"yuksel2011parameterization\">Yuksel et al. (2011)</cite>, abstract"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "> [...] we mathematically prove that\n",
                 "centripetal parameterization of Catmull--Rom curves\n",
                 "guarantees that the curve segments cannot form cusps or local self-intersections,\n",
                 "while such undesired features can be formed\n",
                 "with all other possible parameterizations within this class.\n",
                 ">\n",
-                "> ---<cite data-cite=\"yuksel2011parameterization\">Yuksel et al. (2011)</cite>, Section 1: \"Introduction\""
+                "> ---<cite data-cite-t=\"yuksel2011parameterization\">Yuksel et al. (2011)</cite>, Section 1: \"Introduction\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "> Cusps and self-intersections are very common with Catmull--Rom curves\n",
                 "for most parameterization choices. In fact, as we will show here,\n",
                 "the only parameterization choice that guarantees\n",
                 "no cusps and self-intersections within\n",
                 "curve segments is centripetal parameterization.\n",
                 ">\n",
-                "> ---<cite data-cite=\"yuksel2011parameterization\">Yuksel et al. (2011)</cite>, Section 3: \"Cusps and Self-Intersections\""
+                "> ---<cite data-cite-t=\"yuksel2011parameterization\">Yuksel et al. (2011)</cite>, Section 3: \"Cusps and Self-Intersections\""
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.9"
+            "version": "3.11.1"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/euclidean/catmull-rom-uniform.ipynb` & `splines-0.3.0/doc/euclidean/catmull-rom-uniform.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9799840525820254%*

 * *Differences: {"'cells'": "{1: {'source': ['# Uniform Catmull--Rom Splines']}, 2: {'source': {insert: [(0, "*

 * *            '\'<cite data-cite-t="catmull1974splines">Catmull and Rom (1974)</cite>\\n\'), (1, '*

 * *            "'presented a class of splines which can be described mathematically,\\n'), (3, 'with "*

 * *            "what is referred to as equation (1):\\n')], delete: [3, 1, 0]}}, 3: {'source': "*

 * *            '{insert: [(13, \'> ---<cite data-cite-t="catmull1974splines">Catmull and Rom '*

 * *            '(1974)</cite>, sectio […]*

```diff
@@ -11,25 +11,25 @@
                 "[back to overview](catmull-rom.ipynb)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Uniform Catmull-Rom Splines"
+                "# Uniform Catmull--Rom Splines"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "In <cite data-cite=\"catmull1974splines\">Catmull and Rom (1974)</cite>,\n",
-                "a class of splines is presented which can be,\n",
+                "<cite data-cite-t=\"catmull1974splines\">Catmull and Rom (1974)</cite>\n",
+                "presented a class of splines which can be described mathematically,\n",
                 "in its most generic form,\n",
-                "described mathematically with what is referred to as equation (1):\n",
+                "with what is referred to as equation (1):\n",
                 "\n",
                 "\\begin{equation*}\n",
                 "F(s) =\n",
                 "\\frac{\n",
                 "\\sum x_i(s) w_i(s)\n",
                 "}{\n",
                 "\\sum w_i(s)\n",
@@ -51,23 +51,23 @@
                 "shall deal only with blending functions that are zero\n",
                 "outside of some given interval.\n",
                 "Also we require that\n",
                 "$\\sum w_i(s)$ does not vanish for any $s$.\n",
                 "We shall normalize $w_i(s)$ so that\n",
                 "$\\sum w_i(s) = 1$ for all $s$.\n",
                 ">\n",
-                "> ---<cite data-cite=\"catmull1974splines\">Catmull and Rom (1974)</cite>, section 3, \"Blending Functions\""
+                "> ---<cite data-cite-t=\"catmull1974splines\">Catmull and Rom (1974)</cite>, section 3, \"Blending Functions\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The components of the equation are further constrained\n",
-                "to produce a interpolating function:"
+                "to produce an interpolating function:"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "> Consider the following case:\n",
@@ -77,15 +77,15 @@
                 "The function $F(s)$ defined in equation (1)\n",
                 "will thus be an interpolating function.\n",
                 "Intuitively, this says that if all of the functions\n",
                 "that have an effect at a point,\n",
                 "pass through the point,\n",
                 "then the average of the functions will pass through the point.\n",
                 ">\n",
-                "> ---<cite data-cite=\"catmull1974splines\">Catmull and Rom (1974)</cite>, section 2: \"The Model\""
+                "> ---<cite data-cite-t=\"catmull1974splines\">Catmull and Rom (1974)</cite>, section 2: \"The Model\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "<div class=\"alert alert-warning\">\n",
@@ -110,15 +110,15 @@
                 "This means that $F(s)$ will be an interpolating function.\n",
                 "On the other hand\n",
                 "if the width of $w_i(s)$ is greater than $k+2$\n",
                 "then $x_i(s)$ will have an effect on the curve\n",
                 "outside the interpolation interval.\n",
                 "$F(s)$ will then be an approximating function.\n",
                 ">\n",
-                "> ---<cite data-cite=\"catmull1974splines\">Catmull and Rom (1974)</cite>, section 2: \"The Model\""
+                "> ---<cite data-cite-t=\"catmull1974splines\">Catmull and Rom (1974)</cite>, section 2: \"The Model\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "After limiting the scope of the paper to *interpolating* splines,\n",
@@ -134,29 +134,29 @@
                 "parametric\n",
                 "space\n",
                 "we can, without\n",
                 "loss\n",
                 "of\n",
                 "generality, place $s_j=j$.\n",
                 ">\n",
-                "> ---<cite data-cite=\"catmull1974splines\">Catmull and Rom (1974)</cite>, section 2: \"The Model\""
+                "> ---<cite data-cite-t=\"catmull1974splines\">Catmull and Rom (1974)</cite>, section 2: \"The Model\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Whether or not generality is lost,\n",
                 "this means that the rest of the paper doesn't give any hints\n",
                 "how to construct non-uniform splines.\n",
-                "For those who are interested anyway,\n",
-                "we show how to do that in\n",
-                "[the notebook about non-uniform Catmull--Rom splines](catmull-rom-non-uniform.ipynb)\n",
-                "and once again in\n",
-                "[the notebook about the Barry--Goldman algorithm](catmull-rom-barry-goldman.ipynb)."
+                "For those who are interested nevertheless,\n",
+                "we show how to do that in the\n",
+                "[notebook about non-uniform Catmull--Rom splines](catmull-rom-non-uniform.ipynb)\n",
+                "and once again in the\n",
+                "[notebook about the Barry--Goldman algorithm](catmull-rom-barry-goldman.ipynb)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "After the aforementioned constraints\n",
@@ -167,15 +167,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "> Cardinal function: a function that is $1$ at some\n",
                 "knot, $0$ at all other knots and can be anything in\n",
                 "between the other knots. It satisfies $F_i(s_j) = \\delta_{ij}$.\n",
                 ">\n",
-                "> ---<cite data-cite=\"catmull1974splines\">Catmull and Rom (1974)</cite>, section 1: \"Introduction\""
+                "> ---<cite data-cite-t=\"catmull1974splines\">Catmull and Rom (1974)</cite>, section 1: \"Introduction\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "... the gratuitously generic equation (1) is made a bit more concrete:"
@@ -209,15 +209,15 @@
                 "\\end{equation*}\n",
                 ">\n",
                 "> In essence we see that for a polynomial case\n",
                 "our cardinal functions are a blend of Lagrange polynomials.\n",
                 "When calculating $C_{0,k}(s)$,\n",
                 "$w(s)$ should be centered about $\\frac{k}{2}$.\n",
                 ">\n",
-                "> ---<cite data-cite=\"catmull1974splines\">Catmull and Rom (1974)</cite>, section 4: \"Calculating Cardinal Functions\""
+                "> ---<cite data-cite-t=\"catmull1974splines\">Catmull and Rom (1974)</cite>, section 4: \"Calculating Cardinal Functions\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This looks like something we can work with,\n",
@@ -283,34 +283,34 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Blending Functions\n",
                 "\n",
-                "<cite data-cite=\"catmull1974splines\">Catmull and Rom (1974)</cite>\n",
-                "leaves the choice of blending function to the reader.\n",
-                "It shows two plots (figure 1 and figure 3) for a custom blending function\n",
+                "<cite data-cite-t=\"catmull1974splines\">Catmull and Rom (1974)</cite>\n",
+                "leave the choice of blending function to the reader.\n",
+                "They show two plots (figure 1 and figure 3) for a custom blending function\n",
                 "stitched together from two B\u00e9zier curves,\n",
-                "but it doesn't show the cardinal function nor an actual spline\n",
+                "but they don't show the cardinal function nor an actual spline\n",
                 "created from it.\n",
                 "\n",
                 "The only other concrete suggestion is to use B-spline basis functions\n",
                 "as blending functions.\n",
                 "A quadratic B-spline basis function is shown in figure 2\n",
                 "and both cardinal functions and example curves are shown\n",
                 "that utilize both quadratic and cubic B-spline basis functions\n",
                 "(figures 4 through 7).\n",
                 "No mathematical description of B-spline basis functions is given,\n",
-                "instead the paper refers to\n",
-                "<cite data-cite=\"gordon1974bspline\">Gordon and Riesenfeld (1974)</cite>.\n",
+                "instead they refer to\n",
+                "<cite data-cite-t=\"gordon1974bspline\">Gordon and Riesenfeld (1974)</cite>.\n",
                 "That paper provides a pair of equations (3.1 and 3.2)\n",
                 "that can be used to recursively construct B-spline basis functions.\n",
                 "Simplified to the *uniform* case,\n",
-                "this leads to the base case (degree 0) ..."
+                "this leads to the base case (i.e. degree zero) ..."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -319,15 +319,15 @@
                 "B0"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "... which can be used to obtain the linear (degree 1) basis functions:"
+                "... which can be used to obtain the linear (i.e. degree one) basis functions:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -378,15 +378,15 @@
                 "grid_lines([0, 1, 2], [0, 1])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The quadratic (degree 2) basis functions can be obtained like this:"
+                "The quadratic (i.e. degree two) basis functions can be obtained like this:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -421,16 +421,17 @@
                 "grid_lines([-1, 0, 1, 2], [0, 1])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This should be the same function as shown in figure 2 of\n",
-                "<cite data-cite=\"catmull1974splines\">Catmull and Rom (1974)</cite>."
+                "This should be the same function as shown by\n",
+                "<cite data-cite-t=\"catmull1974splines\">Catmull and Rom (1974)</cite>\n",
+                "in figure 2."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Cardinal Functions\n",
@@ -474,16 +475,17 @@
                 "grid_lines(range(-2, 3), [0, 1])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This should be the same function as shown in figure 4 of\n",
-                "<cite data-cite=\"catmull1974splines\">Catmull and Rom (1974)</cite>."
+                "This should be the same function as shown by\n",
+                "<cite data-cite-t=\"catmull1974splines\">Catmull and Rom (1974)</cite>\n",
+                "in figure 4."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The paper does not show that,\n",
@@ -627,15 +629,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Basis Polynomials\n",
                 "\n",
                 "The piecewise expression for the cardinal function\n",
                 "is a bit unwieldy to work with,\n",
-                "so let's bring it into a form we know how to deal with.\n",
+                "so let's bring it into a form we already know how to deal with.\n",
                 "\n",
                 "We are splitting the piecewise expression into four separate pieces,\n",
                 "each one to be evaluated at $0 \\le t \\le 1$.\n",
                 "We are also reversing the order of the pieces,\n",
                 "to match our intended control point order:"
             ]
         },
@@ -704,15 +706,15 @@
                 "control_points = sp.Matrix(sp.symbols('xbm3:7'))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "As usual, we look at the fifth polynomial segment\n",
+                "As usual, we look at the fifth polynomial segment $\\boldsymbol{p}_4(t)$\n",
                 "(from $\\boldsymbol{x}_4$ to $\\boldsymbol{x}_5$):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -763,16 +765,16 @@
                 "M_CR.pull_out(sp.S.Half)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This matrix also appears in section 6 of\n",
-                "<cite data-cite=\"catmull1974splines\">Catmull and Rom (1974)</cite>."
+                "<cite data-cite-t=\"catmull1974splines\">Catmull and Rom (1974)</cite>\n",
+                "show this matrix in section 6."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "In case you want to copy&paste it, here's a plain text version:"
@@ -840,33 +842,35 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "pd4.evaluated_at(t, 0)"
+                "start_tangent = pd4.evaluated_at(t, 0)\n",
+                "start_tangent"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "pd4.evaluated_at(t, 1)"
+                "end_tangent = pd4.evaluated_at(t, 1)\n",
+                "end_tangent"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "These two expressions can be generalized to\n",
-                "(as already shown in\n",
-                "[the notebook about Catmull--Rom properties](catmull-rom-properties.ipynb#Tangent-Vectors)):\n",
+                "-- as already shown in\n",
+                "[the notebook about Catmull--Rom properties](catmull-rom-properties.ipynb#Tangent-Vectors):\n",
                 "\n",
                 "\\begin{equation*}\n",
                 "\\boldsymbol{\\dot{x}}_i =\n",
                 "\\frac{\\boldsymbol{x}_{i+1} - \\boldsymbol{x}_{i-1}}{2}\n",
                 "\\end{equation*}"
             ]
         },
@@ -887,31 +891,119 @@
                 "&= \\boldsymbol{x}_i + \\frac{\\boldsymbol{\\dot{x}}_i}{3}\n",
                 "= \\boldsymbol{x}_i + \\frac{\\boldsymbol{x}_{i+1} - \\boldsymbol{x}_{i-1}}{6}\\\\\n",
                 "\\boldsymbol{\\tilde{x}}_i^{(-)}\n",
                 "&= \\boldsymbol{x}_i - \\frac{\\boldsymbol{\\dot{x}}_i}{3}\n",
                 "= \\boldsymbol{x}_i - \\frac{\\boldsymbol{x}_{i+1} - \\boldsymbol{x}_{i-1}}{6}\n",
                 "\\end{align*}"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "x4, x5 = control_points[1:3]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "x4tilde = x4 + start_tangent.expr / 3\n",
+                "x4tilde"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "x5tilde = x5 - end_tangent.expr / 3\n",
+                "x5tilde"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "tags": []
+            },
+            "source": [
+                "## Using Quadrangle Interpolation\n",
+                "\n",
+                "Remember the [notebook about quadrangle interpolation](quadrangle.ipynb)?\n",
+                "It showed us how to calculate the quadrangle points\n",
+                "given the B\u00e9zier control points:\n",
+                "\n",
+                "\\begin{align*}\n",
+                "\\boldsymbol{\\bar{x}}_i^{(+)} &=\n",
+                "\\frac{3}{2} \\boldsymbol{\\tilde{x}}_i^{(+)} -\n",
+                "\\frac{1}{2} \\boldsymbol{x}_{i+1}\\\\\n",
+                "\\boldsymbol{\\bar{x}}_i^{(-)} &=\n",
+                "\\frac{3}{2} \\boldsymbol{\\tilde{x}}_i^{(-)} -\n",
+                "\\frac{1}{2} \\boldsymbol{x}_{i-1}\n",
+                "\\end{align*}"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "x4bar = 3 * x4tilde / 2 - x5 / 2\n",
+                "x4bar"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "x5bar = 3 * x5tilde / 2 - x4 / 2\n",
+                "x5bar"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Generalizing these expressions\n",
+                "and juggling the terms around a bit, we get\n",
+                "\n",
+                "\\begin{equation*}\n",
+                "\\boldsymbol{\\bar{x}}_i^{(+)} =\n",
+                "\\boldsymbol{\\bar{x}}_i^{(-)} =\n",
+                "\\boldsymbol{x}_i - \\frac{\n",
+                "(\\boldsymbol{x}_{i+1} - \\boldsymbol{x}_i) +\n",
+                "(\\boldsymbol{x}_{i-1} - \\boldsymbol{x}_i)\n",
+                "}{4}.\n",
+                "\\end{equation*}"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.10.9"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/euclidean/catmull-rom.ipynb` & `splines-0.3.0/doc/euclidean/catmull-rom.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9915079365079364%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'is a specific member of a whole family of splines "*

 * *            'introduced by\\n\'), (4, \'<cite data-cite-t="catmull1974splines">Catmull and Rom '*

 * *            "(1974)</cite>.\\n')], delete: [8, 7, 6, 5, 4, 3]}}, 2: {'source': {insert: [(1, '-- "*

 * *            'as presented by\\n\'), (2, \'<cite data-cite-t="overhauser1968parabolic">Overhauser '*

 * *            "(1968)</cite> --\\n')], delete: [2, 1]}}, 3: {'source': {insert: [(1, 'is available "*

 * *            "in the cla […]*

```diff
@@ -14,42 +14,38 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Catmull--Rom Splines\n",
                 "\n",
                 "What is nowadays known as *Catmull--Rom spline*\n",
-                "(named after\n",
-                "[Edwin Catmull](https://en.wikipedia.org/wiki/Edwin_Catmull)\n",
-                "and\n",
-                "[Raphael Rom](https://en.wikipedia.org/wiki/Raphael_Rom))\n",
-                "is a specific member of a whole family of splines introduced in\n",
-                "<cite data-cite=\"catmull1974splines\">A Class of Local Interpolating Splines (1974)</cite>.\n",
+                "is a specific member of a whole family of splines introduced by\n",
+                "<cite data-cite-t=\"catmull1974splines\">Catmull and Rom (1974)</cite>.\n",
                 "That paper only describes *uniform* splines,\n",
                 "but their definition can be straightforwardly extended\n",
                 "to the *non-uniform* case."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Contrary to popular belief, *Overhauser splines*\n",
-                "(as presented in\n",
-                "<cite data-cite=\"overhauser1968parabolic\">Overhauser (1968)</cite>)\n",
+                "-- as presented by\n",
+                "<cite data-cite-t=\"overhauser1968parabolic\">Overhauser (1968)</cite> --\n",
                 "are not the same!"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "A Python implementation of Catmull--Rom splines\n",
-                "is available in the\n",
-                "[splines.CatmullRom](../python-module/splines.rst#splines.CatmullRom) class."
+                "is available in the class\n",
+                "[splines.CatmullRom](../python-module/splines.rst#splines.CatmullRom)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx-toctree": {
                     "maxdepth": 2
```

### Comparing `splines-0.2.0/doc/euclidean/catmull_rom.py` & `splines-0.3.0/doc/euclidean/catmull_rom.py`

 * *Files identical despite different names*

### Comparing `splines-0.2.0/doc/euclidean/end-conditions-natural.ipynb` & `splines-0.3.0/doc/euclidean/end-conditions-natural.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995814307458143%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(0, 'Natural end conditions are naturally a good fit "*

 * *            "for\\n'), (1, '[natural splines](natural-uniform.ipynb#End-Conditions).\\n'), (2, "*

 * *            "'And in case you were wondering,\\n')], delete: [0]}}, 15: {'source': {insert: [(1, "*

 * *            "'(a.k.a. velocity, a.k.a. tangent vector):')], delete: [1]}}}"}*

```diff
@@ -27,15 +27,17 @@
                 "it's easy to get to the uniform case by setting $\\Delta_i = 1$."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "In case you were wondering,\n",
+                "Natural end conditions are naturally a good fit for\n",
+                "[natural splines](natural-uniform.ipynb#End-Conditions).\n",
+                "And in case you were wondering,\n",
                 "natural end conditions are sometimes also called \"relaxed\" end conditions."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -140,15 +142,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We need the first derivative\n",
-                "(a.k.a velocity, a.k.a. tangent vector):"
+                "(a.k.a. velocity, a.k.a. tangent vector):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `splines-0.2.0/doc/euclidean/end-conditions.ipynb` & `splines-0.3.0/doc/euclidean/hermite.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.980406746031746%*

 * *Differences: {"'cells'": "{1: {'source': ['# Hermite Splines\\n', '\\n', '[Hermite "*

 * *            "splines](https://en.wikipedia.org/wiki/Cubic_Hermite_spline)\\n', '(named after\\n', "*

 * *            "'[Charles Hermite](https://en.wikipedia.org/wiki/Charles_Hermite))\\n', 'are the "*

 * *            "building blocks for many other types of interpolating polynomial splines,\\n', 'for "*

 * *            "example\\n', '[natural splines](natural.ipynb) and\\n', '[Catmull--Rom "*

 * *            "splines](catmull-rom.ipynb).\\n', '\\n', 'A Py […]*

```diff
@@ -11,24 +11,40 @@
                 "[back to Euclidean splines](index.ipynb)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# End Conditions"
+                "# Hermite Splines\n",
+                "\n",
+                "[Hermite splines](https://en.wikipedia.org/wiki/Cubic_Hermite_spline)\n",
+                "(named after\n",
+                "[Charles Hermite](https://en.wikipedia.org/wiki/Charles_Hermite))\n",
+                "are the building blocks for many other types of interpolating polynomial splines,\n",
+                "for example\n",
+                "[natural splines](natural.ipynb) and\n",
+                "[Catmull--Rom splines](catmull-rom.ipynb).\n",
+                "\n",
+                "A Python implementation of (cubic) Hermite splines is available in the\n",
+                "[splines.CubicHermite](../python-module/splines.rst#splines.CubicHermite)\n",
+                "class."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "nbsphinx-toctree": {}
+                "nbsphinx-toctree": {
+                    "maxdepth": 2
+                }
             },
             "source": [
-                "* [Natural End Conditions](end-conditions-natural.ipynb)"
+                "* [Properties](hermite-properties.ipynb)\n",
+                "* [Derivation (Uniform)](hermite-uniform.ipynb)\n",
+                "* [Derivation (Non-Uniform)](hermite-non-uniform.ipynb)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
@@ -40,13 +56,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.1"
+            "version": "3.9.1+"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/euclidean/helper.py` & `splines-0.3.0/doc/euclidean/helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Helper functions for plotting."""
+from cycler import cycler as _cycler
 import matplotlib.pyplot as _plt
 import numpy as _np
 import sympy as _sp
 
 
 def plot_slopes_1d(slopes, values, grid, scale=1, ax=None, **kwargs):
     """Plot incoming and outging slopes for 1D spline."""
@@ -127,21 +128,23 @@
     ax.autoscale()
 
 
 def plot_basis(*args, ax=None, parameter=_sp.Symbol('t'), labels=None):
     """Plot a polynomial basis (given as SymPy expressions)."""
     if ax is None:
         ax = _plt.gca()
+    ax.set_prop_cycle(_plt.rcParams['axes.prop_cycle'][:5] + _cycler(
+        linestyle=['-', '--', ':', '-.', (0, (4.5, 1.5, 1, 1.5, 1, 1.5))]))
     plot_sympy(*args, (parameter, 0, 1))
     grid_lines([0, 1], [0, 1], ax=ax)
     if labels is None:
         labels = args
     if labels:
         ax.legend([latexify(l) for l in labels])
-    ax.set_xlabel(latexify(parameter))
+    ax.set_xlabel(latexify(parameter), labelpad=-4)
     ax.set_ylabel('weight')
 
 
 def plot_x_3_to_6(points, ax):
     """Plot labels x3 to x6."""
     options = dict(
         ha="center",
@@ -154,7 +157,14 @@
     )
     ax.text(*points[0], r'$\mathbf{x}_3$', **options)
     ax.text(*points[1], r'$\mathbf{x}_4$', **options)
     ax.text(*points[2], r'$\mathbf{x}_5$', **options)
     ax.text(*points[3], r'$\mathbf{x}_6$', **options)
     # Plot invisible points to make sure autoscaling doesn't crop the text
     ax.scatter(*points.T, marker='', c='chartreuse')
+
+
+def show_animation(ani, default_mode='reflect'):
+    display({
+        'text/html': ani.to_jshtml(default_mode=default_mode),
+        'text/plain': 'Animations can only be shown in HTML output, sorry!',
+    }, raw=True)
```

### Comparing `splines-0.2.0/doc/euclidean/hermite-non-uniform.ipynb` & `splines-0.3.0/doc/euclidean/hermite-non-uniform.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9903880243319898%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '[back to overview](hermite.ipynb) -\\n'), (3, "*

 * *            "'[properties](hermite-properties.ipynb) -\\n'), (4, '[derivation "*

 * *            "(uniform)](hermite-uniform.ipynb)')], delete: [2]}}, 2: {'source': {insert: [(3, 'but "*

 * *            "the first approach can be carried out very similarly,\\n')], delete: [3]}}, 3: "*

 * *            "{'source': {insert: [(0, 'from pprint import pprint\\n')]}}, 21: {'source': ['## "*

 * *            "Basis Matrix\\n', '\\n', 'In contrast […]*

```diff
@@ -4,15 +4,17 @@
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "source": [
                 "This notebook is part of https://github.com/AudioSceneDescriptionFormat/splines, see also https://splines.readthedocs.io/.\n",
                 "\n",
-                "[back to overview](hermite.ipynb)"
+                "[back to overview](hermite.ipynb) -\n",
+                "[properties](hermite-properties.ipynb) -\n",
+                "[derivation (uniform)](hermite-uniform.ipynb)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Non-Uniform Cubic Hermite Splines\n",
@@ -57,27 +59,28 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "<div class=\"alert alert-info\">\n",
                 "\n",
                 "We show the second approach here,\n",
-                "but the first approach can be done very similarly,\n",
+                "but the first approach can be carried out very similarly,\n",
                 "with only very few changed steps.\n",
                 "The appropriate changes are mentioned below.\n",
                 "\n",
                 "</div>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "from pprint import pprint\n",
                 "import sympy as sp\n",
                 "sp.init_printing(order='grevlex')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -245,15 +248,19 @@
                 "display(x4, x5, xd4.subs(delta), xd5.subs(delta))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Basis Matrix"
+                "## Basis Matrix\n",
+                "\n",
+                "In contrast to the uniform case,\n",
+                "where the same basis matrix could be used for all segments,\n",
+                "here we need a different matrix for each segment."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -305,15 +312,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(_.expr)"
+                "pprint(_.expr)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -323,15 +330,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(_.expr)"
+                "pprint(_.expr)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Basis Polynomials"
@@ -347,15 +354,15 @@
                 "b_H.factor().subs(delta).simplify().T"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Those are the *non-uniform* Hermite basis functions.\n",
+                "Those are the *non-uniform* (cubic) Hermite basis functions.\n",
                 "Not surprisingly, they are different for each segment,\n",
                 "because generally the values $\\Delta_i$ are different\n",
                 "in the non-uniform case."
             ]
         },
         {
             "cell_type": "markdown",
@@ -365,15 +372,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "To quickly check whether the matrix $M_{H,4}$ does what we expect,\n",
-                "let's plot an example segment:"
+                "let's plot an example segment."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -509,15 +516,15 @@
             "metadata": {},
             "source": [
                 "<div class=\"alert alert-info\">\n",
                 "\n",
                 "If you did *not* re-scale $t$ in the beginning of the derivation,\n",
                 "you can use the matrix $M_{H,i}$ to calculate the monomial coefficients\n",
                 "of each segment (as shown in the example code above) and be done with it.\n",
-                "The following simplification does only apply\n",
+                "The following simplification only applies\n",
                 "if you *did* re-scale $t$.\n",
                 "\n",
                 "</div>"
             ]
         },
         {
             "cell_type": "markdown",
@@ -551,18 +558,20 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "control_values_H_scaled = sp.Matrix([x4.name,\n",
-                "                                     x5.name,\n",
-                "                                     (t5 - t4) * xd4.name,\n",
-                "                                     (t5 - t4) * xd5.name])\n",
+                "control_values_H_scaled = sp.Matrix([\n",
+                "    x4.name,\n",
+                "    x5.name,\n",
+                "    (t5 - t4) * xd4.name,\n",
+                "    (t5 - t4) * xd5.name,\n",
+                "])\n",
                 "control_values_H_scaled.subs(delta)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -574,18 +583,20 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sp.Eq(\n",
                 "    sp.simplify(M_H.expr * control_values_H.name),\n",
-                "    sp.simplify(sp.Matrix([[ 2, -2,  1,  1],\n",
-                "                           [-3,  3, -2, -1],\n",
-                "                           [ 0,  0,  1,  0],\n",
-                "                           [ 1,  0,  0,  0]]) * control_values_H_scaled))"
+                "    sp.simplify(sp.Matrix([\n",
+                "        [ 2, -2,  1,  1],\n",
+                "        [-3,  3, -2, -1],\n",
+                "        [ 0,  0,  1,  0],\n",
+                "        [ 1,  0,  0,  0],\n",
+                "    ]) * control_values_H_scaled))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "<div class=\"alert alert-info\">\n",
@@ -604,20 +615,20 @@
                 "assert _ == True"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Long story short,\n",
+                "To make a long story short,\n",
                 "to implement a *non-uniform* cubic Hermite spline segment,\n",
                 "we can simply re-scale the parameter to a range from $0$ to $1$\n",
                 "(by substituting $t \\to \\frac{t - t_i}{t_{i+1} - t_i}$),\n",
                 "multiply both given tangent vectors by $\\Delta_i = t_{i+1} - t_i$\n",
-                "and then simply use the implementation of\n",
+                "and then use the implementation of\n",
                 "the *uniform* cubic Hermite spline segment."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -639,27 +650,27 @@
                 "If we want to maintain the original lengths of our tangent vectors,\n",
                 "we can simply scale them by $\\Delta_i$ beforehand."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.11.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/euclidean/hermite-properties.ipynb` & `splines-0.3.0/doc/euclidean/hermite-properties.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9808705817426399%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '[back to overview](hermite.ipynb) -\\n'), (3, "*

 * *            "'[derivation (uniform)](hermite-uniform.ipynb) -\\n'), (4, '[derivation "*

 * *            "(non-uniform)](hermite-non-uniform.ipynb)')], delete: [2]}}, 1: {'source': {insert: "*

 * *            "[(3, 'where for each polynomial segment\\n')], delete: [3]}}, 2: {'source': {insert: "*

 * *            "[(0, 'However, *cubic Hermite splines* are so overwhelmingly common\\n'), (1, 'that "*

 * *            "they are often simply r […]*

```diff
@@ -4,25 +4,27 @@
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "source": [
                 "This notebook is part of https://github.com/AudioSceneDescriptionFormat/splines, see also https://splines.readthedocs.io/.\n",
                 "\n",
-                "[back to overview](hermite.ipynb)"
+                "[back to overview](hermite.ipynb) -\n",
+                "[derivation (uniform)](hermite-uniform.ipynb) -\n",
+                "[derivation (non-uniform)](hermite-non-uniform.ipynb)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Properties of Hermite Splines\n",
                 "\n",
                 "Hermite splines are interpolating polynomial splines,\n",
-                "where for each polynomial segment,\n",
+                "where for each polynomial segment\n",
                 "the desired value at the start and end is given (obviously!),\n",
                 "as well as the values of a certain number of derivatives\n",
                 "at the start and/or the end.\n",
                 "\n",
                 "Most commonly, *cubic* (= degree 3) Hermite splines are used.\n",
                 "Cubic polynomials have 4 coefficients to be chosen freely,\n",
                 "and those are determined for each segment of a cubic Hermite spline\n",
@@ -48,21 +50,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "However, *cubic Hermite splines* are so overwhelmingly common\n",
-                "that they are often simply referred to as *Hermite splines*."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "that they are often simply referred to as *Hermite splines*.\n",
                 "From this point forward, we will only be considering *cubic* Hermite splines."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -90,23 +86,24 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from helper import plot_slopes_1d, plot_spline_2d, plot_tangents_2d, grid_lines"
+                "from helper import plot_spline_1d, plot_slopes_1d, grid_lines\n",
+                "from helper import plot_spline_2d, plot_tangents_2d"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Let's look at a one-dimensional spline first.\n",
-                "We provide a list of values (to be interpolated)\n",
+                "Here are some values (to be interpolated)\n",
                 "and a list of associated parameter values\n",
                 "(or time instances, if you will)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -119,15 +116,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Since (cubic) Hermite splines ask for the first derivative\n",
                 "at the beginning and end of each segment,\n",
-                "we provide a list of slopes (outgoing, incoming, outgoing, incoming, ...)."
+                "we have to come up with a list of slopes (outgoing, incoming, outgoing, incoming, ...)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -163,25 +160,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "times = np.linspace(grid[0], grid[-1], 100)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "plt.plot(times, s1.evaluate(times))\n",
-                "plt.scatter(grid, values)\n",
+                "plot_spline_1d(s1)\n",
                 "plot_slopes_1d(slopes, values, grid)\n",
                 "grid_lines(grid)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -203,15 +190,16 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The derivative of a curve is its tangent vector,\n",
-                "so we provide a list of them (outgoing, incoming, outgoing, incoming, ...):"
+                "so here is a list of associated tangent vectors\n",
+                "(outgoing, incoming, outgoing, incoming, ...):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -296,46 +284,45 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Hermite splines are by default $C^0$ continuous.\n",
                 "If adjacent tangents are chosen to point into the same direction,\n",
                 "the spline becomes $G^1$ continuous.\n",
-                "\n",
                 "If on top of having the same direction,\n",
                 "adjacent tangents are chosen to have the same length,\n",
                 "that makes the spline $C^1$ continuous.\n",
                 "An example for that are [Catmull--Rom splines](catmull-rom.ipynb).\n",
                 "[Kochanek--Bartels splines](kochanek-bartels.ipynb)\n",
                 "can also be $C^1$ continuous,\n",
-                "but only if their \"continuity\" parameter $C$ is 0.\n",
+                "but only if their \"continuity\" parameter $C$ is zero.\n",
                 "\n",
                 "There is one unique choice of all of a cubic Hermite spline's tangents\n",
-                "(given certain [end conditions](end-conditions.ipynb))\n",
+                "-- given certain [end conditions](end-conditions.ipynb) --\n",
                 "that leads to continuous second derivatives at all vertices,\n",
                 "making the spline $C^2$ continuous.\n",
                 "This is what [natural splines](natural.ipynb) are all about."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.2"
+            "version": "3.11.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/euclidean/hermite-uniform.ipynb` & `splines-0.3.0/doc/euclidean/hermite-uniform.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9871045794861154%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '[back to overview](hermite.ipynb) -\\n'), (3, "*

 * *            "'[properties](hermite-properties.ipynb) -\\n'), (4, '[derivation "*

 * *            "(non-uniform)](hermite-non-uniform.ipynb)')], delete: [2]}}, 40: {'source': {insert: "*

 * *            "[(2, 'However, instead of calculating from right to left,\\n'), (3, 'we can also "*

 * *            "start at the left and\\n'), (4, 'multiply the monomial basis with the Hermite basis "*

 * *            "matrix $M_\\\\text{H}$,\\n'), (5, […]*

```diff
@@ -4,15 +4,17 @@
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "source": [
                 "This notebook is part of https://github.com/AudioSceneDescriptionFormat/splines, see also https://splines.readthedocs.io/.\n",
                 "\n",
-                "[back to overview](hermite.ipynb)"
+                "[back to overview](hermite.ipynb) -\n",
+                "[properties](hermite-properties.ipynb) -\n",
+                "[derivation (non-uniform)](hermite-non-uniform.ipynb)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Uniform Cubic Hermite Splines\n",
@@ -373,28 +375,61 @@
                 "print(_.expr)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "Now we have a new way to write the polynomial\n",
+                "$\\boldsymbol{p}_4(t)$,\n",
+                "given our four control values.\n",
+                "We take those control values,\n",
+                "left-multiply them by the Hermite basis matrix $M_\\text{H}$\n",
+                "(which gives us a column vector of coefficients),\n",
+                "which we can then left-multiply by the monomial basis:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "sp.MatMul(b_monomial, M_H.expr, control_values_H.name)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "## Basis Polynomials\n",
                 "\n",
-                "Multiplying the monomial basis with this matrix\n",
-                "yields the *Hermite basis polynomials*:"
+                "However, instead of calculating from right to left,\n",
+                "we can also start at the left and\n",
+                "multiply the monomial basis with the Hermite basis matrix $M_\\text{H}$,\n",
+                "which yields (a row vector containing) the *Hermite basis polynomials*:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "b_H = NamedMatrix(r'{b_\\text{H}}', b_monomial * M_H.expr)\n",
-                "b_H.factor().simplify().T"
+                "b_H.factor().T"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The multiplication of this row vector\n",
+                "with the column vector of control values\n",
+                "again produces the polynomial $\\boldsymbol{p}_4(t)$."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Let's plot the basis polynomials\n",
@@ -443,15 +478,15 @@
                 "While $t$ progresses towards $1$,\n",
                 "both functions must relinquish their influence\n",
                 "to the other two basis functions.\n",
                 "\n",
                 "At the end (when $t=1$),\n",
                 "the basis function associated with $\\boldsymbol{x}_{i+1}$\n",
                 "is the only one that has a non-zero value.\n",
-                "More concretely, it has the value $1$.\n",
+                "More specifically, it has the value $1$.\n",
                 "Finally,\n",
                 "the basis function associated with $\\boldsymbol{\\dot{x}}_{i+1}$\n",
                 "is the only one with a non-zero first derivative.\n",
                 "In fact, it has a first derivative of exactly $+1$\n",
                 "(the function values leading up to that have to be negative\n",
                 "because the final function value has to be $0$).\n",
                 "\n",
@@ -475,15 +510,15 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Example Plot\n",
                 "\n",
                 "To quickly check whether the matrix $M_H$ does what we expect,\n",
-                "let's plot an example segment:"
+                "let's plot an example segment."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -591,21 +626,21 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "What about using four positions (and no tangent vectors) instead?\n",
                 "\n",
-                "Let's use the point $\\boldsymbol{\\tilde{x}}_4$ as a \"handle\"\n",
+                "Let's use the point $\\boldsymbol{\\tilde{x}}_4$ as a \"drag point\"\n",
                 "(connected to $\\boldsymbol{x}_4$) that controls the tangent vector.\n",
                 "Same for $\\boldsymbol{\\tilde{x}}_5$ (connected to $\\boldsymbol{x}_5$).\n",
                 "\n",
                 "And since the tangents looked unwieldily long in the plot above\n",
                 "(compared to the effect they have on the shape of the curve),\n",
-                "let's put the handles only at a third of the length of the tangents,\n",
+                "let's put the drag points only at a third of the length of the tangents,\n",
                 "shall we?"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -677,17 +712,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "M_HtoB.expr = sp.Matrix([[expr.coeff(cv) for cv in control_values_H.name]\n",
-                "                         for expr in control_values_B.expr])\n",
-                "M_HtoB.pull_out(sp.S.One / 3)"
+                "M_HtoB.expr = sp.Matrix([\n",
+                "    [expr.coeff(cv) for cv in control_values_H.name]\n",
+                "    for expr in control_values_B.expr])\n",
+                "M_HtoB"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -822,27 +858,27 @@
                 "plt.annotate(r'$\\quad\\tilde{\\bf{x}}_0$', points[1])\n",
                 "plt.annotate(r'$\\tilde{\\bf{x}}_1\\quad$', points[2], ha='right');"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.11.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/euclidean/hermite.ipynb` & `splines-0.3.0/doc/euclidean/kochanek-bartels.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9563905423280423%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(0, 'Kochanek--Bartels splines (a.k.a. TCB splines) "*

 * *            "are\\n'), (1, 'named after\\n'), (2, '<cite "*

 * *            'data-cite-t="kochanek1984tcb">Kochanek and Bartels (1984)</cite>.\\n\'), (4, \'A '*

 * *            "Python implementation is available in the class\\n'), (5, "*

 * *            "'[splines.KochanekBartels](../python-module/splines.rst#splines.KochanekBartels).')], "*

 * *            "delete: [12, 11, 10, 8, 7, 6, 5, 4, 3, 2, 1, 0]}}, 3: {'source': ['* "*

 * *        […]*

```diff
@@ -11,40 +11,40 @@
                 "[back to Euclidean splines](index.ipynb)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Hermite Splines\n",
-                "\n",
-                "[Hermite splines](https://en.wikipedia.org/wiki/Cubic_Hermite_spline)\n",
-                "(named after\n",
-                "[Charles Hermite](https://en.wikipedia.org/wiki/Charles_Hermite))\n",
-                "are the building blocks for many other types of interpolating polynomial splines,\n",
-                "for example\n",
-                "[natural splines](natural.ipynb) and\n",
-                "[Catmull--Rom splines](catmull-rom.ipynb).\n",
+                "# Kochanek--Bartels Splines"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Kochanek--Bartels splines (a.k.a. TCB splines) are\n",
+                "named after\n",
+                "<cite data-cite-t=\"kochanek1984tcb\">Kochanek and Bartels (1984)</cite>.\n",
                 "\n",
-                "A Python implementation of (cubic) Hermite splines is available in the\n",
-                "[splines.CubicHermite](../python-module/splines.rst#splines.CubicHermite)\n",
-                "class."
+                "A Python implementation is available in the class\n",
+                "[splines.KochanekBartels](../python-module/splines.rst#splines.KochanekBartels)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx-toctree": {
                     "maxdepth": 2
                 }
             },
             "source": [
-                "* [Properties](hermite-properties.ipynb)\n",
-                "* [Derivation (Uniform)](hermite-uniform.ipynb)\n",
-                "* [Derivation (Non-Uniform)](hermite-non-uniform.ipynb)"
+                "* [Properties](kochanek-bartels-properties.ipynb)\n",
+                "* [Derivation (Uniform)](kochanek-bartels-uniform.ipynb)\n",
+                "* [Derivation (Non-Uniform)](kochanek-bartels-non-uniform.ipynb)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
@@ -56,13 +56,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.1+"
+            "version": "3.9.7"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/euclidean/index.ipynb` & `splines-0.3.0/doc/index.ipynb`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9092261904761905%*

 * *Differences: {"'cells'": "{0: {'source': ['This notebook is part of "*

 * *            'https://github.com/AudioSceneDescriptionFormat/splines, see also '*

 * *            "https://splines.readthedocs.io/.']}, 3: {'metadata': {replace: OrderedDict([('tags', "*

 * *            "['nbsphinx-toctree'])])}, 'source': ['* [Introduction](intro.rst)\\n', '* [Polynomial "*

 * *            "Curves in Euclidean Space](euclidean/index.ipynb)\\n', '* [Rotation "*

 * *            "Splines](rotation/index.ipynb)\\n', '* [Python Module](python-module.rst)\\n', […]*

```diff
@@ -2,59 +2,101 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "source": [
-                "This notebook is part of https://github.com/AudioSceneDescriptionFormat/splines, see also https://splines.readthedocs.io/.\n",
-                "\n",
-                "[back to overview](../index.ipynb)"
+                "This notebook is part of https://github.com/AudioSceneDescriptionFormat/splines, see also https://splines.readthedocs.io/."
             ]
         },
         {
-            "cell_type": "markdown",
-            "metadata": {},
+            "cell_type": "raw",
+            "metadata": {
+                "jupyter": {
+                    "source_hidden": true
+                },
+                "raw_mimetype": "text/restructuredtext",
+                "tags": []
+            },
             "source": [
-                "# Polynomial Curves in Euclidean Space"
+                ".. include:: ../README.rst"
+            ]
+        },
+        {
+            "cell_type": "raw",
+            "metadata": {
+                "jupyter": {
+                    "source_hidden": true
+                },
+                "raw_mimetype": "text/html",
+                "tags": []
+            },
+            "source": [
+                "<details>\n",
+                "<summary>click here to see full table of contents</summary>"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "nbsphinx-toctree": {}
+                "tags": [
+                    "nbsphinx-toctree"
+                ]
+            },
+            "source": [
+                "* [Introduction](intro.rst)\n",
+                "* [Polynomial Curves in Euclidean Space](euclidean/index.ipynb)\n",
+                "* [Rotation Splines](rotation/index.ipynb)\n",
+                "* [Python Module](python-module.rst)\n",
+                "* [References](references.rst)"
+            ]
+        },
+        {
+            "cell_type": "raw",
+            "metadata": {
+                "jupyter": {
+                    "source_hidden": true
+                },
+                "raw_mimetype": "text/html",
+                "tags": []
+            },
+            "source": [
+                "</details>"
+            ]
+        },
+        {
+            "cell_type": "raw",
+            "metadata": {
+                "jupyter": {
+                    "source_hidden": true
+                },
+                "raw_mimetype": "text/restructuredtext",
+                "tags": []
             },
             "source": [
-                "* [Polynomial Parametric Curves](polynomials.ipynb)\n",
-                "* [Lagrange Interpolation](lagrange.ipynb)\n",
-                "* [Hermite Splines](hermite.ipynb)\n",
-                "* [Natural Splines](natural.ipynb)\n",
-                "* [B\u00e9zier Splines](bezier.ipynb)\n",
-                "* [Catmull--Rom Splines](catmull-rom.ipynb)\n",
-                "* [Kochanek--Bartels Splines](kochanek-bartels.ipynb)\n",
-                "* [End Conditions](end-conditions.ipynb)\n",
-                "* [Piecewise Monotone Interpolation](piecewise-monotone.ipynb)"
+                ".. include:: how-to-navigate.rst"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.1+"
+            "version": "3.11.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/euclidean/kochanek-bartels-non-uniform.ipynb` & `splines-0.3.0/doc/euclidean/kochanek-bartels-non-uniform.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987284593621399%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(2, \'<cite data-cite-t="kochanek1984tcb">Kochanek and '*

 * *            "Bartels (1984)</cite>\\n'), (3, 'mainly talk about uniform splines.\\n'), (5, 'do "*

 * *            "they briefly mention the non-uniform case\\n')], delete: [5, 3, 2]}}, 2: {'source': "*

 * *            '{insert: [(34, \'> ---<cite data-cite-t="kochanek1984tcb">Kochanek and Bartels '*

 * *            "(1984)</cite>, section 4')], delete: [34]}}, 6: {'source': {insert: [(6, '[notebook "*

 * *            "about Catmull […]*

```diff
@@ -13,18 +13,18 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Non-Uniform Kochanek--Bartels Splines\n",
                 "\n",
-                "<cite data-cite=\"kochanek1984tcb\">Kochanek and Bartels (1984)</cite>\n",
-                "mainly talks about uniform splines.\n",
+                "<cite data-cite-t=\"kochanek1984tcb\">Kochanek and Bartels (1984)</cite>\n",
+                "mainly talk about uniform splines.\n",
                 "Only in section 4 -- \"Adjustments for Parameter Step Size\" --\n",
-                "the authors briefly mention the non-uniform case\n",
+                "do they briefly mention the non-uniform case\n",
                 "and provide equations for \"adjusted tangent vectors\":"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -58,15 +58,15 @@
                 "DD_i\n",
                 "\\frac{2 N_{i-1}}{N_{i-1} + N_i}\\\\\n",
                 "\\text{adjusted } DS_i &=\n",
                 "DS_i\n",
                 "\\frac{2 N_i}{N_{i-1} + N_i}\n",
                 "\\end{align*}\n",
                 ">\n",
-                "> ---<cite data-cite=\"kochanek1984tcb\">Kochanek and Bartels (1984)</cite>, section 4, \"Adjustments for Parameter Step Size\""
+                "> ---<cite data-cite-t=\"kochanek1984tcb\">Kochanek and Bartels (1984)</cite>, section 4"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "In their notation,\n",
@@ -112,15 +112,15 @@
             "source": [
                 "We can see that the uniform tangents are re-scaled\n",
                 "but their direction is unchanged.\n",
                 "\n",
                 "This is a hint that\n",
                 "-- although the paper claims to be using Catmull--Rom splines --\n",
                 "we'll get different results than in the\n",
-                "[notebooks about Catmull--Rom splines](catmull-rom-properties.ipynb#Tangent-Vectors)."
+                "[notebook about Catmull--Rom splines](catmull-rom-properties.ipynb#Tangent-Vectors)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -132,16 +132,17 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We'll need the Hermite basis matrix\n",
                 "that we derived in the\n",
                 "[notebook about uniform Hermite splines](hermite-uniform.ipynb#Basis-Matrix)\n",
-                "and which is also shown in equation 2 of\n",
-                "<cite data-cite=\"kochanek1984tcb\">Kochanek and Bartels (1984)</cite>:"
+                "and which is also shown by\n",
+                "<cite data-cite-t=\"kochanek1984tcb\">Kochanek and Bartels (1984)</cite>\n",
+                "in equation 2:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -245,17 +246,17 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This doesn't look too bad,\n",
-                "let's plot the same thing with the\n",
+                "let's plot the same thing with\n",
                 "[splines.CatmullRom](../python-module/splines.rst#splines.CatmullRom)\n",
-                "class for comparison."
+                "for comparison."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `splines-0.2.0/doc/euclidean/kochanek-bartels-properties.ipynb` & `splines-0.3.0/doc/euclidean/kochanek-bartels-properties.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9820140692640693%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'Kochanek--Bartels splines\\n'), (10, '$T$ for "*

 * *            "*tension*,\\n'), (11, '$C$ for *continuity* and\\n'), (12, '$B$ for *bias*.\\n'), "*

 * *            "(15, 'If the *tension* parameter also has its default value $T = 0$,\\n')], delete: "*

 * *            "[15, 12, 11, 10, 2]}}, 2: {'source': ['import splines\\n', 'from helper import "*

 * *            'plot_spline_2d\']}, 3: {\'source\': ["Let\'s use a bespoke plotting function\\n", '*

 * *            "'from [kochanek_barte […]*

```diff
@@ -13,192 +13,162 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Properties of Kochanek--Bartels Splines\n",
                 "\n",
-                "Kochanek--Bartels splines (a.k.a. TCB splines)\n",
+                "Kochanek--Bartels splines\n",
                 "are interpolating cubic polynomial splines,\n",
                 "with three user-defined parameters per vertex\n",
                 "(of course they can also be chosen to be\n",
                 "the same three values for the whole spline),\n",
                 "which can be used to change the shape and velocity of the spline.\n",
                 "\n",
                 "These three parameters are called\n",
-                "$T$ for \"tension\",\n",
-                "$C$ for \"continuity\" and\n",
-                "$B$ for \"bias\".\n",
+                "$T$ for *tension*,\n",
+                "$C$ for *continuity* and\n",
+                "$B$ for *bias*.\n",
                 "With the default values of $C = 0$ and $B = 0$,\n",
                 "a Kochanek--Bartels spline is identical to a *cardinal spline*.\n",
-                "If the \"tension\" parameter also has its default value $T = 0$,\n",
+                "If the *tension* parameter also has its default value $T = 0$,\n",
                 "it is also identical to a [Catmull--Rom spline](catmull-rom.ipynb)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import splines"
+                "import splines\n",
+                "from helper import plot_spline_2d"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Let's import a plotting function from [helper.py](helper.py) ..."
+                "Let's use a bespoke plotting function\n",
+                "from [kochanek_bartels.py](kochanek_bartels.py)\n",
+                "to illustrate the TCB parameters:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from helper import plot_spline_2d"
+                "from kochanek_bartels import plot_tcb"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "... and use it to implement a bespoke plotting function\n",
-                "to illustrate the TCB parameters:"
+                "## Tension"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import matplotlib.pyplot as plt\n",
-                "import numpy as np\n",
-                "\n",
-                "def plot_tcb(*tcb, ax=None):\n",
-                "    \"\"\"Plot four TCB examples.\"\"\"\n",
-                "    if ax is None:\n",
-                "        ax = plt.gca()\n",
-                "    vertices = [\n",
-                "        (-3.5, 0),\n",
-                "        (-1, 1.5),\n",
-                "        (0, 0.1),\n",
-                "        (1, 1.5),\n",
-                "        (3.5, 0),\n",
-                "        (1, -1.5),\n",
-                "        (0, -0.1),\n",
-                "        (-1, -1.5),\n",
-                "    ]\n",
-                "    for idx, tcb in zip([1, 7, 3, 5], tcb):\n",
-                "        all_tcb = np.zeros((len(vertices), 3))\n",
-                "        all_tcb[idx] = tcb\n",
-                "        s = splines.KochanekBartels(\n",
-                "            vertices, tcb=all_tcb, endconditions='closed')\n",
-                "        label = ', '.join(\n",
-                "            f'{name} = {value}'\n",
-                "            for name, value in zip('TCB', tcb)\n",
-                "            if value)\n",
-                "        plot_spline_2d(s, chords=False, label=label, ax=ax)\n",
-                "    plot_spline_2d(\n",
-                "        splines.KochanekBartels(vertices, endconditions='closed'),\n",
-                "        color='lightgrey', chords=False, ax=ax)\n",
-                "    lines = [l for l in ax.get_lines() if not l.get_label().startswith('_')]\n",
-                "    # https://matplotlib.org/tutorials/intermediate/legend_guide.html#multiple-legends-on-the-same-axes\n",
-                "    ax.add_artist(ax.legend(\n",
-                "        handles=lines[:2], bbox_to_anchor=(0, 0., 0.5, 1),\n",
-                "        loc='center', numpoints=3))\n",
-                "    ax.legend(\n",
-                "        handles=lines[2:], bbox_to_anchor=(0.5, 0., 0.5, 1),\n",
-                "        loc='center', numpoints=3)"
+                "plot_tcb((0.5, 0, 0), (1, 0, 0), (-0.5, 0, 0), (-1, 0, 0))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Tension"
+                "## Continuity"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plot_tcb((0.5, 0, 0), (1, 0, 0), (-0.5, 0, 0), (-1, 0, 0))"
+                "plot_tcb((0, -0.5, 0), (0, -1, 0), (0, 0.5, 0), (0, 1, 0))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Continuity"
+                "Note that the cases $T = 1$ and $C = -1$\n",
+                "have a very similar shape\n",
+                "(a.k.a. [image](https://en.wikipedia.org/wiki/Image_(mathematics))),\n",
+                "but they have a different timing\n",
+                "(and therefore different velocities):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plot_tcb((0, -0.5, 0), (0, -1, 0), (0, 0.5, 0), (0, 1, 0))"
+                "plot_tcb((1, 0, 0), (0, -1, 0), (0.5, 0, 0), (0, -0.5, 0))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Note that the cases $T = 1$ and $C = -1$\n",
-                "have a very similar shape (a.k.a. \"image\"),\n",
-                "but they have a different timing\n",
-                "(and therefore different velocities):"
+                "A value of $C=-1$ on adjacent vertices leads to linear segments\n",
+                "with piecewise constant speeds:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plot_tcb((1, 0, 0), (0, -1, 0), (0.5, 0, 0), (0, -0.5, 0))"
+                "vertices1 = [(0, 0), (1, 1), (0, 2), (3, 2), (4, 1), (3, 0)]\n",
+                "s1a = splines.KochanekBartels(vertices1, tcb=(0, -1, 0), endconditions='closed')\n",
+                "plot_spline_2d(s1a, chords=False)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "A value of $C=-1$ on adjacent vertices leads to linear segments:"
+                "A value of $T=1$ will lead to linear segments as well,\n",
+                "but the speed will fluctuate in each segment,\n",
+                "coming to a complete halt at each control point:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "vertices1 = [(0, 0), (1, 1), (0, 2), (3, 2), (4, 1), (3, 0)]\n",
-                "s1 = splines.KochanekBartels(vertices1, tcb=(0, -1, 0), endconditions='closed')\n",
-                "plot_spline_2d(s1, chords=False)"
+                "s1b = splines.KochanekBartels(vertices1, tcb=(1, 0, 0), endconditions='closed')\n",
+                "plot_spline_2d(s1b, chords=False)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Bias"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This could also be called \"overshoot\" (if $B > 0$)\n",
-                "and \"undershoot\" (if $B < 0$):"
+                "This could also be called *overshoot* (if $B > 0$)\n",
+                "and *undershoot* (if $B < 0$):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -246,15 +216,17 @@
                 "plot_spline_2d(s3, chords=False)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Combinations"
+                "## Combinations\n",
+                "\n",
+                "Of course, multiple parameters can be combined:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -270,27 +242,27 @@
             "source": [
                 "plot_tcb((1, 0, 1), (-1, 0, 1), (0, -1, 1), (0, 1, -1))"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.11.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/euclidean/kochanek-bartels-uniform.ipynb` & `splines-0.3.0/doc/euclidean/kochanek-bartels-uniform.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998155871046738%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(3, '-- see also equation 3 of the paper by\\n'), (4, '<cite "*

 * *            'data-cite-t="kochanek1984tcb">Kochanek and Bartels (1984)</cite>:\\n\')], delete: [4, '*

 * *            "3]}}, 3: {'source': {insert: [(2, 'Deriving *TCB splines* is all about inserting the "*

 * *            "parameters\\n')], delete: [2]}}, 4: {'source': {insert: [(2, '<cite "*

 * *            'data-cite-t="kochanek1984tcb">Kochanek and Bartels (1984)</cite>\\n\'), (3, \'show '*

 * *            "the usage of $T$ […]*

```diff
@@ -21,16 +21,16 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "As a starting point,\n",
                 "remember the\n",
                 "[tangent vectors of uniform Catmull--Rom splines](catmull-rom-properties.ipynb#Tangent-Vectors)\n",
-                "(see also equation 3 of\n",
-                "<cite data-cite=\"kochanek1984tcb\">the Kochanek/Bartels (1984) paper</cite>):\n",
+                "-- see also equation 3 of the paper by\n",
+                "<cite data-cite-t=\"kochanek1984tcb\">Kochanek and Bartels (1984)</cite>:\n",
                 "\n",
                 "\\begin{equation*}\n",
                 "\\boldsymbol{\\dot{x}}_i = \\frac{\\boldsymbol{x}_{i+1} - \\boldsymbol{x}_{i-1}}{2},\n",
                 "\\end{equation*}\n",
                 "\n",
                 "which can be re-written as\n",
                 "\n",
@@ -44,26 +44,26 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Parameters\n",
                 "\n",
-                "*TCB splines* are all about inserting the parameters\n",
+                "Deriving *TCB splines* is all about inserting the parameters\n",
                 "$T$, $C$ and $B$ into this equation."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Tension\n",
                 "\n",
-                "The usage of $T$ is shown in equation 4 of\n",
-                "<cite data-cite=\"kochanek1984tcb\">the Kochanek/Bartels (1984) paper</cite>:\n",
+                "<cite data-cite-t=\"kochanek1984tcb\">Kochanek and Bartels (1984)</cite>\n",
+                "show the usage of $T$ in equation 4:\n",
                 "\n",
                 "\\begin{equation*}\n",
                 "\\boldsymbol{\\dot{x}}_i = (1 - T_i) \\frac{\n",
                 "(\\boldsymbol{x}_i - \\boldsymbol{x}_{i-1}) +\n",
                 "(\\boldsymbol{x}_{i+1} - \\boldsymbol{x}_i)\n",
                 "}{2}\n",
                 "\\end{equation*}"
@@ -86,19 +86,19 @@
                 "This also happens to be the requirement for a spline to be $C^1$ continuous."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The \"continuity\" parameter $C$\n",
+                "The *continuity* parameter $C$\n",
                 "allows us to break this continuity if we so desire,\n",
                 "leading to different incoming and outgoing tangent vectors\n",
-                "(see equations 5 and 6 in\n",
-                "<cite data-cite=\"kochanek1984tcb\">the Kochanek/Bartels (1984) paper</cite>):\n",
+                "-- see equations 5 and 6 in the paper by\n",
+                "<cite data-cite-t=\"kochanek1984tcb\">Kochanek and Bartels (1984)</cite>:\n",
                 "\n",
                 "\\begin{align*}\n",
                 "\\boldsymbol{\\dot{x}}_i^{(-)} &= \\frac{\n",
                 "(1 - C_i) (\\boldsymbol{x}_i - \\boldsymbol{x}_{i-1}) +\n",
                 "(1 + C_i) (\\boldsymbol{x}_{i+1} - \\boldsymbol{x}_i)\n",
                 "}{2}\\\\\n",
                 "\\boldsymbol{\\dot{x}}_i^{(+)} &= \\frac{\n",
@@ -110,16 +110,16 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Bias\n",
                 "\n",
-                "The usage of $B$ is shown in equation 7 of\n",
-                "<cite data-cite=\"kochanek1984tcb\">the Kochanek/Bartels (1984) paper</cite>:\n",
+                "<cite data-cite-t=\"kochanek1984tcb\">Kochanek and Bartels (1984)</cite>\n",
+                "show the usage of $B$ in equation 7:\n",
                 "\n",
                 "\\begin{equation*}\n",
                 "\\boldsymbol{\\dot{x}}_i = \\frac{\n",
                 "(1 + B_i) (\\boldsymbol{x}_i - \\boldsymbol{x}_{i-1}) +\n",
                 "(1 - B_i) (\\boldsymbol{x}_{i+1} - \\boldsymbol{x}_i)\n",
                 "}{2}\n",
                 "\\end{equation*}"
@@ -129,16 +129,16 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### All Three Combined\n",
                 "\n",
                 "To get the tangent vectors of a TCB spline,\n",
                 "the three equations can be combined\n",
-                "(see equations 8 and 9 in\n",
-                "<cite data-cite=\"kochanek1984tcb\">the Kochanek/Bartels (1984) paper</cite>):\n",
+                "-- see equations 8 and 9 in the paper by\n",
+                "<cite data-cite=\"kochanek1984tcb\">Kochanek Bartels (1984)</cite>:\n",
                 "\n",
                 "\\begin{align*}\n",
                 "\\boldsymbol{\\dot{x}}_i^{(+)} &= \\frac{\n",
                 "(1 - T_i) (1 + C_i) (1 + B_i) (\\boldsymbol{x}_i - \\boldsymbol{x}_{i-1}) +\n",
                 "(1 - T_i) (1 - C_i) (1 - B_i) (\\boldsymbol{x}_{i+1} - \\boldsymbol{x}_i)\n",
                 "}{2}\\\\\n",
                 "\\boldsymbol{\\dot{x}}_i^{(-)} &= \\frac{\n",
@@ -152,29 +152,28 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "<div class=\"alert alert-info\">\n",
                 "\n",
                 "Note\n",
                 "\n",
-                "There is an error in equation (6.11) of \n",
-                "<cite data-cite=\"millington2009matrices\">Ian Millington's paper</cite>.\n",
+                "There is an error in equation (6.11) from \n",
+                "<cite data-cite-t=\"millington2009matrices\">Millington (2009)</cite>.\n",
                 "All subscripts of $x$ are wrong,\n",
                 "most likely copy-pasted from the preceding equation.\n",
                 "\n",
                 "</div>"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "To simplify the results we will get later, we introduce the following shorthands\n",
-                "(as suggested in\n",
-                "<cite data-cite=\"millington2009matrices\">Millington's paper</cite>):\n",
+                "<cite data-cite=\"millington2009matrices\">(Millington 2009)</cite>:\n",
                 "\n",
                 "\\begin{align*}\n",
                 "a_i &= (1 - T_i) (1 + C_i) (1 + B_i),\\\\\n",
                 "b_i &= (1 - T_i) (1 - C_i) (1 - B_i),\\\\\n",
                 "c_i &= (1 - T_i) (1 - C_i) (1 + B_i),\\\\\n",
                 "d_i &= (1 - T_i) (1 + C_i) (1 - B_i),\n",
                 "\\end{align*}"
@@ -200,17 +199,17 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Calculation\n",
                 "\n",
-                "The tangent vectors are sufficient to implement\n",
+                "The above tangent vectors are sufficient to implement\n",
                 "Kochanek--Bartels splines\n",
-                "(via [Hermite splines](hermite.ipynb)).\n",
+                "via [Hermite splines](hermite.ipynb).\n",
                 "In the rest of this notebook we are deriving\n",
                 "the basis matrix and the basis polynomials\n",
                 "for comparison with other spline types."
             ]
         },
         {
             "cell_type": "code",
@@ -353,15 +352,15 @@
                 "### Basis Matrix"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We try to find a transformation\n",
+                "Let's try to find a transformation\n",
                 "from the control values defined above\n",
                 "to *Hermite control values*:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -499,25 +498,24 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "To be able to plot the basis functions,\n",
-                "let's substitute $a_4$, $b_4$, $c_5$ and $d_5$ back in (which isn't pretty):"
+                "let's substitute $a_4$, $b_4$, $c_5$ and $d_5$ back in:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "b_KB = b_KB.subs_symbols(a4, b4, c5, d5).simplify()\n",
-                "b_KB.T.pull_out(sp.S.Half)"
+                "b_KB = b_KB.subs_symbols(a4, b4, c5, d5).simplify()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Let's use a helper function from [helper.py](helper.py):"
```

### Comparing `splines-0.2.0/doc/euclidean/lagrange.ipynb` & `splines-0.3.0/doc/euclidean/lagrange.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9619734317146276%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(2, 'Assume we have $N$ time instants $t_i$, with $0 \\\\le "*

 * *            "i < N$ ...')], delete: [2]}}, 4: {'source': ['ts = -1.5, 0.5, 1.7, 3.5, 4']}, 7: "*

 * *            '{\'source\': {insert: [(2, \'some "reasonable" interpolated values when evaluated at '*

 * *            "time values in between.\\n'), (5, '$\\\\ell_i(t)$\\n'), (7, 'which will be weighted "*

 * *            "by the associated $x_i$.\\n'), (11, 'L(t) = \\\\sum_{i=0}^{N-1} x_i "*

 * *            '\\\\ell_i(t)\\n\')],  […]*

```diff
@@ -36,24 +36,24 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## One-dimensional Example\n",
                 "\n",
-                "Assume we have $N$ time instants $t_i$, with $0 \\le i < N$:"
+                "Assume we have $N$ time instants $t_i$, with $0 \\le i < N$ ..."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ts = -1.5, 0.5, 1.7, 3, 4"
+                "ts = -1.5, 0.5, 1.7, 3.5, 4"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "... and for each time instant we are given an associated value $x_i$:"
@@ -70,24 +70,24 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Our task is now to find a function that yields\n",
                 "the given $x_i$ values for the given times $t_i$ and\n",
-                "some \"reasonable\" interpolated values when evaluated at time values in-between.\n",
+                "some \"reasonable\" interpolated values when evaluated at time values in between.\n",
                 "\n",
                 "The idea of Lagrange interpolation is to create a separate polynomial\n",
-                "$\\ell_j(t)$\n",
+                "$\\ell_i(t)$\n",
                 "for each of the $N$ given time instants,\n",
-                "which will be weighted by the associated $x_j$.\n",
+                "which will be weighted by the associated $x_i$.\n",
                 "The final interpolation function is the weighted sum of these $N$ polynomials:\n",
                 "\n",
                 "\\begin{equation*}\n",
-                "L(t) = \\sum_{j=0}^{N-1} x_j \\ell_j(t)\n",
+                "L(t) = \\sum_{i=0}^{N-1} x_i \\ell_i(t)\n",
                 "\\end{equation*}"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -101,26 +101,30 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "To satisfy the second point,\n",
                 "let's create a product with a term for each of the relevant times\n",
                 "and make each of those factors vanish when evaluated at their associated time.\n",
-                "As an example we look at the basis for $t_3 = 3$:"
+                "For example, let's look at the basis for $i = 3$:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def maybe_polynomial_3(t):\n",
                 "    t = np.asarray(t)\n",
-                "    return (t - (-1.5)) * (t - 0.5) * (t - 1.7) * (t - 4)"
+                "    return (\n",
+                "        (t - (-1.5)) *\n",
+                "        (t - 0.5) *\n",
+                "        (t - 1.7) *\n",
+                "        (t - 4))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -130,46 +134,41 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "As we can see, this indeed fulfills the second requirement.\n",
                 "Note that we were given 5 time instants,\n",
-                "but we need only 4 product terms\n",
-                "(corresponding to the 4 roots of the polynomial).\n",
-                "Mathematically, this could be written as\n",
-                "\n",
-                "\\begin{equation*}\n",
-                "\\ell_j(t) \\overset{?}{=} \\prod_{\\substack{i=0\\\\i \\ne j}}^{N-1} t - t_i.\n",
-                "\\end{equation*}"
+                "but we only need 4 product terms\n",
+                "(corresponding to the 4 roots of the polynomial)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Now, for the first requirement,\n",
-                "we can divide each term to yield $1$ when evaluated at $t = 3$\n",
+                "we can divide each term to yield $1$ when evaluated at $t = t_3 = 3.5$\n",
                 "(luckily, this will not violate the second requirement).\n",
                 "If each term is $1$, the whole product will also be $1$:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def polynomial_3(t):\n",
                 "    t = np.asarray(t)\n",
                 "    return (\n",
-                "        (t - (-1.5)) / (3 - (-1.5)) *\n",
-                "        (t - 0.5) / (3 - 0.5) *\n",
-                "        (t - 1.7) / (3 - 1.7) *\n",
-                "        (t - 4) / (3 - 4))"
+                "        (t - (-1.5)) / (3.5 - (-1.5)) *\n",
+                "        (t - 0.5) / (3.5 - 0.5) *\n",
+                "        (t - 1.7) / (3.5 - 1.7) *\n",
+                "        (t - 4) / (3.5 - 4))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -184,27 +183,14 @@
                 "That's it!"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Generally,\n",
-                "Lagrange basis polynomials can be written as\n",
-                "\n",
-                "\\begin{equation*}\n",
-                "\\ell_j(t) = \\prod_{\\substack{i=0\\\\i \\ne j}}^{N-1}\n",
-                "\\frac{t - t_i}{t_j - t_i}.\n",
-                "\\end{equation*}"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
                 "To get a better idea what's going on between the given time instances $t_i$,\n",
                 "let's plot this polynomial\n",
                 "(with a little help from [helper.py](helper.py)):"
             ]
         },
         {
             "cell_type": "code",
@@ -238,16 +224,21 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We can see from its shape that this is a polynomial of degree 4,\n",
                 "which makes sense because the product we are using has 4 terms\n",
                 "containing one $t$ each.\n",
                 "We can also see that it has the value $0$ at each of the initially provided\n",
-                "time instances $t_i$, except for $t_3 = 3$, where it has the value $1$.\n",
-                "\n",
+                "time instances $t_i$, except for $t_3 = 3.5$, where it has the value $1$."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "The above calculation can be easily generalized to be able to get\n",
                 "any one of the set of polynomials defined by an arbitrary list of time instants:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -265,26 +256,39 @@
                 "    ])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Now we can calculate and visualize all 5 polynomials\n",
+                "Putting this in mathematic notation,\n",
+                "Lagrange basis polynomials can be written as\n",
+                "\n",
+                "\\begin{equation*}\n",
+                "\\ell_i(t) = \\prod_{\\substack{j=0\\\\i \\ne j}}^{N-1}\n",
+                "\\frac{t - t_j}{t_i - t_j}.\n",
+                "\\end{equation*}"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Now we can calculate and visualize all 5 basis polynomials\n",
                 "for our 5 given time instants:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "polys = np.column_stack([lagrange_polynomial(ts, i, plot_times)\n",
-                "                         for i in range(len(ts))])"
+                "polys = np.column_stack(\n",
+                "    [lagrange_polynomial(ts, i, plot_times) for i in range(len(ts))])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -293,17 +297,17 @@
                 "grid_lines(ts, [0, 1])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Finally, the interpolated values can be obtained\n",
-                "by applying the given $x_i$ values as weights to the polynomials\n",
-                "and summing everything together:"
+                "Finally, the interpolated values $L(t)$ can be obtained\n",
+                "by applying the given $x_i$ values as weights to the polynomials $\\ell_i(t)$\n",
+                "and summing everything up together:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -335,18 +339,15 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Neville's Algorithm\n",
                 "\n",
                 "An alternative way to calculate interpolated values is\n",
-                "[Neville's algorithm](https://en.wikipedia.org/wiki/Neville%27s_algorithm)\n",
-                "(see also\n",
-                "<cite data-cite=\"barry1988recursive\">Barry and Goldman (1988)</cite>,\n",
-                "figure 2).\n",
+                "[Neville's algorithm](https://en.wikipedia.org/wiki/Neville's_algorithm).\n",
                 "We mention this algorithm mainly because it is referenced in the\n",
                 "[derivation of non-uniform Catmull--Rom splines](catmull-rom-non-uniform.ipynb)\n",
                 "and the\n",
                 "[description of the Barry--Goldman algorithm](catmull-rom-barry-goldman.ipynb)."
             ]
         },
         {
@@ -384,45 +385,96 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "In each stage of the algorithm,\n",
                 "linear interpolation is used to interpolate between adjacent values,\n",
-                "leading to one fewer value than in the stage before.\n",
+                "leading to one less value than in the stage before.\n",
                 "The new values are used as input to the next stage and so on.\n",
                 "When there is only one value left, this value is the result.\n",
                 "\n",
                 "The only tricky part is\n",
                 "to choose the appropriate time interval for each interpolation.\n",
                 "In the first stage,\n",
                 "the intervals between the given time values are used.\n",
                 "In the second stage,\n",
                 "each time interval is combined with the following one,\n",
-                "leading to one fewer time intervals in total.\n",
+                "leading to one less time intervals in total.\n",
                 "In the third stage,\n",
                 "each time interval is combined with the following two intervals,\n",
                 "and so on until the last stage,\n",
                 "where all time intervals are combined into a single large interval."
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "<cite data-cite-t=\"barry1988recursive\">Barry and Goldman (1988)</cite>\n",
+                "show (in figure 2) the cubic case,\n",
+                "which looks something like this:\n",
+                "\n",
+                "\\begin{equation*}\n",
+                "\\def\\negspace{\\!\\!\\!\\!\\!\\!}\n",
+                "\\begin{array}{ccccccccccccc}\n",
+                "&&&&&&\n",
+                "\\boldsymbol{p}_{0,1,2,3}\n",
+                "&&&&&&\n",
+                "\\\\\n",
+                "&&&&&\n",
+                "\\negspace \\frac{t_3 - t}{t_3 - t_0} \\negspace\n",
+                "&&\n",
+                "\\negspace \\frac{t - t_0}{t_3 - t_0} \\negspace\n",
+                "&&&&&\n",
+                "\\\\\n",
+                "&&&& \\boldsymbol{p}_{0,1,2} &&&& \\boldsymbol{p}_{1,2,3} &&&&\n",
+                "\\\\\n",
+                "&&\n",
+                "& \\negspace \\frac{t_2 - t}{t_2 - t_0} \\negspace && \\negspace \\frac{t - t_0}{t_2 - t_0} \\negspace &\n",
+                "& \\negspace \\frac{t_3 - t}{t_3 - t_1} \\negspace && \\negspace \\frac{t - t_1}{t_3 - t_1} \\negspace &\n",
+                "&&\n",
+                "\\\\\n",
+                "&& \\boldsymbol{p}_{0,1} &&&& \\boldsymbol{p}_{1,2} &&&& \\boldsymbol{p}_{2,3} &&\n",
+                "\\\\\n",
+                "& \\negspace \\frac{t_1 - t}{t_1 - t_0} \\negspace && \\negspace \\frac{t - t_0}{t_1 - t_0} \\negspace &\n",
+                "& \\negspace \\frac{t_2 - t}{t_2 - t_1} \\negspace && \\negspace \\frac{t - t_1}{t_2 - t_1} \\negspace &\n",
+                "& \\negspace \\frac{t_3 - t}{t_3 - t_2} \\negspace && \\negspace \\frac{t - t_2}{t_3 - t_2} \\negspace &\n",
+                "\\\\\n",
+                "\\boldsymbol{x}_0 &&&& \\boldsymbol{x}_1 &&&& \\boldsymbol{x}_2 &&&& \\boldsymbol{x}_3\n",
+                "\\end{array}\n",
+                "\\end{equation*}"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The polynomial $\\boldsymbol{p}_{0,1,2,3}(t)$ at the apex\n",
+                "can be evaluated for $t_0 \\le t \\le t_3$.\n",
+                "For a detailed explanation of this triangular scheme, see the\n",
+                "[notebook about the Barry--Goldman algorithm](catmull-rom-barry-goldman.ipynb#Triangular-Schemes).\n",
+                "Neville's algorithm can be implemented for arbitrary degree:"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def neville(xs, ts, t):\n",
                 "    \"\"\"Lagrange interpolation using Neville's algorithm.\n",
                 "    \n",
                 "    Returns the interpolated value(s) at time(s) *t*,\n",
                 "    given the values *xs* at times *ts*.\n",
                 "    \n",
                 "    \"\"\"\n",
-                "    assert len(xs) == len(ts)\n",
+                "    if len(xs) != len(ts):\n",
+                "        raise ValueError('xs and ts must have the same length')\n",
                 "    while len(xs) > 1:\n",
                 "        step = len(ts) - len(xs) + 1\n",
                 "        xs = [\n",
                 "            lerp(*args, t)\n",
                 "            for args in zip(zip(xs, xs[1:]), zip(ts, ts[step:]))]\n",
                 "    return xs[0]"
             ]
@@ -438,15 +490,15 @@
                 "grid_lines(ts)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Two-dimensional Example\n",
+                "## Two-Dimensional Example\n",
                 "\n",
                 "Lagrange interpolation can of course also be used in higher-dimensional spaces.\n",
                 "To show this, let's create a little class:"
             ]
         },
         {
             "cell_type": "code",
@@ -494,15 +546,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "l1 = Lagrange([(2, -2), (-1, 0), (1.3, 0.5), (3.14, 0), (1, -1)], ts)"
+                "l1 = Lagrange([(2, -2), (-1, 0), (0.3, 0.5), (3.14, -1), (1, -1)], ts)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -512,66 +564,143 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Runge's Phenomenon\n",
                 "\n",
-                "This seems to work reasonably well,\n",
+                "This seems to work to some degree,\n",
                 "but as indicated above,\n",
                 "Lagrange implementation has a severe limitation.\n",
                 "This limitation gets more apparent when using more vertices,\n",
                 "which leads to a higher-degree polynomial."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "vertices = [\n",
-                "    (1, 0),\n",
-                "    (1, 2),\n",
-                "    (3, 0),\n",
+                "vertices1 = [\n",
+                "    (-2, 3),\n",
+                "    (1, 1),\n",
+                "    (3, -1),\n",
                 "    (2, -1),\n",
                 "    (2.5, 1.5),\n",
                 "    (5, 2),\n",
                 "    (6, 1),\n",
                 "    (5, 0),\n",
-                "    (6, -1),\n",
-                "    (7, 2),\n",
-                "    (4, 3),\n",
-                "]\n",
-                "times = range(len(vertices))"
+                "    (6.5, -1),\n",
+                "    (7, 0),\n",
+                "    (6, 3),\n",
+                "]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "l2 = Lagrange(vertices, times)\n",
+                "l2 = Lagrange(vertices1, range(len(vertices1)))\n",
                 "plot_spline_2d(l2)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Here we see a severe overshooting effect,\n",
                 "most pronounced at the beginning and the end of the curve.\n",
+                "Moving some vertices can make this even worse.\n",
                 "This effect is called\n",
                 "[Runge's phenomenon](https://en.wikipedia.org/wiki/Runge's_phenomenon).\n",
-                "\n",
+                "A possible mitigation for this overshooting\n",
+                "is to use so-called\n",
+                "[Chebyshev nodes](https://en.wikipedia.org/wiki/Chebyshev_nodes)\n",
+                "as time instances:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "def chebyshev_nodes(a, b, n):\n",
+                "    k = np.arange(n) + 1\n",
+                "    nodes = np.cos(np.pi * (2 * k - 1) / (2 * n))\n",
+                "    return (a + b) / 2 - (b - a) * nodes / 2"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "l3 = Lagrange(vertices1, chebyshev_nodes(0, len(vertices1) - 1, len(vertices1)))\n",
+                "plot_spline_2d(l3)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "This is definitely better.\n",
+                "But it gets worse again when we move a few of the vertices."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "vertices2 = [\n",
+                "    (0, -1),\n",
+                "    (1, 1),\n",
+                "    (3, -1),\n",
+                "    (2.5, 1.5),\n",
+                "    (5, 2),\n",
+                "    (6, 0.5),\n",
+                "    (6, 0),\n",
+                "    (4, -1),\n",
+                "    (6.5, -1),\n",
+                "    (7, 2),\n",
+                "    (8, 0),\n",
+                "]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "l4 = Lagrange(vertices2, chebyshev_nodes(0, len(vertices2) - 1, len(vertices2)))\n",
+                "plot_spline_2d(l4)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "Long story short,\n",
-                "Lagrange interpolation is typically not usable for drawing curves.\n",
-                "For comparison, let's use the same positions and time values\n",
-                "and create a [Catmull--Rom spline](catmull-rom.ipynb):"
+                "Lagrange interpolation is typically not suitable for drawing curves.\n",
+                "For comparison, and as a teaser for the following sections,\n",
+                "let's use the same vertices to create\n",
+                "a uniform [Catmull--Rom spline](catmull-rom.ipynb):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -581,15 +710,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "cr_spline = splines.CatmullRom(vertices, times)"
+                "cr_spline = splines.CatmullRom(vertices2)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -597,42 +726,66 @@
                 "plot_spline_2d(cr_spline)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This clearly doesn't have the overshooting problem we saw above.\n",
-                "\n",
+                "And to get an even better fit, we can try a\n",
+                "[centripetal Catmull--Rom spline](catmull-rom-properties.ipynb#Centripetal-Parameterization):"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "cr_centripetal_spline = splines.CatmullRom(vertices2, alpha=0.5)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "plot_spline_2d(cr_centripetal_spline)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "<div class=\"alert alert-info\">\n",
                 "\n",
                 "Note\n",
                 "\n",
-                "The [splines.CatmullRom](../python-module/splines.rst#splines.CatmullRom) class\n",
+                "The class [splines.CatmullRom](../python-module/splines.rst#splines.CatmullRom)\n",
                 "uses [\"natural\" end conditions](end-conditions-natural.ipynb) by default.\n",
                 "\n",
                 "</div>"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.2"
+            "version": "3.11.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/euclidean/natural-non-uniform.ipynb` & `splines-0.3.0/doc/euclidean/natural-non-uniform.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9854662698412698%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '[back to overview](natural.ipynb) -\\n'), (3, "*

 * *            "'[properties](natural-properties.ipynb) -\\n'), (4, '[derivation "*

 * *            "(uniform)](natural-uniform.ipynb)')], delete: [2]}}, 3: {'source': ['from utility "*

 * *            "import NamedExpression, dotproduct']}, 5: {'source': {insert: [(2, 'but now we must "*

 * *            "allow arbitrary parameter values:')], delete: [2]}}, 7: {'source': ['b_monomial = "*

 * *            "t**3, t**2, t, 1']}, 9: {'source':  […]*

```diff
@@ -4,15 +4,17 @@
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "source": [
                 "This notebook is part of https://github.com/AudioSceneDescriptionFormat/splines, see also https://splines.readthedocs.io/.\n",
                 "\n",
-                "[back to overview](natural.ipynb)"
+                "[back to overview](natural.ipynb) -\n",
+                "[properties](natural-properties.ipynb) -\n",
+                "[derivation (uniform)](natural-uniform.ipynb)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Non-Uniform Natural Splines\n",
@@ -34,15 +36,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from utility import NamedExpression"
+                "from utility import NamedExpression, dotproduct"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -52,15 +54,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Just like in the uniform case,\n",
                 "we are considering two adjacent spline segments,\n",
-                "but this time we must allow arbitrary parameter values:"
+                "but now we must allow arbitrary parameter values:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -70,16 +72,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "b_monomial = sp.Matrix([t**3, t**2, t, 1]).T\n",
-                "b_monomial"
+                "b_monomial = t**3, t**2, t, 1"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -90,29 +91,20 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "b_monomial.dot(coefficients3)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
                 "p3 = NamedExpression(\n",
                 "    'pbm3',\n",
-                "    b_monomial.dot(coefficients3).subs(t, (t - t3)/(t4 - t3)))\n",
+                "    dotproduct(b_monomial, coefficients3).subs(t, (t - t3)/(t4 - t3)))\n",
                 "p4 = NamedExpression(\n",
                 "    'pbm4',\n",
-                "    b_monomial.dot(coefficients4).subs(t, (t - t4)/(t5 - t4)))\n",
+                "    dotproduct(b_monomial, coefficients4).subs(t, (t - t4)/(t5 - t4)))\n",
                 "display(p3, p4)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -184,15 +176,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "for c, e in coefficients.items():\n",
-                "    display(NamedExpression(c, e.subs(deltas)))"
+                "    display(NamedExpression(c, e.factor().subs(deltas).simplify()))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -246,15 +238,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We are not showing the full matrix here,\n",
-                "because it would be quite a bit more complicated and less helpful than\n",
+                "because it would be quite a bit more complicated and less instructive than\n",
                 "in the uniform case."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -303,27 +295,27 @@
                 "Other end conditions can be derived as shown in\n",
                 "[the notebook about uniform \"natural\" splines](natural-uniform.ipynb#End-Conditions)."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.2"
+            "version": "3.11.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/euclidean/natural-uniform.ipynb` & `splines-0.3.0/doc/euclidean/natural-uniform.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9831507485569986%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '[back to overview](natural.ipynb) -\\n'), (3, "*

 * *            "'[properties](natural-properties.ipynb) -\\n'), (4, '[derivation "*

 * *            "(non-uniform)](natural-non-uniform.ipynb)')], delete: [2]}}, 1: {'source': {insert: "*

 * *            "[(5, 'is chosen to be $1$.\\n')], delete: [5]}}, 3: {'source': ['We import some "*

 * *            "helpers from [utility.py](utility.py):']}, 4: {'source': ['from utility import "*

 * *            'NamedExpression, dotproduct\']}, 7: {\'s […]*

```diff
@@ -4,27 +4,29 @@
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "source": [
                 "This notebook is part of https://github.com/AudioSceneDescriptionFormat/splines, see also https://splines.readthedocs.io/.\n",
                 "\n",
-                "[back to overview](natural.ipynb)"
+                "[back to overview](natural.ipynb) -\n",
+                "[properties](natural-properties.ipynb) -\n",
+                "[derivation (non-uniform)](natural-non-uniform.ipynb)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Uniform Natural Splines\n",
                 "\n",
                 "For deriving natural splines,\n",
                 "we first look at the *uniform* case,\n",
                 "which means that the parameter interval in each segment\n",
-                "is chosen to be 1.\n",
+                "is chosen to be $1$.\n",
                 "\n",
                 "The more general case with arbitrary parameter intervals\n",
                 "is derived in a separate\n",
                 "[notebook about non-uniform natural splines](natural-non-uniform.ipynb)."
             ]
         },
         {
@@ -37,25 +39,24 @@
                 "sp.init_printing(order='grevlex')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We import a helper class for named SymPy expressions\n",
-                "from [utility.py](utility.py):"
+                "We import some helpers from [utility.py](utility.py):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from utility import NamedExpression"
+                "from utility import NamedExpression, dotproduct"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -77,42 +78,49 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "a3, a4, b3, b4, c3, c4, d3, d4 = sp.symbols('a:dbm3:5')"
+                "coefficients3 = sp.symbols('a:dbm3')[::-1]\n",
+                "coefficients4 = sp.symbols('a:dbm4')[::-1]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We are using the [monomial basis](polynomials.ipynb)\n",
-                "to define the two polynomials ..."
+                "We apply these coefficients to the [monomial basis](polynomials.ipynb) ..."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "b_monomial = sp.Matrix([t**3, t**2, t, 1]).T"
+                "b_monomial = t**3, t**2, t, 1"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "... to define the two polynomials ..."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "p3 = NamedExpression('pbm3', d3 * t**3 + c3 * t**2 + b3 * t + a3)\n",
-                "p4 = NamedExpression('pbm4', d4 * t**3 + c4 * t**2 + b4 * t + a4)\n",
+                "p3 = NamedExpression('pbm3', dotproduct(b_monomial, coefficients3))\n",
+                "p4 = NamedExpression('pbm4', dotproduct(b_monomial, coefficients4))\n",
                 "display(p3, p4)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -168,15 +176,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "coefficients = sp.solve(equations, [a3, a4, b3, b4, c3, c4, d3, d4])\n",
+                "coefficients = sp.solve(equations, coefficients3 + coefficients4)\n",
                 "for c, e in coefficients.items():\n",
                 "    display(NamedExpression(c, e))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -400,22 +408,19 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Clamped\n",
                 "\n",
-                "We can simply provide arbitrarily chosen values for the end tangents.\n",
-                "This is called *clamped* end conditions."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "We can simply provide arbitrarily chosen values\n",
+                "$D_\\text{begin}$ and $D_\\text{end}$\n",
+                "for the end tangents.\n",
+                "This is called *clamped* end conditions.\n",
+                "\n",
                 "\\begin{align*}\n",
                 "\\dot{\\boldsymbol{x}}_0 &= D_\\text{begin}\\\\\n",
                 "\\dot{\\boldsymbol{x}}_{N-1} &= D_\\text{end}\n",
                 "\\end{align*}"
             ]
         },
         {
@@ -532,27 +537,27 @@
                 "[linalg.solve()](https://numpy.org/doc/stable/reference/generated/numpy.linalg.solve.html)\n",
                 "function to solve the system of equations."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.11.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/euclidean/natural.ipynb` & `splines-0.3.0/doc/euclidean/natural.ipynb`

 * *Files identical despite different names*

### Comparing `splines-0.2.0/doc/euclidean/piecewise-monotone.ipynb` & `splines-0.3.0/doc/euclidean/piecewise-monotone.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9829061179208027%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(13, '-- see also [Monotone "*

 * *            "Interpolation](#Monotone-Interpolation) below.')], delete: [13]}}, 2: {'source': "*

 * *            "{insert: [(1, 'one-dimensional piecewise monotone cubic splines\\n'), (2, 'is "*

 * *            "available in the class\\n'), (3, "*

 * *            "'[splines.PiecewiseMonotoneCubic](../python-module/splines.rst#splines.PiecewiseMonotoneCubic).')], "*

 * *            'delete: [4, 3, 2, 1]}}, 12: {\'source\': {insert: [(5, "    label=\'Catmull–Rom […]*

```diff
@@ -24,26 +24,25 @@
                 "to a monotone function.\n",
                 "This makes sure that there are no overshoots beyond the given data points.\n",
                 "In other words, if the data points are within certain bounds,\n",
                 "all interpolated data will also be within those same bounds.\n",
                 "It follows that if all data points are non-negative,\n",
                 "interpolated data will be non-negative as well.\n",
                 "Furthermore, this makes sure that monotone data leads to a monotone interpolant\n",
-                "(see also [Monotone Interpolation](#Monotone-Interpolation) below)."
+                "-- see also [Monotone Interpolation](#Monotone-Interpolation) below."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "A Python implementation of\n",
-                "piecewise monotone one-dimensional cubic splines\n",
-                "is available in the\n",
-                "[splines.PiecewiseMonotoneCubic](../python-module/splines.rst#splines.PiecewiseMonotoneCubic)\n",
-                "class."
+                "one-dimensional piecewise monotone cubic splines\n",
+                "is available in the class\n",
+                "[splines.PiecewiseMonotoneCubic](../python-module/splines.rst#splines.PiecewiseMonotoneCubic)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The SciPy package provides a similar tool with the\n",
@@ -132,32 +131,32 @@
             "outputs": [],
             "source": [
                 "plot_spline_1d(\n",
                 "    splines.PiecewiseMonotoneCubic(values, times, closed=True),\n",
                 "    label='piecewise monotone')\n",
                 "plot_spline_1d(\n",
                 "    splines.CatmullRom(values, times, endconditions='closed'),\n",
-                "    label='Catmull\u2013Rom')\n",
+                "    label='Catmull\u2013Rom', linestyle='--')\n",
                 "plot_spline_1d(\n",
                 "    splines.Natural(values, times, endconditions='closed'),\n",
-                "    label='natural spline')\n",
+                "    label='natural spline', linestyle='-.')\n",
                 "plt.legend()\n",
                 "grid_lines(times)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def plot_piecewise_monotone(*args, **kwargs):\n",
                 "    s = splines.PiecewiseMonotoneCubic(*args, **kwargs)\n",
                 "    plot_spline_1d(s)\n",
-                "    grid_lines(x=s.grid)"
+                "    grid_lines(s.grid)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -220,62 +219,70 @@
             "source": [
                 "> In this paper we derive necessary and sufficient conditions for a cubic to be\n",
                 "monotone in an interval. These conditions are then used to develop an algorithm which\n",
                 "constructs a $\\mathscr{C}^1$ monotone piecewise cubic interpolant to monotone data. The curve\n",
                 "produced contains no extraneous \"bumps\" or \"wiggles\", which makes it more readily\n",
                 "acceptable to scientists and engineers.\n",
                 ">\n",
-                "> ---<cite data-cite=\"fritsch1980monotone\">(Fritsch and Carlson 1980)</cite>, section 1: \"Introduction\""
+                "> ---<cite data-cite-t=\"fritsch1980monotone\">Fritsch and Carlson (1980)</cite>, section 1"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "<cite data-cite=\"fritsch1980monotone\">(Fritsch and Carlson 1980)</cite>\n",
-                "derives necessary and sufficient conditions\n",
+                "<cite data-cite-t=\"fritsch1980monotone\">Fritsch and Carlson (1980)</cite>\n",
+                "derive necessary and sufficient conditions\n",
                 "for a cubic curve segment to be monotone,\n",
                 "based on the slopes of the secant lines (i.e. the piecewise linear interpolant)\n",
                 "and their endpoint derivatives.\n",
                 "Furthermore, they provide a two-step algorithm\n",
                 "to generate piecewise monotone cubics:\n",
                 "\n",
                 "1. calculate initial tangents (with whatever method)\n",
-                "2. tweak the ones that don't fulfill the monotonicity conditions"
+                "2. tweak the ones that don't fulfill the monotonicity conditions\n",
+                "\n",
+                "For the first step, they suggest using the *standard three-point difference*,\n",
+                "which we have already seen in the\n",
+                "[tangent vectors of non-uniform Catmull--Rom splines](catmull-rom-non-uniform.ipynb#Tangent-Vectors)\n",
+                "and which is implemented in the class\n",
+                "[splines.CatmullRom](../python-module/splines.rst#splines.CatmullRom)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "> To implement Step 1 we have found the standard three-point difference formula to\n",
                 "be satisfactory for $d_2$, $d_3$, $\\cdots$, $d_{n-1}$.\n",
                 ">\n",
-                "> ---<cite data-cite=\"fritsch1980monotone\">(Fritsch and Carlson 1980)</cite>, section 4: \"Monotone piecewise cubic interpolation algorithm\""
+                "> ---<cite data-cite-t=\"fritsch1980monotone\">Fritsch and Carlson (1980)</cite>, section 4"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "> This is what de Boor [<cite data-cite=\"de_boor1978splines\">1978</cite>, p. 53] calls cubic Bessel interpolation, in which\n",
                 "the interior derivatives are set using the standard three point difference formula.\n",
                 ">\n",
-                "> ---<cite data-cite=\"fritsch1980monotone\">(Fritsch and Carlson 1980)</cite>, section 5: \"Numerical examples\""
+                "> ---<cite data-cite-t=\"fritsch1980monotone\">Fritsch and Carlson (1980)</cite>, section 5"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "In the 2001 edition of\n",
-                "<cite data-cite=\"de_boor1978splines\">(de Boor 1978)</cite>,\n",
+                "<div class=\"alert alert-info\">\n",
+                "\n",
+                "In the 2001 edition of the book by\n",
+                "<cite data-cite-t=\"de_boor1978splines\">Boor (1978)</cite>,\n",
                 "*piecewise cubic Bessel interpolation* is defined on page 42.\n",
-                "We have already seen the *standard three-point difference* in the\n",
-                "[tangent vectors of non-uniform Catmull--Rom splines](catmull-rom-non-uniform.ipynb#Tangent-Vectors)."
+                "\n",
+                "</div>"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "For the following equations, we define the slope of the secant lines as\n",
@@ -305,17 +312,17 @@
                 "</div>"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Based on <cite data-cite=\"fritsch1980monotone\">(Fritsch and Carlson 1980)</cite>,\n",
-                "<cite data-cite=\"dougherty1989nonnegativity\">(Dougherty et al. 1989)</cite>\n",
-                "provides (in equation 4.2) an algorithm for modifying the initial slopes\n",
+                "Based on <cite data-cite-t=\"fritsch1980monotone\">Fritsch and Carlson (1980)</cite>,\n",
+                "<cite data-cite-t=\"dougherty1989nonnegativity\">Dougherty et al. (1989)</cite>\n",
+                "provide (in equation 4.2) an algorithm for modifying the initial slopes\n",
                 "to ensure monotonicity.\n",
                 "Adapted to our notation, it looks like this:\n",
                 "\n",
                 "\\begin{equation*}\n",
                 "\\dot{x}_i \\leftarrow\n",
                 "\\begin{cases}\n",
                 "\\min(\\max(0, \\dot{x}_i), 3 \\min(|S_{i-1}|, |S_i|)), & \\sigma_i > 0,\\\\\n",
@@ -327,28 +334,27 @@
                 "where $\\sigma_i = \\operatorname{sgn}(S_i)$ if $S_i S_{i-1} > 0$ and $\\sigma_i=0$ otherwise."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This algoritm is implemented in the\n",
-                "[splines.PiecewiseMonotoneCubic](../python-module/splines.rst#splines.PiecewiseMonotoneCubic)\n",
-                "class."
+                "This algorithm is implemented in the class\n",
+                "[splines.PiecewiseMonotoneCubic](../python-module/splines.rst#splines.PiecewiseMonotoneCubic)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## PCHIP/PCHIM\n",
                 "\n",
                 "A different approach for obtaining slopes that ensure monotonicity\n",
-                "is described in\n",
-                "<cite data-cite=\"fritsch1984monotone\">(Fritsch and Butland 1984)</cite>,\n",
+                "is described by\n",
+                "<cite data-cite-t=\"fritsch1984monotone\">Fritsch and Butland (1984)</cite>,\n",
                 "equation (5):\n",
                 "\n",
                 "\\begin{equation*}\n",
                 "G(S_1, S_2, h_1, h_2) =\n",
                 "\\begin{cases}\n",
                 "\\frac{S_1 S_2}{\\alpha S_2 + (1 - \\alpha) S_1} \\quad & \\text{if } S_1 S_2 > 0,\\\\\n",
                 "0 & \\text{otherwise,}\n",
@@ -410,28 +416,28 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This has been implemented in a\n",
-                "[Fortran](https://en.wikipedia.org/wiki/Fortran) package described in\n",
-                "<cite data-cite=\"fritsch1982pchip\">(Fritsch 1982)</cite>,\n",
-                "which has coined the acronym PCHIP,\n",
+                "[Fortran](https://en.wikipedia.org/wiki/Fortran) package described by\n",
+                "<cite data-cite-t=\"fritsch1982pchip\">Fritsch (1982)</cite>,\n",
+                "who has coined the acronym PCHIP,\n",
                 "originally meaning *Piecewise Cubic Hermite Interpolation Package*."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "> It features software to produce a monotone and \"visually pleasing\"\n",
                 "interpolant to monotone data.\n",
                 ">\n",
-                "> ---<cite data-cite=\"fritsch1982pchip\">(Fritsch 1982)</cite>"
+                "> ---<cite data-cite-t=\"fritsch1982pchip\">Fritsch (1982)</cite>"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The package contains many Fortran subroutines,\n",
@@ -440,15 +446,16 @@
                 "*Piecewise Cubic Hermite Interpolation to Monotone data*."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The source code (including some later modifications) is available at https://people.sc.fsu.edu/~jburkardt/f77_src/pchip/pchip.html.\n",
+                "The source code (including some later modifications) is available\n",
+                "[online](https://netlib.org/slatec/pchip/dpchim.f).\n",
                 "This is the code snippet responsible for calculating the slopes:\n",
                 "\n",
                 "```\n",
                 "C\n",
                 "C        USE BRODLIE MODIFICATION OF BUTLAND FORMULA.\n",
                 "C\n",
                 "   45    CONTINUE\n",
@@ -524,17 +531,17 @@
                 "assert sp.simplify(G2 - G3) == 0"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "... and they are in fact also equivalent\n",
+                "... and that they are in fact also equivalent\n",
                 "to the aforementioned equation from\n",
-                "<cite data-cite=\"fritsch1984monotone\">(Fritsch and Butland 1984)</cite>:"
+                "<cite data-cite-t=\"fritsch1984monotone\">Fritsch and Butland (1984)</cite>:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -551,16 +558,16 @@
                 "if one of the slopes is very close to zero."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Yet another variation of this theme is shown in\n",
-                "<cite data-cite=\"moler2004numerical\">(Moler 2004)</cite>, section 3.4,\n",
+                "Yet another variation of this theme is shown by\n",
+                "<cite data-cite-t=\"moler2004numerical\">Moler (2004)</cite>, section 3.4,\n",
                 "which defines the slope $d_k$ as a weighted harmonic mean\n",
                 "of the two neighboring secant slopes:\n",
                 "\n",
                 "\\begin{equation*}\n",
                 "\\frac{w_1 + w_2}{d_k} =\n",
                 "\\frac{w_1}{\\delta_{k-1}} +\n",
                 "\\frac{w_2}{\\delta_k},\n",
@@ -614,15 +621,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The `PCHIM` algorithm,\n",
                 "which is nowadays known by the less self-explanatory name PCHIP,\n",
-                "is available in the *SciPy* package in form of the\n",
+                "is available in the SciPy package in form of the\n",
                 "[pchip_interpolate()](https://docs.scipy.org/doc/scipy/reference/generated/scipy.interpolate.pchip_interpolate.html)\n",
                 "function and the\n",
                 "[PchipInterpolator](https://docs.scipy.org/doc/scipy/reference/generated/scipy.interpolate.PchipInterpolator.html)\n",
                 "class."
             ]
         },
         {
@@ -654,21 +661,21 @@
             "outputs": [],
             "source": [
                 "def compare_pchip(values, times):\n",
                 "    plot_times = np.linspace(times[0], times[-1], 100)\n",
                 "    plt.plot(\n",
                 "        plot_times,\n",
                 "        PchipInterpolator(times, values)(plot_times),\n",
-                "        label='PCHIP')\n",
+                "        label='PCHIP', linestyle='--')\n",
                 "    plt.plot(\n",
                 "        plot_times,\n",
                 "        splines.PiecewiseMonotoneCubic(values, times).evaluate(plot_times),\n",
-                "        label='PiecewiseMonotoneCubic')\n",
+                "        label='PiecewiseMonotoneCubic', linestyle='-.')\n",
                 "    plt.legend()\n",
-                "    grid_lines(x=times)"
+                "    grid_lines(times)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -721,15 +728,15 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Monotone Interpolation\n",
                 "\n",
                 "When using the aforementioned piecewise monotone algorithms with monotone data,\n",
-                "the whole interpolant will be monotone.\n",
+                "the entire interpolant will be monotone.\n",
                 "\n",
                 "The class\n",
                 "[splines.MonotoneCubic](../python-module/splines.rst#splines.MonotoneCubic)\n",
                 "works very much the same as\n",
                 "[splines.PiecewiseMonotoneCubic](../python-module/splines.rst#splines.PiecewiseMonotoneCubic),\n",
                 "except that it only allows monotone data values.\n",
                 "\n",
@@ -763,15 +770,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "fig, ax = plt.subplots()\n",
                 "plot_spline_1d(s)\n",
                 "ax.scatter(s.get_time(probes), probes)\n",
-                "grid_lines(x=s.grid)"
+                "grid_lines(s.grid)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "If the solution is not unique (i.e. on plateaus),\n",
@@ -809,14 +816,75 @@
                 "    assert False"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "However, in some situations it might be useful\n",
+                "to automatically infer the same slope at the beginning and end of the spline.\n",
+                "This can be achieved with the `cyclic` flag."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "s = splines.MonotoneCubic([0, 1, 5])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "s_cyclic = splines.MonotoneCubic([0, 1, 5], cyclic=True)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "plot_spline_1d(s, label='not cyclic')\n",
+                "plot_spline_1d(s_cyclic, label='cyclic')\n",
+                "grid_lines(s.grid)\n",
+                "plt.legend();"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The `cyclic` flag is only allowed if the first and last slope is `None`:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "try:\n",
+                "    splines.MonotoneCubic([0, 1, 5], slopes=[1, None, None], cyclic=True)\n",
+                "except Exception as e:\n",
+                "    print(e)\n",
+                "    assert 'cyclic' in str(e)\n",
+                "else:\n",
+                "    assert False"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "## End Conditions\n",
                 "\n",
                 "[The usual end conditions](end-conditions.ipynb)\n",
                 "don't necessarily lead to a monotone interpolant,\n",
                 "therefore we need to come up with custom end conditions\n",
                 "that preserve monotonicity."
             ]
@@ -826,26 +894,26 @@
             "metadata": {},
             "source": [
                 "> For the end derivatives, the noncentered three\n",
                 "point difference formula may be used, although it is sometimes necessary to modify $d_1$\n",
                 "and/or $d_n$ if the signs are not appropriate. In these cases we have obtained better results\n",
                 "setting $d_1$ or $d_n$ equal to zero, rather than equal to the slope of the secant line.\n",
                 ">\n",
-                "> ---<cite data-cite=\"fritsch1980monotone\">(Fritsch and Carlson 1980)</cite>, section 4: \"Monotone piecewise cubic interpolation algorithm\""
+                "> ---<cite data-cite-t=\"fritsch1980monotone\">Fritsch and Carlson (1980)</cite>, section 4"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "<cite data-cite=\"fritsch1980monotone\">(Fritsch and Carlson 1980)</cite>\n",
-                "recommends using the *noncentered three point difference formula*,\n",
-                "however, it fails to mention what that actually is.\n",
-                "Luckily, we can have a look at the code at\n",
-                "https://people.sc.fsu.edu/~jburkardt/f77_src/pchip/pchip.html:\n",
+                "<cite data-cite-t=\"fritsch1980monotone\">Fritsch and Carlson (1980)</cite>\n",
+                "recommend using the *noncentered three point difference formula*,\n",
+                "however, they fail to mention what that actually is.\n",
+                "Luckily, we can have a look at the\n",
+                "[code](https://netlib.org/slatec/pchip/dpchim.f):\n",
                 "\n",
                 "```\n",
                 "C\n",
                 "C  SET D(1) VIA NON-CENTERED THREE-POINT FORMULA, ADJUSTED TO BE\n",
                 "C     SHAPE-PRESERVING.\n",
                 "C\n",
                 "      HSUM = H1 + H2\n",
@@ -881,22 +949,22 @@
             "metadata": {},
             "source": [
                 "> This defines the `pchip` slopes at interior breakpoints,\n",
                 "but the slopes $d_1$ and $d_n$ at either end of the data interval\n",
                 "are determined by a slightly different,\n",
                 "one-sided analysis. The details are in `pchiptx.m`.\n",
                 ">\n",
-                "> ---<cite data-cite=\"moler2004numerical\">(Moler 2004)</cite>, section 3.4"
+                "> ---<cite data-cite-t=\"moler2004numerical\">Moler (2004)</cite>, section 3.4"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Section 3.6 of <cite data-cite=\"moler2004numerical\">(Moler 2004)</cite>\n",
+                "In section 3.6, <cite data-cite-t=\"moler2004numerical\">Moler (2004)</cite>\n",
                 "shows the implementation of `pchiptx.m`:\n",
                 "\n",
                 "```octave\n",
                 "function d = pchipend(h1,h2,del1,del2)\n",
                 "%  Noncentered, shape-preserving, three-point formula.\n",
                 "    d = ((2*h1+h2)*del1 - h1*del2)/(h1+h2);\n",
                 "    if sign(d) ~= sign(del1)\n",
@@ -944,36 +1012,36 @@
             "outputs": [],
             "source": [
                 "def plot_pchip(values, grid, **kwargs):\n",
                 "    pchip = PchipInterpolator(grid, values)\n",
                 "    times = np.linspace(grid[0], grid[-1], 100)\n",
                 "    plt.plot(times, pchip(times), **kwargs)\n",
                 "    plt.scatter(grid, pchip(grid))\n",
-                "    grid_lines(x=grid)"
+                "    grid_lines(grid)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "plot_pchip([0, 1, 0], [0, 1, 2])\n",
-                "plot_pchip([0, 1, 1], [0, 1, 2])\n",
+                "plot_pchip([0, 1, 1], [0, 1, 2], linestyle='--')\n",
                 "grid_lines([0, 1, 2])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "plot_pchip([0, 1, 0], [0, 1, 4])\n",
-                "plot_pchip([0, 1, 0], [0, 1, 1.5])\n",
+                "plot_pchip([0, 1, 0], [0, 1, 1.5], linestyle='--')\n",
                 "grid_lines([0, 1, 1.5, 4])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1004,15 +1072,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "plot_piecewise_monotone([0, 1, 0], grid=[0, 1, 1.5])\n",
                 "plot_piecewise_monotone([0, 1, 0], grid=[0, 1, 4])\n",
-                "grid_lines(x=[0, 1, 1.5, 4])"
+                "grid_lines([0, 1, 1.5, 4])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The initial and final slopes of\n",
@@ -1072,27 +1140,27 @@
             "source": [
                 "compare_pchip([1, 2, 1.9, 1], [1, 3, 4, 6])"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.11.1"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/euclidean/polynomials.ipynb` & `splines-0.3.0/doc/euclidean/polynomials.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.968530433006536%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, '# Parametric Polynomial Curves\\n'), (3, '*polynomial "*

 * *            "splines*\\n')], delete: [3, 0]}}, 3: {'source': {insert: [(1, "*

 * *            '"sp.init_printing(order=\'grevlex\')\\n"), (2, \'from helper import plot_basis, '*

 * *            "plot_sympy, grid_lines, plot_spline_2d')], delete: [1]}}, 4: {'source': {insert: [(4, "*

 * *            "'You can think about it as *time* (e.g. in seconds),\\n')], delete: [5, 3]}}, 7: "*

 * *            "{'source': {insert: [(1, 'is th […]*

```diff
@@ -9,41 +9,50 @@
                 "This notebook is part of https://github.com/AudioSceneDescriptionFormat/splines, see also https://splines.readthedocs.io/."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Polynomial Parametric Curves\n",
+                "# Parametric Polynomial Curves\n",
                 "\n",
                 "The building blocks for\n",
-                "[polynomial splines](index.ipynb)\n",
+                "*polynomial splines*\n",
                 "are of course [polynomials](https://en.wikipedia.org/wiki/Polynomial)."
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "But first things first,\n",
+                "let's import [SymPy](https://www.sympy.org/)\n",
+                "and a few helper functions from [helper.py](helper.py):"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import sympy as sp\n",
-                "sp.init_printing(order='grevlex')"
+                "sp.init_printing(order='grevlex')\n",
+                "from helper import plot_basis, plot_sympy, grid_lines, plot_spline_2d"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We are mostly interested in *univariate* splines,\n",
                 "i.e. curves with one free parameter,\n",
                 "which are built using polynomials with a single parameter.\n",
-                "\n",
                 "Here we are calling this parameter $t$.\n",
-                "You can think about it as time (e.g. in seconds),\n",
+                "You can think about it as *time* (e.g. in seconds),\n",
                 "but it doesn't have to represent time."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -63,15 +72,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The arguably simplest set of basis functions\n",
-                "is the *monomial basis*,\n",
+                "is the *monomial basis*, a.k.a. *power basis*,\n",
                 "which simply consists of all powers of $t$ up to the given degree:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -81,26 +90,35 @@
                 "b_monomial"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "In this example we are using polynomials of degree 3,\n",
+                "In this example we are creating polynomials of degree 3,\n",
                 "which are also called *cubic* polynomials."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "The ordering of the basis functions is purely a matter of convention,\n",
+                "here we are sorting them in order of descending powers."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "These basis functions are multiplied by (constant) *coefficients*.\n",
                 "We are writing the coefficients with bold symbols,\n",
                 "because apart from simple scalars (for one-dimensional functions),\n",
-                "these symbols can also represent vectors in two- or three-dimensional space."
+                "these symbols can also represent vectors in two- or three-dimensional space\n",
+                "(and even higher-dimensional spaces)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -130,25 +148,15 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This is a cubic polynomial in its *canonical form*\n",
                 "(because it uses monomial basis functions).\n",
                 "\n",
-                "Let's take a closer look at those basis functions\n",
-                "(with some help from [helper.py](helper.py)):"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from helper import plot_basis"
+                "Let's take a closer look at those basis functions:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -181,23 +189,14 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from helper import plot_sympy, grid_lines"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
                 "plot_sympy(example_polynomial, (t, 0, 1))\n",
                 "grid_lines([0, 1], [0, 0.5, 1])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -215,34 +214,36 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Any polynomial can be rewritten using any set of basis functions\n",
-                "(of appropriate degree)."
+                "(as long as the degree of the basis functions matches the degree of the polynomial)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "In later sections we will see more basis functions,\n",
                 "for example those that are used for\n",
                 "[Hermite](hermite-uniform.ipynb),\n",
                 "[B\u00e9zier](bezier-de-casteljau.ipynb) and\n",
-                "[Catmull--Rom](catmull-rom-uniform.ipynb) splines."
+                "[Catmull--Rom](catmull-rom-uniform.ipynb) splines.\n",
+                "In those sections we will also see how to convert\n",
+                "between different bases by means of matrix multiplication."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "In the previous example,\n",
-                "we have used scalar coefficients\n",
+                "we used scalar coefficients\n",
                 "to create a one-dimensional polynomial.\n",
                 "We can use two-dimensional coefficients\n",
                 "to create two-dimensional polynomial curves.\n",
                 "Let's create a little class to try this:"
             ]
         },
         {
@@ -276,39 +277,29 @@
                 "The `@` operator is used here to do\n",
                 "[NumPy's matrix multiplication](https://numpy.org/doc/stable/reference/generated/numpy.matmul.html).\n",
                 "\n",
                 "</div>"
             ]
         },
         {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Since this class has the same interface as the splines\n",
-                "that will be discussed in later sections,\n",
-                "we can use a spline helper function from [helper.py](helper.py)\n",
-                "for plotting:"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from helper import plot_spline_2d"
+                "poly_2d = CubicPolynomial([-1.5, 5], [1.5, -8.5], [1, 4], [3, 2])"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "poly_2d = CubicPolynomial([-1.5, 5], [1.5, -8.5], [1, 4], [3, 2])"
+                "Since this class has the same interface as the splines\n",
+                "that will be discussed in later sections,\n",
+                "we can use a spline helper function for plotting:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -324,27 +315,27 @@
                 "The class [splines.Monomial](../python-module/splines.rst#splines.Monomial)\n",
                 "can be used to try this with arbitrary polynomial degree."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.2"
+            "version": "3.11.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/euclidean/utility.py` & `splines-0.3.0/doc/euclidean/utility.py`

 * *Files 7% similar despite different names*

```diff
@@ -219,7 +219,20 @@
     elif isinstance(expr, sp.MatrixBase):
         # .simplify() behaves differently on mutable and immutable matrices,
         # see https://github.com/sympy/sympy/issues/2647
         return sp.MatrixBase.simplify(expr.inv())
     elif isinstance(expr, sp.MatrixExpr):
         return expr.inverse()
     raise TypeError('Unable to invert')
+
+
+# This is unrelated to the above, and it probably should be moved.
+def dotproduct(vec1, vec2):
+    """Dot product of two iterables.
+
+    Stops when the shorter one is exhausted.
+
+    See https://docs.python.org/3/library/itertools.html#itertools-recipes
+
+    """
+    import operator
+    return sum(map(operator.mul, vec1, vec2))
```

### Comparing `splines-0.2.0/doc/rotation/barry-goldman.ipynb` & `splines-0.3.0/doc/rotation/barry-goldman.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984760802469135%*

 * *Differences: {"'cells'": "{12: {'source': {insert: [(1, 'we use the class\\n'), (2, "*

 * *            "'[splines.quaternion.BarryGoldman](../python-module/splines.quaternion.rst#splines.quaternion.BarryGoldman):')], "*

 * *            'delete: [3, 2, 1]}}, 28: {\'source\': {insert: [(0, "A big advantage of De '*

 * *            'Casteljau\'s algorithm is\\n"), (2, \'it directly provides the corresponding tangent '*

 * *            "vector.\\n'), (5, 'which makes re-parameterization for constant angular speed\\n')], "*

 * *            "delete:  […]*

```diff
@@ -150,17 +150,16 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "For the next example,\n",
-                "we use the\n",
-                "[splines.quaternion.BarryGoldman](../python-module/splines.quaternion.rst#splines.quaternion.BarryGoldman)\n",
-                "class:"
+                "we use the class\n",
+                "[splines.quaternion.BarryGoldman](../python-module/splines.quaternion.rst#splines.quaternion.BarryGoldman):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -311,20 +310,20 @@
                 "## Constant Angular Speed"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "A big advantage of de Casteljau's algorithm is\n",
+                "A big advantage of De Casteljau's algorithm is\n",
                 "that when evaluating a spline at a given parameter value,\n",
-                "it directly provides the appropriate tangent vector.\n",
+                "it directly provides the corresponding tangent vector.\n",
                 "When using the Barry--Goldman algorithm,\n",
                 "the tangent vector has to be calculated separately,\n",
-                "which make re-parameterization for constant angular speed\n",
+                "which makes re-parameterization for constant angular speed\n",
                 "very inefficient."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -355,24 +354,24 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from splines import ConstantSpeedAdapter"
+                "from splines import UnitSpeedAdapter"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "bg3 = ConstantSpeedAdapter(BarryGoldmanWithDerivative(rotations, alpha=0.5))"
+                "bg3 = UnitSpeedAdapter(BarryGoldmanWithDerivative(rotations, alpha=0.5))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "<div class=\"alert alert-warning\">\n",
```

### Comparing `splines-0.2.0/doc/rotation/catmull-rom-non-uniform.ipynb` & `splines-0.3.0/doc/rotation/catmull-rom-non-uniform.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976541244488226%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(6, '> ---<cite "*

 * *            'data-cite-t="shoemake1985animating">Shoemake (1985)</cite>, section 6: '*

 * *            '"Questions"\')], delete: [6]}}, 2: {\'source\': {insert: [(2, "[De Casteljau\'s '*

 * *            'algorithm with Slerp](de-casteljau.ipynb)\\n"), (7, \'-- as shown in\\n\'), (8, '*

 * *            "'[the notebook about non-uniform Euclidean Bézier "*

 * *            "splines](../euclidean/bezier-non-uniform.ipynb).\\n'), (9, 'This is implemented in "*

 * *            "the  […]*

```diff
@@ -17,33 +17,32 @@
             "source": [
                 "# Non-Uniform Catmull--Rom-Like Rotation Splines\n",
                 "\n",
                 "> What is the best way to allow\n",
                 "varying intervals between sequence points in parameter\n",
                 "space?\n",
                 ">\n",
-                "> ---<cite data-cite=\"shoemake1985animating\">Shoemake (1985)</cite>, section 6: \"Questions\""
+                "> ---<cite data-cite-t=\"shoemake1985animating\">Shoemake (1985)</cite>, section 6: \"Questions\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "In the [uniform case](catmull-rom-uniform.ipynb)\n",
                 "we have used\n",
-                "[de Casteljau's algorithm with Slerp](de-casteljau.ipynb)\n",
+                "[De Casteljau's algorithm with Slerp](de-casteljau.ipynb)\n",
                 "to create a \"cubic\" rotation spline.\n",
                 "To extend this to the non-uniform case,\n",
                 "we can transform the parameter $t \\to \\frac{t - t_i}{t_{i+1} - t_i}$\n",
                 "for each spline segment\n",
-                "(as shown in\n",
-                "[the notebook about non-uniform Euclidean B\u00e9zier splines](../euclidean/bezier-non-uniform.ipynb)).\n",
-                "This is implemented in the\n",
-                "[splines.quaternion.DeCasteljau](../python-module/splines.quaternion.rst#splines.quaternion.DeCasteljau)\n",
-                "class."
+                "-- as shown in\n",
+                "[the notebook about non-uniform Euclidean B\u00e9zier splines](../euclidean/bezier-non-uniform.ipynb).\n",
+                "This is implemented in the class\n",
+                "[splines.quaternion.DeCasteljau](../python-module/splines.quaternion.rst#splines.quaternion.DeCasteljau)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Assuming the control points at the start and the end of each segment are given\n",
@@ -126,15 +125,15 @@
                 "within the parameter interval from $t_i$ to $t_{i+1}$\n",
                 "and\n",
                 "$\\vec{\\omega}_i$ is the angular velocity\n",
                 "of the Catmull--Rom-like quaternion curve\n",
                 "at the control point $q_i$\n",
                 "(which is reached at parameter value $t_i$).\n",
                 "Finally, $\\tilde{q}_i^{(-)}$ and $\\tilde{q}_i^{(+)}$\n",
-                "are the control quaternions before and after $q_i$, respectively."
+                "are the B\u00e9zier-like control quaternions before and after $q_i$, respectively."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -153,16 +152,16 @@
                 "    ]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This approach is also implemented in the\n",
-                "[splines.quaternion.CatmullRom](../python-module/splines.quaternion.rst#splines.quaternion.CatmullRom) class."
+                "This approach is also implemented in the class\n",
+                "[splines.quaternion.CatmullRom](../python-module/splines.quaternion.rst#splines.quaternion.CatmullRom)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "To illustrate this, let's load NumPy,\n",
@@ -244,15 +243,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "grid1 = np.array([0, 0.5, 2, 5, 6, 7, 9])"
+                "grid1 = 0, 0.5, 2, 5, 6, 7, 9"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -340,15 +339,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "For\n",
-                "[chordal parameterization of Euclidean splines](../euclidean/catmull-rom-properties.ipynb#Chordal-Parameterization)\n",
+                "[chordal parameterization of Euclidean splines](../euclidean/catmull-rom-properties.ipynb#Chordal-Parameterization),\n",
                 "we used the Euclidean distance as basis for calculating the time intervals.\n",
                 "For rotation splines,\n",
                 "it makes more sense to use rotation angles,\n",
                 "which are proportional to the lengths of the great arcs\n",
                 "between control quaternions:"
             ]
         },
@@ -399,15 +398,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "For\n",
-                "[centripetal parameterization of Euclidean splines](../euclidean/catmull-rom-properties.ipynb#Centripetal-Parameterization)\n",
+                "[centripetal parameterization of Euclidean splines](../euclidean/catmull-rom-properties.ipynb#Centripetal-Parameterization),\n",
                 "we used the square root of the Euclidean distances,\n",
                 "here we use the square root of the rotation angles:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -430,16 +429,16 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "ani = animate_rotations({\n",
                 "    'uniform': evaluate(uniform),\n",
-                "    'chordal': evaluate(chordal),\n",
                 "    'centripetal': evaluate(centripetal),\n",
+                "    'chordal': evaluate(chordal),\n",
                 "})"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -448,19 +447,19 @@
                 "display_animation(ani, default_mode='loop')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The\n",
+                "The class\n",
                 "[splines.quaternion.CatmullRom](../python-module/splines.quaternion.rst#splines.quaternion.CatmullRom)\n",
-                "class provides a parameter `alpha` that allows arbitrary parameterization\n",
+                "provides a parameter `alpha` that allows arbitrary parameterization\n",
                 "between *uniform* and *chordal*\n",
-                "(see also [parameterized parameterization of Euclidean splines](../euclidean/catmull-rom-properties.ipynb#Parameterized-Parameterization))."
+                "-- see also [parameterized parameterization of Euclidean splines](../euclidean/catmull-rom-properties.ipynb#Parameterized-Parameterization)."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
```

### Comparing `splines-0.2.0/doc/rotation/catmull-rom-uniform.ipynb` & `splines-0.3.0/doc/rotation/catmull-rom-uniform.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995908111516679%*

 * *Differences: {"'cells'": '{2: {\'source\': {insert: [(1, "[De Casteljau\'s algorithm with '*

 * *            'Slerp](de-casteljau.ipynb)\\n")], delete: [1]}}, 5: {\'source\': {insert: [(5, '*

 * *            "'Furthermore, adding a (non-zero length) tangent vector to a unit quaternion\\n')], "*

 * *            "delete: [5]}}, 55: {'source': {insert: [(5, '-- which is a flat, three-dimensional "*

 * *            'Euclidean space --\\n\')], delete: [5]}}, 73: {\'source\': {insert: [(1, "so let\'s '*

 * *            'create a closed curve.")], del […]*

```diff
@@ -19,15 +19,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We have seen how to use\n",
-                "[de Casteljau's algorithm with Slerp](de-casteljau.ipynb)\n",
+                "[De Casteljau's algorithm with Slerp](de-casteljau.ipynb)\n",
                 "to create \"cubic\" B\u00e9zier-like quaternion curve segments.\n",
                 "However, if we only have a sequence of rotations to be interpolated\n",
                 "and no additional B\u00e9zier control quaternions are provided,\n",
                 "it would be great if we could compute\n",
                 "the missing control quaternions automatically\n",
                 "from neighboring quaternions."
             ]
@@ -63,15 +63,15 @@
             "metadata": {},
             "source": [
                 "Applying this to rotations is unfortunately not very straightforward.\n",
                 "When unit quaternions are moving along the the unit hypersphere,\n",
                 "their velocity vectors are tangential to that hypersphere,\n",
                 "which means that the velocity vectors are generally\n",
                 "not unit quaternions themselves.\n",
-                "Furthermore, adding a tangent vector to a unit quaternion\n",
+                "Furthermore, adding a (non-zero length) tangent vector to a unit quaternion\n",
                 "never leads to a unit quaternion as a result."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -576,15 +576,15 @@
             "metadata": {},
             "source": [
                 "The *logarithmic map* operation\n",
                 "transforms a unit quaternion\n",
                 "into a vector that's a member of the\n",
                 "tangent space at the identity quaternion (a.k.a. $\\boldsymbol{1}$).\n",
                 "In this tangent space\n",
-                "-- which is a three-dimensional Euclidean space --\n",
+                "-- which is a flat, three-dimensional Euclidean space --\n",
                 "we can add and scale components without worrying about curvature.\n",
                 "Using the *exponential map* operation,\n",
                 "the result can be projected back onto the unit hypersphere.\n",
                 "This way,\n",
                 "we can take the equation for the tangent vector in Euclidean space ...\n",
                 "\n",
                 "\\begin{equation*}\n",
@@ -751,15 +751,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We don't want to worry about end conditions here,\n",
-                "therefore we create a closed curve."
+                "so let's create a closed curve."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -843,15 +843,15 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Shoemake's Approach\n",
                 "\n",
                 "In section 4.2,\n",
-                "<cite data-cite=\"shoemake1985animating\">Shoemake (1985)</cite>\n",
+                "<cite data-cite-t=\"shoemake1985animating\">Shoemake (1985)</cite>\n",
                 "provides two function definitions:\n",
                 "\n",
                 "\\begin{align*}\n",
                 "\\operatorname{Double}(p, q) &= 2 (p \\cdot q) q - p\\\\\n",
                 "\\operatorname{Bisect}(p, q) &= \\frac{p + q}{\\|p + q\\|}\n",
                 "\\end{align*}"
             ]
@@ -906,15 +906,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "> For the numerically knowledgeable, this construction\n",
                 "approximates the derivative at points of a sampled function by\n",
                 "averaging the central differences of the sample sequence.\n",
                 ">\n",
-                "> ---<cite data-cite=\"shoemake1985animating\">Shoemake (1985)</cite>, footnote on page 249"
+                "> ---<cite data-cite-t=\"shoemake1985animating\">Shoemake (1985)</cite>, footnote on page 249"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -1001,15 +1001,15 @@
                 "segment itself. That is, we are spinning three times\n",
                 "faster than spherical interpolation along the arc.\n",
                 "Fortunately we can correct the speed by merely\n",
                 "truncating the end segments to one third their original\n",
                 "length, so that $a_n$ is closer to $q_n$ and $b_{n+1}$ closer to\n",
                 "$q_{n+1}$.\n",
                 ">\n",
-                "> ---<cite data-cite=\"shoemake1985animating\">Shoemake (1985)</cite>, section 4.4: \"Tangents revisited\"\n",
+                "> ---<cite data-cite-t=\"shoemake1985animating\">Shoemake (1985)</cite>, section 4.4: \"Tangents revisited\"\n",
                 "\n",
                 "</div>"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `splines-0.2.0/doc/rotation/cumulative-form.ipynb` & `splines-0.3.0/doc/rotation/cumulative-form.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984011926283516%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(3, \'<cite data-cite-t="kim1995general">Kim, Kim and Shin '*

 * *            '(1995)</cite>\\n\'), (4, \'is the following:\\n\'), (8, "-- as it\'s for example done '*

 * *            'with [Bézier splines](../euclidean/bezier.ipynb) --\\n")], delete: [8, 4, 3]}}, 9: '*

 * *            '{\'source\': ["Let\'s import a few helper functions from [helper.py](helper.py):"]}, '*

 * *            '18: {\'source\': {insert: [(3, \'<cite data-cit-te="kim1995general">Kim, Kim and Shin '*

 * *            […]*

```diff
@@ -14,20 +14,20 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Cumulative Form\n",
                 "\n",
                 "The basic idea, as proposed by\n",
-                "<cite data-cite=\"kim1995general\">Kim, Kim and Shin (1995)</cite>\n",
-                "(section 4) is the following:\n",
+                "<cite data-cite-t=\"kim1995general\">Kim, Kim and Shin (1995)</cite>\n",
+                "is the following:\n",
                 "\n",
                 "Instead of representing a curve as a sum of basis functions\n",
                 "weighted by its control point's position vectors $p_i$\n",
-                "(as it's for example done with [B\u00e9zier splines](../euclidean/bezier.ipynb)),\n",
+                "-- as it's for example done with [B\u00e9zier splines](../euclidean/bezier.ipynb) --\n",
                 "they suggest to use the relative difference vectors $\\Delta p_i$ between successive control points.\n",
                 "\n",
                 "These relative difference vectors can then be \"translated\" to *local* rotations\n",
                 "(replacing additions with multiplications),\n",
                 "leading to a form of rotation splines."
             ]
         },
@@ -148,15 +148,15 @@
                 "import numpy as np"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "[helper.py](helper.py)"
+                "Let's import a few helper functions from [helper.py](helper.py):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -239,15 +239,15 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Cumulative B\u00e9zier/Bernstein Curve\n",
                 "\n",
                 "After the piecewise Slerp,\n",
-                "<cite data-cite=\"kim1995general\">Kim, Kim and Shin (1995)</cite>\n",
+                "<cite data-cit-te=\"kim1995general\">Kim, Kim and Shin (1995)</cite>\n",
                 "show (in section 5.1) how to create a *cumulative form*\n",
                 "inspired by B\u00e9zier splines, i.e. using Bernstein polynomials."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -284,15 +284,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We can get the Bernstein basis polynomials via the function\n",
-                "[splines.Bernstein.basis()](../python-module/splines.rst#splines.Bernstein.basis):"
+                "[splines.Bernstein.basis()](../python-module/splines.rst#splines.Bernstein.basis) ..."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -416,27 +416,27 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Comparison with De Casteljau's Algorithm\n",
                 "\n",
                 "> This B\u00e9zier quaternion curve has a different\n",
                 "> shape from the B\u00e9zier quaternion curve\n",
-                "> of <cite data-cite=\"shoemake1985animating\">Shoemake (1985)</cite>. \n",
+                "> of <cite data-cite-t=\"shoemake1985animating\">Shoemake (1985)</cite>. \n",
                 ">\n",
-                "> --<cite data-cite=\"kim1995general\">Kim, Kim and Shin (1995)</cite>, section 5.1"
+                "> --<cite data-cite-t=\"kim1995general\">Kim, Kim and Shin (1995)</cite>, section 5.1"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The method described by <cite data-cite=\"shoemake1985animating\">Shoemake (1985)</cite>\n",
+                "The method described by <cite data-cite-t=\"shoemake1985animating\">Shoemake (1985)</cite>\n",
                 "is shown in [a separate notebook](de-casteljau.ipynb).\n",
-                "An implementation is available in the\n",
-                "[splines.quaternion.DeCasteljau](../python-module/splines.quaternion.rst#splines.quaternion.DeCasteljau) class:"
+                "An implementation is available in the class\n",
+                "[splines.quaternion.DeCasteljau](../python-module/splines.quaternion.rst#splines.quaternion.DeCasteljau):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `splines-0.2.0/doc/rotation/de-casteljau.ipynb` & `splines-0.3.0/doc/rotation/de-casteljau.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9935809817754262%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(2, \'<cite data-cite-t="shoemake1985animating">Shoemake '*

 * *            "(1985)</cite>,\\n'), (3, 'who famously introduced quaternions to the field of "*

 * *            'computer graphics,\\n\'), (4, \'suggests to apply a variant of\\n\'), (5, "[De '*

 * *            'Casteljau\'s Algorithm](../euclidean/bezier-de-casteljau.ipynb)\\n")], delete: [5, 4, '*

 * *            "3, 2]}}, 5: {'source': {insert: [(2, '<cite "*

 * *            'data-cite-t="shoemake1985animating">Shoemake (1985)</ […]*

```diff
@@ -13,18 +13,18 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# De Casteljau's Algorithm With Slerp\n",
                 "\n",
-                "In <cite data-cite=\"shoemake1985animating\">Shoemake (1985)</cite>,\n",
-                "which famously introduces quaternions to the field of computer graphics,\n",
-                "Shoemake suggests to apply a variant of\n",
-                "[de Casteljau's Algorithm](../euclidean/bezier-de-casteljau.ipynb)\n",
+                "<cite data-cite-t=\"shoemake1985animating\">Shoemake (1985)</cite>,\n",
+                "who famously introduced quaternions to the field of computer graphics,\n",
+                "suggests to apply a variant of\n",
+                "[De Casteljau's Algorithm](../euclidean/bezier-de-casteljau.ipynb)\n",
                 "to a unit quaternion control polygon,\n",
                 "using [Slerp](slerp.ipynb) instead of linear interpolations."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -56,15 +56,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## \"Cubic\"\n",
                 "\n",
-                "<cite data-cite=\"shoemake1985animating\">Shoemake (1985)</cite>\n",
+                "<cite data-cite-t=\"shoemake1985animating\">Shoemake (1985)</cite>\n",
                 "only talks about the \"cubic\" case,\n",
                 "consisting of three nested applications of Slerp.\n",
                 "Since this is done in a curved space,\n",
                 "the resulting curve is of course not simply a polynomial of degree 3,\n",
                 "but something quite a bit more involved.\n",
                 "Therefore, we use the term \"cubic\" in quotes.\n",
                 "Shoemake doesn't talk about the \"degree\" of the curves at all,\n",
@@ -232,24 +232,40 @@
             "metadata": {},
             "source": [
                 "## Constant Angular Speed\n",
                 "\n",
                 "> Is there a way to construct a curve parameterized by arc length?\n",
                 "> This would be very useful.\n",
                 ">\n",
-                "> --<cite data-cite=\"shoemake1985animating\">Shoemake (1985)</cite>, section 6: \"Questions\""
+                "> --<cite data-cite-t=\"shoemake1985animating\">Shoemake (1985)</cite>, section 6: \"Questions\""
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Remember\n",
+                "[arc-length parameterization of Euclidean splines](../euclidean/re-parameterization.ipynb#Arc-Length-Parameterization)?\n",
+                "We used the class\n",
+                "[splines.UnitSpeedAdapter](../python-module/splines.rst#splines.UnitSpeedAdapter)\n",
+                "which happens to be implemented in a way\n",
+                "that it is also usable for rotation splines, how convenient!\n",
+                "The only requirement is that the second derivative\n",
+                "of the wrapped spline yields an angular velocity vector,\n",
+                "which is nothing else than the instantaneous rotation axis\n",
+                "scaled by the angular speed."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from splines import ConstantSpeedAdapter"
+                "from splines import UnitSpeedAdapter"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -264,15 +280,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "s2 = ConstantSpeedAdapter(s1)"
+                "s2 = UnitSpeedAdapter(s1)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `splines-0.2.0/doc/rotation/end-conditions-natural.ipynb` & `splines-0.3.0/doc/rotation/end-conditions-natural.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990354938271605%*

 * *Differences: {"'cells'": "{7: {'source': {insert: [(1, 'and the class\\n'), (2, "*

 * *            "'[splines.quaternion.DeCasteljau](../python-module/splines.quaternion.rst#splines.quaternion.DeCasteljau):')], "*

 * *            'delete: [3, 2, 1]}}}'}*

```diff
@@ -91,17 +91,16 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Let's first import NumPy, a few helpers from [helper.py](helper.py)\n",
-                "and the\n",
-                "[splines.quaternion.DeCasteljau](../python-module/splines.quaternion.rst#splines.quaternion.DeCasteljau)\n",
-                "class:"
+                "and the class\n",
+                "[splines.quaternion.DeCasteljau](../python-module/splines.quaternion.rst#splines.quaternion.DeCasteljau):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `splines-0.2.0/doc/rotation/helper.py` & `splines-0.3.0/doc/rotation/helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """Helper functions for plotting rotations."""
-from functools import partial
 from math import radians, degrees, atan2, asin
 
 import matplotlib
 from matplotlib.animation import FuncAnimation
 from matplotlib.colors import LightSource
 import matplotlib.pyplot as plt
 from mpl_toolkits.mplot3d import Axes3D, proj3d
 from mpl_toolkits.mplot3d.art3d import Poly3DCollection
 import numpy as np
 
 from splines.quaternion import UnitQuaternion
 
-
-shade_colors = partial(Axes3D._shade_colors, 'dummy')
-generate_normals = partial(Axes3D._generate_normals, 'dummy')
+try:
+    # The helper functions have been moved in Matplotlib 3.7.0,
+    # see https://github.com/matplotlib/matplotlib/pull/23914
+    from mpl_toolkits.mplot3d.art3d import _shade_colors, _generate_normals
+except ImportError:
+    from functools import partial
+    _shade_colors = partial(Axes3D._shade_colors, 'dummy')
+    _generate_normals = partial(Axes3D._generate_normals, 'dummy')
 
 
 def faces():
     """Quadratic faces for an F-shaped object."""
     top = np.array([[1, 1, 1], [-1, 1, 1], [-1, -1, 1], [1, -1, 1]])
     north = np.array([[1,  1, -1], [-1,  1, -1], [-1,  1,  1], [1,  1,  1]])
     east = np.array([[1,  1, -1], [1,  1,  1], [1, -1,  1], [1, -1, -1]])
@@ -78,15 +82,15 @@
 def create_polys(rot, *, ls=None):
     if not isinstance(rot, UnitQuaternion):
         rot = UnitQuaternion.from_unit_xyzw(rot)
     polys = np.array([list(map(rot.rotate_vector, face)) for face in faces()])
     if ls is None:
         ls = LightSource()
     color = 'white'
-    facecolors = shade_colors(color, generate_normals(polys), ls)
+    facecolors = _shade_colors(color, _generate_normals(polys), ls)
     return polys, facecolors
 
 
 def create_empty_collection(ax):
     alpha = 1
     linewidth = 0.5
     edgecolor = 'black'
```

### Comparing `splines-0.2.0/doc/rotation/index.ipynb` & `splines-0.3.0/doc/euclidean/index.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9717261904761905%*

 * *Differences: {"'cells'": "{1: {'source': ['# Polynomial Curves in Euclidean Space\\n', '\\n', 'This section is "*

 * *            "mostly about different types of\\n', 'univariate non-rational polynomial splines\\n', "*

 * *            "'in one-, two- and three-dimensional Euclidean space --\\n', 'for an application in a "*

 * *            "four-dimensional space, see\\n', '[the section about 4D quaternion "*

 * *            "interpolation](../rotation/naive-4d-interpolation.ipynb).\\n', '\\n', 'But before "*

 * *            "diving into [splin […]*

```diff
@@ -11,54 +11,69 @@
                 "[back to overview](../index.ipynb)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Rotation Splines"
+                "# Polynomial Curves in Euclidean Space\n",
+                "\n",
+                "This section is mostly about different types of\n",
+                "univariate non-rational polynomial splines\n",
+                "in one-, two- and three-dimensional Euclidean space --\n",
+                "for an application in a four-dimensional space, see\n",
+                "[the section about 4D quaternion interpolation](../rotation/naive-4d-interpolation.ipynb).\n",
+                "\n",
+                "But before diving into [splines](splines.rst)\n",
+                "-- and before even defining what they are --\n",
+                "we will discuss a few basics about polynomial curves\n",
+                "and a spline-less interpolation method called\n",
+                "[Lagrange interpolation](lagrange.ipynb).\n",
+                "\n",
+                "Many of the approaches shown in this section\n",
+                "will later be adapted to the context of\n",
+                "[rotation splines](../rotation/index.ipynb)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "tags": [
-                    "nbsphinx-toctree"
-                ]
+                "nbsphinx-toctree": {}
             },
             "source": [
-                "* [Quaternions](quaternions.ipynb)\n",
-                "* [Spherical Linear Interpolation (Slerp)](slerp.ipynb)\n",
-                "* [De Casteljau's Algorithm With Slerp](de-casteljau.ipynb)\n",
-                "* [Uniform Catmull--Rom-Like Quaternion Splines](catmull-rom-uniform.ipynb)\n",
-                "* [Non-Uniform Catmull--Rom-Like Quaternion Splines](catmull-rom-non-uniform.ipynb)\n",
-                "* [Kochanek--Bartels-like Rotation Splines](kochanek-bartels.ipynb)\n",
-                "* [\"Natural\" End Conditions](end-conditions-natural.ipynb)\n",
-                "* [Barry--Goldman Algorithm With Slerp](barry-goldman.ipynb)\n",
-                "* [Cumulative Form](cumulative-form.ipynb)\n",
-                "* [Naive 4D Quaternion Interpolation](naive-4d-interpolation.ipynb)\n",
-                "* [Naive Interpolation of Euler Angles](naive-euler-angles-interpolation.ipynb)"
+                "* [Parametric Polynomial Curves](polynomials.ipynb)\n",
+                "* [Lagrange Interpolation](lagrange.ipynb)\n",
+                "* [Splines](splines.rst)\n",
+                "* [Hermite Splines](hermite.ipynb)\n",
+                "* [Natural Splines](natural.ipynb)\n",
+                "* [B\u00e9zier Splines](bezier.ipynb)\n",
+                "* [Quadrangle Interpolation](quadrangle.ipynb)\n",
+                "* [Catmull--Rom Splines](catmull-rom.ipynb)\n",
+                "* [Kochanek--Bartels Splines](kochanek-bartels.ipynb)\n",
+                "* [End Conditions](end-conditions.ipynb)\n",
+                "* [Piecewise Monotone Interpolation](piecewise-monotone.ipynb)\n",
+                "* [Re-Parameterization](re-parameterization.ipynb)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.9"
+            "version": "3.11.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `splines-0.2.0/doc/rotation/kochanek-bartels.ipynb` & `splines-0.3.0/doc/rotation/kochanek-bartels.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982096354166667%*

 * *Differences: {"'cells'": '{2: {\'source\': {insert: [(2, "[De Casteljau\'s algorithm with '*

 * *            'Slerp](de-casteljau.ipynb).\\n")], delete: [2]}}, 10: {\'source\': [\'A Python '*

 * *            "implementation of these equations is available in the class\\n', "*

 * *            "'[splines.quaternion.KochanekBartels](../python-module/splines.quaternion.rst#splines.quaternion.KochanekBartels).']}, "*

 * *            '16: {\'source\': ["Let\'s define a few example rotations ..."]}, 30: {\'source\': '*

 * *            "{insert: [(2, ' […]*

```diff
@@ -20,15 +20,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Remember [Kochanek--Bartels splines in Euclidean space](../euclidean/kochanek-bartels.ipynb)?\n",
                 "We can try to \"translate\" those to quaternions by using\n",
-                "[de Casteljau's algorithm with Slerp](de-casteljau.ipynb).\n",
+                "[De Casteljau's algorithm with Slerp](de-casteljau.ipynb).\n",
                 "We only need a way to create the appropriate incoming and outgoing\n",
                 "control quaternions,\n",
                 "similarly to what we did to create\n",
                 "[Catmull--Rom-like rotation splines](catmull-rom-non-uniform.ipynb)."
             ]
         },
         {
@@ -159,16 +159,16 @@
                 "are the control quaternions before and after $q_i$, respectively."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "A Python implementation of these equations is available in the\n",
-                "[splines.quaternion.KochanekBartels](../python-module/splines.quaternion.rst#splines.quaternion.KochanekBartels) class."
+                "A Python implementation of these equations is available in the class\n",
+                "[splines.quaternion.KochanekBartels](../python-module/splines.quaternion.rst#splines.quaternion.KochanekBartels)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -214,15 +214,15 @@
                 "from helper import angles2quat, animate_rotations, display_animation"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We define a few example rotations ..."
+                "Let's define a few example rotations ..."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -374,15 +374,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Just like in the Euclidean case,\n",
                 "$B = -1$ followed by $B = 1$ can be used to create linear\n",
-                "(i.e. [Slerp](slerp.ipynb)) segments."
+                "-- i.e. [Slerp](slerp.ipynb) -- segments."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `splines-0.2.0/doc/rotation/naive-4d-interpolation.ipynb` & `splines-0.3.0/doc/rotation/naive-4d-interpolation.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988695243248815%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(5, '> --<cite "*

 * *            'data-cite-t="shoemake1985animating">Shoemake (1985)</cite>, section 5.4\')], delete: '*

 * *            "[5]}}, 3: {'source': {insert: [(9, '> --<cite "*

 * *            'data-cite-t="shoemake1985animating">Shoemake (1985)</cite>, section 6\')], delete: '*

 * *            "[9]}}, 23: {'source': {delete: [2]}}, 28: {'source': {insert: [(1, "*

 * *            "'[UnitSpeedAdapter](../python-module/splines.rst#splines.UnitSpeedAdapter):')], "*

 * *            "delete:  […]*

```diff
@@ -48,15 +48,15 @@
             "metadata": {},
             "source": [
                 "> If, for some application, more speed is essential,\n",
                 "> non-spherical quaternion splines will undoubtedly be faster\n",
                 "> than angle interpolation,\n",
                 "> while still free of axis bias and gimbal lock.\n",
                 ">\n",
-                "> --<cite data-cite=\"shoemake1985animating\">Shoemake (1985)</cite>, section 5.4"
+                "> --<cite data-cite-t=\"shoemake1985animating\">Shoemake (1985)</cite>, section 5.4"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "> Abandoning the unit sphere,\n",
@@ -64,15 +64,15 @@
                 "> of arbitrary quaternions.\n",
                 "> How do standard interpolation methods applied there\n",
                 "> behave when mapped back to matrices?\n",
                 "> Note that we now have little guidance in picking the inverse image for a matrix,\n",
                 "> and that cusp-free $\\mathbf{R}^4$ paths\n",
                 "> do not always project to cusp-free $S^3$ paths.\n",
                 ">\n",
-                "> --<cite data-cite=\"shoemake1985animating\">Shoemake (1985)</cite>, section 6"
+                "> --<cite data-cite-t=\"shoemake1985animating\">Shoemake (1985)</cite>, section 6"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -262,15 +262,14 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "To get a different temporal behavior,\n",
                 "let's try using [centripetal parameterization](../euclidean/catmull-rom-properties.ipynb#Centripetal-Parameterization).\n",
-                "\n",
                 "Note that this guarantees the absence\n",
                 "of cusps and self-intersections\n",
                 "in the 4D curve,\n",
                 "but this guarantee doesn't extend to\n",
                 "the projection onto the unit hypersphere."
             ]
         },
@@ -317,24 +316,24 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Let's also try *arc-length parameterization* with the\n",
-                "[ConstantSpeedAdapter](../python-module/splines.rst#splines.ConstantSpeedAdapter):"
+                "[UnitSpeedAdapter](../python-module/splines.rst#splines.UnitSpeedAdapter):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "s3 = splines.ConstantSpeedAdapter(s2)\n",
+                "s3 = splines.UnitSpeedAdapter(s2)\n",
                 "times3 = np.linspace(s3.grid[0], s3.grid[-1], len(times))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -359,15 +358,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "s4 = splines.ConstantSpeedAdapter(\n",
+                "s4 = splines.UnitSpeedAdapter(\n",
                 "    splines.quaternion.CatmullRom(\n",
                 "        rotations, alpha=0.5, endconditions='closed'))\n",
                 "times4 = np.linspace(s4.grid[0], s4.grid[-1], len(times))"
             ]
         },
         {
             "cell_type": "code",
```

### Comparing `splines-0.2.0/doc/rotation/naive-euler-angles-interpolation.ipynb` & `splines-0.3.0/doc/rotation/naive-euler-angles-interpolation.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996693121693121%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'This method for interpolating 3D rotations is not "*

 * *            "recommended at all!\\n')], delete: [2]}}}"}*

```diff
@@ -13,15 +13,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Naive Interpolation of Euler Angles\n",
                 "\n",
-                "This method for interpolating 3D rotations is very much not recommended!\n",
+                "This method for interpolating 3D rotations is not recommended at all!\n",
                 "\n",
                 "Since 3D rotations can be represented by a list of three angles,\n",
                 "it might be tempting to simply interpolate those angles independently.\n",
                 "\n",
                 "Let's try it and see what happens, shall we?"
             ]
         },
```

### Comparing `splines-0.2.0/doc/rotation/quaternions.ipynb` & `splines-0.3.0/doc/rotation/quaternions.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9904175460875031%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(8, 'It is important to note that\\n')], delete: [8]}}, 6: "*

 * *            "{'source': {insert: [(4, 'as 4x4 real matrices\\n'), (5, '<cite "*

 * *            'data-cite="mcdonald2010quaternions">(McDonald 2010)</cite>.\')], delete: [6, 5, 4]}}, '*

 * *            "11: {'source': {insert: [(13, 'More specifically, the antipodal points $q$ and $-q$ "*

 * *            "represent the same rotation\\n'), (14, '-- see [Negation](#Negation) below.\\n')], "*

 * *            "delete: [13]}}, 19: {'s […]*

```diff
@@ -66,15 +66,15 @@
                 "Their original algebraic representation is\n",
                 "\n",
                 "\\begin{equation*}\n",
                 "q = w + x\\mathbf{i} + y\\mathbf{j} + z\\mathbf{k},\n",
                 "\\end{equation*}\n",
                 "\n",
                 "where $\\mathbf{i}^2 = \\mathbf{j}^2 = \\mathbf{k}^2 = \\mathbf{ijk} = -1$.\n",
-                "It it important to note that\n",
+                "It is important to note that\n",
                 "the order in which the *basic quaternions*\n",
                 "$\\mathbf{i}$,\n",
                 "$\\mathbf{j}$ and\n",
                 "$\\mathbf{k}$\n",
                 "are multiplied matters:\n",
                 "$\\mathbf{ij} = \\mathbf{k}$, $\\mathbf{ji} = -\\mathbf{k}$\n",
                 "(i.e. their multiplication is\n",
@@ -120,17 +120,16 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "There are even more ways to represent quaterions,\n",
                 "for example\n",
                 "as 2x2 complex matrices\n",
                 "or\n",
-                "as 4x4 real matrices,\n",
-                "see for example\n",
-                "<cite data-cite=\"mcdonald2010quaternions\">McDonald (2010)</cite>."
+                "as 4x4 real matrices\n",
+                "<cite data-cite=\"mcdonald2010quaternions\">(McDonald 2010)</cite>."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Unit Quaternions"
@@ -183,15 +182,16 @@
                 "\\begin{equation*}\n",
                 "q = \\left(\\cos \\frac{\\alpha}{2}, \\vec{n} \\sin \\frac{\\alpha}{2}\\right)\n",
                 "\\end{equation*}\n",
                 "\n",
                 "Unit quaternions are a *double cover* over the rotation group\n",
                 "(a.k.a. [SO(3)](https://en.wikipedia.org/wiki/3D_rotation_group)),\n",
                 "which means that each rotation can be associated with two distinct quaternions.\n",
-                "More concretely, the antipodal points $q$ and $-q$ represent the same rotation.\n",
+                "More specifically, the antipodal points $q$ and $-q$ represent the same rotation\n",
+                "-- see [Negation](#Negation) below.\n",
                 "\n",
                 "More details can be found on\n",
                 "[Wikipedia](https://en.wikipedia.org/wiki/Quaternions_and_spatial_rotation)."
             ]
         },
         {
             "cell_type": "markdown",
@@ -269,15 +269,15 @@
                 "and unit quaternions,\n",
                 "we can freely choose from a multitude of\n",
                 "[axes conventions](https://en.wikipedia.org/wiki/Axes_conventions).\n",
                 "Here we choose a (global) coordinate system where\n",
                 "the x-axis points towards the right margin of the page and\n",
                 "the y-axis points towards the top of the page.\n",
                 "We are using a right-handed coordinate system,\n",
-                "which leaves the z-axis pointing out of the page, towards the viewer.\n",
+                "which leaves the z-axis pointing out of the page, towards the reader.\n",
                 "The helper function `angles2quat()` takes three angles (in degrees)\n",
                 "which are applied in this order:\n",
                 "\n",
                 "* *azimuth*: rotation around the (global) z-axis\n",
                 "* *elevation*: rotation around the (previously rotated local) x-axis\n",
                 "* *roll*: rotation around the (previously rotated local) y-axis\n",
                 "\n",
@@ -311,16 +311,19 @@
                 "we can apply a *local* rotation $q_3$ (relative to this new coordinate system)\n",
                 "by right-multiplication: $q_2 q_3$.\n",
                 "In other words, applying a rotation of $q_2$\n",
                 "followed by a rotation of $q_3$\n",
                 "(relative to the local coordinate system defined by $q_2$)\n",
                 "is equivalent to applying a single rotation $q_2 q_3$.\n",
                 "\n",
-                "In general, changing the order of rotations changes the resulting rotation\n",
-                "($q_m q_n \\ne q_n q_m$):"
+                "In general, changing the order of rotations changes the resulting rotation:\n",
+                "\n",
+                "\\begin{equation*}\n",
+                "q_m q_n \\ne q_n q_m\n",
+                "\\end{equation*}"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -341,14 +344,37 @@
                 "A multiplication with this (on either side) leads to an unchanged rotation."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "Even though quaternion multiplication is *non-commutative*,\n",
+                "it is still [associative](https://en.wikipedia.org/wiki/Associative_property),\n",
+                "which means that if there are multiple multiplications in a row,\n",
+                "they can be grouped arbitrarily, leading to the same overall result:\n",
+                "\n",
+                "\\begin{equation*}\n",
+                "(q_1 q_2) q_3 = q_1 (q_2 q_3)\n",
+                "\\end{equation*}"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "plot_rotation({'$(bc)a$': (b * c) * a, '$b(ca)$': b * (c * a)});"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "## Inverse"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -462,15 +488,15 @@
                 "## Exponentiation"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Raising a unit quaternion to an integer exponent\n",
+                "Raising a unit quaternion to an integer power\n",
                 "simply means applying the same rotation multiple times:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -492,16 +518,16 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Using an exponent of $-1$ is equivalent to taking the inverse\n",
-                "(see [above](#Inverse)),\n",
-                "negative integer exponents apply the inverse rotation multiple times.\n",
+                "-- see [above](#Inverse).\n",
+                "Negative integer exponents apply the inverse rotation multiple times.\n",
                 "Non-integer exponents lead to partial rotations,\n",
                 "with the exponent $k$ being proportional to the rotation angle.\n",
                 "The rotation axis $\\vec{n}$ is unchanged by exponentiation."
             ]
         },
         {
             "cell_type": "markdown",
@@ -577,14 +603,38 @@
                 "= \\left(-w, -\\vec{v}\\right)\n",
                 "= \\left(\n",
                 "\\cos \\frac{\\alpha + 2 \\pi}{2},\n",
                 "\\vec{n} \\sin \\frac{\\alpha + 2 \\pi}{2}\n",
                 "\\right)\n",
                 "\\end{equation*}"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Canonicalization\n",
+                "\n",
+                "When we are given multiple rotations\n",
+                "and we want to represent them as quaternions,\n",
+                "we have to take care of the ambiguity caused by the double cover property\n",
+                "-- see [Slerp Visualization](slerp.ipynb#Visualization)\n",
+                "for an example of this ambiguity.\n",
+                "\n",
+                "One way to do that is to make sure that in a sequence of rotations\n",
+                "(which we want to use as the control points of a spline, for example),\n",
+                "the angle (in 4D space) between neighboring quaternions\n",
+                "is at most 90 degrees (which corresponds to a 180 degree rotation in 3D space).\n",
+                "For any pair of quaternions where this is not the case,\n",
+                "one of the quaternions can simply be negated.\n",
+                "The function\n",
+                "[splines.quaternion.canonicalized()](../python-module/splines.quaternion.rst#splines.quaternion.canonicalized)\n",
+                "can be used to create an iterator of canonicalized quaternions\n",
+                "from an iterable of arbitrary quaternions."
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `splines-0.2.0/doc/rotation/slerp.ipynb` & `splines-0.3.0/doc/rotation/slerp.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9942139373843003%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(5, \'<cite data-cite-t="shoemake1985animating">Shoemake '*

 * *            "(1985)</cite>,\\n'), (6, 'section 3.3.\\n')], delete: [6, 5]}}, 3: {'source': "*

 * *            '{insert: [(0, \'<cite data-cite-t="shoemake1985animating">Shoemake '*

 * *            "(1985)</cite>\\n')], delete: [0]}}, 4: {'source': {insert: [(1, '*inner product "*

 * *            "space* (i.e. a vector space that also has an inner product),\\n')], delete: [1]}}, "*

 * *            "22: {'source': {insert: [(0, 'If […]*

```diff
@@ -16,16 +16,16 @@
             "metadata": {},
             "source": [
                 "# Spherical Linear Interpolation (Slerp)\n",
                 "\n",
                 "The term \"Slerp\" for \"**s**pherical **l**inear int**erp**olation\"\n",
                 "(a.k.a. \"great arc in-betweening\")\n",
                 "has been coined by\n",
-                "<cite data-cite=\"shoemake1985animating\">Shoemake (1985)</cite>\n",
-                "(section 3.3).\n",
+                "<cite data-cite-t=\"shoemake1985animating\">Shoemake (1985)</cite>,\n",
+                "section 3.3.\n",
                 "It describes an interpolation (with constant angular velocity)\n",
                 "along the shortest path (a.k.a. geodesic) on the unit hypersphere\n",
                 "between two quaternions $q_1$ and $q_2$.\n",
                 "It is defined as:\n",
                 "\n",
                 "\\begin{equation*}\n",
                 "\\operatorname{Slerp}(q_1, q_2; u) =\n",
@@ -52,15 +52,15 @@
                 "\\end{align*}"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "<cite data-cite=\"shoemake1985animating\">Shoemake (1985)</cite>\n",
+                "<cite data-cite-t=\"shoemake1985animating\">Shoemake (1985)</cite>\n",
                 "also provides an alternative formulation\n",
                 "(attributed to Glenn Davis):\n",
                 "\n",
                 "\\begin{equation*}\n",
                 "\\operatorname{Slerp}(q_1, q_2; u) =\n",
                 "\\frac{\\sin (1-u) \\theta}{\\sin \\theta} q_1 +\n",
                 "\\frac{\\sin u \\theta}{\\sin \\theta} q_2,\n",
@@ -71,15 +71,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Latter equation works for unit-length elements of any arbitrary-dimensional\n",
-                "inner product space (i.e. a vector space that also has an inner product),\n",
+                "*inner product space* (i.e. a vector space that also has an inner product),\n",
                 "while the preceding equations only work for quaternions."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -256,18 +256,19 @@
                 "np.degrees(q1.rotation_to(q2).angle)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "If this angle is smaller than 180\u00b0,\n",
+                "If this angle is smaller than 180 degrees,\n",
                 "we know that we will get the smallest difference in rotation.\n",
-                "If it is larger than 180\u00b0,\n",
-                "we can negate the second quaternion to get a smaller rotation."
+                "If it is larger than 180 degrees,\n",
+                "we can negate the second quaternion to get a smaller rotation\n",
+                "-- see [canonicalization](quaternions.ipynb#Canonicalization)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -275,15 +276,16 @@
                 "ani_times = np.linspace(0, 1, 50)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We show both the original target quaternion and its antipodal point here:"
+                "We show both the original target quaternion and its antipodal point\n",
+                "in this animation:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -303,27 +305,15 @@
                 "display_animation(ani, default_mode='reflect')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "`slerp(q1, q2)` and `slerp(q1, -q2)` move along the same great circle,\n",
-                "albeit in different directions.\n",
-                "In total, they cover half the circumference of that great circle,\n",
-                "which means a rotation angle of 360 degrees.\n",
-                "Note that `q2` and `-q2` represent the same rotation\n",
-                "(because of the *double cover* property)."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Let's create some still images:"
+                "Let's create some still images as well:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -352,14 +342,26 @@
                 "}, figsize=(8, 3))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "`slerp(q1, q2)` and `slerp(q1, -q2)` move along the same great circle,\n",
+                "albeit in different directions.\n",
+                "In total, they cover half the circumference of that great circle,\n",
+                "which means a rotation angle of 360 degrees.\n",
+                "Note that `q2` and `-q2` represent the same rotation\n",
+                "(because of the *double cover* property)."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "## Piecewise Slerp\n",
                 "\n",
                 "The class\n",
                 "[PiecewiseSlerp](../python-module/splines.quaternion.rst#splines.quaternion.PiecewiseSlerp)\n",
                 "provides a rotation spline that consists of Slerp sections\n",
                 "between the given quaternions."
             ]
@@ -474,15 +476,15 @@
                 "    return Quaternion(scalar, vector).normalized()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "As a first example, we try an angle below 180\u00b0 ..."
+                "As a first example, we try an angle below 180 degrees ..."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -646,15 +648,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Now the difference is clearly visible,\n",
                 "but depending on the application you might want to limit your rotations\n",
-                "to $\\pm 180\u00b0$ anyway, so this might not be relevant."
+                "to $\\pm 180$ degrees anyway, so this might not be relevant."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
```

### Comparing `splines-0.2.0/setup.py` & `splines-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,33 @@
+from pathlib import Path
+
 from setuptools import setup
 
 # "import" __version__
 __version__ = 'unknown'
-for line in open('src/splines/__init__.py'):
-    if line.startswith('__version__'):
-        exec(line)
-        break
+with Path('src/splines/__init__.py').open() as f:
+    for line in f:
+        if line.startswith('__version__'):
+            exec(line)
+            break
 
 setup(
     name='splines',
     packages=['splines'],
     package_dir={'': 'src'},
     version=__version__,
     author='Matthias Geier',
     author_email='Matthias.Geier@gmail.com',
     description='Splines in Euclidean Space and Beyond',
-    long_description=open('README.rst').read(),
+    long_description=Path('README.rst').read_text(),
     install_requires=['NumPy'],
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     license='MIT',
     keywords='splines curves interpolation quaternions'.split(),
+    url='https://splines.readthedocs.io/',
     project_urls={
         'Documentation': 'https://splines.readthedocs.io/',
         'Source Code': 'https://github.com/AudioSceneDescriptionFormat/splines/',
         'Bug Tracker': 'https://github.com/AudioSceneDescriptionFormat/splines/issues/',
     },
     platforms='any',
     classifiers=[
```

### Comparing `splines-0.2.0/src/splines/__init__.py` & `splines-0.3.0/src/splines/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 """Piecewise polynomial curves (in Euclidean space).
 
-.. rubric:: Submodules
+.. topic:: Submodules
 
-.. autosummary::
+    .. autosummary::
 
-    quaternion
+        quaternion
 
 """
 from bisect import bisect_right as _bisect_right, bisect_left as _bisect_left
 from itertools import accumulate as _accumulate
 from math import factorial as _factorial
 
 import numpy as _np
 
 
-__version__ = '0.2.0'
+__version__ = '0.3.0'
 
 
 class Monomial:
     """Piecewise polynomial curve, see __init__()."""
 
-    def __init__(self, segments, grid):
+    def __init__(self, segments, grid=None):
         r"""Piecewise polynomial curve using monomial basis.
 
         See :ref:`/euclidean/polynomials.ipynb`.
 
         Coefficients can have arbitrary dimension.
         An arbitrary polynomial degree :math:`d` can be used by specifying
         :math:`d + 1` coefficients per segment.
-        The :math:`i`-th segment is evaluated using this equation:
+        The :math:`i`-th segment is evaluated using
 
         .. math::
 
             \boldsymbol{p}_i(t) = \sum_{k=0}^d
                 \boldsymbol{a}_{i,k} \left(\frac{t - t_i}{t_{i+1} - t_i}\right)^k
-                \text{ for } t_i \leq t < t_{i+1}
+                \text{ for } t_i \leq t < t_{i+1}.
 
         This is similar to `scipy.interpolate.PPoly`, which states:
 
-            "High-order polynomials in the power basis can be numerically
+            High-order polynomials in the power basis can be numerically
             unstable.  Precision problems can start to appear for orders
-            larger than 20-30."
+            larger than 20-30.
 
-        This shouldn't be a problem since most commonly splines of degree 3
+        This shouldn't be a problem, since most commonly splines of degree 3
         (i.e. cubic splines) are used.
 
         :param segments: Sequence of polynomial segments.
             Each segment :math:`\boldsymbol{a}_i` contains coefficients
             for the monomial basis (in order of decreasing degree).
-            Different segments can have different polynomial degree.
+            Different segments can have different polynomial degrees.
         :param grid: Sequence of parameter values :math:`t_i` corresponding to
             segment boundaries.  Must be strictly increasing.
+            If not specified, a uniform grid is used (0, 1, 2, 3, ...).
+        :type grid: optional
 
         """
         self.segments = [_np.array(coefficients, copy=True)
                          for coefficients in segments]
         if grid is None:
             grid = range(len(segments) + 1)
         self.grid = list(grid)
@@ -79,16 +81,15 @@
     """Piecewise Bézier curve, see __init__()."""
 
     @staticmethod
     def basis(degree, t):
         r"""Bernstein basis polynomials of given *degree*, evaluated at *t*.
 
         Returns a list of values corresponding to
-        :math:`i = 0, \ldots, n`, given the degree :math:`n`,
-        using the formula
+        :math:`i = 0, \ldots, n`, given the degree :math:`n`, using
 
         .. math::
 
             b_{i,n}(t) = {n \choose i} t^i \left( 1 - t \right)^{n - i},
 
         with the *binomial coefficient*
         :math:`{n \choose i} = \frac{n!}{i!(n - i)!}`.
@@ -116,27 +117,36 @@
         self.segments = [_np.array(control_points, copy=True)
                          for control_points in segments]
         if grid is None:
             grid = range(len(segments) + 1)
         self.grid = list(grid)
 
     def evaluate(self, t, n=0):
-        """Get value at the given parameter value(s)."""
+        """Get value at the given parameter value(s) *t*.
+
+        Only ``n=0`` is currently supported.
+
+        """
         if n != 0:
             raise NotImplementedError('Derivatives are not implemented yet')
         if not _np.isscalar(t):
             return _np.array([self.evaluate(time, n) for time in t])
         idx = _check_param('t', t, self.grid)
         t0, t1 = self.grid[idx:idx + 2]
         t = (t - t0) / (t1 - t0)
         control_points = self.segments[idx]
         degree = len(control_points) - 1
-        return sum(
-            a * b
-            for a, b in zip(control_points, self.basis(degree, t)))
+        basis = self.basis(degree, t)
+        return _dotproduct(control_points, basis)
+
+
+def _dotproduct(vec1, vec2):
+    # See https://docs.python.org/3/library/itertools.html#itertools-recipes
+    import operator
+    return sum(map(operator.mul, vec1, vec2))
 
 
 def _check_param(name, param, grid):
     if param < grid[0]:
         raise ValueError(f'{name} too small: {param}')
     elif param < grid[-1]:
         idx = _bisect_right(grid, param) - 1
@@ -258,15 +268,15 @@
     def __init__(self, vertices, tangents, grid=None):
         """Cubic Hermite curve.
 
         See :ref:`/euclidean/hermite.ipynb`.
 
         :param vertices: Sequence of vertices.
         :param tangents: Sequence of tangent vectors
-            (two per segment, outgoing and incoming).
+            (two per segment: outgoing and incoming).
         :param grid: Sequence of parameter values.
             Must be strictly increasing.
             If not specified, a uniform grid is used (0, 1, 2, 3, ...).
         :type grid: optional
 
         """
         if len(vertices) < 2:
@@ -311,15 +321,15 @@
         return (delta0 * v_1 + delta_1 * v0) / (delta0 + delta_1)
 
     def __init__(self, vertices, grid=None, *, alpha=None,
                  endconditions='natural'):
         """Catmull--Rom spline.
 
         This class implements one specific member of the family of
-        splines described in :cite:`catmull1974splines`,
+        splines described by :cite:t:`catmull1974splines`,
         which is commonly known as *Catmull--Rom spline*:
         The cubic spline that can be constructed by linear Lagrange
         interpolation (and extrapolation) followed by quadratic B-spline
         blending, or equivalently, quadratic Lagrange interpolation
         followed by linear B-spline blending.
 
         The implementation used in this class, however, does nothing of
@@ -329,20 +339,21 @@
         See :ref:`/euclidean/catmull-rom.ipynb`.
 
         :param vertices: Sequence of vertices.
         :param grid: Sequence of parameter values.
             Must be strictly increasing.
             If not specified, a uniform grid is used (0, 1, 2, 3, ...).
         :type grid: optional
-        :param alpha: TODO
+        :param alpha: See
+            :ref:`/euclidean/catmull-rom-properties.ipynb#Parameterized-Parameterization`.
         :type alpha: optional
         :param endconditions: Start/end conditions. Can be ``'closed'``,
-            ``'natural'`` or pair of tangent vectors (a.k.a. "clamped").
+            ``'natural'`` or a pair of tangent vectors (a.k.a. "clamped").
             If ``'closed'``, the first vertex is re-used as last vertex
-            and an additional *grid* time has to be specified.
+            and an additional *grid* value has to be specified.
         :type endconditions: optional
 
         """
         closed = endconditions == 'closed'
         vertices = _check_vertices(vertices, closed=closed)
         grid = _check_grid(grid, alpha, vertices)
         start, end, zip_vertices, zip_grid = _check_endconditions(
@@ -387,20 +398,21 @@
         :param grid: Sequence of parameter values.
             Must be strictly increasing.
             If not specified, a uniform grid is used (0, 1, 2, 3, ...).
         :type grid: optional
         :param tcb: Sequence of *tension*, *continuity* and *bias* triples.
             TCB values can only be given for the interior vertices.
         :type tcb: optional
-        :param alpha: TODO
+        :param alpha: See
+            :ref:`/euclidean/catmull-rom-properties.ipynb#Parameterized-Parameterization`.
         :type alpha: optional
         :param endconditions: Start/end conditions. Can be ``'closed'``,
-            ``'natural'`` or pair of tangent vectors (a.k.a. "clamped").
+            ``'natural'`` or a pair of tangent vectors (a.k.a. "clamped").
             If ``'closed'``, the first vertex is re-used as last vertex
-            and an additional *grid* time has to be specified.
+            and an additional *grid* value has to be specified.
         :type endconditions: optional
 
         """
         closed = endconditions == 'closed'
         if closed:
             tcb_slots = len(vertices)
         else:
@@ -437,20 +449,21 @@
         See :ref:`/euclidean/natural.ipynb`.
 
         :param vertices: Sequence of vertices.
         :param grid: Sequence of parameter values.
             Must be strictly increasing.
             If not specified, a uniform grid is used (0, 1, 2, 3, ...).
         :type grid: optional
-        :param alpha: TODO
+        :param alpha: See
+            :ref:`/euclidean/catmull-rom-properties.ipynb#Parameterized-Parameterization`.
         :type alpha: optional
         :param endconditions: Start/end conditions. Can be ``'closed'``,
-            ``'natural'`` or pair of tangent vectors (a.k.a. "clamped").
+            ``'natural'`` or a pair of tangent vectors (a.k.a. "clamped").
             If ``'closed'``, the first vertex is re-used as last vertex
-            and an additional *grid* time has to be specified.
+            and an additional *grid* value has to be specified.
         :type endconditions: optional
 
         """
         N = len(vertices)
         A = _np.zeros((N, N))
         b = _np.zeros_like(vertices)
         closed = endconditions == 'closed'
@@ -654,36 +667,61 @@
 
         CubicHermite.__init__(self, values, final_slopes, grid)
 
 
 class MonotoneCubic(PiecewiseMonotoneCubic):
     """Monotone cubic curve, see __init__()."""
 
-    def __init__(self, values, *args, **kwargs):
+    def __init__(
+            self, values, grid=None, slopes=None, *,
+            alpha=None, cyclic=False,
+            **kwargs):
         """Monotone cubic curve.
 
         This takes the same arguments as `PiecewiseMonotoneCubic`
-        (except ``closed``), but it raises an error if the given values
-        are not montone.
+        (except ``closed`` is replaced by ``cyclic``),
+        but it raises an error if the given values are not montone.
 
         See :ref:`/euclidean/piecewise-monotone.ipynb#Monotone-Interpolation`.
 
         """
         if 'closed' in kwargs:
             raise TypeError('The "closed" argument is not allowed')
-        PiecewiseMonotoneCubic.__init__(self, values, *args, **kwargs)
+
+        grid = _check_grid(grid, alpha, values)
+        if cyclic:
+            if slopes is None:
+                slopes = [None] * len(values)
+            if (slopes[0], slopes[-1]) != (None, None):
+                raise ValueError(
+                    'If "cyclic", the first and last slope must be None')
+            temp_values = (
+                values[-2],
+                values[-1],
+                values[-1] + (values[1] - values[0]))
+            temp_grid = (
+                grid[-2],
+                grid[-1],
+                grid[-1] + (grid[1] - grid[0]))
+            temp_spline = PiecewiseMonotoneCubic(temp_values, grid=temp_grid)
+            cyclic_slope = temp_spline.evaluate(temp_grid[1], 1)
+            slopes[0] = cyclic_slope
+            slopes[-1] = cyclic_slope
+
+        # NB: "alpha" has already been applied, we don't have to pass it on:
+        PiecewiseMonotoneCubic.__init__(self, values, grid, slopes, **kwargs)
         diffs = _np.diff(values)
         if not (all(diffs >= 0) or all(diffs <= 0)):
             raise ValueError('Only monotone values are allowed')
 
     # TODO: rename to something with "solve"?
     def get_time(self, value):
-        """Get the time instance for the given value.
+        """Get the time instance for the given *value*.
 
-        If the solution is not unique (i.e. there is a plateau),
+        If the solution is not unique (i.e. if there is a plateau),
         ``None`` is returned.
 
         """
         if not _np.isscalar(value):
             return _np.array([self.get_time(v) for v in value])
 
         values = self.evaluate(self.grid)
@@ -716,26 +754,30 @@
         roots = roots[_np.isreal(roots) & (roots >= 0) & (roots <= 1)]
         assert len(roots) == 1 and _np.isreal(roots)
         time, = roots.real
         t0, t1 = self.grid[idx:idx + 2]
         return time * (t1 - t0) + t0
 
 
-class ConstantSpeedAdapter:
-    """Re-parameterize a spline to have constant speed, see __init__()."""
+class UnitSpeedAdapter:
+    """Re-parameterize a spline to have unit speed, see __init__()."""
 
     def __init__(self, curve):
-        """Re-parameterize a spline to have constant speed.
+        """Re-parameterize a spline to have a constant speed of 1.
 
-        For splines in Euclidean space this amounts to arc-length
-        parameterization.
+        For splines in Euclidean space this amounts to
+        :ref:`/euclidean/re-parameterization.ipynb#Arc-Length-Parameterization`.
 
         However, this class is implemented in a way that also allows using
-        rotation splines which will be re-parameterized to have constant
-        angular speed.
+        rotation splines, which will be re-parameterized to have a
+        :ref:`/rotation/de-casteljau.ipynb#Constant-Angular-Speed` of 1.
+        For this to work, the second derivative of *curve* must yield
+        an angular velocity vector.
+        See `splines.quaternion.DeCasteljau` for an example of a
+        compatible rotation spline.
 
         The parameter *s* represents the cumulative arc-length or the
         cumulative rotation angle, respectively.
 
         """
         self.curve = curve
         lengths = (
@@ -774,33 +816,40 @@
         def length(t):
             return self._integrated_speed(idx, t0, t) - s
 
         from scipy.optimize import bisect
         return bisect(length, t0, t1)
 
     def evaluate(self, s):
+        """Get value at the given parameter value(s) *s*."""
         if not _np.isscalar(s):
             return _np.array([self.evaluate(s) for s in s])
         return self.curve.evaluate(self._s2t(s))
 
 
 class NewGridAdapter:
     """Re-parameterize a spline with new grid values, see __init__()."""
 
-    def __init__(self, curve, new_grid=1):
+    def __init__(self, curve, new_grid=1, cyclic=False):
         """Re-parameterize a spline with new grid values.
 
+        This can be used for both Euclidean splines and rotation splines.
+
         :param curve: A spline.
         :param new_grid: If a single number is given, the new parameter
             will range from 0 to that number.  Otherwise, a sequence
             of numbers has to be given, one for each grid value.
             Instead of a value, ``None`` can be specified to choose a
             value automatically.
             The first and last value cannot be ``None``.
         :type new_grid: optional
+        :param cyclic: If ``True``, the slope of the re-parameterization
+            function (but not necessarily the speed of the final spline!)
+            will be the same at the beginning and end of the spline.
+        :type cyclic: optional
 
         """
         if _np.isscalar(new_grid):
             new_grid = [0] + [None] * (len(curve.grid) - 2) + [new_grid]
         if len(new_grid) != len(curve.grid):
             raise ValueError('new_grid must have same length as curve.grid')
         if new_grid[0] is None or new_grid[-1] is None:
@@ -808,20 +857,22 @@
         old_values, new_values = [], []
         for old, new in zip(curve.grid, new_grid):
             # TODO: allow NaN?
             if new is None:
                 continue
             new_values.append(new)
             old_values.append(old)
-        self._new2old = MonotoneCubic1D(old_values, grid=new_values)
+        self._new2old = MonotoneCubic(
+            old_values, grid=new_values, cyclic=cyclic)
         self.grid = []
         for old, new in zip(curve.grid, new_grid):
             if new is None:
                 new = self._new2old.get_time(old)
             self.grid.append(new)
         self.curve = curve
 
     def evaluate(self, u):
+        """Get value at the given parameter value(s) *u*."""
         if not _np.isscalar(u):
             return _np.array([self.evaluate(u) for u in u])
         idx = _check_param('u', u, self.grid)
         return self.curve.evaluate(self._new2old.evaluate(u))
```

### Comparing `splines-0.2.0/src/splines/quaternion.py` & `splines-0.3.0/src/splines/quaternion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Quaternions and unit-quaternion splines."""
 import math as _math
 
 import numpy as _np
-from . import _check_param
+from . import _check_param, _dotproduct
 
 
 class Quaternion:
     """A very simple quaternion class.
 
-    This is the base class for the more relevant `UnitQuaternion` class.
+    This is the base class for the more relevant class `UnitQuaternion`.
 
     See the `notebook about quaternions`__.
 
     __ ../rotation/quaternions.ipynb
 
     """
 
@@ -107,25 +107,23 @@
         x, y, z, w = self.xyzw
         return UnitQuaternion.from_unit_xyzw(
             (x / norm, y / norm, z / norm, w / norm))
 
     def dot(self, other):
         """Dot product of two quaternions.
 
-        This is the 4-dimensional dot product, yielding a scalar result.
+        This is the four-dimensional dot product, yielding a scalar result.
         This operation is commutative.
 
         Note that this is different from the quaternion multiplication
         (``q1 * q2``), which produces another quaternion
         (and is noncommutative).
 
         """
-        # NB: math.prod() is available since Python 3.8
-        prod = _np.multiply.reduce
-        return sum(map(prod, zip(self.xyzw, other.xyzw)))
+        return _dotproduct(self.xyzw, other.xyzw)
 
     @property
     def norm(self):
         """Length of the quaternion in 4D space."""
         x, y, z, w = self.xyzw
         return _math.sqrt(x**2 + y**2 + z**2 + w**2)
 
@@ -169,39 +167,44 @@
         s = angle / (2 * norm)
         return cls.exp_map((s * x, s * y, s * z))
 
     @classmethod
     def from_unit_xyzw(cls, xyzw):
         """Create a unit quaternion from another unit quaternion.
 
-        :param xyzw: Components of a unit quaternion (`scalar` last).
+        :param xyzw: Components of a unit quaternion (``scalar`` last).
             This will *not* be normalized, it must already have unit length.
 
         """
         x, y, z, w = xyzw
         return super().__new__(cls, w, (x, y, z))
 
     def __pow__(self, alpha):
         if not _np.isscalar(alpha):
             return _np.array([self.__pow__(a) for a in alpha])
-        if self.scalar >= 1:
+        if abs(self.scalar) >= 1:
             return super().__new__(UnitQuaternion, self.scalar, self.vector)
         return UnitQuaternion.exp_map(alpha * self.log_map())
 
     inverse = Quaternion.conjugate
     """Multiplicative inverse.
 
     For unit quaternions, this is the same as `conjugate()`.
 
     """
 
     @classmethod
     def exp_map(cls, value):
         """Exponential map from :math:`R^3` to unit quaternions.
 
+        The *exponential map* operation transforms
+        a three-dimensional vector that's a member of the
+        tangent space at the identity quaternion
+        into a unit quaternion.
+
         This is the inverse operation to `log_map()`.
 
         :param value: Element of the tangent space at the quaternion identity.
         :type value: 3-tuple
 
         """
         x, y, z = value
@@ -211,16 +214,22 @@
             return super().__new__(cls, one, (zero, zero, zero))
         s = _math.sin(norm) / norm
         return super().__new__(cls, _math.cos(norm), (s * x, s * y, s * z))
 
     def log_map(self):
         """Logarithmic map from unit quaternions to :math:`R^3`.
 
-        :returns: Corresponding vector in the tangent space at the
-            quaternion identity.
+        The *logarithmic map* operation transforms a unit quaternion
+        into a three-dimensional vector that's a member of the
+        tangent space at the identity quaternion.
+
+        This is the inverse operation to `exp_map()`.
+
+        :returns: Corresponding three-element vector in the tangent
+            space at the quaternion identity.
 
         """
         if self.scalar >= 1:
             return _np.zeros_like(self.vector)
         length = self.angle / 2
         return self.axis * length
 
@@ -241,17 +250,17 @@
 
     def rotation_to(self, other):
         """Rotation required to rotate *self* into *other*.
 
         See :ref:`/rotation/quaternions.ipynb#Relative-Rotation-(Global-Frame-of-Reference)`.
 
         :param other: Target rotation.
-        :type other: UnitQuaternion
+        :type other: ``UnitQuaternion``
 
-        :returns: Relative rotation (as `UnitQuaternion`).
+        :returns: Relative rotation -- as ``UnitQuaternion``.
 
         """
         return other * self.inverse()
 
     def rotate_vector(self, v):
         """Apply rotation to a 3D vector.
 
@@ -265,25 +274,31 @@
 
 
 def slerp(one, two, t):
     """Spherical Linear intERPolation.
 
     See :ref:`/rotation/slerp.ipynb`.
 
-    :param one: Start quaternion.
-    :param two: End quaternion.
+    :param one: Start rotation.
+    :type one: ``UnitQuaternion``
+    :param two: End rotation.
+    :type two: ``UnitQuaternion``
     :param t: Parameter value(s) between 0 and 1.
 
     """
     return (two * one.inverse())**t * one
 
 
 def canonicalized(quaternions):
-    """Iterator adapter to ensure minimal angles between *quaternions*."""
-    p = UnitQuaternion.from_unit_xyzw((0, 0, 0, 1))
+    """Iterator adapter to ensure minimal angles between *quaternions*.
+
+    See :ref:`/rotation/quaternions.ipynb#Canonicalization`.
+
+    """
+    p = UnitQuaternion()
     for q in quaternions:
         if p.dot(q) < 0:
             q = -q
         yield q
         p = q
 
 
@@ -315,31 +330,36 @@
             raise ValueError(
                 'Number of grid values must be same as '
                 'quaternions (one more for closed curves)')
         self.quaternions = quaternions
         self.grid = list(grid)
 
     def evaluate(self, t, n=0):
+        """Get value at the given parameter value(s) *t*.
+
+        Only ``n=0`` is currently supported.
+
+        """
         if n != 0:
             raise NotImplementedError('Derivatives are not implemented yet')
         if not _np.isscalar(t):
             return _np.array([self.evaluate(t) for t in t])
         idx = _check_param('t', t, self.grid)
         t0, t1 = self.grid[idx:idx + 2]
         return slerp(
             self.quaternions[idx],
             self.quaternions[idx + 1],
             (t - t0) / (t1 - t0))
 
 
 class DeCasteljau:
-    """Spline using De Casteljau's algorithm, see __init__()."""
+    """Rotation spline using De Casteljau's algorithm, see __init__()."""
 
     def __init__(self, segments, grid=None):
-        """Spline using De Casteljau's algorithm with `slerp()`.
+        """Rotation spline using De Casteljau's algorithm with `slerp()`.
 
         See `the corresponding notebook`__ for details.
 
         __ ../rotation/de-casteljau.ipynb
 
         :param segments: Sequence of segments,
             each one consisting of multiple control quaternions.
@@ -364,15 +384,15 @@
         self.grid = list(grid)
 
     def evaluate(self, t, n=0):
         """Get value or angular velocity at given parameter value(s).
 
         :param t: Parameter value(s).
         :param n: Use ``0`` for calculating the value (a quaternion),
-            ``1`` for the angular velocity (a 3-element vector).
+            ``1`` for the angular velocity (a three-element vector).
         :type n: {0, 1}, optional
 
         """
         if not _np.isscalar(t):
             return _np.array([self.evaluate(t, n) for t in t])
         segment, t, delta_t = self._select_segment_and_normalize_t(t)
         if n == 0:
@@ -453,23 +473,21 @@
             Must be strictly increasing.
             If not specified, a uniform grid is used (0, 1, 2, 3, ...).
         :type grid: optional
         :param tcb: Sequence of *tension*, *continuity* and *bias* triples.
             TCB values can only be given for the interior quaternions.
             If only two quaternions are given, TCB values are ignored.
         :type tcb: optional
-        :param alpha: TODO
+        :param alpha: See
+            :ref:`/euclidean/catmull-rom-properties.ipynb#Parameterized-Parameterization`.
         :type alpha: optional
-        :param endconditions: Start/end conditions. Can be ``'closed'``,
-            ``'natural'`` or pair of tangent vectors (a.k.a. "clamped").
-
-            TODO: clamped
-
+        :param endconditions: Start/end conditions. Can be ``'closed'`` or
+            ``'natural'``.
             If ``'closed'``, the first rotation is re-used as last rotation
-            and an additional *grid* time has to be specified.
+            and an additional *grid* value has to be specified.
         :type endconditions: optional
 
         """
         closed = endconditions == 'closed'
         if closed:
             tcb_slots = len(quaternions)
         else:
@@ -619,53 +637,134 @@
     See rotation/end-conditions-natural.ipynb.
 
     """
     return first.rotation_to(third)**(1 / 2) * first
 
 
 class BarryGoldman:
-    """Rotation spline using Barry--Goldman algorithm, see __init__()."""
+    """Rotation spline using the Barry--Goldman algorithm, see __init__()."""
 
     def __init__(self, quaternions, grid=None, *, alpha=None):
-        """Rotation spline using Barry--Goldman algorithm.
+        """Rotation spline using the Barry--Goldman algorithm with `slerp()`.
 
         Always closed (for now).
 
+        See :ref:`/rotation/barry-goldman.ipynb`.
+
         """
         # TODO: what happens when exactly 2 quaternions are given?
         self.quaternions = _check_quaternions(quaternions, closed=True)
         self.grid = list(_check_grid(grid, alpha, self.quaternions))
 
     def evaluate(self, t):
+        """Get value at the given parameter value(s) *t*."""
         if not _np.isscalar(t):
             return _np.array([self.evaluate(t) for t in t])
         idx = _check_param('t', t, self.grid)
         q0, q1 = self.quaternions[idx:idx + 2]
         t0, t1 = self.grid[idx:idx + 2]
         if idx == 0:
-            q_1 = self.quaternions[-2]
-            if q_1.dot(q0) < 0:
-                q_1 = -q_1
-            t_1 = t0 - (self.grid[-1] - self.grid[-2])
+            q_1 = _cycle_prefix(self.quaternions)
+            t_1 = _cycle_prefix_t(self.grid)
         else:
             q_1 = self.quaternions[idx - 1]
             t_1 = self.grid[idx - 1]
         if idx + 2 == len(self.quaternions):
-            q2 = self.quaternions[1]
-            if q1.dot(q2) < 0:
-                q2 = -q2
+            q2 = _cycle_suffix(self.quaternions)
             assert len(self.quaternions) == len(self.grid)
-            t2 = t1 + (self.grid[1] - self.grid[0])
+            t2 = _cycle_suffix_t(self.grid)
         else:
             q2 = self.quaternions[idx + 2]
             t2 = self.grid[idx + 2]
         slerp_0_1 = slerp(q0, q1, (t - t0) / (t1 - t0))
         return slerp(
             slerp(
                 slerp(q_1, q0, (t - t_1) / (t0 - t_1)),
                 slerp_0_1,
                 (t - t_1) / (t1 - t_1)),
             slerp(
                 slerp_0_1,
                 slerp(q1, q2, (t - t1) / (t2 - t1)),
                 (t - t0) / (t2 - t0)),
             (t - t0) / (t1 - t0))
+
+
+def _cycle_prefix(quaternions):
+    prefix = quaternions[-2]
+    if prefix.dot(quaternions[0]) < 0:
+        prefix = -prefix
+    return prefix
+
+
+def _cycle_prefix_t(grid):
+    return grid[0] - (grid[-1] - grid[-2])
+
+
+def _cycle_suffix(quaternions):
+    suffix = quaternions[1]
+    if quaternions[-1].dot(suffix) < 0:
+        suffix = -suffix
+    return suffix
+
+
+def _cycle_suffix_t(grid):
+    return grid[-1] + (grid[1] - grid[0])
+
+
+class Squad:
+    """Spherical Quadrangle Interpolation, see __init__()."""
+
+    def __init__(self, quaternions, grid=None, *, alpha=None):
+        """Spherical Quadrangle Interpolation.
+
+        Always closed (for now).
+
+        See :ref:`/rotation/squad.ipynb`.
+
+        """
+        self.quaternions = _check_quaternions(quaternions, closed=True)
+        self.grid = list(_check_grid(grid, alpha, self.quaternions))
+        qs = (
+            _cycle_prefix(self.quaternions),
+            *self.quaternions,
+            _cycle_suffix(self.quaternions),
+        )
+        ts = (
+            _cycle_prefix_t(self.grid),
+            *self.grid,
+            _cycle_suffix_t(self.grid),
+        )
+        control_points = []
+
+        triples = [zip(arg, arg[1:], arg[2:]) for arg in (qs, ts)]
+        for (q_1, q0, q1), (t_1, t0, t1) in zip(*triples):
+            control_points.extend([
+                UnitQuaternion.exp_map(
+                    - (t1 - t0) / (2 * (t1 - t_1)) * (
+                        q0.rotation_to(q1).log_map() +
+                        (t1 - t0) * q0.rotation_to(q_1).log_map() / (t0 - t_1)
+                    )
+                ) * q0,
+                q0,
+                q0,
+                UnitQuaternion.exp_map(
+                    - (t0 - t_1) / (2 * (t1 - t_1)) * (
+                        (t0 - t_1) * q0.rotation_to(q1).log_map() / (t1 - t0) +
+                        q0.rotation_to(q_1).log_map()
+                    )
+                ) * q0,
+            ])
+        del control_points[:2]
+        self.segments = [
+            control_points[i:i + 4]
+            for i in range(0, len(control_points), 4)
+        ]
+
+    def evaluate(self, t):
+        """Get value at the given parameter value(s) *t*."""
+        if not _np.isscalar(t):
+            return _np.array([self.evaluate(t) for t in t])
+        idx = _check_param('t', t, self.grid)
+        q0, s0, s1, q1 = self.segments[idx]
+        t0, t1 = self.grid[idx:idx + 2]
+        t = (t - t0) / (t1 - t0)
+        return slerp(slerp(q0, q1, t), slerp(s0, s1, t), 2 * t * (1 - t))
```

### Comparing `splines-0.2.0/src/splines.egg-info/PKG-INFO` & `splines-0.3.0/src/splines.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 Metadata-Version: 2.1
 Name: splines
-Version: 0.2.0
+Version: 0.3.0
 Summary: Splines in Euclidean Space and Beyond
-Home-page: UNKNOWN
+Home-page: https://splines.readthedocs.io/
 Author: Matthias Geier
 Author-email: Matthias.Geier@gmail.com
 License: MIT
 Project-URL: Documentation, https://splines.readthedocs.io/
 Project-URL: Source Code, https://github.com/AudioSceneDescriptionFormat/splines/
 Project-URL: Bug Tracker, https://github.com/AudioSceneDescriptionFormat/splines/issues/
 Keywords: splines,curves,interpolation,quaternions
 Platform: any
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE
 
 Splines in Euclidean Space and Beyond
 =====================================
 
 ... with focus on univariate, non-uniform piecewise cubic polynomial curves
 in one, two and three spatial dimensions, as well as rotation splines.
 
 Installation
-    ``python3 -m pip install splines``
+    ``python -m pip install splines``
 
 Online documentation
     https://splines.readthedocs.io/
 
 Documentation notebooks on Binder
-    https://mybinder.org/v2/gh/AudioSceneDescriptionFormat/splines/master?filepath=doc/index.ipynb
+    https://mybinder.org/v2/gh/AudioSceneDescriptionFormat/splines/master?labpath=doc/index.ipynb
 
 Source code repository (and issue tracker)
     https://github.com/AudioSceneDescriptionFormat/splines
 
 License
     MIT -- see the file ``LICENSE`` for details.
 
-
-
```

### Comparing `splines-0.2.0/src/splines.egg-info/SOURCES.txt` & `splines-0.3.0/src/splines.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,82 +1,74 @@
-.editorconfig
-.gitignore
-.readthedocs.yml
 LICENSE
 MANIFEST.in
 README.rst
-autobuild.sh
-setup.cfg
+pyproject.toml
 setup.py
-.binder/README
-.binder/apt.txt
-.binder/postBuild
-.binder/requirements.txt
-.github/workflows/docs.yml
-.github/workflows/tests.yml
 doc/conf.py
-doc/favicon.svg
+doc/how-to-navigate.rst
 doc/index.ipynb
-doc/ipython_kernel_config.py
+doc/intro.rst
 doc/python-module.rst
-doc/references.bib
 doc/references.rst
 doc/requirements.txt
+doc/_templates/autosummary/module.rst
 doc/euclidean/barry_goldman.py
 doc/euclidean/bezier-de-casteljau.ipynb
 doc/euclidean/bezier-non-uniform.ipynb
 doc/euclidean/bezier-properties.ipynb
 doc/euclidean/bezier.ipynb
 doc/euclidean/casteljau.py
 doc/euclidean/catmull-rom-barry-goldman.ipynb
 doc/euclidean/catmull-rom-non-uniform.ipynb
 doc/euclidean/catmull-rom-properties.ipynb
 doc/euclidean/catmull-rom-uniform.ipynb
 doc/euclidean/catmull-rom.ipynb
 doc/euclidean/catmull_rom.py
 doc/euclidean/end-conditions-natural.ipynb
-doc/euclidean/end-conditions.ipynb
+doc/euclidean/end-conditions.rst
 doc/euclidean/helper.py
 doc/euclidean/hermite-non-uniform.ipynb
 doc/euclidean/hermite-properties.ipynb
 doc/euclidean/hermite-uniform.ipynb
 doc/euclidean/hermite.ipynb
 doc/euclidean/index.ipynb
-doc/euclidean/ipython_kernel_config.py
 doc/euclidean/kochanek-bartels-non-uniform.ipynb
 doc/euclidean/kochanek-bartels-properties.ipynb
 doc/euclidean/kochanek-bartels-uniform.ipynb
 doc/euclidean/kochanek-bartels.ipynb
+doc/euclidean/kochanek_bartels.py
 doc/euclidean/lagrange.ipynb
 doc/euclidean/natural-non-uniform.ipynb
 doc/euclidean/natural-properties.ipynb
 doc/euclidean/natural-uniform.ipynb
 doc/euclidean/natural.ipynb
 doc/euclidean/piecewise-monotone.ipynb
 doc/euclidean/polynomials.ipynb
+doc/euclidean/quadrangle.ipynb
+doc/euclidean/re-parameterization.ipynb
+doc/euclidean/splines.rst
 doc/euclidean/utility.py
 doc/python-module/splines.quaternion.rst
 doc/python-module/splines.rst
 doc/rotation/barry-goldman.ipynb
 doc/rotation/catmull-rom-non-uniform.ipynb
 doc/rotation/catmull-rom-uniform.ipynb
 doc/rotation/cumulative-form.ipynb
 doc/rotation/de-casteljau.ipynb
 doc/rotation/end-conditions-natural.ipynb
 doc/rotation/helper.py
 doc/rotation/index.ipynb
-doc/rotation/ipython_kernel_config.py
 doc/rotation/kochanek-bartels.ipynb
 doc/rotation/naive-4d-interpolation.ipynb
 doc/rotation/naive-euler-angles-interpolation.ipynb
 doc/rotation/quaternions.ipynb
 doc/rotation/slerp.ipynb
+doc/rotation/squad.ipynb
 src/splines/__init__.py
 src/splines/quaternion.py
 src/splines.egg-info/PKG-INFO
 src/splines.egg-info/SOURCES.txt
 src/splines.egg-info/dependency_links.txt
 src/splines.egg-info/requires.txt
 src/splines.egg-info/top_level.txt
 src/splines.egg-info/zip-safe
-tests/requirements.txt
 tests/test_catmullrom.py
```

