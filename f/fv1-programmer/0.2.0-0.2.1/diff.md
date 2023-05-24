# Comparing `tmp/fv1_programmer-0.2.0.tar.gz` & `tmp/fv1_programmer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fv1_programmer-0.2.0.tar", max compression
+gzip compressed data, was "fv1_programmer-0.2.1.tar", max compression
```

## Comparing `fv1_programmer-0.2.0.tar` & `fv1_programmer-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2023-05-24 01:57:51.370519 fv1_programmer-0.2.0/LICENSE
--rw-r--r--   0        0        0      454 2023-05-24 01:57:51.370519 fv1_programmer-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-05-24 01:57:51.370519 fv1_programmer-0.2.0/adaptor/__init__.py
--rw-r--r--   0        0        0     1140 2023-05-24 01:57:51.370519 fv1_programmer-0.2.0/adaptor/adapter.py
--rw-r--r--   0        0        0     1083 2023-05-24 01:57:51.370519 fv1_programmer-0.2.0/adaptor/mcp2221.py
--rw-r--r--   0        0        0        0 2023-05-24 01:57:51.370519 fv1_programmer-0.2.0/eeprom/__init__.py
--rw-r--r--   0        0        0     5331 2023-05-24 01:57:51.370519 fv1_programmer-0.2.0/eeprom/eeprom.py
--rw-r--r--   0        0        0        0 2023-05-24 01:57:51.370519 fv1_programmer-0.2.0/fv1_programmer/__init__.py
--rw-r--r--   0        0        0     2896 2023-05-24 01:57:51.370519 fv1_programmer-0.2.0/fv1_programmer/main.py
--rw-r--r--   0        0        0     1203 2023-05-24 01:57:51.370519 fv1_programmer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1629 1970-01-01 00:00:00.000000 fv1_programmer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-24 02:08:12.341973 fv1_programmer-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1693 2023-05-24 02:08:12.341973 fv1_programmer-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-24 02:08:12.341973 fv1_programmer-0.2.1/adaptor/__init__.py
+-rw-r--r--   0        0        0     1140 2023-05-24 02:08:12.341973 fv1_programmer-0.2.1/adaptor/adapter.py
+-rw-r--r--   0        0        0     1083 2023-05-24 02:08:12.341973 fv1_programmer-0.2.1/adaptor/mcp2221.py
+-rw-r--r--   0        0        0        0 2023-05-24 02:08:12.341973 fv1_programmer-0.2.1/eeprom/__init__.py
+-rw-r--r--   0        0        0     5331 2023-05-24 02:08:12.341973 fv1_programmer-0.2.1/eeprom/eeprom.py
+-rw-r--r--   0        0        0        0 2023-05-24 02:08:12.341973 fv1_programmer-0.2.1/fv1_programmer/__init__.py
+-rw-r--r--   0        0        0     2896 2023-05-24 02:08:12.341973 fv1_programmer-0.2.1/fv1_programmer/main.py
+-rw-r--r--   0        0        0     1203 2023-05-24 02:08:12.345973 fv1_programmer-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 fv1_programmer-0.2.1/PKG-INFO
```

### Comparing `fv1_programmer-0.2.0/LICENSE` & `fv1_programmer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.0/adaptor/adapter.py` & `fv1_programmer-0.2.1/adaptor/adapter.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.0/adaptor/mcp2221.py` & `fv1_programmer-0.2.1/adaptor/mcp2221.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.0/eeprom/eeprom.py` & `fv1_programmer-0.2.1/eeprom/eeprom.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.0/fv1_programmer/main.py` & `fv1_programmer-0.2.1/fv1_programmer/main.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.0/pyproject.toml` & `fv1_programmer-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fv1-programmer"
-version = "0.2.0"
+version = "0.2.1"
 description = "An EEPROM programming tool for the FV-1 DSP"
 authors = ["Mark Melvin <mark.melvin@audiofab.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
```

