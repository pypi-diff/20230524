# Comparing `tmp/pygeoshader-0.1.0a0.tar.gz` & `tmp/pygeoshader-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeoshader-0.1.0a0.tar", max compression
+gzip compressed data, was "pygeoshader-0.1.0a1.tar", max compression
```

## Comparing `pygeoshader-0.1.0a0.tar` & `pygeoshader-0.1.0a1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-05-23 08:56:50.297579 pygeoshader-0.1.0a0/LICENSE
--rw-r--r--   0        0        0       41 2023-05-23 08:56:50.297749 pygeoshader-0.1.0a0/README.md
--rw-r--r--   0        0        0       37 2023-05-23 22:44:26.289340 pygeoshader-0.1.0a0/pygeoshader/__init__.py
--rw-r--r--   0        0        0      444 2023-05-23 22:44:26.289614 pygeoshader-0.1.0a0/pygeoshader/load_raster.py
--rw-r--r--   0        0        0      541 2023-05-23 22:44:26.540848 pygeoshader-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 pygeoshader-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-24 14:11:48.469966 pygeoshader-0.1.0a1/LICENSE
+-rw-r--r--   0        0        0      974 2023-05-24 14:11:48.469966 pygeoshader-0.1.0a1/README.md
+-rw-r--r--   0        0        0      836 2023-05-24 14:11:48.469966 pygeoshader-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-05-24 14:11:48.469966 pygeoshader-0.1.0a1/src/pygeoshader/__init__.py
+-rw-r--r--   0        0        0      449 2023-05-24 14:11:48.469966 pygeoshader-0.1.0a1/src/pygeoshader/load_raster.py
+-rw-r--r--   0        0        0     1404 1970-01-01 00:00:00.000000 pygeoshader-0.1.0a1/PKG-INFO
```

### Comparing `pygeoshader-0.1.0a0/LICENSE` & `pygeoshader-0.1.0a1/LICENSE`

 * *Files identical despite different names*

