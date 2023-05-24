# Comparing `tmp/xgh_say_hello-0.0.0.tar.gz` & `tmp/xgh_say_hello-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgh_say_hello-0.0.0.tar", last modified: Wed Apr 26 00:56:19 2023, max compression
+gzip compressed data, was "xgh_say_hello-0.0.1.tar", last modified: Wed May 24 01:03:04 2023, max compression
```

## Comparing `xgh_say_hello-0.0.0.tar` & `xgh_say_hello-0.0.1.tar`

### file list

```diff
@@ -1,9 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 00:56:19.137260 xgh_say_hello-0.0.0/
--rw-rw-rw-   0        0        0      196 2023-04-26 00:56:19.137260 xgh_say_hello-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-26 00:56:19.138260 xgh_say_hello-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      220 2023-04-26 00:56:15.000000 xgh_say_hello-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 00:56:19.135259 xgh_say_hello-0.0.0/xgh_say_hello.egg-info/
--rw-rw-rw-   0        0        0      196 2023-04-26 00:56:19.000000 xgh_say_hello-0.0.0/xgh_say_hello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      156 2023-04-26 00:56:19.000000 xgh_say_hello-0.0.0/xgh_say_hello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 00:56:19.000000 xgh_say_hello-0.0.0/xgh_say_hello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 00:56:19.000000 xgh_say_hello-0.0.0/xgh_say_hello.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 01:03:04.019847 xgh_say_hello-0.0.1/
+-rw-rw-rw-   0        0        0      196 2023-05-24 01:03:04.019847 xgh_say_hello-0.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-24 01:03:04.008847 xgh_say_hello-0.0.1/say_hello/
+-rw-rw-rw-   0        0        0        0 2023-05-24 00:56:43.000000 xgh_say_hello-0.0.1/say_hello/__init__.py
+-rw-rw-rw-   0        0        0       87 2023-04-26 00:48:21.000000 xgh_say_hello-0.0.1/say_hello/say_hello.py
+-rw-rw-rw-   0        0        0       42 2023-05-24 01:03:04.019847 xgh_say_hello-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      301 2023-05-24 00:59:58.000000 xgh_say_hello-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 01:03:04.017846 xgh_say_hello-0.0.1/xgh_say_hello.egg-info/
+-rw-rw-rw-   0        0        0      196 2023-05-24 01:03:03.000000 xgh_say_hello-0.0.1/xgh_say_hello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-24 01:03:03.000000 xgh_say_hello-0.0.1/xgh_say_hello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 01:03:03.000000 xgh_say_hello-0.0.1/xgh_say_hello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-24 01:03:03.000000 xgh_say_hello-0.0.1/xgh_say_hello.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2023-05-24 01:03:03.000000 xgh_say_hello-0.0.1/xgh_say_hello.egg-info/top_level.txt
```

