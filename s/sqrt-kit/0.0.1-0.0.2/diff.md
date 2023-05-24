# Comparing `tmp/sqrt-kit-0.0.1.tar.gz` & `tmp/sqrt-kit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqrt-kit-0.0.1.tar", last modified: Wed May 24 12:21:13 2023, max compression
+gzip compressed data, was "sqrt-kit-0.0.2.tar", last modified: Wed May 24 12:23:07 2023, max compression
```

## Comparing `sqrt-kit-0.0.1.tar` & `sqrt-kit-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 12:21:13.139632 sqrt-kit-0.0.1/
--rw-rw-rw-   0        0        0      109 2023-05-24 12:21:13.138631 sqrt-kit-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-24 12:21:13.140632 sqrt-kit-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      249 2023-05-24 12:20:00.000000 sqrt-kit-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 12:21:13.126620 sqrt-kit-0.0.1/sqrt-kit/
--rw-rw-rw-   0        0        0        0 2023-05-24 12:20:28.000000 sqrt-kit-0.0.1/sqrt-kit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 12:21:13.135628 sqrt-kit-0.0.1/sqrt_kit.egg-info/
--rw-rw-rw-   0        0        0      109 2023-05-24 12:21:12.000000 sqrt-kit-0.0.1/sqrt_kit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-05-24 12:21:12.000000 sqrt-kit-0.0.1/sqrt_kit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 12:21:12.000000 sqrt-kit-0.0.1/sqrt_kit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-24 12:21:12.000000 sqrt-kit-0.0.1/sqrt_kit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 12:23:07.064882 sqrt-kit-0.0.2/
+-rw-rw-rw-   0        0        0      109 2023-05-24 12:23:07.063881 sqrt-kit-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-24 12:23:07.065884 sqrt-kit-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      249 2023-05-24 12:22:53.000000 sqrt-kit-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:23:07.049869 sqrt-kit-0.0.2/sqrt-kit/
+-rw-rw-rw-   0        0        0        0 2023-05-24 12:20:28.000000 sqrt-kit-0.0.2/sqrt-kit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:23:07.061879 sqrt-kit-0.0.2/sqrt_kit.egg-info/
+-rw-rw-rw-   0        0        0      109 2023-05-24 12:23:06.000000 sqrt-kit-0.0.2/sqrt_kit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-05-24 12:23:06.000000 sqrt-kit-0.0.2/sqrt_kit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 12:23:06.000000 sqrt-kit-0.0.2/sqrt_kit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-24 12:23:06.000000 sqrt-kit-0.0.2/sqrt_kit.egg-info/top_level.txt
```

