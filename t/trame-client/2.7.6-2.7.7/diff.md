# Comparing `tmp/trame-client-2.7.6.tar.gz` & `tmp/trame-client-2.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-client-2.7.6.tar", last modified: Mon May 15 21:25:18 2023, max compression
+gzip compressed data, was "trame-client-2.7.7.tar", last modified: Mon May 15 23:48:12 2023, max compression
```

## Comparing `trame-client-2.7.6.tar` & `trame-client-2.7.7.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.662747 trame-client-2.7.6/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-05-15 21:24:45.000000 trame-client-2.7.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      234 2023-05-15 21:24:45.000000 trame-client-2.7.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3518 2023-05-15 21:25:18.662747 trame-client-2.7.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2785 2023-05-15 21:24:45.000000 trame-client-2.7.6/README.rst
--rw-r--r--   0 root         (0) root         (0)      842 2023-05-15 21:25:18.662747 trame-client-2.7.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 21:24:45.000000 trame-client-2.7.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.650747 trame-client-2.7.6/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.650747 trame-client-2.7.6/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame/modules/www.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.650747 trame-client-2.7.6/trame/ui/
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame/ui/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.650747 trame-client-2.7.6/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      137 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame/widgets/client.py
--rw-r--r--   0 root         (0) root         (0)       75 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame/widgets/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.650747 trame-client-2.7.6/trame_client/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/LICENSE
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.654747 trame-client-2.7.6/trame_client/encoders/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/encoders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/encoders/numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.654747 trame-client-2.7.6/trame_client/module/
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.654747 trame-client-2.7.6/trame_client/module/vue2-www/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.654747 trame-client-2.7.6/trame_client/module/vue2-www/css/
--rw-r--r--   0 root         (0) root         (0)     1588 2023-05-15 21:25:06.000000 trame-client-2.7.6/trame_client/module/vue2-www/css/app.0b077e70.css
--rw-r--r--   0 root         (0) root         (0)     3963 2023-05-15 21:25:06.000000 trame-client-2.7.6/trame_client/module/vue2-www/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.658747 trame-client-2.7.6/trame_client/module/vue2-www/js/
--rw-r--r--   0 root         (0) root         (0)    23163 2023-05-15 21:25:06.000000 trame-client-2.7.6/trame_client/module/vue2-www/js/app.4ae908a0.js
--rw-r--r--   0 root         (0) root         (0)   169923 2023-05-15 21:25:06.000000 trame-client-2.7.6/trame_client/module/vue2-www/js/chunk-vendors.ec946a94.js
--rw-r--r--   0 root         (0) root         (0)     4506 2023-05-15 21:25:06.000000 trame-client-2.7.6/trame_client/module/vue2-www/logo.png
--rw-r--r--   0 root         (0) root         (0)   107302 2023-05-15 21:25:06.000000 trame-client-2.7.6/trame_client/module/vue2-www/vue.global.js
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/module/vue2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.658747 trame-client-2.7.6/trame_client/module/vue3-www/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.658747 trame-client-2.7.6/trame_client/module/vue3-www/assets/
--rw-r--r--   0 root         (0) root         (0)   107764 2023-05-15 21:25:13.000000 trame-client-2.7.6/trame_client/module/vue3-www/assets/index-e4900adb.js
--rw-r--r--   0 root         (0) root         (0)     3940 2023-05-15 21:25:13.000000 trame-client-2.7.6/trame_client/module/vue3-www/index.html
--rw-r--r--   0 root         (0) root         (0)     4506 2023-05-15 21:25:12.000000 trame-client-2.7.6/trame_client/module/vue3-www/logo.png
--rw-r--r--   0 root         (0) root         (0)   128872 2023-05-15 21:25:12.000000 trame-client-2.7.6/trame_client/module/vue3-www/vue.global.js
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/module/vue3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.658747 trame-client-2.7.6/trame_client/resources/
--rw-r--r--   0 root         (0) root         (0)     7243 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/resources/attributes.json
--rw-r--r--   0 root         (0) root         (0)        2 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/resources/events.json
--rw-r--r--   0 root         (0) root         (0)      580 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/resources/vue.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.662747 trame-client-2.7.6/trame_client/ui/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2301 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/ui/core.py
--rw-r--r--   0 root         (0) root         (0)      575 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/ui/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.662747 trame-client-2.7.6/trame_client/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      205 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/utils/defaults.py
--rw-r--r--   0 root         (0) root         (0)      552 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.662747 trame-client-2.7.6/trame_client/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19678 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/widgets/core.py
--rw-r--r--   0 root         (0) root         (0)     3482 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/widgets/generator.py
--rw-r--r--   0 root         (0) root         (0)   193844 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/widgets/html.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-05-15 21:24:45.000000 trame-client-2.7.6/trame_client/widgets/trame.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:25:18.654747 trame-client-2.7.6/trame_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3518 2023-05-15 21:25:18.000000 trame-client-2.7.6/trame_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1448 2023-05-15 21:25:18.000000 trame-client-2.7.6/trame_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 21:25:18.000000 trame-client-2.7.6/trame_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-15 21:25:18.000000 trame-client-2.7.6/trame_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:48:12.041784 trame-client-2.7.7/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-05-15 23:47:37.000000 trame-client-2.7.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      234 2023-05-15 23:47:37.000000 trame-client-2.7.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-05-15 23:48:12.041784 trame-client-2.7.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-05-15 23:47:37.000000 trame-client-2.7.7/README.rst
+-rw-r--r--   0 root         (0) root         (0)      842 2023-05-15 23:48:12.041784 trame-client-2.7.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 23:47:37.000000 trame-client-2.7.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:48:12.033784 trame-client-2.7.7/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:48:12.033784 trame-client-2.7.7/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame/modules/www.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:48:12.033784 trame-client-2.7.7/trame/ui/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame/ui/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:48:12.033784 trame-client-2.7.7/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      137 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame/widgets/client.py
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame/widgets/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:48:12.033784 trame-client-2.7.7/trame_client/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:48:12.033784 trame-client-2.7.7/trame_client/encoders/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/encoders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/encoders/numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:48:12.033784 trame-client-2.7.7/trame_client/module/
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:48:12.033784 trame-client-2.7.7/trame_client/module/vue2-www/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:48:12.037784 trame-client-2.7.7/trame_client/module/vue2-www/css/
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-05-15 23:47:59.000000 trame-client-2.7.7/trame_client/module/vue2-www/css/app.0b077e70.css
+-rw-r--r--   0 root         (0) root         (0)     3963 2023-05-15 23:47:59.000000 trame-client-2.7.7/trame_client/module/vue2-www/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:48:12.037784 trame-client-2.7.7/trame_client/module/vue2-www/js/
+-rw-r--r--   0 root         (0) root         (0)    23564 2023-05-15 23:47:59.000000 trame-client-2.7.7/trame_client/module/vue2-www/js/app.93852572.js
+-rw-r--r--   0 root         (0) root         (0)   170437 2023-05-15 23:47:59.000000 trame-client-2.7.7/trame_client/module/vue2-www/js/chunk-vendors.b42af71c.js
+-rw-r--r--   0 root         (0) root         (0)     4506 2023-05-15 23:47:59.000000 trame-client-2.7.7/trame_client/module/vue2-www/logo.png
+-rw-r--r--   0 root         (0) root         (0)   107302 2023-05-15 23:47:59.000000 trame-client-2.7.7/trame_client/module/vue2-www/vue.global.js
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/module/vue2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:48:12.037784 trame-client-2.7.7/trame_client/module/vue3-www/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:48:12.037784 trame-client-2.7.7/trame_client/module/vue3-www/assets/
+-rw-r--r--   0 root         (0) root         (0)   108146 2023-05-15 23:48:06.000000 trame-client-2.7.7/trame_client/module/vue3-www/assets/index-ccad3410.js
+-rw-r--r--   0 root         (0) root         (0)     3940 2023-05-15 23:48:06.000000 trame-client-2.7.7/trame_client/module/vue3-www/index.html
+-rw-r--r--   0 root         (0) root         (0)     4506 2023-05-15 23:48:06.000000 trame-client-2.7.7/trame_client/module/vue3-www/logo.png
+-rw-r--r--   0 root         (0) root         (0)   128872 2023-05-15 23:48:06.000000 trame-client-2.7.7/trame_client/module/vue3-www/vue.global.js
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/module/vue3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:48:12.037784 trame-client-2.7.7/trame_client/resources/
+-rw-r--r--   0 root         (0) root         (0)     7243 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/resources/attributes.json
+-rw-r--r--   0 root         (0) root         (0)        2 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/resources/events.json
+-rw-r--r--   0 root         (0) root         (0)      580 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/resources/vue.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:48:12.037784 trame-client-2.7.7/trame_client/ui/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/ui/core.py
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/ui/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:48:12.037784 trame-client-2.7.7/trame_client/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      205 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/utils/defaults.py
+-rw-r--r--   0 root         (0) root         (0)      552 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:48:12.041784 trame-client-2.7.7/trame_client/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19678 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/widgets/core.py
+-rw-r--r--   0 root         (0) root         (0)     3482 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/widgets/generator.py
+-rw-r--r--   0 root         (0) root         (0)   193844 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/widgets/html.py
+-rw-r--r--   0 root         (0) root         (0)     4670 2023-05-15 23:47:37.000000 trame-client-2.7.7/trame_client/widgets/trame.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:48:12.033784 trame-client-2.7.7/trame_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-05-15 23:48:12.000000 trame-client-2.7.7/trame_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-05-15 23:48:12.000000 trame-client-2.7.7/trame_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 23:48:12.000000 trame-client-2.7.7/trame_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-15 23:48:12.000000 trame-client-2.7.7/trame_client.egg-info/top_level.txt
```

### Comparing `trame-client-2.7.6/LICENSE` & `trame-client-2.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.6/PKG-INFO` & `trame-client-2.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-client
-Version: 2.7.6
+Version: 2.7.7
 Summary: Internal client of trame
 Author: Kitware Inc.
 License: MIT
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-client-2.7.6/README.rst` & `trame-client-2.7.7/README.rst`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.6/setup.cfg` & `trame-client-2.7.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-client
-version = 2.7.6
+version = 2.7.7
 description = Internal client of trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = MIT
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-client-2.7.6/trame_client/LICENSE` & `trame-client-2.7.7/trame_client/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.6/trame_client/encoders/numpy.py` & `trame-client-2.7.7/trame_client/encoders/numpy.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.6/trame_client/module/vue2-www/css/app.0b077e70.css` & `trame-client-2.7.7/trame_client/module/vue2-www/css/app.0b077e70.css`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.6/trame_client/module/vue2-www/index.html` & `trame-client-2.7.7/trame_client/module/vue2-www/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -78,8 +78,8 @@
           transform: rotate(0deg); /* Firefox 16+, IE 10+, Opera */
         }
         100% {
           -webkit-transform: rotate(360deg); /* Chrome, Opera 15+, Safari 3.1+ */
           -ms-transform: rotate(360deg); /* IE 9 */
           transform: rotate(360deg); /* Firefox 16+, IE 10+, Opera */
         }
-      }</style><script defer="defer" src="js/chunk-vendors.ec946a94.js"></script><script defer="defer" src="js/app.4ae908a0.js"></script><link href="css/app.0b077e70.css" rel="stylesheet"></head><body style="margin: 0; padding: 0;"><noscript><strong>We're sorry but trame built by Kitware doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript><div id="app"><div style="position:absolute;top:0;left:0;width:100%;height:100%;z-index:1000;"><div class="trame__loader"></div><div class="trame__message">Loading...</div></div></div></body></html>
+      }</style><script defer="defer" src="js/chunk-vendors.b42af71c.js"></script><script defer="defer" src="js/app.93852572.js"></script><link href="css/app.0b077e70.css" rel="stylesheet"></head><body style="margin: 0; padding: 0;"><noscript><strong>We're sorry but trame built by Kitware doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript><div id="app"><div style="position:absolute;top:0;left:0;width:100%;height:100%;z-index:1000;"><div class="trame__loader"></div><div class="trame__message">Loading...</div></div></div></body></html>
```

### Comparing `trame-client-2.7.6/trame_client/module/vue2-www/js/app.4ae908a0.js` & `trame-client-2.7.7/trame_client/module/vue2-www/js/app.93852572.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -175,15 +175,15 @@
                     return t.priority - e.priority
                 }
 
                 function O(t) {
                     L.addAttachement = t
                 }
                 const A = 2e6,
-                    j = {
+                    k = {
                         priority: 0,
                         async decorate(t) {
                             if (null === t || void 0 === t) return t;
                             if (t.constructor && t.constructor === File) {
                                 const {
                                     name: e,
                                     lastModified: n,
@@ -211,22 +211,22 @@
                                     content: a,
                                     _filter: ["content"]
                                 }
                             }
                             return t
                         }
                     },
-                    k = {
+                    j = {
                         priority: 0,
                         async decorate(t) {
                             if (null === t || void 0 === t) return t;
                             if ("string" === typeof t) return t;
                             if (t.constructor && t.constructor === FileList || t.length) {
                                 const e = [];
-                                for (let n = 0; n < t.length; n++) e.push(await j.decorate(t[n]));
+                                for (let n = 0; n < t.length; n++) e.push(await k.decorate(t[n]));
                                 return e
                             }
                             return t
                         }
                     },
                     U = {
                         priority: 0,
@@ -234,46 +234,46 @@
                             if (null === t || void 0 === t) return t;
                             if ("string" === typeof t) return t;
                             if (t.constructor && t.constructor === Object) {
                                 const e = {},
                                     n = Object.keys(t);
                                 for (let s = 0; s < n.length; s++) {
                                     const r = n[s];
-                                    e[r] = t[r], e[r] = await k.decorate(e[r]), e[r] = await j.decorate(e[r])
+                                    e[r] = t[r], e[r] = await j.decorate(e[r]), e[r] = await k.decorate(e[r])
                                 }
                                 return e
                             }
                             return t
                         }
                     },
-                    E = [j, k, U];
+                    N = [k, j, U];
 
-                function Z(t) {
-                    E.push(t), E.sort(x)
+                function E(t) {
+                    N.push(t), N.sort(x)
                 }
                 async function V(t) {
                     let e = t;
-                    for (let n = 0; n < E.length; n++) {
+                    for (let n = 0; n < N.length; n++) {
                         if (null === e || void 0 === e) return e;
-                        e = await E[n].decorate(e)
+                        e = await N[n].decorate(e)
                     }
                     return e
                 }
-                const I = ["type", "key", "keyCode", "controlKey", "altKey", "shiftKey", "position", "spinX", "spinY", "pixelX", "pixelY"];
+                const Z = ["type", "key", "keyCode", "controlKey", "altKey", "shiftKey", "position", "spinX", "spinY", "pixelX", "pixelY"];
 
-                function N(t) {
+                function I(t) {
                     const e = {};
-                    for (let n = 0; n < I.length; n++) {
-                        const s = I[n];
+                    for (let n = 0; n < Z.length; n++) {
+                        const s = Z[n];
                         s in t && (e[s] = t[s])
                     }
                     return e
                 }
                 var P = {
-                    event: N
+                    event: I
                 };
                 n(6977);
 
                 function B(t, e = [], n = 1e3, s = 2) {
                     if (null === t) return null;
                     for (let r = 0; r < e.length; r++) {
                         const i = Array.isArray(n) ? n[r] : n,
@@ -323,43 +323,43 @@
                         } catch (s) {
                             continue
                         }
                     }
                     return e
                 }
 
-                function q(t, e, n) {
+                function J(t, e, n) {
                     const s = {
                             id: t
                         },
                         r = e ? `${e}: ` : "";
                     return Array.isArray(n) ? (s.name = `${r}[]`, n.length && (s.children = []), s) : null !== n && n ? "function" === typeof n ? (s.name = `${r}function`, s) : "object" === typeof n ? (s.name = `${r}{}`, Object.keys(n).length && (s.children = []), s) : (s.name = `${r}${n}`, s) : (s.name = `${r}${n}`, s)
                 }
 
-                function z(t, e, n, s) {
-                    const r = q(e, n, s);
-                    t.push(r), r.children && J(e, r.children, s)
+                function q(t, e, n, s) {
+                    const r = J(e, n, s);
+                    t.push(r), r.children && z(e, r.children, s)
                 }
 
-                function J(t, e, n) {
+                function z(t, e, n) {
                     if (Array.isArray(n)) {
                         const s = null;
-                        for (let r = 0; r < n.length; r++) z(e, `${t}_${r}`, s, n[r])
+                        for (let r = 0; r < n.length; r++) q(e, `${t}_${r}`, s, n[r])
                     } else {
                         const s = Object.keys(n);
                         for (let r = 0; r < s.length; r++) {
                             const i = s[r];
-                            z(e, `${t}_${r}`, i, n[i])
+                            q(e, `${t}_${r}`, i, n[i])
                         }
                     }
                 }
 
                 function G(t) {
                     const e = [];
-                    return J("", e, t), e
+                    return z("", e, t), e
                 }
                 var X = {
                     download: M,
                     get: K,
                     safe: F,
                     tree: G,
                     vtk: P,
@@ -435,15 +435,15 @@
                         }, s)) : console.error(`Lookup error: Vue.use(${e}, ${JSON.stringify(s)})`)
                     })), t.includes("trame__favicon") && e.trame__favicon && (document.querySelector("link[rel=icon]").href = e.trame__favicon), t.includes("trame__title") && e.trame__title && (document.title = e.trame__title)
                 }
                 class it {
                     constructor(t, e = null, n = []) {
                         this.name = "Default trame application", this.vueInstance = t, this.client = (null === t || void 0 === t ? void 0 : t.client) || e, this.exclude = (null === t || void 0 === t ? void 0 : t.exclude) || n, this.subscriptions = [], this.state = {}, this.keyTS = {}, this.ts = 0, this.trameTemplateTS = 0, this.trameTemplate = {
                             template: "<div>Too early for trame template</div>"
-                        }, this.dirtyKeys = new Set, this.registerDecorator = Z;
+                        }, this.dirtyKeys = new Set, this.registerDecorator = E;
                         const s = async t => {
                             const e = [],
                                 n = Object.keys(t);
                             for (let a = 0; a < n.length; a++) {
                                 var s;
                                 let r = !0;
                                 const i = n[a],
@@ -877,15 +877,15 @@
                         }, [e("path", {
                             attrs: {
                                 d: "M4,1C2.89,1 2,1.89 2,3V7C2,8.11 2.89,9 4,9H1V11H13V9H10C11.11,9 12,8.11 12,7V3C12,1.89 11.11,1 10,1H4M4,3H10V7H4V3M14,13C12.89,13 12,13.89 12,15V19C12,20.11 12.89,21 14,21H11V23H23V21H20C21.11,21 22,20.11 22,19V15C22,13.89 21.11,13 20,13H14M3.88,13.46L2.46,14.88L4.59,17L2.46,19.12L3.88,20.54L6,18.41L8.12,20.54L9.54,19.12L7.41,17L9.54,14.88L8.12,13.46L6,15.59L3.88,13.46M14,15H20V19H14V15Z"
                             }
                         })]), t._v(" " + t._s(t.message) + " ")])])])
                     },
                     At = [],
-                    jt = {
+                    kt = {
                         name: "Reconnect",
                         props: {
                             message: {
                                 type: String,
                                 default: "Click to reconnect..."
                             },
                             maxRetry: {
@@ -914,32 +914,32 @@
                             }), this.delay)))
                         },
                         beforeDestroy() {
                             this.resetRetry()
                         },
                         inject: ["trame"]
                     },
-                    kt = jt,
+                    jt = kt,
                     Ut = {
                         container: "style_container_n4xKQ",
                         center: "style_center_xzh58",
                         button: "style_button_kGhdk"
                     };
 
-                function Et(t) {
+                function Nt(t) {
                     this["$style"] = Ut.locals || Ut
                 }
-                var Zt = (0, lt.Z)(kt, Ot, At, !1, Et, null, null),
-                    Vt = Zt.exports,
-                    It = function() {
+                var Et = (0, lt.Z)(jt, Ot, At, !1, Nt, null, null),
+                    Vt = Et.exports,
+                    Zt = function() {
                         var t = this;
                         t._self._c;
                         return t._t("default", null, null, t.state)
                     },
-                    Nt = [];
+                    It = [];
 
                 function Pt(...t) {
                     const e = {};
                     for (let n = 0; n < t.length; n++) e[t[n]] = null;
                     return e
                 }
 
@@ -988,36 +988,36 @@
                         provide() {
                             return {
                                 state: this
                             }
                         }
                     },
                     Ht = Dt,
-                    Mt = (0, lt.Z)(Ht, It, Nt, !1, null, null, null),
+                    Mt = (0, lt.Z)(Ht, Zt, It, !1, null, null, null),
                     Kt = Mt.exports;
                 let Ft = 1;
 
-                function qt() {
+                function Jt() {
                     return "trame_style_elem_" + Ft++
                 }
-                var zt, Jt, Gt = {
+                var qt, zt, Gt = {
                         name: "TrameStyle",
                         props: {
                             css: {
                                 type: String,
                                 default: ""
                             }
                         },
                         watch: {
                             css(t) {
                                 this.updateStyle(t)
                             }
                         },
                         created() {
-                            this.elemId = qt(), this.updateStyle(this.css)
+                            this.elemId = Jt(), this.updateStyle(this.css)
                         },
                         beforeDestroy() {
                             this.removeStyle()
                         },
                         methods: {
                             updateStyle(t) {
                                 let e = document.querySelector(`#${this.elemId}`);
@@ -1026,51 +1026,68 @@
                             removeStyle() {
                                 const t = document.querySelector(`#${this.elemId}`);
                                 t && t.parentNode.removeChild(t)
                             }
                         }
                     },
                     Xt = Gt,
-                    Yt = (0, lt.Z)(Xt, zt, Jt, !1, null, null, null),
+                    Yt = (0, lt.Z)(Xt, qt, zt, !1, null, null, null),
                     Qt = Yt.exports,
                     Wt = {
                         name: "TrameExec",
                         props: ["event"],
                         methods: {
                             exec(t) {
                                 void 0 === t ? this.$emit("exec", this.event) : this.$emit("exec", t)
                             }
                         }
                     };
+                n(2262), n(4506);
                 const {
                     inject: te,
                     ref: ee,
                     onBeforeMount: ne,
                     onBeforeUnmount: se,
                     watch: re
                 } = window.Vue;
                 var ie = {
                         props: ["name"],
                         setup(t) {
                             const e = te("trame"),
-                                n = ee(null);
+                                n = ee(null),
+                                s = ee(null);
+
+                            function r(n, s) {
+                                const r = JSON.parse(JSON.stringify(e.state.get(t.name)));
+                                let i = r;
+                                const a = String(n).split(".");
+                                for (let t = 0; t < a.length - 1; t++) i = i[a[t]];
+                                i[a.at(-1)] = s, e.state.set(t.name, r)
+                            }
+
+                            function i(n) {
+                                e.state.set(t.name, n)
+                            }
 
-                            function s() {
-                                const s = e.state.get(t.name);
-                                s !== n.value && (n.value = s)
+                            function a() {
+                                const r = e.state.get(t.name);
+                                s.value !== t.name && (s.value = t.name), r !== n.value && (n.value = r)
                             }
-                            return re((() => t.name), s), ne((() => {
-                                e.$on("stateChange", s), s()
+                            return re((() => t.name), a), ne((() => {
+                                e.$on("stateChange", a), a()
                             })), se((() => {
-                                e.$off("stateChange", s)
+                                e.$off("stateChange", a)
                             })), {
-                                computed: n
+                                computedValue: n,
+                                computedName: s,
+                                updateNested: r,
+                                update: i
                             }
                         },
-                        template: '<slot :value="computed"></slot>'
+                        template: '<slot :keyName="computedName" :update="update" :updateNested="updateNested" :value="computedValue"></slot>'
                     },
                     ae = {
                         TrameApp: wt,
                         TrameConnect: ut,
                         TrameLoading: xt,
                         TrameReconnect: Vt,
                         TrameTemplate: yt,
@@ -1209,8 +1226,8 @@
             s.forEach(e.bind(null, 0)), s.push = e.bind(null, s.push.bind(s))
         }();
     var s = n.O(void 0, [998], (function() {
         return n(4031)
     }));
     s = n.O(s)
 })();
-//# sourceMappingURL=app.4ae908a0.js.map
+//# sourceMappingURL=app.93852572.js.map
```

### Comparing `trame-client-2.7.6/trame_client/module/vue2-www/js/chunk-vendors.ec946a94.js` & `trame-client-2.7.7/trame_client/module/vue2-www/js/chunk-vendors.b42af71c.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -133,16 +133,16 @@
                     var r = [null];
                     r.push.apply(r, t);
                     var u = Function.bind.apply(e, r),
                         o = new u;
                     return n && p(o, n.prototype), o
                 }, h.apply(null, arguments)
             }
-            var d = n(4063),
-                v = n.n(d),
+            var v = n(4063),
+                d = n.n(v),
                 y = n(2503),
                 g = n.n(y);
 
             function m(e, t) {
                 var n = Object.keys(e);
                 if (Object.getOwnPropertySymbols) {
                     var r = Object.getOwnPropertySymbols(e);
@@ -464,23 +464,23 @@
                 return e && e.isA ? e.getState() : e
             }
 
             function he(e) {
                 setTimeout(e, 0)
             }
 
-            function de(e, t) {
+            function ve(e, t) {
                 var n = performance.now();
                 e.finally((function() {
                     var e = performance.now() - n;
                     t(e)
                 }))
             }
 
-            function ve() {
+            function de() {
                 var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {},
                     t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                 fe(t);
                 var n = [];
                 if (Number.isInteger(t.mtime) || (t.mtime = ++$), "classHierarchy" in t) {
                     if (!(t.classHierarchy instanceof L)) {
                         for (var r = new L, u = 0; u < t.classHierarchy.length; u++) r.push(t.classHierarchy[u]);
@@ -606,15 +606,15 @@
                             return !1
                         }
                         throw Y("Set Enum with invalid argument (String/Number) ".concat(n, ", ").concat(r)), new TypeError("Set Enum with invalid argument (String/Number)")
                     }
                 },
                 object: function(e, t, n) {
                     return function(r) {
-                        return !v()(t[n.name], r) && (t[n.name] = r, e.modified(), !0)
+                        return !d()(t[n.name], r) && (t[n.name] = r, e.modified(), !0)
                     }
                 }
             };
 
             function Ae(e) {
                 if ("object" === u(e)) {
                     var t = me[e.type];
@@ -1189,21 +1189,21 @@
                 formatNumbersWithThousandSeparator: se,
                 get: ge,
                 getArray: Fe,
                 getCurrentGlobalMTime: z,
                 getStateArrayMapFunc: De,
                 isVtkObject: ke,
                 keystore: Ue,
-                measurePromiseExecution: de,
+                measurePromiseExecution: ve,
                 moveToProtected: Be,
                 newInstance: Pe,
                 newTypedArray: re,
                 newTypedArrayFrom: ue,
                 normalizeWheel: Ge,
-                obj: ve,
+                obj: de,
                 proxy: Me,
                 proxyPropertyMapping: _e,
                 proxyPropertyState: $e,
                 safeArrays: fe,
                 set: Ce,
                 setArray: be,
                 setGet: Ee,
@@ -1663,23 +1663,23 @@
                 l = n(4121),
                 p = n(1246),
                 D = Array;
             e.exports = function(e) {
                 var t = o(e),
                     n = c(this),
                     h = arguments.length,
-                    d = h > 1 ? arguments[1] : void 0,
-                    v = void 0 !== d;
-                v && (d = r(d, h > 2 ? arguments[2] : void 0));
+                    v = h > 1 ? arguments[1] : void 0,
+                    d = void 0 !== v;
+                d && (v = r(v, h > 2 ? arguments[2] : void 0));
                 var y, g, m, A, C, E, F = p(t),
                     b = 0;
                 if (!F || this === D && a(F))
-                    for (y = s(t), g = n ? new this(y) : D(y); y > b; b++) E = v ? d(t[b], b) : t[b], f(g, b, E);
+                    for (y = s(t), g = n ? new this(y) : D(y); y > b; b++) E = d ? v(t[b], b) : t[b], f(g, b, E);
                 else
-                    for (A = l(t, F), C = A.next, g = n ? new this : []; !(m = u(C, A)).done; b++) E = v ? i(A, d, [m.value, b], !0) : m.value, f(g, b, E);
+                    for (A = l(t, F), C = A.next, g = n ? new this : []; !(m = u(C, A)).done; b++) E = d ? i(A, v, [m.value, b], !0) : m.value, f(g, b, E);
                 return g.length = b, g
             }
         },
         1318: function(e, t, n) {
             var r = n(5656),
                 u = n(1400),
                 o = n(6244),
@@ -2163,20 +2163,20 @@
                 u = n(1236).f,
                 o = n(8880),
                 i = n(8052),
                 a = n(3072),
                 c = n(9920),
                 s = n(4705);
             e.exports = function(e, t) {
-                var n, f, l, p, D, h, d = e.target,
-                    v = e.global,
+                var n, f, l, p, D, h, v = e.target,
+                    d = e.global,
                     y = e.stat;
-                if (f = v ? r : y ? r[d] || a(d, {}) : (r[d] || {}).prototype, f)
+                if (f = d ? r : y ? r[v] || a(v, {}) : (r[v] || {}).prototype, f)
                     for (l in t) {
-                        if (D = t[l], e.dontCallGetSet ? (h = u(f, l), p = h && h.value) : p = f[l], n = s(v ? l : d + (y ? "." : "#") + l, e.forced), !n && void 0 !== p) {
+                        if (D = t[l], e.dontCallGetSet ? (h = u(f, l), p = h && h.value) : p = f[l], n = s(d ? l : v + (y ? "." : "#") + l, e.forced), !n && void 0 !== p) {
                             if (typeof D == typeof p) continue;
                             c(D, p)
                         }(e.sham || p && p.sham) && o(D, "sham", !0), i(f, l, D, e)
                     }
             }
         },
         7293: function(e) {
@@ -2213,29 +2213,29 @@
                         return "split" === e && (n = {}, n.constructor = {}, n.constructor[s] = function() {
                             return n
                         }, n.flags = "", n[p] = /./ [p]), n.exec = function() {
                             return t = !0, null
                         }, n[p](""), !t
                     }));
                 if (!D || !h || n) {
-                    var d = r(/./ [p]),
-                        v = t(p, "" [e], (function(e, t, n, u, i) {
+                    var v = r(/./ [p]),
+                        d = t(p, "" [e], (function(e, t, n, u, i) {
                             var a = r(e),
                                 c = t.exec;
                             return c === o || c === f.exec ? D && !i ? {
                                 done: !0,
-                                value: d(t, n, u)
+                                value: v(t, n, u)
                             } : {
                                 done: !0,
                                 value: a(n, t, u)
                             } : {
                                 done: !1
                             }
                         }));
-                    u(String.prototype, e, v[0]), u(f, p, v[1])
+                    u(String.prototype, e, d[0]), u(f, p, d[1])
                 }
                 l && c(f[p], "sham", !0)
             }
         },
         2104: function(e, t, n) {
             var r = n(4374),
                 u = Function.prototype,
@@ -2386,16 +2386,16 @@
                 a = r("".replace),
                 c = r("".slice),
                 s = /\$([$&'`]|\d{1,2}|<[^>]*>)/g,
                 f = /\$([$&'`]|\d{1,2})/g;
             e.exports = function(e, t, n, r, l, p) {
                 var D = n + e.length,
                     h = r.length,
-                    d = f;
-                return void 0 !== l && (l = u(l), d = s), a(p, d, (function(u, a) {
+                    v = f;
+                return void 0 !== l && (l = u(l), v = s), a(p, v, (function(u, a) {
                     var s;
                     switch (i(a, 0)) {
                         case "$":
                             return "$";
                         case "&":
                             return e;
                         case "`":
@@ -2503,40 +2503,40 @@
                 c = n(111),
                 s = n(8880),
                 f = n(2597),
                 l = n(5465),
                 p = n(6200),
                 D = n(3501),
                 h = "Object already initialized",
-                d = a.TypeError,
-                v = a.WeakMap,
+                v = a.TypeError,
+                d = a.WeakMap,
                 y = function(e) {
                     return o(e) ? u(e) : r(e, {})
                 },
                 g = function(e) {
                     return function(t) {
                         var n;
-                        if (!c(t) || (n = u(t)).type !== e) throw d("Incompatible receiver, " + e + " required");
+                        if (!c(t) || (n = u(t)).type !== e) throw v("Incompatible receiver, " + e + " required");
                         return n
                     }
                 };
             if (i || l.state) {
-                var m = l.state || (l.state = new v);
+                var m = l.state || (l.state = new d);
                 m.get = m.get, m.has = m.has, m.set = m.set, r = function(e, t) {
-                    if (m.has(e)) throw d(h);
+                    if (m.has(e)) throw v(h);
                     return t.facade = e, m.set(e, t), t
                 }, u = function(e) {
                     return m.get(e) || {}
                 }, o = function(e) {
                     return m.has(e)
                 }
             } else {
                 var A = p("state");
                 D[A] = !0, r = function(e, t) {
-                    if (f(e, A)) throw d(h);
+                    if (f(e, A)) throw v(h);
                     return t.facade = e, s(e, A, t), t
                 }, u = function(e) {
                     return f(e, A) ? e[A] : {}
                 }, o = function(e) {
                     return f(e, A)
                 }
             }
@@ -2581,42 +2581,42 @@
                 c = n(2788),
                 s = function() {},
                 f = [],
                 l = a("Reflect", "construct"),
                 p = /^\s*(?:class|function)\b/,
                 D = r(p.exec),
                 h = !p.exec(s),
-                d = function(e) {
+                v = function(e) {
                     if (!o(e)) return !1;
                     try {
                         return l(s, f, e), !0
                     } catch (t) {
                         return !1
                     }
                 },
-                v = function(e) {
+                d = function(e) {
                     if (!o(e)) return !1;
                     switch (i(e)) {
                         case "AsyncFunction":
                         case "GeneratorFunction":
                         case "AsyncGeneratorFunction":
                             return !1
                     }
                     try {
                         return h || !!D(p, c(e))
                     } catch (t) {
                         return !0
                     }
                 };
-            v.sham = !0, e.exports = !l || u((function() {
+            d.sham = !0, e.exports = !l || u((function() {
                 var e;
-                return d(d.call) || !d(Object) || !d((function() {
+                return v(v.call) || !v(Object) || !v((function() {
                     e = !0
                 })) || e
-            })) ? v : d
+            })) ? d : v
         },
         4705: function(e, t, n) {
             var r = n(7293),
                 u = n(614),
                 o = /#|\.prototype\./,
                 i = function(e, t) {
                     var n = c[a(e)];
@@ -2682,47 +2682,47 @@
                 f = n(4121),
                 l = n(1246),
                 p = n(9212),
                 D = TypeError,
                 h = function(e, t) {
                     this.stopped = e, this.result = t
                 },
-                d = h.prototype;
+                v = h.prototype;
             e.exports = function(e, t, n) {
-                var v, y, g, m, A, C, E, F = n && n.that,
+                var d, y, g, m, A, C, E, F = n && n.that,
                     b = !(!n || !n.AS_ENTRIES),
                     w = !(!n || !n.IS_RECORD),
                     B = !(!n || !n.IS_ITERATOR),
                     S = !(!n || !n.INTERRUPTED),
                     x = r(t, F),
                     O = function(e) {
-                        return v && p(v, "normal", e), new h(!0, e)
+                        return d && p(d, "normal", e), new h(!0, e)
                     },
                     P = function(e) {
                         return b ? (o(e), S ? x(e[0], e[1], O) : x(e[0], e[1])) : S ? x(e, O) : x(e)
                     };
-                if (w) v = e.iterator;
-                else if (B) v = e;
+                if (w) d = e.iterator;
+                else if (B) d = e;
                 else {
                     if (y = l(e), !y) throw D(i(e) + " is not iterable");
                     if (a(y)) {
                         for (g = 0, m = c(e); m > g; g++)
-                            if (A = P(e[g]), A && s(d, A)) return A;
+                            if (A = P(e[g]), A && s(v, A)) return A;
                         return new h(!1)
                     }
-                    v = f(e, y)
+                    d = f(e, y)
                 }
-                C = w ? e.next : v.next;
-                while (!(E = u(C, v)).done) {
+                C = w ? e.next : d.next;
+                while (!(E = u(C, d)).done) {
                     try {
                         A = P(E.value)
                     } catch (j) {
-                        p(v, "throw", j)
+                        p(d, "throw", j)
                     }
-                    if ("object" == typeof A && A && s(d, A)) return A
+                    if ("object" == typeof A && A && s(v, A)) return A
                 }
                 return new h(!1)
             }
         },
         9212: function(e, t, n) {
             var r = n(6916),
                 u = n(9670),
@@ -2771,28 +2771,28 @@
                 c = n(3061),
                 s = n(9518),
                 f = n(7674),
                 l = n(8003),
                 p = n(8880),
                 D = n(8052),
                 h = n(5112),
-                d = n(7497),
-                v = n(3383),
+                v = n(7497),
+                d = n(3383),
                 y = i.PROPER,
                 g = i.CONFIGURABLE,
-                m = v.IteratorPrototype,
-                A = v.BUGGY_SAFARI_ITERATORS,
+                m = d.IteratorPrototype,
+                A = d.BUGGY_SAFARI_ITERATORS,
                 C = h("iterator"),
                 E = "keys",
                 F = "values",
                 b = "entries",
                 w = function() {
                     return this
                 };
-            e.exports = function(e, t, n, i, h, v, B) {
+            e.exports = function(e, t, n, i, h, d, B) {
                 c(n, t, i);
                 var S, x, O, P = function(e) {
                         if (e === h && T) return T;
                         if (!A && e in I) return I[e];
                         switch (e) {
                             case E:
                                 return function() {
@@ -2813,55 +2813,55 @@
                     },
                     j = t + " Iterator",
                     k = !1,
                     I = e.prototype,
                     R = I[C] || I["@@iterator"] || h && I[h],
                     T = !A && R || P(h),
                     U = "Array" == t && I.entries || R;
-                if (U && (S = s(U.call(new e)), S !== Object.prototype && S.next && (o || s(S) === m || (f ? f(S, m) : a(S[C]) || D(S, C, w)), l(S, j, !0, !0), o && (d[j] = w))), y && h == F && R && R.name !== F && (!o && g ? p(I, "name", F) : (k = !0, T = function() {
+                if (U && (S = s(U.call(new e)), S !== Object.prototype && S.next && (o || s(S) === m || (f ? f(S, m) : a(S[C]) || D(S, C, w)), l(S, j, !0, !0), o && (v[j] = w))), y && h == F && R && R.name !== F && (!o && g ? p(I, "name", F) : (k = !0, T = function() {
                         return u(R, this)
                     })), h)
                     if (x = {
                             values: P(F),
-                            keys: v ? T : P(E),
+                            keys: d ? T : P(E),
                             entries: P(b)
                         }, B)
                         for (O in x)(A || k || !(O in I)) && D(I, O, x[O]);
                     else r({
                         target: t,
                         proto: !0,
                         forced: A || k
                     }, x);
                 return o && !B || I[C] === T || D(I, C, T, {
                     name: h
-                }), d[t] = T, x
+                }), v[t] = T, x
             }
         },
         3383: function(e, t, n) {
             "use strict";
             var r, u, o, i = n(7293),
                 a = n(614),
                 c = n(111),
                 s = n(30),
                 f = n(9518),
                 l = n(8052),
                 p = n(5112),
                 D = n(1913),
                 h = p("iterator"),
-                d = !1;
-            [].keys && (o = [].keys(), "next" in o ? (u = f(f(o)), u !== Object.prototype && (r = u)) : d = !0);
-            var v = !c(r) || i((function() {
+                v = !1;
+            [].keys && (o = [].keys(), "next" in o ? (u = f(f(o)), u !== Object.prototype && (r = u)) : v = !0);
+            var d = !c(r) || i((function() {
                 var e = {};
                 return r[h].call(e) !== e
             }));
-            v ? r = {} : D && (r = s(r)), a(r[h]) || l(r, h, (function() {
+            d ? r = {} : D && (r = s(r)), a(r[h]) || l(r, h, (function() {
                 return this
             })), e.exports = {
                 IteratorPrototype: r,
-                BUGGY_SAFARI_ITERATORS: d
+                BUGGY_SAFARI_ITERATORS: v
             }
         },
         7497: function(e) {
             e.exports = {}
         },
         6244: function(e, t, n) {
             var r = n(7466);
@@ -2878,25 +2878,25 @@
                 c = n(6530).CONFIGURABLE,
                 s = n(2788),
                 f = n(9909),
                 l = f.enforce,
                 p = f.get,
                 D = String,
                 h = Object.defineProperty,
-                d = r("".slice),
-                v = r("".replace),
+                v = r("".slice),
+                d = r("".replace),
                 y = r([].join),
                 g = a && !u((function() {
                     return 8 !== h((function() {}), "length", {
                         value: 8
                     }).length
                 })),
                 m = String(String).split("String"),
                 A = e.exports = function(e, t, n) {
-                    "Symbol(" === d(D(t), 0, 7) && (t = "[" + v(D(t), /^Symbol\(([^)]*)\)/, "$1") + "]"), n && n.getter && (t = "get " + t), n && n.setter && (t = "set " + t), (!i(e, "name") || c && e.name !== t) && (a ? h(e, "name", {
+                    "Symbol(" === v(D(t), 0, 7) && (t = "[" + d(D(t), /^Symbol\(([^)]*)\)/, "$1") + "]"), n && n.getter && (t = "get " + t), n && n.setter && (t = "set " + t), (!i(e, "name") || c && e.name !== t) && (a ? h(e, "name", {
                         value: t,
                         configurable: !0
                     }) : e.name = t), g && n && i(n, "arity") && e.length !== n.arity && h(e, "length", {
                         value: n.arity
                     });
                     try {
                         n && i(n, "constructor") && n.constructor ? a && h(e, "prototype", {
@@ -2922,37 +2922,37 @@
             var r, u, o, i, a, c = n(7854),
                 s = n(9974),
                 f = n(1236).f,
                 l = n(261).set,
                 p = n(8572),
                 D = n(6833),
                 h = n(1528),
-                d = n(1036),
-                v = n(5268),
+                v = n(1036),
+                d = n(5268),
                 y = c.MutationObserver || c.WebKitMutationObserver,
                 g = c.document,
                 m = c.process,
                 A = c.Promise,
                 C = f(c, "queueMicrotask"),
                 E = C && C.value;
             if (!E) {
                 var F = new p,
                     b = function() {
                         var e, t;
-                        v && (e = m.domain) && e.exit();
+                        d && (e = m.domain) && e.exit();
                         while (t = F.get()) try {
                             t()
                         } catch (n) {
                             throw F.head && r(), n
                         }
                         e && e.enter()
                     };
-                D || v || d || !y || !g ? !h && A && A.resolve ? (i = A.resolve(void 0), i.constructor = A, a = s(i.then, i), r = function() {
+                D || d || v || !y || !g ? !h && A && A.resolve ? (i = A.resolve(void 0), i.constructor = A, a = s(i.then, i), r = function() {
                     a(b)
-                }) : v ? r = function() {
+                }) : d ? r = function() {
                     m.nextTick(b)
                 } : (l = s(l, c), r = function() {
                     l(b)
                 }) : (u = !0, o = g.createTextNode(""), new y(b).observe(o, {
                     characterData: !0
                 }), r = function() {
                     o.data = u = !u
@@ -3029,19 +3029,19 @@
             })) ? function(e, t) {
                 var n = f(e),
                     u = arguments.length,
                     i = 1,
                     p = c.f,
                     D = s.f;
                 while (u > i) {
-                    var d, v = l(arguments[i++]),
-                        y = p ? h(a(v), p(v)) : a(v),
+                    var v, d = l(arguments[i++]),
+                        y = p ? h(a(d), p(d)) : a(d),
                         g = y.length,
                         m = 0;
-                    while (g > m) d = y[m++], r && !o(D, v, d) || (n[d] = v[d])
+                    while (g > m) v = y[m++], r && !o(D, d, v) || (n[v] = d[v])
                 }
                 return n
             } : p
         },
         30: function(e, t, n) {
             var r, u = n(9670),
                 o = n(6048),
@@ -3050,16 +3050,16 @@
                 c = n(490),
                 s = n(317),
                 f = n(6200),
                 l = ">",
                 p = "<",
                 D = "prototype",
                 h = "script",
-                d = f("IE_PROTO"),
-                v = function() {},
+                v = f("IE_PROTO"),
+                d = function() {},
                 y = function(e) {
                     return p + h + l + e + p + "/" + h + l
                 },
                 g = function(e) {
                     e.write(y("")), e.close();
                     var t = e.parentWindow.Object;
                     return e = null, t
@@ -3074,17 +3074,17 @@
                         r = new ActiveXObject("htmlfile")
                     } catch (t) {}
                     A = "undefined" != typeof document ? document.domain && r ? g(r) : m() : g(r);
                     var e = i.length;
                     while (e--) delete A[D][i[e]];
                     return A()
                 };
-            a[d] = !0, e.exports = Object.create || function(e, t) {
+            a[v] = !0, e.exports = Object.create || function(e, t) {
                 var n;
-                return null !== e ? (v[D] = u(e), n = new v, v[D] = null, n[d] = e) : n = A(), void 0 === t ? n : o.f(n, t)
+                return null !== e ? (d[D] = u(e), n = new d, d[D] = null, n[v] = e) : n = A(), void 0 === t ? n : o.f(n, t)
             }
         },
         6048: function(e, t, n) {
             var r = n(9781),
                 u = n(3353),
                 o = n(3070),
                 i = n(9670),
@@ -3278,37 +3278,37 @@
                 c = n(5112),
                 s = n(7871),
                 f = n(3823),
                 l = n(1913),
                 p = n(7392),
                 D = u && u.prototype,
                 h = c("species"),
-                d = !1,
-                v = o(r.PromiseRejectionEvent),
+                v = !1,
+                d = o(r.PromiseRejectionEvent),
                 y = i("Promise", (function() {
                     var e = a(u),
                         t = e !== String(u);
                     if (!t && 66 === p) return !0;
                     if (l && (!D["catch"] || !D["finally"])) return !0;
                     if (!p || p < 51 || !/native code/.test(e)) {
                         var n = new u((function(e) {
                                 e(1)
                             })),
                             r = function(e) {
                                 e((function() {}), (function() {}))
                             },
                             o = n.constructor = {};
-                        if (o[h] = r, d = n.then((function() {})) instanceof r, !d) return !0
+                        if (o[h] = r, v = n.then((function() {})) instanceof r, !v) return !0
                     }
-                    return !t && (s || f) && !v
+                    return !t && (s || f) && !d
                 }));
             e.exports = {
                 CONSTRUCTOR: y,
-                REJECTION_EVENT: v,
-                SUBCLASSING: d
+                REJECTION_EVENT: d,
+                SUBCLASSING: v
             }
         },
         2492: function(e, t, n) {
             var r = n(7854);
             e.exports = r.Promise
         },
         9478: function(e, t, n) {
@@ -3393,45 +3393,45 @@
                 c = n(2309),
                 s = n(30),
                 f = n(9909).get,
                 l = n(9441),
                 p = n(7168),
                 D = c("native-string-replace", String.prototype.replace),
                 h = RegExp.prototype.exec,
-                d = h,
-                v = u("".charAt),
+                v = h,
+                d = u("".charAt),
                 y = u("".indexOf),
                 g = u("".replace),
                 m = u("".slice),
                 A = function() {
                     var e = /a/,
                         t = /b*/g;
                     return r(h, e, "a"), r(h, t, "a"), 0 !== e.lastIndex || 0 !== t.lastIndex
                 }(),
                 C = a.BROKEN_CARET,
                 E = void 0 !== /()??/.exec("")[1],
                 F = A || E || C || l || p;
-            F && (d = function(e) {
+            F && (v = function(e) {
                 var t, n, u, a, c, l, p, F = this,
                     b = f(F),
                     w = o(e),
                     B = b.raw;
-                if (B) return B.lastIndex = F.lastIndex, t = r(d, B, w), F.lastIndex = B.lastIndex, t;
+                if (B) return B.lastIndex = F.lastIndex, t = r(v, B, w), F.lastIndex = B.lastIndex, t;
                 var S = b.groups,
                     x = C && F.sticky,
                     O = r(i, F),
                     P = F.source,
                     j = 0,
                     k = w;
-                if (x && (O = g(O, "y", ""), -1 === y(O, "g") && (O += "g"), k = m(w, F.lastIndex), F.lastIndex > 0 && (!F.multiline || F.multiline && "\n" !== v(w, F.lastIndex - 1)) && (P = "(?: " + P + ")", k = " " + k, j++), n = new RegExp("^(?:" + P + ")", O)), E && (n = new RegExp("^" + P + "$(?!\\s)", O)), A && (u = F.lastIndex), a = r(h, x ? n : F, k), x ? a ? (a.input = m(a.input, j), a[0] = m(a[0], j), a.index = F.lastIndex, F.lastIndex += a[0].length) : F.lastIndex = 0 : A && a && (F.lastIndex = F.global ? a.index + a[0].length : u), E && a && a.length > 1 && r(D, a[0], n, (function() {
+                if (x && (O = g(O, "y", ""), -1 === y(O, "g") && (O += "g"), k = m(w, F.lastIndex), F.lastIndex > 0 && (!F.multiline || F.multiline && "\n" !== d(w, F.lastIndex - 1)) && (P = "(?: " + P + ")", k = " " + k, j++), n = new RegExp("^(?:" + P + ")", O)), E && (n = new RegExp("^" + P + "$(?!\\s)", O)), A && (u = F.lastIndex), a = r(h, x ? n : F, k), x ? a ? (a.input = m(a.input, j), a[0] = m(a[0], j), a.index = F.lastIndex, F.lastIndex += a[0].length) : F.lastIndex = 0 : A && a && (F.lastIndex = F.global ? a.index + a[0].length : u), E && a && a.length > 1 && r(D, a[0], n, (function() {
                         for (c = 1; c < arguments.length - 2; c++) void 0 === arguments[c] && (a[c] = void 0)
                     })), a && S)
                     for (a.groups = l = s(null), c = 0; c < S.length; c++) p = S[c], l[p[0]] = a[p[1]];
                 return a
-            }), e.exports = d
+            }), e.exports = v
         },
         7066: function(e, t, n) {
             "use strict";
             var r = n(9670);
             e.exports = function() {
                 var e = r(this),
                     t = "";
@@ -3594,16 +3594,16 @@
                 c = 38,
                 s = 700,
                 f = 72,
                 l = 128,
                 p = "-",
                 D = /[^\0-\u007E]/,
                 h = /[.\u3002\uFF0E\uFF61]/g,
-                d = "Overflow: input needs wider integers to process",
-                v = o - i,
+                v = "Overflow: input needs wider integers to process",
+                d = o - i,
                 y = RangeError,
                 g = r(h.exec),
                 m = Math.floor,
                 A = String.fromCharCode,
                 C = r("".charCodeAt),
                 E = r([].join),
                 F = r([].push),
@@ -3625,46 +3625,46 @@
                 },
                 x = function(e) {
                     return e + 22 + 75 * (e < 26)
                 },
                 O = function(e, t, n) {
                     var r = 0;
                     e = n ? m(e / s) : e >> 1, e += m(e / t);
-                    while (e > v * a >> 1) e = m(e / v), r += o;
-                    return m(r + (v + 1) * e / (e + c))
+                    while (e > d * a >> 1) e = m(e / d), r += o;
+                    return m(r + (d + 1) * e / (e + c))
                 },
                 P = function(e) {
                     var t = [];
                     e = S(e);
                     var n, r, c = e.length,
                         s = l,
                         D = 0,
                         h = f;
                     for (n = 0; n < e.length; n++) r = e[n], r < 128 && F(t, A(r));
-                    var v = t.length,
-                        g = v;
-                    v && F(t, p);
+                    var d = t.length,
+                        g = d;
+                    d && F(t, p);
                     while (g < c) {
                         var C = u;
                         for (n = 0; n < e.length; n++) r = e[n], r >= s && r < C && (C = r);
                         var b = g + 1;
-                        if (C - s > m((u - D) / b)) throw y(d);
+                        if (C - s > m((u - D) / b)) throw y(v);
                         for (D += (C - s) * b, s = C, n = 0; n < e.length; n++) {
-                            if (r = e[n], r < s && ++D > u) throw y(d);
+                            if (r = e[n], r < s && ++D > u) throw y(v);
                             if (r == s) {
                                 var w = D,
                                     B = o;
                                 while (1) {
                                     var P = B <= h ? i : B >= h + a ? a : B - h;
                                     if (w < P) break;
                                     var j = w - P,
                                         k = o - P;
                                     F(t, A(x(P + j % k))), w = m(j / k), B += o
                                 }
-                                F(t, A(x(w))), h = O(D, b, g == v), D = 0, g++
+                                F(t, A(x(w))), h = O(D, b, g == d), D = 0, g++
                             }
                         }
                         D++, s++
                     }
                     return E(t, "")
                 };
             e.exports = function(e) {
@@ -3703,16 +3703,16 @@
                 c = n(2104),
                 s = n(9974),
                 f = n(614),
                 l = n(2597),
                 p = n(7293),
                 D = n(490),
                 h = n(206),
-                d = n(317),
-                v = n(8053),
+                v = n(317),
+                d = n(8053),
                 y = n(6833),
                 g = n(5268),
                 m = a.setImmediate,
                 A = a.clearImmediate,
                 C = a.process,
                 E = a.Dispatch,
                 F = a.Function,
@@ -3738,28 +3738,28 @@
                 j = function(e) {
                     O(e.data)
                 },
                 k = function(e) {
                     a.postMessage(w(e), r.protocol + "//" + r.host)
                 };
             m && A || (m = function(e) {
-                v(arguments.length, 1);
+                d(arguments.length, 1);
                 var t = f(e) ? e : F(e),
                     n = h(arguments, 1);
                 return S[++B] = function() {
                     c(t, void 0, n)
                 }, u(B), B
             }, A = function(e) {
                 delete S[e]
             }, g ? u = function(e) {
                 C.nextTick(P(e))
             } : E && E.now ? u = function(e) {
                 E.now(P(e))
-            } : b && !y ? (o = new b, i = o.port2, o.port1.onmessage = j, u = s(i.postMessage, i)) : a.addEventListener && f(a.postMessage) && !a.importScripts && r && "file:" !== r.protocol && !p(k) ? (u = k, a.addEventListener("message", j, !1)) : u = x in d("script") ? function(e) {
-                D.appendChild(d("script"))[x] = function() {
+            } : b && !y ? (o = new b, i = o.port2, o.port1.onmessage = j, u = s(i.postMessage, i)) : a.addEventListener && f(a.postMessage) && !a.importScripts && r && "file:" !== r.protocol && !p(k) ? (u = k, a.addEventListener("message", j, !1)) : u = x in v("script") ? function(e) {
+                D.appendChild(v("script"))[x] = function() {
                     D.removeChild(this), O(e)
                 }
             } : function(e) {
                 setTimeout(P(e), 0)
             }), e.exports = {
                 set: m,
                 clear: A
@@ -3931,39 +3931,59 @@
                 c = n(9920),
                 s = n(2626),
                 f = n(9587),
                 l = n(6277),
                 p = n(8340),
                 D = n(5392),
                 h = n(9781),
-                d = n(1913);
-            e.exports = function(e, t, n, v) {
+                v = n(1913);
+            e.exports = function(e, t, n, d) {
                 var y = "stackTraceLimit",
-                    g = v ? 2 : 1,
+                    g = d ? 2 : 1,
                     m = e.split("."),
                     A = m[m.length - 1],
                     C = r.apply(null, m);
                 if (C) {
                     var E = C.prototype;
-                    if (!d && u(E, "cause") && delete E.cause, !n) return C;
+                    if (!v && u(E, "cause") && delete E.cause, !n) return C;
                     var F = r("Error"),
                         b = t((function(e, t) {
-                            var n = l(v ? t : e, void 0),
-                                r = v ? new C(e) : new C;
+                            var n = l(d ? t : e, void 0),
+                                r = d ? new C(e) : new C;
                             return void 0 !== n && o(r, "message", n), D(r, b, r.stack, 2), this && i(E, this) && f(r, this, b), arguments.length > g && p(r, arguments[g]), r
                         }));
                     if (b.prototype = E, "Error" !== A ? a ? a(b, F) : c(b, F, {
                             name: !0
-                        }) : h && y in C && (s(b, C, y), s(b, C, "prepareStackTrace")), c(b, C), !d) try {
+                        }) : h && y in C && (s(b, C, y), s(b, C, "prepareStackTrace")), c(b, C), !v) try {
                         E.name !== A && o(E, "name", A), E.constructor = b
                     } catch (w) {}
                     return b
                 }
             }
         },
+        2262: function(e, t, n) {
+            "use strict";
+            var r = n(2109),
+                u = n(7908),
+                o = n(6244),
+                i = n(9303),
+                a = n(1223);
+            r({
+                target: "Array",
+                proto: !0
+            }, {
+                at: function(e) {
+                    var t = u(this),
+                        n = o(t),
+                        r = i(e),
+                        a = r >= 0 ? r : n + r;
+                    return a < 0 || a >= n ? void 0 : t[a]
+                }
+            }), a("at")
+        },
         6992: function(e, t, n) {
             "use strict";
             var r = n(5656),
                 u = n(1223),
                 o = n(7497),
                 i = n(9909),
                 a = n(3070).f,
@@ -3984,20 +4004,20 @@
             }), (function() {
                 var e = h(this),
                     t = e.target,
                     n = e.kind,
                     r = e.index++;
                 return !t || r >= t.length ? (e.target = void 0, s(void 0, !0)) : s("keys" == n ? r : "values" == n ? t[r] : [r, t[r]], !1)
             }), "values");
-            var d = o.Arguments = o.Array;
-            if (u("keys"), u("values"), u("entries"), !f && l && "values" !== d.name) try {
-                a(d, "name", {
+            var v = o.Arguments = o.Array;
+            if (u("keys"), u("values"), u("entries"), !f && l && "values" !== v.name) try {
+                a(v, "name", {
                     value: "values"
                 })
-            } catch (v) {}
+            } catch (d) {}
         },
         7658: function(e, t, n) {
             "use strict";
             var r = n(2109),
                 u = n(7908),
                 o = n(6244),
                 i = n(3658),
@@ -4044,31 +4064,31 @@
                 c = n(5117),
                 s = n(1340),
                 f = n(7293),
                 l = n(4362),
                 p = n(9341),
                 D = n(8886),
                 h = n(256),
-                d = n(7392),
-                v = n(8008),
+                v = n(7392),
+                d = n(8008),
                 y = [],
                 g = u(y.sort),
                 m = u(y.push),
                 A = f((function() {
                     y.sort(void 0)
                 })),
                 C = f((function() {
                     y.sort(null)
                 })),
                 E = p("sort"),
                 F = !f((function() {
-                    if (d) return d < 70;
+                    if (v) return v < 70;
                     if (!(D && D > 3)) {
                         if (h) return !0;
-                        if (v) return v < 603;
+                        if (d) return d < 603;
                         var e, t, n, r, u = "";
                         for (e = 65; e < 76; e++) {
                             switch (t = String.fromCharCode(e), e) {
                                 case 66:
                                 case 69:
                                 case 70:
                                 case 72:
@@ -4199,53 +4219,53 @@
                 c = n(7293),
                 s = n(614),
                 f = n(2190),
                 l = n(206),
                 p = n(8044),
                 D = n(6293),
                 h = String,
-                d = u("JSON", "stringify"),
-                v = a(/./.exec),
+                v = u("JSON", "stringify"),
+                d = a(/./.exec),
                 y = a("".charAt),
                 g = a("".charCodeAt),
                 m = a("".replace),
                 A = a(1..toString),
                 C = /[\uD800-\uDFFF]/g,
                 E = /^[\uD800-\uDBFF]$/,
                 F = /^[\uDC00-\uDFFF]$/,
                 b = !D || c((function() {
                     var e = u("Symbol")();
-                    return "[null]" != d([e]) || "{}" != d({
+                    return "[null]" != v([e]) || "{}" != v({
                         a: e
-                    }) || "{}" != d(Object(e))
+                    }) || "{}" != v(Object(e))
                 })),
                 w = c((function() {
-                    return '"\\udf06\\ud834"' !== d("\udf06\ud834") || '"\\udead"' !== d("\udead")
+                    return '"\\udf06\\ud834"' !== v("\udf06\ud834") || '"\\udead"' !== v("\udead")
                 })),
                 B = function(e, t) {
                     var n = l(arguments),
                         r = p(t);
                     if (s(r) || void 0 !== e && !f(e)) return n[1] = function(e, t) {
                         if (s(r) && (t = i(r, this, h(e), t)), !f(t)) return t
-                    }, o(d, null, n)
+                    }, o(v, null, n)
                 },
                 S = function(e, t, n) {
                     var r = y(n, t - 1),
                         u = y(n, t + 1);
-                    return v(E, e) && !v(F, u) || v(F, e) && !v(E, r) ? "\\u" + A(g(e, 0), 16) : e
+                    return d(E, e) && !d(F, u) || d(F, e) && !d(E, r) ? "\\u" + A(g(e, 0), 16) : e
                 };
-            d && r({
+            v && r({
                 target: "JSON",
                 stat: !0,
                 arity: 3,
                 forced: b || w
             }, {
                 stringify: function(e, t, n) {
                     var r = l(arguments),
-                        u = o(b ? B : d, null, r);
+                        u = o(b ? B : v, null, r);
                     return w && "string" == typeof u ? m(u, C, S) : u
                 }
             })
         },
         6977: function(e, t, n) {
             "use strict";
             var r = n(2109),
@@ -4256,18 +4276,18 @@
                 c = n(7293),
                 s = RangeError,
                 f = String,
                 l = Math.floor,
                 p = u(a),
                 D = u("".slice),
                 h = u(1..toFixed),
-                d = function(e, t, n) {
-                    return 0 === t ? n : t % 2 === 1 ? d(e, t - 1, n * e) : d(e * e, t / 2, n)
+                v = function(e, t, n) {
+                    return 0 === t ? n : t % 2 === 1 ? v(e, t - 1, n * e) : v(e * e, t / 2, n)
                 },
-                v = function(e) {
+                d = function(e) {
                     var t = 0,
                         n = e;
                     while (n >= 4096) t += 12, n /= 4096;
                     while (n >= 2) t += 1, n /= 2;
                     return t
                 },
                 y = function(e, t, n) {
@@ -4305,18 +4325,18 @@
                         l = [0, 0, 0, 0, 0, 0],
                         h = "",
                         A = "0";
                     if (c < 0 || c > 20) throw s("Incorrect fraction digits");
                     if (a != a) return "NaN";
                     if (a <= -1e21 || a >= 1e21) return f(a);
                     if (a < 0 && (h = "-", a = -a), a > 1e-21)
-                        if (t = v(a * d(2, 69, 1)) - 69, n = t < 0 ? a * d(2, -t, 1) : a / d(2, t, 1), n *= 4503599627370496, t = 52 - t, t > 0) {
+                        if (t = d(a * v(2, 69, 1)) - 69, n = t < 0 ? a * v(2, -t, 1) : a / v(2, t, 1), n *= 4503599627370496, t = 52 - t, t > 0) {
                             y(l, 0, n), r = c;
                             while (r >= 7) y(l, 1e7, 0), r -= 7;
-                            y(l, d(10, r, 1), 0), r = t - 1;
+                            y(l, v(10, r, 1), 0), r = t - 1;
                             while (r >= 23) g(l, 1 << 23), r -= 23;
                             g(l, 1 << r), y(l, 1, 1), g(l, 2), A = m(l)
                         } else y(l, 0, n), y(l, 1 << -t, 0), A = m(l) + p("0", c);
                     return c > 0 ? (u = A.length, A = h + (u <= c ? "0." + p("0", c - u) + A : D(A, 0, u - c) + "." + D(A, u - c))) : A = h + A, A
                 }
             })
         },
@@ -4400,16 +4420,16 @@
                 c = n(1913),
                 s = n(5268),
                 f = n(7854),
                 l = n(6916),
                 p = n(8052),
                 D = n(7674),
                 h = n(8003),
-                d = n(6340),
-                v = n(9662),
+                v = n(6340),
+                d = n(9662),
                 y = n(614),
                 g = n(111),
                 m = n(5787),
                 A = n(6707),
                 C = n(261).set,
                 E = n(5948),
                 F = n(842),
@@ -4519,15 +4539,15 @@
                             ie({
                                 done: !1
                             }, u, e)
                         }
                     }
                 };
             if (j && (N = function(e) {
-                    m(this, L), v(e), l(r, this);
+                    m(this, L), d(e), l(r, this);
                     var t = R(this);
                     try {
                         e(oe(ae, t), oe(ie, t))
                     } catch (n) {
                         ie(t, n)
                     }
                 }, L = N.prototype, r = function(e) {
@@ -4570,15 +4590,15 @@
             a({
                 global: !0,
                 constructor: !0,
                 wrap: !0,
                 forced: j
             }, {
                 Promise: N
-            }), h(N, P, !1, !0), d(P)
+            }), h(N, P, !1, !0), v(P)
         },
         7727: function(e, t, n) {
             "use strict";
             var r = n(2109),
                 u = n(1913),
                 o = n(2492),
                 i = n(7293),
@@ -4763,14 +4783,40 @@
                     t = i(e.source),
                     n = i(c(e));
                 return "/" + t + "/" + n
             }), {
                 unsafe: !0
             })
         },
+        4506: function(e, t, n) {
+            "use strict";
+            var r = n(2109),
+                u = n(1702),
+                o = n(4488),
+                i = n(9303),
+                a = n(1340),
+                c = n(7293),
+                s = u("".charAt),
+                f = c((function() {
+                    return "\ud842" !== "𠮷".at(-2)
+                }));
+            r({
+                target: "String",
+                proto: !0,
+                forced: f
+            }, {
+                at: function(e) {
+                    var t = a(o(this)),
+                        n = t.length,
+                        r = i(e),
+                        u = r >= 0 ? r : n + r;
+                    return u < 0 || u >= n ? void 0 : s(t, u)
+                }
+            })
+        },
         2023: function(e, t, n) {
             "use strict";
             var r = n(2109),
                 u = n(1702),
                 o = n(3929),
                 i = n(4488),
                 a = n(1340),
@@ -4819,16 +4865,16 @@
                 c = n(8554),
                 s = n(7850),
                 f = n(1340),
                 l = n(8173),
                 p = n(4706),
                 D = n(647),
                 h = n(5112),
-                d = n(1913),
-                v = h("replace"),
+                v = n(1913),
+                d = h("replace"),
                 y = TypeError,
                 g = o("".indexOf),
                 m = o("".replace),
                 A = o("".slice),
                 C = Math.max,
                 E = function(e, t, n) {
                     return n > e.length ? -1 : "" === t ? n : g(e, t, n)
@@ -4840,16 +4886,16 @@
                 replaceAll: function(e, t) {
                     var n, r, o, h, F, b, w, B, S, x = i(this),
                         O = 0,
                         P = 0,
                         j = "";
                     if (!c(e)) {
                         if (n = s(e), n && (r = f(i(p(e))), !~g(r, "g"))) throw y("`.replaceAll` does not allow non-global regexes");
-                        if (o = l(e, v), o) return u(o, e, x, t);
-                        if (d && n) return m(f(x), e, t)
+                        if (o = l(e, d), o) return u(o, e, x, t);
+                        if (v && n) return m(f(x), e, t)
                     }
                     h = f(x), F = f(e), b = a(t), b || (t = f(t)), w = F.length, B = C(1, w), O = E(h, F, 0);
                     while (-1 !== O) S = b ? f(t(F, O, h)) : D(F, h, O, [], void 0, t), j += A(h, P, O) + S, P = O + w, O = E(h, F, O + B);
                     return P < h.length && (j += A(h, P)), j
                 }
             })
         },
@@ -4863,16 +4909,16 @@
                 c = n(9670),
                 s = n(614),
                 f = n(8554),
                 l = n(9303),
                 p = n(7466),
                 D = n(1340),
                 h = n(4488),
-                d = n(1530),
-                v = n(8173),
+                v = n(1530),
+                d = n(8173),
                 y = n(647),
                 g = n(7651),
                 m = n(5112),
                 A = m("replace"),
                 C = Math.max,
                 E = Math.min,
                 F = o([].concat),
@@ -4897,37 +4943,37 @@
                         }, e
                     }, "7" !== "".replace(e, "$<a>")
                 }));
             i("replace", (function(e, t, n) {
                 var o = O ? "$" : "$0";
                 return [function(e, n) {
                     var r = h(this),
-                        o = f(e) ? void 0 : v(e, A);
+                        o = f(e) ? void 0 : d(e, A);
                     return o ? u(o, e, r, n) : u(t, D(r), e, n)
                 }, function(e, u) {
                     var i = c(this),
                         a = D(e);
                     if ("string" == typeof u && -1 === w(u, o) && -1 === w(u, "$<")) {
                         var f = n(t, i, a, u);
                         if (f.done) return f.value
                     }
                     var h = s(u);
                     h || (u = D(u));
-                    var v = i.global;
-                    if (v) {
+                    var d = i.global;
+                    if (d) {
                         var m = i.unicode;
                         i.lastIndex = 0
                     }
                     var A = [];
                     while (1) {
                         var x = g(i, a);
                         if (null === x) break;
-                        if (b(A, x), !v) break;
+                        if (b(A, x), !d) break;
                         var O = D(x[0]);
-                        "" === O && (i.lastIndex = d(a, p(i.lastIndex), m))
+                        "" === O && (i.lastIndex = v(a, p(i.lastIndex), m))
                     }
                     for (var P = "", j = 0, k = 0; k < A.length; k++) {
                         x = A[k];
                         for (var I = D(x[0]), R = C(E(l(x.index), a.length), 0), T = [], U = 1; U < x.length; U++) b(T, S(x[U]));
                         var N = x.groups;
                         if (h) {
                             var L = F([I], T, R, a);
@@ -4951,42 +4997,42 @@
                 s = n(7976),
                 f = n(1340),
                 l = n(7045),
                 p = n(9920),
                 D = o.Symbol,
                 h = D && D.prototype;
             if (u && c(D) && (!("description" in h) || void 0 !== D().description)) {
-                var d = {},
-                    v = function() {
+                var v = {},
+                    d = function() {
                         var e = arguments.length < 1 || void 0 === arguments[0] ? void 0 : f(arguments[0]),
                             t = s(h, this) ? new D(e) : void 0 === e ? D() : D(e);
-                        return "" === e && (d[t] = !0), t
+                        return "" === e && (v[t] = !0), t
                     };
-                p(v, D), v.prototype = h, h.constructor = v;
+                p(d, D), d.prototype = h, h.constructor = d;
                 var y = "Symbol(test)" == String(D("test")),
                     g = i(h.valueOf),
                     m = i(h.toString),
                     A = /^Symbol\((.*)\)[^)]+$/,
                     C = i("".replace),
                     E = i("".slice);
                 l(h, "description", {
                     configurable: !0,
                     get: function() {
                         var e = g(this);
-                        if (a(d, e)) return "";
+                        if (a(v, e)) return "";
                         var t = m(e),
                             n = y ? E(t, 7, -1) : C(t, A, "$1");
                         return "" === n ? void 0 : n
                     }
                 }), r({
                     global: !0,
                     constructor: !0,
                     forced: !0
                 }, {
-                    Symbol: v
+                    Symbol: d
                 })
             }
         },
         3948: function(e, t, n) {
             var r = n(7854),
                 u = n(8324),
                 o = n(8509),
@@ -5026,16 +5072,16 @@
                 c = n(5143),
                 s = n(8052),
                 f = n(9190),
                 l = n(8003),
                 p = n(3061),
                 D = n(9909),
                 h = n(5787),
-                d = n(614),
-                v = n(2597),
+                v = n(614),
+                d = n(2597),
                 y = n(9974),
                 g = n(648),
                 m = n(9670),
                 A = n(111),
                 C = n(1340),
                 E = n(30),
                 F = n(9114),
@@ -5139,15 +5185,15 @@
                             if (u = b(m(r.value)), i = u.next, (a = o(i, u)).done || (c = o(i, u)).done || !o(i, u).done) throw z("Expected sequence with length 2");
                             W(this.entries, {
                                 key: C(a.value),
                                 value: C(c.value)
                             })
                         }
                     } else
-                        for (var f in e) v(e, f) && W(this.entries, {
+                        for (var f in e) d(e, f) && W(this.entries, {
                             key: f,
                             value: C(e[f])
                         })
                 },
                 parseQuery: function(e) {
                     if (e) {
                         var t, n, r = Y(e, "&"),
@@ -5255,47 +5301,47 @@
                     enumerable: !0
                 }), l(le, P), r({
                     global: !0,
                     constructor: !0,
                     forced: !c
                 }, {
                     URLSearchParams: le
-                }), !c && d(M)) {
+                }), !c && v(M)) {
                 var De = i($.has),
                     he = i($.set),
-                    de = function(e) {
+                    ve = function(e) {
                         if (A(e)) {
                             var t, n = e.body;
                             if (g(n) === P) return t = e.headers ? new M(e.headers) : new M, De(t, "content-type") || he(t, "content-type", "application/x-www-form-urlencoded;charset=UTF-8"), E(e, {
                                 body: F(0, C(n)),
                                 headers: F(0, t)
                             })
                         }
                         return e
                     };
-                if (d(N) && r({
+                if (v(N) && r({
                         global: !0,
                         enumerable: !0,
                         dontCallGetSet: !0,
                         forced: !0
                     }, {
                         fetch: function(e) {
-                            return N(e, arguments.length > 1 ? de(arguments[1]) : {})
+                            return N(e, arguments.length > 1 ? ve(arguments[1]) : {})
                         }
-                    }), d(L)) {
-                    var ve = function(e) {
-                        return h(this, _), new L(e, arguments.length > 1 ? de(arguments[1]) : {})
+                    }), v(L)) {
+                    var de = function(e) {
+                        return h(this, _), new L(e, arguments.length > 1 ? ve(arguments[1]) : {})
                     };
-                    _.constructor = ve, ve.prototype = _, r({
+                    _.constructor = de, de.prototype = _, r({
                         global: !0,
                         constructor: !0,
                         dontCallGetSet: !0,
                         forced: !0
                     }, {
-                        Request: ve
+                        Request: de
                     })
                 }
             }
             e.exports = {
                 URLSearchParams: le,
                 getState: I
             }
@@ -5313,16 +5359,16 @@
                 c = n(9974),
                 s = n(1702),
                 f = n(8052),
                 l = n(7045),
                 p = n(5787),
                 D = n(2597),
                 h = n(1574),
-                d = n(8457),
-                v = n(1589),
+                v = n(8457),
+                d = n(1589),
                 y = n(8710).codeAt,
                 g = n(3197),
                 m = n(1340),
                 A = n(8003),
                 C = n(8053),
                 E = n(5556),
                 F = n(9909),
@@ -5476,19 +5522,19 @@
                     "@": 1,
                     "[": 1,
                     "\\": 1,
                     "]": 1,
                     "^": 1,
                     "|": 1
                 }),
-                de = function(e, t) {
+                ve = function(e, t) {
                     var n = y(e, 0);
                     return n > 32 && n < 127 && !D(t, e) ? e : encodeURIComponent(e)
                 },
-                ve = {
+                de = {
                     ftp: 21,
                     file: null,
                     http: 80,
                     https: 443,
                     ws: 80,
                     wss: 443
                 },
@@ -5543,15 +5589,15 @@
                     var u, o, i, a, c = this,
                         s = t || Ce,
                         f = 0,
                         l = "",
                         p = !1,
                         h = !1,
                         y = !1;
-                    e = m(e), t || (c.scheme = "", c.username = "", c.password = "", c.host = null, c.port = null, c.path = [], c.query = null, c.fragment = null, c.cannotBeABaseURL = !1, e = M(e, ue, ""), e = M(e, oe, "$1")), e = M(e, ie, ""), u = d(e);
+                    e = m(e), t || (c.scheme = "", c.username = "", c.password = "", c.host = null, c.port = null, c.path = [], c.query = null, c.fragment = null, c.cannotBeABaseURL = !1, e = M(e, ue, ""), e = M(e, oe, "$1")), e = M(e, ie, ""), u = v(e);
                     while (f <= u.length) {
                         switch (o = u[f], s) {
                             case Ce:
                                 if (!o || !R(Z, o)) {
                                     if (t) return q;
                                     s = Fe;
                                     continue
@@ -5562,23 +5608,23 @@
                                 if (o && (R(X, o) || "+" == o || "-" == o || "." == o)) l += z(o);
                                 else {
                                     if (":" != o) {
                                         if (t) return q;
                                         l = "", s = Fe, f = 0;
                                         continue
                                     }
-                                    if (t && (c.isSpecial() != D(ve, l) || "file" == l && (c.includesCredentials() || null !== c.port) || "file" == c.scheme && !c.host)) return;
-                                    if (c.scheme = l, t) return void(c.isSpecial() && ve[c.scheme] == c.port && (c.port = null));
+                                    if (t && (c.isSpecial() != D(de, l) || "file" == l && (c.includesCredentials() || null !== c.port) || "file" == c.scheme && !c.host)) return;
+                                    if (c.scheme = l, t) return void(c.isSpecial() && de[c.scheme] == c.port && (c.port = null));
                                     l = "", "file" == c.scheme ? s = Re : c.isSpecial() && n && n.scheme == c.scheme ? s = be : c.isSpecial() ? s = xe : "/" == u[f + 1] ? (s = we, f++) : (c.cannotBeABaseURL = !0, L(c.path, ""), s = Me)
                                 }
                                 break;
                             case Fe:
                                 if (!n || n.cannotBeABaseURL && "#" != o) return q;
                                 if (n.cannotBeABaseURL && "#" == o) {
-                                    c.scheme = n.scheme, c.path = v(n.path), c.query = n.query, c.fragment = "", c.cannotBeABaseURL = !0, s = $e;
+                                    c.scheme = n.scheme, c.path = d(n.path), c.query = n.query, c.fragment = "", c.cannotBeABaseURL = !0, s = $e;
                                     break
                                 }
                                 s = "file" == n.scheme ? Re : Be;
                                 continue;
                             case be:
                                 if ("/" != o || "/" != u[f + 1]) {
                                     s = Be;
@@ -5590,23 +5636,23 @@
                                 if ("/" == o) {
                                     s = Pe;
                                     break
                                 }
                                 s = Le;
                                 continue;
                             case Be:
-                                if (c.scheme = n.scheme, o == r) c.username = n.username, c.password = n.password, c.host = n.host, c.port = n.port, c.path = v(n.path), c.query = n.query;
+                                if (c.scheme = n.scheme, o == r) c.username = n.username, c.password = n.password, c.host = n.host, c.port = n.port, c.path = d(n.path), c.query = n.query;
                                 else if ("/" == o || "\\" == o && c.isSpecial()) s = Se;
-                                else if ("?" == o) c.username = n.username, c.password = n.password, c.host = n.host, c.port = n.port, c.path = v(n.path), c.query = "", s = _e;
+                                else if ("?" == o) c.username = n.username, c.password = n.password, c.host = n.host, c.port = n.port, c.path = d(n.path), c.query = "", s = _e;
                                 else {
                                     if ("#" != o) {
-                                        c.username = n.username, c.password = n.password, c.host = n.host, c.port = n.port, c.path = v(n.path), c.path.length--, s = Le;
+                                        c.username = n.username, c.password = n.password, c.host = n.host, c.port = n.port, c.path = d(n.path), c.path.length--, s = Le;
                                         continue
                                     }
-                                    c.username = n.username, c.password = n.password, c.host = n.host, c.port = n.port, c.path = v(n.path), c.query = n.query, c.fragment = "", s = $e
+                                    c.username = n.username, c.password = n.password, c.host = n.host, c.port = n.port, c.path = d(n.path), c.query = n.query, c.fragment = "", s = $e
                                 }
                                 break;
                             case Se:
                                 if (!c.isSpecial() || "/" != o && "\\" != o) {
                                     if ("/" != o) {
                                         c.username = n.username, c.password = n.password, c.host = n.host, c.port = n.port, s = Le;
                                         continue
@@ -5622,26 +5668,26 @@
                                 if ("/" != o && "\\" != o) {
                                     s = Pe;
                                     continue
                                 }
                                 break;
                             case Pe:
                                 if ("@" == o) {
-                                    p && (l = "%40" + l), p = !0, i = d(l);
+                                    p && (l = "%40" + l), p = !0, i = v(l);
                                     for (var g = 0; g < i.length; g++) {
                                         var A = i[g];
                                         if (":" != A || y) {
-                                            var C = de(A, he);
+                                            var C = ve(A, he);
                                             y ? c.password += C : c.username += C
                                         } else y = !0
                                     }
                                     l = ""
                                 } else if (o == r || "/" == o || "?" == o || "#" == o || "\\" == o && c.isSpecial()) {
                                     if (p && "" == l) return G;
-                                    f -= d(l).length + 1, l = "", s = je
+                                    f -= v(l).length + 1, l = "", s = je
                                 } else l += o;
                                 break;
                             case je:
                             case ke:
                                 if (t && "file" == c.scheme) {
                                     s = Ue;
                                     continue
@@ -5663,15 +5709,15 @@
                                 break;
                             case Ie:
                                 if (!R(K, o)) {
                                     if (o == r || "/" == o || "?" == o || "#" == o || "\\" == o && c.isSpecial() || t) {
                                         if ("" != l) {
                                             var E = P(l, 10);
                                             if (E > 65535) return W;
-                                            c.port = c.isSpecial() && E === ve[c.scheme] ? null : E, l = ""
+                                            c.port = c.isSpecial() && E === de[c.scheme] ? null : E, l = ""
                                         }
                                         if (t) return;
                                         s = Ne;
                                         continue
                                     }
                                     return W
                                 }
@@ -5680,31 +5726,31 @@
                             case Re:
                                 if (c.scheme = "file", "/" == o || "\\" == o) s = Te;
                                 else {
                                     if (!n || "file" != n.scheme) {
                                         s = Le;
                                         continue
                                     }
-                                    if (o == r) c.host = n.host, c.path = v(n.path), c.query = n.query;
-                                    else if ("?" == o) c.host = n.host, c.path = v(n.path), c.query = "", s = _e;
+                                    if (o == r) c.host = n.host, c.path = d(n.path), c.query = n.query;
+                                    else if ("?" == o) c.host = n.host, c.path = d(n.path), c.query = "", s = _e;
                                     else {
                                         if ("#" != o) {
-                                            ge(T(v(u, f), "")) || (c.host = n.host, c.path = v(n.path), c.shortenPath()), s = Le;
+                                            ge(T(d(u, f), "")) || (c.host = n.host, c.path = d(n.path), c.shortenPath()), s = Le;
                                             continue
                                         }
-                                        c.host = n.host, c.path = v(n.path), c.query = n.query, c.fragment = "", s = $e
+                                        c.host = n.host, c.path = d(n.path), c.query = n.query, c.fragment = "", s = $e
                                     }
                                 }
                                 break;
                             case Te:
                                 if ("/" == o || "\\" == o) {
                                     s = Ue;
                                     break
                                 }
-                                n && "file" == n.scheme && !ge(T(v(u, f), "")) && (ye(n.path[0], !0) ? L(c.path, n.path[0]) : c.host = n.host), s = Le;
+                                n && "file" == n.scheme && !ge(T(d(u, f), "")) && (ye(n.path[0], !0) ? L(c.path, n.path[0]) : c.host = n.host), s = Le;
                                 continue;
                             case Ue:
                                 if (o == r || "/" == o || "\\" == o || "?" == o || "#" == o) {
                                     if (!t && ye(l)) s = Le;
                                     else if ("" == l) {
                                         if (c.host = "", t) return;
                                         s = Ne
@@ -5727,24 +5773,24 @@
                                 else c.query = "", s = _e;
                                 break;
                             case Le:
                                 if (o == r || "/" == o || "\\" == o && c.isSpecial() || !t && ("?" == o || "#" == o)) {
                                     if (Ae(l) ? (c.shortenPath(), "/" == o || "\\" == o && c.isSpecial() || L(c.path, "")) : me(l) ? "/" == o || "\\" == o && c.isSpecial() || L(c.path, "") : ("file" == c.scheme && !c.path.length && ye(l) && (c.host && (c.host = ""), l = I(l, 0) + ":"), L(c.path, l)), l = "", "file" == c.scheme && (o == r || "?" == o || "#" == o))
                                         while (c.path.length > 1 && "" === c.path[0]) _(c.path);
                                     "?" == o ? (c.query = "", s = _e) : "#" == o && (c.fragment = "", s = $e)
-                                } else l += de(o, De);
+                                } else l += ve(o, De);
                                 break;
                             case Me:
-                                "?" == o ? (c.query = "", s = _e) : "#" == o ? (c.fragment = "", s = $e) : o != r && (c.path[0] += de(o, le));
+                                "?" == o ? (c.query = "", s = _e) : "#" == o ? (c.fragment = "", s = $e) : o != r && (c.path[0] += ve(o, le));
                                 break;
                             case _e:
-                                t || "#" != o ? o != r && ("'" == o && c.isSpecial() ? c.query += "%27" : c.query += "#" == o ? "%23" : de(o, le)) : (c.fragment = "", s = $e);
+                                t || "#" != o ? o != r && ("'" == o && c.isSpecial() ? c.query += "%27" : c.query += "#" == o ? "%23" : ve(o, le)) : (c.fragment = "", s = $e);
                                 break;
                             case $e:
-                                o != r && (c.fragment += de(o, pe));
+                                o != r && (c.fragment += ve(o, pe));
                                 break
                         }
                         f++
                     }
                 },
                 parseHost: function(e) {
                     var t, n, r;
@@ -5754,26 +5800,26 @@
                         this.host = t
                     } else if (this.isSpecial()) {
                         if (e = g(e), R(ne, e)) return J;
                         if (t = ae(e), null === t) return J;
                         this.host = t
                     } else {
                         if (R(re, e)) return J;
-                        for (t = "", n = d(e), r = 0; r < n.length; r++) t += de(n[r], le);
+                        for (t = "", n = v(e), r = 0; r < n.length; r++) t += ve(n[r], le);
                         this.host = t
                     }
                 },
                 cannotHaveUsernamePasswordPort: function() {
                     return !this.host || this.cannotBeABaseURL || "file" == this.scheme
                 },
                 includesCredentials: function() {
                     return "" != this.username || "" != this.password
                 },
                 isSpecial: function() {
-                    return D(ve, this.scheme)
+                    return D(de, this.scheme)
                 },
                 shortenPath: function() {
                     var e = this.path,
                         t = e.length;
                     !t || "file" == this.scheme && 1 == t && ye(e[0], !0) || e.length--
                 },
                 serialize: function() {
@@ -5810,28 +5856,28 @@
                 setProtocol: function(e) {
                     this.parse(m(e) + ":", Ce)
                 },
                 getUsername: function() {
                     return this.username
                 },
                 setUsername: function(e) {
-                    var t = d(m(e));
+                    var t = v(m(e));
                     if (!this.cannotHaveUsernamePasswordPort()) {
                         this.username = "";
-                        for (var n = 0; n < t.length; n++) this.username += de(t[n], he)
+                        for (var n = 0; n < t.length; n++) this.username += ve(t[n], he)
                     }
                 },
                 getPassword: function() {
                     return this.password
                 },
                 setPassword: function(e) {
-                    var t = d(m(e));
+                    var t = v(m(e));
                     if (!this.cannotHaveUsernamePasswordPort()) {
                         this.password = "";
-                        for (var n = 0; n < t.length; n++) this.password += de(t[n], he)
+                        for (var n = 0; n < t.length; n++) this.password += ve(t[n], he)
                     }
                 },
                 getHost: function() {
                     var e = this.host,
                         t = this.port;
                     return null === e ? "" : null === t ? fe(e) : fe(e) + ":" + t
                 },
@@ -6044,15 +6090,15 @@
                 }() : s,
                 l = n(1405)(),
                 p = Object.getPrototypeOf || function(e) {
                     return e.__proto__
                 },
                 D = {},
                 h = "undefined" === typeof Uint8Array ? r : p(Uint8Array),
-                d = {
+                v = {
                     "%AggregateError%": "undefined" === typeof AggregateError ? r : AggregateError,
                     "%Array%": Array,
                     "%ArrayBuffer%": "undefined" === typeof ArrayBuffer ? r : ArrayBuffer,
                     "%ArrayIteratorPrototype%": l ? p([][Symbol.iterator]()) : r,
                     "%AsyncFromSyncIteratorPrototype%": r,
                     "%AsyncFunction%": D,
                     "%AsyncGenerator%": D,
@@ -6115,30 +6161,30 @@
                     "%WeakMap%": "undefined" === typeof WeakMap ? r : WeakMap,
                     "%WeakRef%": "undefined" === typeof WeakRef ? r : WeakRef,
                     "%WeakSet%": "undefined" === typeof WeakSet ? r : WeakSet
                 };
             try {
                 null.error
             } catch (P) {
-                var v = p(p(P));
-                d["%Error.prototype%"] = v
+                var d = p(p(P));
+                v["%Error.prototype%"] = d
             }
             var y = function e(t) {
                     var n;
                     if ("%AsyncFunction%" === t) n = a("async function () {}");
                     else if ("%GeneratorFunction%" === t) n = a("function* () {}");
                     else if ("%AsyncGeneratorFunction%" === t) n = a("async function* () {}");
                     else if ("%AsyncGenerator%" === t) {
                         var r = e("%AsyncGeneratorFunction%");
                         r && (n = r.prototype)
                     } else if ("%AsyncIteratorPrototype%" === t) {
                         var u = e("%AsyncGenerator%");
                         u && (n = p(u.prototype))
                     }
-                    return d[t] = n, n
+                    return v[t] = n, n
                 },
                 g = {
                     "%ArrayBufferPrototype%": ["ArrayBuffer", "prototype"],
                     "%ArrayPrototype%": ["Array", "prototype"],
                     "%ArrayProto_entries%": ["Array", "prototype", "entries"],
                     "%ArrayProto_forEach%": ["Array", "prototype", "forEach"],
                     "%ArrayProto_keys%": ["Array", "prototype", "keys"],
@@ -6206,16 +6252,16 @@
                     var r = [];
                     return F(e, B, (function(e, t, n, u) {
                         r[r.length] = n ? F(u, S, "$1") : t || e
                     })), r
                 },
                 O = function(e, t) {
                     var n, r = e;
-                    if (A(g, r) && (n = g[r], r = "%" + n[0] + "%"), A(d, r)) {
-                        var o = d[r];
+                    if (A(g, r) && (n = g[r], r = "%" + n[0] + "%"), A(v, r)) {
+                        var o = v[r];
                         if (o === D && (o = y(r)), "undefined" === typeof o && !t) throw new i("intrinsic " + e + " exists, but is not available. Please file an issue!");
                         return {
                             alias: n,
                             name: r,
                             value: o
                         }
                     }
@@ -6231,28 +6277,28 @@
                     a = o.name,
                     s = o.value,
                     f = !1,
                     l = o.alias;
                 l && (r = l[0], E(n, C([0, 1], l)));
                 for (var p = 1, D = !0; p < n.length; p += 1) {
                     var h = n[p],
-                        v = b(h, 0, 1),
+                        d = b(h, 0, 1),
                         y = b(h, -1);
-                    if (('"' === v || "'" === v || "`" === v || '"' === y || "'" === y || "`" === y) && v !== y) throw new u("property names with quotes must have matching quotes");
-                    if ("constructor" !== h && D || (f = !0), r += "." + h, a = "%" + r + "%", A(d, a)) s = d[a];
+                    if (('"' === d || "'" === d || "`" === d || '"' === y || "'" === y || "`" === y) && d !== y) throw new u("property names with quotes must have matching quotes");
+                    if ("constructor" !== h && D || (f = !0), r += "." + h, a = "%" + r + "%", A(v, a)) s = v[a];
                     else if (null != s) {
                         if (!(h in s)) {
                             if (!t) throw new i("base intrinsic for " + e + " exists, but the property is not available.");
                             return
                         }
                         if (c && p + 1 >= n.length) {
                             var g = c(s, h);
                             D = !!g, s = D && "get" in g && !("originalValue" in g.get) ? g.get : s[h]
                         } else D = A(s, h), s = s[h];
-                        D && !f && (d[a] = s)
+                        D && !f && (v[a] = s)
                     }
                 }
                 return s
             }
         },
         1221: function(e) {
             "use strict";
@@ -6432,17 +6478,17 @@
                         a = t && "[object String]" === o.call(e),
                         l = [];
                     if (!t && !n && !r) throw new TypeError("Object.keys called on a non-object");
                     var p = s && n;
                     if (a && e.length > 0 && !u.call(e, 0))
                         for (var D = 0; D < e.length; ++D) l.push(String(D));
                     if (r && e.length > 0)
-                        for (var d = 0; d < e.length; ++d) l.push(String(d));
+                        for (var v = 0; v < e.length; ++v) l.push(String(v));
                     else
-                        for (var v in e) p && "prototype" === v || !u.call(e, v) || l.push(String(v));
+                        for (var d in e) p && "prototype" === d || !u.call(e, d) || l.push(String(d));
                     if (c)
                         for (var y = h(e), g = 0; g < f.length; ++g) y && "constructor" === f[g] || !u.call(e, f[g]) || l.push(f[g]);
                     return l
                 }
             }
             e.exports = r
         },
@@ -6519,54 +6565,54 @@
                         void 0 === l && (l = {});
                         var p = l.methods;
                         void 0 === p && (p = {});
                         var D = l.computed;
                         void 0 === D && (D = {});
                         var h = l.components;
                         void 0 === h && (h = {});
-                        var d = {
+                        var v = {
                             $data: {},
                             $props: {},
                             $options: {},
                             components: {},
                             computed: {},
                             methods: {}
                         };
                         Object.keys(r).forEach((function(e) {
-                            void 0 === s[e] && (d.$data[e] = r[e])
+                            void 0 === s[e] && (v.$data[e] = r[e])
                         })), Object.keys(u).forEach((function(e) {
-                            void 0 === f[e] && (d.$props[e] = u[e])
+                            void 0 === f[e] && (v.$props[e] = u[e])
                         })), Object.keys(c).forEach((function(e) {
-                            void 0 === p[e] && (d.methods[e] = c[e])
+                            void 0 === p[e] && (v.methods[e] = c[e])
                         })), Object.keys(a).forEach((function(e) {
-                            void 0 === D[e] && (d.computed[e] = a[e])
+                            void 0 === D[e] && (v.computed[e] = a[e])
                         })), Object.keys(i).forEach((function(e) {
-                            void 0 === h[e] && (d.components[e] = i[e])
+                            void 0 === h[e] && (v.components[e] = i[e])
                         }));
-                        var v = Object.keys(d.methods || {}),
-                            y = Object.keys(d.$data || {}),
-                            g = Object.keys(d.$props || {}),
+                        var d = Object.keys(v.methods || {}),
+                            y = Object.keys(v.$data || {}),
+                            g = Object.keys(v.$props || {}),
                             m = Object.keys(this.templateProps),
-                            A = y.concat(g).concat(v).concat(m),
-                            C = (F = t, b = {}, v.forEach((function(e) {
+                            A = y.concat(g).concat(d).concat(m),
+                            C = (F = t, b = {}, d.forEach((function(e) {
                                 return n(F, b, e)
                             })), b),
                             E = function(e) {
                                 var t = {};
                                 return e.forEach((function(e) {
                                     e && Object.getOwnPropertyNames(e).forEach((function(r) {
                                         return n(e, t, r)
                                     }))
                                 })), t
-                            }([d.$data, d.$props, C, this.templateProps]);
+                            }([v.$data, v.$props, C, this.templateProps]);
                         return e({
                             template: this.template || "<div></div>",
                             props: A,
-                            computed: d.computed,
-                            components: d.components,
+                            computed: v.computed,
+                            components: v.components,
                             provide: this.$parent._provided
                         }, {
                             props: E
                         })
                     }
                     var F, b
                 }
@@ -6641,24 +6687,24 @@
                         } catch (r) {}
                         if ("get" in n || "set" in n) throw TypeError("Accessors not supported!");
                         return "value" in n && (e[t] = n.value), e
                     },
                     h = {
                         f: D
                     },
-                    d = function(e, t) {
+                    v = function(e, t) {
                         return {
                             enumerable: !(1 & e),
                             configurable: !(2 & e),
                             writable: !(4 & e),
                             value: t
                         }
                     },
-                    v = i ? function(e, t, n) {
-                        return h.f(e, t, d(1, n))
+                    d = i ? function(e, t, n) {
+                        return h.f(e, t, v(1, n))
                     } : function(e, t, n) {
                         return e[t] = n, e
                     },
                     y = {}.hasOwnProperty,
                     g = function(e, t) {
                         return y.call(e, t)
                     },
@@ -6684,15 +6730,15 @@
                         var r = C("src"),
                             u = "toString",
                             o = ("" + b).split(u);
                         n.inspectSource = function(e) {
                             return b.call(e)
                         }, (e.exports = function(e, n, u, i) {
                             var a = "function" == typeof u;
-                            a && (g(u, "name") || v(u, "name", n)), e[n] !== u && (a && (g(u, r) || v(u, r, e[n] ? "" + e[n] : o.join(String(n)))), e === t ? e[n] = u : i ? e[n] ? e[n] = u : v(e, n, u) : (delete e[n], v(e, n, u)))
+                            a && (g(u, "name") || d(u, "name", n)), e[n] !== u && (a && (g(u, r) || d(u, r, e[n] ? "" + e[n] : o.join(String(n)))), e === t ? e[n] = u : i ? e[n] ? e[n] = u : d(e, n, u) : (delete e[n], d(e, n, u)))
                         })(Function.prototype, u, (function() {
                             return "function" == typeof this && this[r] || b.call(this)
                         }))
                     })),
                     B = function(e) {
                         if ("function" != typeof e) throw TypeError(e + " is not a function!");
                         return e
@@ -6721,17 +6767,17 @@
                     O = function(e, r, u) {
                         var o, i, a, c, s = e & O.F,
                             f = e & O.G,
                             l = e & O.S,
                             p = e & O.P,
                             D = e & O.B,
                             h = f ? t : l ? t[r] || (t[r] = {}) : (t[r] || {})[x],
-                            d = f ? n : n[r] || (n[r] = {}),
-                            y = d[x] || (d[x] = {});
-                        for (o in f && (u = r), u) i = !s && h && void 0 !== h[o], a = (i ? h : u)[o], c = D && i ? S(a, t) : p && "function" == typeof a ? S(Function.call, a) : a, h && w(h, o, a, e & O.U), d[o] != a && v(d, o, c), p && y[o] != a && (y[o] = a)
+                            v = f ? n : n[r] || (n[r] = {}),
+                            y = v[x] || (v[x] = {});
+                        for (o in f && (u = r), u) i = !s && h && void 0 !== h[o], a = (i ? h : u)[o], c = D && i ? S(a, t) : p && "function" == typeof a ? S(Function.call, a) : a, h && w(h, o, a, e & O.U), v[o] != a && d(v, o, c), p && y[o] != a && (y[o] = a)
                     };
                 t.core = n, O.F = 1, O.G = 2, O.S = 4, O.P = 8, O.B = 16, O.W = 32, O.U = 64, O.R = 128;
                 var P = O,
                     j = Math.ceil,
                     k = Math.floor,
                     I = function(e) {
                         return isNaN(e = +e) ? 0 : (e > 0 ? k : j)(e)
@@ -7073,15 +7119,15 @@
                     hexadecimalInteger: function() {
                         if (!ie.isHexDigit(te)) return De("numeric", ee * Number(Y));
                         Y += le()
                     },
                     string: function() {
                         switch (te) {
                             case "\\":
-                                return le(), void(Y += de());
+                                return le(), void(Y += ve());
                             case '"':
                                 return Q ? (le(), De("string", Y)) : void(Y += le());
                             case "'":
                                 return Q ? void(Y += le()) : (le(), De("string", Y));
                             case "\n":
                             case "\r":
                                 throw Ce(le());
@@ -7164,15 +7210,15 @@
                         var r = n[t],
                             u = fe();
                         if (u !== r) throw Ce(le());
                         le()
                     }
                 }
 
-                function de() {
+                function ve() {
                     var e = fe();
                     switch (e) {
                         case "b":
                             return le(), "\b";
                         case "f":
                             return le(), "\f";
                         case "n":
@@ -7183,15 +7229,15 @@
                             return le(), "\t";
                         case "v":
                             return le(), "\v";
                         case "0":
                             if (le(), ie.isDigit(fe())) throw Ce(le());
                             return "\0";
                         case "x":
-                            return le(), ve();
+                            return le(), de();
                         case "u":
                             return le(), ye();
                         case "\n":
                         case "\u2028":
                         case "\u2029":
                             return le(), "";
                         case "\r":
@@ -7208,15 +7254,15 @@
                             throw Ce(le());
                         case void 0:
                             throw Ce(le())
                     }
                     return le()
                 }
 
-                function ve() {
+                function de() {
                     var e = "",
                         t = fe();
                     if (!ie.isHexDigit(t)) throw Ce(le());
                     if (e += le(), t = fe(), !ie.isHexDigit(t)) throw Ce(le());
                     return e += le(), String.fromCodePoint(parseInt(e, 16))
                 }
 
@@ -7383,15 +7429,15 @@
                                 case null:
                                     return "null";
                                 case !0:
                                     return "true";
                                 case !1:
                                     return "false"
                             }
-                            return "string" === typeof n ? h(n, !1) : "number" === typeof n ? String(n) : "object" === typeof n ? Array.isArray(n) ? y(n) : d(n) : void 0
+                            return "string" === typeof n ? h(n, !1) : "number" === typeof n ? String(n) : "object" === typeof n ? Array.isArray(n) ? y(n) : v(n) : void 0
                         }
 
                         function h(e) {
                             for (var t = {
                                     "'": .1,
                                     '"': .2
                                 }, n = {
@@ -7428,37 +7474,37 @@
                             }
                             var c = o || Object.keys(t).reduce((function(e, n) {
                                 return t[e] < t[n] ? e : n
                             }));
                             return r = r.replace(new RegExp(c, "g"), n[c]), c + r + c
                         }
 
-                        function d(e) {
+                        function v(e) {
                             if (i.indexOf(e) >= 0) throw TypeError("Converting circular structure to JSON5");
                             i.push(e);
                             var t = a;
                             a += c;
                             for (var n, u, o = r || Object.keys(e), s = [], f = 0, l = o; f < l.length; f += 1) {
                                 var p = l[f],
                                     h = D(p, e);
                                 if (void 0 !== h) {
-                                    var d = v(p) + ":";
-                                    "" !== c && (d += " "), d += h, s.push(d)
+                                    var v = d(p) + ":";
+                                    "" !== c && (v += " "), v += h, s.push(v)
                                 }
                             }
                             if (0 === s.length) n = "{}";
                             else if ("" === c) u = s.join(","), n = "{" + u + "}";
                             else {
                                 var y = ",\n" + a;
                                 u = s.join(y), n = "{\n" + a + u + ",\n" + t + "}"
                             }
                             return i.pop(), a = t, n
                         }
 
-                        function v(e) {
+                        function d(e) {
                             if (0 === e.length) return h(e, !0);
                             var t = String.fromCodePoint(e.codePointAt(0));
                             if (!ie.isIdStartChar(t)) return h(e, !0);
                             for (var n = t.length; n < e.length; n++)
                                 if (!ie.isIdContinueChar(String.fromCodePoint(e.codePointAt(n)))) return h(e, !0);
                             return e
                         }
@@ -7631,21 +7677,21 @@
                     }, r.send()
                 }, e.listConnections = () => p
             }
             const h = {
                 endPoint: null
             };
 
-            function d(e, t, n = {}) {
+            function v(e, t, n = {}) {
                 Object.assign(t, h, n), l.destroy(e, t), l.event(e, t, "ProcessReady"), l.event(e, t, "ProcessStopped"), l.event(e, t, "Fetch"), l.event(e, t, "Error"), l.isA(e, t, "ProcessLauncher"), D(e, t)
             }
-            const v = l.newInstance(d);
+            const d = l.newInstance(v);
             var y = {
-                    newInstance: v,
-                    extend: d
+                    newInstance: d,
+                    extend: v
                 },
                 g = n(6559),
                 m = n.n(g);
 
             function A() {
                 const e = {};
                 return e.promise = new Promise((function(t, n) {
@@ -7684,21 +7730,21 @@
                     if (-1 !== t) {
                         const e = o[t].data;
                         return o.splice(t, 1), e
                     }
                     return console.error("Binary attachment key found without matching attachment"), null
                 }
 
-                function d(e) {
+                function v(e) {
                     for (let t in e)
                         if ("string" === typeof e[t] && c.test(e[t])) {
                             const n = e[t],
                                 r = h(n);
                             null !== r && (e[t] = r)
-                        } else "object" === typeof e[t] && d(e[t])
+                        } else "object" === typeof e[t] && v(e[t])
                 }
                 e.onconnect = e => {
                     const n = A(),
                         r = "system:c0:0";
                     return u[r] = n, t.ws.send(JSON.stringify({
                         wslink: "1.0",
                         id: r,
@@ -7794,15 +7840,15 @@
                             const e = u[r.id];
                             e ? e.reject(r.error) : console.error("Server error:", r.error)
                         } else {
                             if (r.result && o.length > 0)
                                 if ("string" === typeof r.result && c.test(r.result)) {
                                     const e = h(r.result);
                                     null !== e && (r.result = e)
-                                } else d(r.result);
+                                } else v(r.result);
                             const e = s.exec(r.id);
                             if (e) {
                                 const t = e[1];
                                 if ("rpc" === t) {
                                     const e = u[r.id];
                                     if (!e) return void console.log("session message id without matching call, dropped", r);
                                     e.resolve(r.result)
@@ -8100,8 +8146,8 @@
                     var n = Object.prototype.toString.call(e).slice(8, -1);
                     return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? (0, r.Z)(e, t) : void 0
                 }
             }
         }
     }
 ]);
-//# sourceMappingURL=chunk-vendors.ec946a94.js.map
+//# sourceMappingURL=chunk-vendors.b42af71c.js.map
```

### Comparing `trame-client-2.7.6/trame_client/module/vue2-www/logo.png` & `trame-client-2.7.7/trame_client/module/vue2-www/logo.png`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.6/trame_client/module/vue2-www/vue.global.js` & `trame-client-2.7.7/trame_client/module/vue2-www/vue.global.js`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.6/trame_client/module/vue3-www/assets/index-e4900adb.js` & `trame-client-2.7.7/trame_client/module/vue3-www/assets/index-ccad3410.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -20,19 +20,19 @@
         if (u.ep) return;
         u.ep = !0;
         const o = r(u);
         fetch(u.href, o)
     }
 })();
 
-function mr(t) {
+function wr(t) {
     if (Array.isArray(t)) return t
 }
 
-function wr(t, e) {
+function Br(t, e) {
     var r = t == null ? null : typeof Symbol < "u" && t[Symbol.iterator] || t["@@iterator"];
     if (r != null) {
         var n = [],
             u = !0,
             o = !1,
             a, i;
         try {
@@ -52,99 +52,99 @@
 
 function ze(t, e) {
     (e == null || e > t.length) && (e = t.length);
     for (var r = 0, n = new Array(e); r < e; r++) n[r] = t[r];
     return n
 }
 
-function Tt(t, e) {
+function xt(t, e) {
     if (t) {
         if (typeof t == "string") return ze(t, e);
         var r = Object.prototype.toString.call(t).slice(8, -1);
         if (r === "Object" && t.constructor && (r = t.constructor.name), r === "Map" || r === "Set") return Array.from(t);
         if (r === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return ze(t, e)
     }
 }
 
-function Br() {
+function Sr() {
     throw new TypeError(`Invalid attempt to destructure non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
 }
 
-function de(t, e) {
-    return mr(t) || wr(t, e) || Tt(t, e) || Br()
+function Fe(t, e) {
+    return wr(t) || Br(t, e) || xt(t, e) || Sr()
 }
 
-function Sr(t) {
+function br(t) {
     return t
 }
 
 function nt(t) {
     if (t === null || t === "null") return null;
     if (t === "true") return !0;
     if (t === "false") return !1;
     if (!(t === void 0 || t === "undefined")) return t[0] === "[" && t[t.length - 1] === "]" ? t.substring(1, t.length - 1).split(",").map(function(e) {
         return nt(e.trim())
     }) : t === "" || Number.isNaN(Number(t)) ? t : Number(t)
 }
 
-function br() {
+function Or() {
     var t = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : !0,
         e = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : window.location.search,
         r = {},
-        n = t ? nt : Sr,
+        n = t ? nt : br,
         u = (e || "").replace(/#.*/, "").replace("?", "").split("&");
     return u.forEach(function(o) {
         var a = o.split("=").map(function(f) {
                 return decodeURIComponent(f)
             }),
-            i = de(a, 2),
+            i = Fe(a, 2),
             c = i[0],
             s = i[1];
         c && (r[c] = s ? n(s) : !0)
     }), r
 }
 var oe = {
     toNativeType: nt,
-    extractURLParameters: br
+    extractURLParameters: Or
 };
 
 function ve(t) {
     return t.charAt(0).toUpperCase() + t.slice(1)
 }
 
-function Or(t, e = {}, r = null) {
+function Tr(t, e = {}, r = null) {
     e.isA || (e.isA = []), r && e.isA.push(r), t.isA || (t.isA = n => e.isA.indexOf(n) !== -1)
 }
 
-function Tr(t, e = {}, r = []) {
+function xr(t, e = {}, r = []) {
     r.forEach(n => {
         t[`set${ve(n)}`] = u => {
             e[n] = u
         }
     })
 }
 
-function xr(t, e = {}, r = []) {
+function jr(t, e = {}, r = []) {
     r.forEach(n => {
         t[`get${ve(n)}`] = () => e[n]
     })
 }
 
-function jr(t, e = {}) {
+function Rr(t, e = {}) {
     const r = t.destroy;
     e.subscriptions || (e.subscriptions = []), t.destroy = () => {
         for (r && r(); e.subscriptions && e.subscriptions.length;) e.subscriptions.pop().unsubscribe();
         Object.keys(e).forEach(n => {
             delete e[n]
         }), e.deleted = !0
     }
 }
 
-function Rr(t, e, r, n = !0) {
+function Lr(t, e, r, n = !0) {
     const u = [],
         o = t.destroy;
 
     function a(c) {
         u[c] = null
     }
 
@@ -177,37 +177,37 @@
         const s = u.length;
         return u.push(c), i(s)
     }, t.destroy = () => {
         o(), u.forEach((c, s) => a(s))
     }
 }
 
-function Lr(...t) {
+function kr(...t) {
     return (...e) => t.filter(r => !!r).forEach(r => r(...e))
 }
 
-function kr(t) {
+function _r(t) {
     return (e = {}) => {
         const r = {},
             n = {};
         return t(n, r, e), Object.freeze(n)
     }
 }
 const b = {
-        chain: Lr,
-        destroy: jr,
-        event: Rr,
-        get: xr,
-        isA: Or,
-        newInstance: kr,
-        set: Tr
+        chain: kr,
+        destroy: Rr,
+        event: Lr,
+        get: jr,
+        isA: Tr,
+        newInstance: _r,
+        set: xr
     },
     st = [];
 
-function _r(t, e) {
+function Ur(t, e) {
     t.start = r => {
         var n = new XMLHttpRequest,
             u = e.endPoint;
         n.open("POST", u, !0), r.headers && (Object.entries(r.headers).forEach(([a, i]) => n.setRequestHeader(a, i)), delete r.headers), n.responseType = "json";
         const o = "response" in n && n.responseType === "json";
         n.onload = a => {
             const i = o ? n.response : JSON.parse(n.response);
@@ -246,33 +246,33 @@
             }
             t.fireError(n)
         }, n.onerror = a => {
             t.fireError(n)
         }, n.send()
     }, t.listConnections = () => st
 }
-const Ur = {
+const $r = {
     endPoint: null
 };
 
-function xt(t, e, r = {}) {
-    Object.assign(e, Ur, r), b.destroy(t, e), b.event(t, e, "ProcessReady"), b.event(t, e, "ProcessStopped"), b.event(t, e, "Fetch"), b.event(t, e, "Error"), b.isA(t, e, "ProcessLauncher"), _r(t, e)
+function jt(t, e, r = {}) {
+    Object.assign(e, $r, r), b.destroy(t, e), b.event(t, e, "ProcessReady"), b.event(t, e, "ProcessStopped"), b.event(t, e, "Fetch"), b.event(t, e, "Error"), b.isA(t, e, "ProcessLauncher"), Ur(t, e)
 }
-const $r = b.newInstance(xt),
-    Nr = {
-        newInstance: $r,
-        extend: xt
+const Nr = b.newInstance(jt),
+    Mr = {
+        newInstance: Nr,
+        extend: jt
     };
-var Mr = /[\u1680\u2000-\u200A\u202F\u205F\u3000]/,
-    Pr = /[\xAA\xB5\xBA\xC0-\xD6\xD8-\xF6\xF8-\u02C1\u02C6-\u02D1\u02E0-\u02E4\u02EC\u02EE\u0370-\u0374\u0376\u0377\u037A-\u037D\u037F\u0386\u0388-\u038A\u038C\u038E-\u03A1\u03A3-\u03F5\u03F7-\u0481\u048A-\u052F\u0531-\u0556\u0559\u0561-\u0587\u05D0-\u05EA\u05F0-\u05F2\u0620-\u064A\u066E\u066F\u0671-\u06D3\u06D5\u06E5\u06E6\u06EE\u06EF\u06FA-\u06FC\u06FF\u0710\u0712-\u072F\u074D-\u07A5\u07B1\u07CA-\u07EA\u07F4\u07F5\u07FA\u0800-\u0815\u081A\u0824\u0828\u0840-\u0858\u0860-\u086A\u08A0-\u08B4\u08B6-\u08BD\u0904-\u0939\u093D\u0950\u0958-\u0961\u0971-\u0980\u0985-\u098C\u098F\u0990\u0993-\u09A8\u09AA-\u09B0\u09B2\u09B6-\u09B9\u09BD\u09CE\u09DC\u09DD\u09DF-\u09E1\u09F0\u09F1\u09FC\u0A05-\u0A0A\u0A0F\u0A10\u0A13-\u0A28\u0A2A-\u0A30\u0A32\u0A33\u0A35\u0A36\u0A38\u0A39\u0A59-\u0A5C\u0A5E\u0A72-\u0A74\u0A85-\u0A8D\u0A8F-\u0A91\u0A93-\u0AA8\u0AAA-\u0AB0\u0AB2\u0AB3\u0AB5-\u0AB9\u0ABD\u0AD0\u0AE0\u0AE1\u0AF9\u0B05-\u0B0C\u0B0F\u0B10\u0B13-\u0B28\u0B2A-\u0B30\u0B32\u0B33\u0B35-\u0B39\u0B3D\u0B5C\u0B5D\u0B5F-\u0B61\u0B71\u0B83\u0B85-\u0B8A\u0B8E-\u0B90\u0B92-\u0B95\u0B99\u0B9A\u0B9C\u0B9E\u0B9F\u0BA3\u0BA4\u0BA8-\u0BAA\u0BAE-\u0BB9\u0BD0\u0C05-\u0C0C\u0C0E-\u0C10\u0C12-\u0C28\u0C2A-\u0C39\u0C3D\u0C58-\u0C5A\u0C60\u0C61\u0C80\u0C85-\u0C8C\u0C8E-\u0C90\u0C92-\u0CA8\u0CAA-\u0CB3\u0CB5-\u0CB9\u0CBD\u0CDE\u0CE0\u0CE1\u0CF1\u0CF2\u0D05-\u0D0C\u0D0E-\u0D10\u0D12-\u0D3A\u0D3D\u0D4E\u0D54-\u0D56\u0D5F-\u0D61\u0D7A-\u0D7F\u0D85-\u0D96\u0D9A-\u0DB1\u0DB3-\u0DBB\u0DBD\u0DC0-\u0DC6\u0E01-\u0E30\u0E32\u0E33\u0E40-\u0E46\u0E81\u0E82\u0E84\u0E87\u0E88\u0E8A\u0E8D\u0E94-\u0E97\u0E99-\u0E9F\u0EA1-\u0EA3\u0EA5\u0EA7\u0EAA\u0EAB\u0EAD-\u0EB0\u0EB2\u0EB3\u0EBD\u0EC0-\u0EC4\u0EC6\u0EDC-\u0EDF\u0F00\u0F40-\u0F47\u0F49-\u0F6C\u0F88-\u0F8C\u1000-\u102A\u103F\u1050-\u1055\u105A-\u105D\u1061\u1065\u1066\u106E-\u1070\u1075-\u1081\u108E\u10A0-\u10C5\u10C7\u10CD\u10D0-\u10FA\u10FC-\u1248\u124A-\u124D\u1250-\u1256\u1258\u125A-\u125D\u1260-\u1288\u128A-\u128D\u1290-\u12B0\u12B2-\u12B5\u12B8-\u12BE\u12C0\u12C2-\u12C5\u12C8-\u12D6\u12D8-\u1310\u1312-\u1315\u1318-\u135A\u1380-\u138F\u13A0-\u13F5\u13F8-\u13FD\u1401-\u166C\u166F-\u167F\u1681-\u169A\u16A0-\u16EA\u16EE-\u16F8\u1700-\u170C\u170E-\u1711\u1720-\u1731\u1740-\u1751\u1760-\u176C\u176E-\u1770\u1780-\u17B3\u17D7\u17DC\u1820-\u1877\u1880-\u1884\u1887-\u18A8\u18AA\u18B0-\u18F5\u1900-\u191E\u1950-\u196D\u1970-\u1974\u1980-\u19AB\u19B0-\u19C9\u1A00-\u1A16\u1A20-\u1A54\u1AA7\u1B05-\u1B33\u1B45-\u1B4B\u1B83-\u1BA0\u1BAE\u1BAF\u1BBA-\u1BE5\u1C00-\u1C23\u1C4D-\u1C4F\u1C5A-\u1C7D\u1C80-\u1C88\u1CE9-\u1CEC\u1CEE-\u1CF1\u1CF5\u1CF6\u1D00-\u1DBF\u1E00-\u1F15\u1F18-\u1F1D\u1F20-\u1F45\u1F48-\u1F4D\u1F50-\u1F57\u1F59\u1F5B\u1F5D\u1F5F-\u1F7D\u1F80-\u1FB4\u1FB6-\u1FBC\u1FBE\u1FC2-\u1FC4\u1FC6-\u1FCC\u1FD0-\u1FD3\u1FD6-\u1FDB\u1FE0-\u1FEC\u1FF2-\u1FF4\u1FF6-\u1FFC\u2071\u207F\u2090-\u209C\u2102\u2107\u210A-\u2113\u2115\u2119-\u211D\u2124\u2126\u2128\u212A-\u212D\u212F-\u2139\u213C-\u213F\u2145-\u2149\u214E\u2160-\u2188\u2C00-\u2C2E\u2C30-\u2C5E\u2C60-\u2CE4\u2CEB-\u2CEE\u2CF2\u2CF3\u2D00-\u2D25\u2D27\u2D2D\u2D30-\u2D67\u2D6F\u2D80-\u2D96\u2DA0-\u2DA6\u2DA8-\u2DAE\u2DB0-\u2DB6\u2DB8-\u2DBE\u2DC0-\u2DC6\u2DC8-\u2DCE\u2DD0-\u2DD6\u2DD8-\u2DDE\u2E2F\u3005-\u3007\u3021-\u3029\u3031-\u3035\u3038-\u303C\u3041-\u3096\u309D-\u309F\u30A1-\u30FA\u30FC-\u30FF\u3105-\u312E\u3131-\u318E\u31A0-\u31BA\u31F0-\u31FF\u3400-\u4DB5\u4E00-\u9FEA\uA000-\uA48C\uA4D0-\uA4FD\uA500-\uA60C\uA610-\uA61F\uA62A\uA62B\uA640-\uA66E\uA67F-\uA69D\uA6A0-\uA6EF\uA717-\uA71F\uA722-\uA788\uA78B-\uA7AE\uA7B0-\uA7B7\uA7F7-\uA801\uA803-\uA805\uA807-\uA80A\uA80C-\uA822\uA840-\uA873\uA882-\uA8B3\uA8F2-\uA8F7\uA8FB\uA8FD\uA90A-\uA925\uA930-\uA946\uA960-\uA97C\uA984-\uA9B2\uA9CF\uA9E0-\uA9E4\uA9E6-\uA9EF\uA9FA-\uA9FE\uAA00-\uAA28\uAA40-\uAA42\uAA44-\uAA4B\uAA60-\uAA76\uAA7A\uAA7E-\uAAAF\uAAB1\uAAB5\uAAB6\uAAB9-\uAABD\uAAC0\uAAC2\uAADB-\uAADD\uAAE0-\uAAEA\uAAF2-\uAAF4\uAB01-\uAB06\uAB09-\uAB0E\uAB11-\uAB16\uAB20-\uAB26\uAB28-\uAB2E\uAB30-\uAB5A\uAB5C-\uAB65\uAB70-\uABE2\uAC00-\uD7A3\uD7B0-\uD7C6\uD7CB-\uD7FB\uF900-\uFA6D\uFA70-\uFAD9\uFB00-\uFB06\uFB13-\uFB17\uFB1D\uFB1F-\uFB28\uFB2A-\uFB36\uFB38-\uFB3C\uFB3E\uFB40\uFB41\uFB43\uFB44\uFB46-\uFBB1\uFBD3-\uFD3D\uFD50-\uFD8F\uFD92-\uFDC7\uFDF0-\uFDFB\uFE70-\uFE74\uFE76-\uFEFC\uFF21-\uFF3A\uFF41-\uFF5A\uFF66-\uFFBE\uFFC2-\uFFC7\uFFCA-\uFFCF\uFFD2-\uFFD7\uFFDA-\uFFDC]|\uD800[\uDC00-\uDC0B\uDC0D-\uDC26\uDC28-\uDC3A\uDC3C\uDC3D\uDC3F-\uDC4D\uDC50-\uDC5D\uDC80-\uDCFA\uDD40-\uDD74\uDE80-\uDE9C\uDEA0-\uDED0\uDF00-\uDF1F\uDF2D-\uDF4A\uDF50-\uDF75\uDF80-\uDF9D\uDFA0-\uDFC3\uDFC8-\uDFCF\uDFD1-\uDFD5]|\uD801[\uDC00-\uDC9D\uDCB0-\uDCD3\uDCD8-\uDCFB\uDD00-\uDD27\uDD30-\uDD63\uDE00-\uDF36\uDF40-\uDF55\uDF60-\uDF67]|\uD802[\uDC00-\uDC05\uDC08\uDC0A-\uDC35\uDC37\uDC38\uDC3C\uDC3F-\uDC55\uDC60-\uDC76\uDC80-\uDC9E\uDCE0-\uDCF2\uDCF4\uDCF5\uDD00-\uDD15\uDD20-\uDD39\uDD80-\uDDB7\uDDBE\uDDBF\uDE00\uDE10-\uDE13\uDE15-\uDE17\uDE19-\uDE33\uDE60-\uDE7C\uDE80-\uDE9C\uDEC0-\uDEC7\uDEC9-\uDEE4\uDF00-\uDF35\uDF40-\uDF55\uDF60-\uDF72\uDF80-\uDF91]|\uD803[\uDC00-\uDC48\uDC80-\uDCB2\uDCC0-\uDCF2]|\uD804[\uDC03-\uDC37\uDC83-\uDCAF\uDCD0-\uDCE8\uDD03-\uDD26\uDD50-\uDD72\uDD76\uDD83-\uDDB2\uDDC1-\uDDC4\uDDDA\uDDDC\uDE00-\uDE11\uDE13-\uDE2B\uDE80-\uDE86\uDE88\uDE8A-\uDE8D\uDE8F-\uDE9D\uDE9F-\uDEA8\uDEB0-\uDEDE\uDF05-\uDF0C\uDF0F\uDF10\uDF13-\uDF28\uDF2A-\uDF30\uDF32\uDF33\uDF35-\uDF39\uDF3D\uDF50\uDF5D-\uDF61]|\uD805[\uDC00-\uDC34\uDC47-\uDC4A\uDC80-\uDCAF\uDCC4\uDCC5\uDCC7\uDD80-\uDDAE\uDDD8-\uDDDB\uDE00-\uDE2F\uDE44\uDE80-\uDEAA\uDF00-\uDF19]|\uD806[\uDCA0-\uDCDF\uDCFF\uDE00\uDE0B-\uDE32\uDE3A\uDE50\uDE5C-\uDE83\uDE86-\uDE89\uDEC0-\uDEF8]|\uD807[\uDC00-\uDC08\uDC0A-\uDC2E\uDC40\uDC72-\uDC8F\uDD00-\uDD06\uDD08\uDD09\uDD0B-\uDD30\uDD46]|\uD808[\uDC00-\uDF99]|\uD809[\uDC00-\uDC6E\uDC80-\uDD43]|[\uD80C\uD81C-\uD820\uD840-\uD868\uD86A-\uD86C\uD86F-\uD872\uD874-\uD879][\uDC00-\uDFFF]|\uD80D[\uDC00-\uDC2E]|\uD811[\uDC00-\uDE46]|\uD81A[\uDC00-\uDE38\uDE40-\uDE5E\uDED0-\uDEED\uDF00-\uDF2F\uDF40-\uDF43\uDF63-\uDF77\uDF7D-\uDF8F]|\uD81B[\uDF00-\uDF44\uDF50\uDF93-\uDF9F\uDFE0\uDFE1]|\uD821[\uDC00-\uDFEC]|\uD822[\uDC00-\uDEF2]|\uD82C[\uDC00-\uDD1E\uDD70-\uDEFB]|\uD82F[\uDC00-\uDC6A\uDC70-\uDC7C\uDC80-\uDC88\uDC90-\uDC99]|\uD835[\uDC00-\uDC54\uDC56-\uDC9C\uDC9E\uDC9F\uDCA2\uDCA5\uDCA6\uDCA9-\uDCAC\uDCAE-\uDCB9\uDCBB\uDCBD-\uDCC3\uDCC5-\uDD05\uDD07-\uDD0A\uDD0D-\uDD14\uDD16-\uDD1C\uDD1E-\uDD39\uDD3B-\uDD3E\uDD40-\uDD44\uDD46\uDD4A-\uDD50\uDD52-\uDEA5\uDEA8-\uDEC0\uDEC2-\uDEDA\uDEDC-\uDEFA\uDEFC-\uDF14\uDF16-\uDF34\uDF36-\uDF4E\uDF50-\uDF6E\uDF70-\uDF88\uDF8A-\uDFA8\uDFAA-\uDFC2\uDFC4-\uDFCB]|\uD83A[\uDC00-\uDCC4\uDD00-\uDD43]|\uD83B[\uDE00-\uDE03\uDE05-\uDE1F\uDE21\uDE22\uDE24\uDE27\uDE29-\uDE32\uDE34-\uDE37\uDE39\uDE3B\uDE42\uDE47\uDE49\uDE4B\uDE4D-\uDE4F\uDE51\uDE52\uDE54\uDE57\uDE59\uDE5B\uDE5D\uDE5F\uDE61\uDE62\uDE64\uDE67-\uDE6A\uDE6C-\uDE72\uDE74-\uDE77\uDE79-\uDE7C\uDE7E\uDE80-\uDE89\uDE8B-\uDE9B\uDEA1-\uDEA3\uDEA5-\uDEA9\uDEAB-\uDEBB]|\uD869[\uDC00-\uDED6\uDF00-\uDFFF]|\uD86D[\uDC00-\uDF34\uDF40-\uDFFF]|\uD86E[\uDC00-\uDC1D\uDC20-\uDFFF]|\uD873[\uDC00-\uDEA1\uDEB0-\uDFFF]|\uD87A[\uDC00-\uDFE0]|\uD87E[\uDC00-\uDE1D]/,
-    Vr = /[\xAA\xB5\xBA\xC0-\xD6\xD8-\xF6\xF8-\u02C1\u02C6-\u02D1\u02E0-\u02E4\u02EC\u02EE\u0300-\u0374\u0376\u0377\u037A-\u037D\u037F\u0386\u0388-\u038A\u038C\u038E-\u03A1\u03A3-\u03F5\u03F7-\u0481\u0483-\u0487\u048A-\u052F\u0531-\u0556\u0559\u0561-\u0587\u0591-\u05BD\u05BF\u05C1\u05C2\u05C4\u05C5\u05C7\u05D0-\u05EA\u05F0-\u05F2\u0610-\u061A\u0620-\u0669\u066E-\u06D3\u06D5-\u06DC\u06DF-\u06E8\u06EA-\u06FC\u06FF\u0710-\u074A\u074D-\u07B1\u07C0-\u07F5\u07FA\u0800-\u082D\u0840-\u085B\u0860-\u086A\u08A0-\u08B4\u08B6-\u08BD\u08D4-\u08E1\u08E3-\u0963\u0966-\u096F\u0971-\u0983\u0985-\u098C\u098F\u0990\u0993-\u09A8\u09AA-\u09B0\u09B2\u09B6-\u09B9\u09BC-\u09C4\u09C7\u09C8\u09CB-\u09CE\u09D7\u09DC\u09DD\u09DF-\u09E3\u09E6-\u09F1\u09FC\u0A01-\u0A03\u0A05-\u0A0A\u0A0F\u0A10\u0A13-\u0A28\u0A2A-\u0A30\u0A32\u0A33\u0A35\u0A36\u0A38\u0A39\u0A3C\u0A3E-\u0A42\u0A47\u0A48\u0A4B-\u0A4D\u0A51\u0A59-\u0A5C\u0A5E\u0A66-\u0A75\u0A81-\u0A83\u0A85-\u0A8D\u0A8F-\u0A91\u0A93-\u0AA8\u0AAA-\u0AB0\u0AB2\u0AB3\u0AB5-\u0AB9\u0ABC-\u0AC5\u0AC7-\u0AC9\u0ACB-\u0ACD\u0AD0\u0AE0-\u0AE3\u0AE6-\u0AEF\u0AF9-\u0AFF\u0B01-\u0B03\u0B05-\u0B0C\u0B0F\u0B10\u0B13-\u0B28\u0B2A-\u0B30\u0B32\u0B33\u0B35-\u0B39\u0B3C-\u0B44\u0B47\u0B48\u0B4B-\u0B4D\u0B56\u0B57\u0B5C\u0B5D\u0B5F-\u0B63\u0B66-\u0B6F\u0B71\u0B82\u0B83\u0B85-\u0B8A\u0B8E-\u0B90\u0B92-\u0B95\u0B99\u0B9A\u0B9C\u0B9E\u0B9F\u0BA3\u0BA4\u0BA8-\u0BAA\u0BAE-\u0BB9\u0BBE-\u0BC2\u0BC6-\u0BC8\u0BCA-\u0BCD\u0BD0\u0BD7\u0BE6-\u0BEF\u0C00-\u0C03\u0C05-\u0C0C\u0C0E-\u0C10\u0C12-\u0C28\u0C2A-\u0C39\u0C3D-\u0C44\u0C46-\u0C48\u0C4A-\u0C4D\u0C55\u0C56\u0C58-\u0C5A\u0C60-\u0C63\u0C66-\u0C6F\u0C80-\u0C83\u0C85-\u0C8C\u0C8E-\u0C90\u0C92-\u0CA8\u0CAA-\u0CB3\u0CB5-\u0CB9\u0CBC-\u0CC4\u0CC6-\u0CC8\u0CCA-\u0CCD\u0CD5\u0CD6\u0CDE\u0CE0-\u0CE3\u0CE6-\u0CEF\u0CF1\u0CF2\u0D00-\u0D03\u0D05-\u0D0C\u0D0E-\u0D10\u0D12-\u0D44\u0D46-\u0D48\u0D4A-\u0D4E\u0D54-\u0D57\u0D5F-\u0D63\u0D66-\u0D6F\u0D7A-\u0D7F\u0D82\u0D83\u0D85-\u0D96\u0D9A-\u0DB1\u0DB3-\u0DBB\u0DBD\u0DC0-\u0DC6\u0DCA\u0DCF-\u0DD4\u0DD6\u0DD8-\u0DDF\u0DE6-\u0DEF\u0DF2\u0DF3\u0E01-\u0E3A\u0E40-\u0E4E\u0E50-\u0E59\u0E81\u0E82\u0E84\u0E87\u0E88\u0E8A\u0E8D\u0E94-\u0E97\u0E99-\u0E9F\u0EA1-\u0EA3\u0EA5\u0EA7\u0EAA\u0EAB\u0EAD-\u0EB9\u0EBB-\u0EBD\u0EC0-\u0EC4\u0EC6\u0EC8-\u0ECD\u0ED0-\u0ED9\u0EDC-\u0EDF\u0F00\u0F18\u0F19\u0F20-\u0F29\u0F35\u0F37\u0F39\u0F3E-\u0F47\u0F49-\u0F6C\u0F71-\u0F84\u0F86-\u0F97\u0F99-\u0FBC\u0FC6\u1000-\u1049\u1050-\u109D\u10A0-\u10C5\u10C7\u10CD\u10D0-\u10FA\u10FC-\u1248\u124A-\u124D\u1250-\u1256\u1258\u125A-\u125D\u1260-\u1288\u128A-\u128D\u1290-\u12B0\u12B2-\u12B5\u12B8-\u12BE\u12C0\u12C2-\u12C5\u12C8-\u12D6\u12D8-\u1310\u1312-\u1315\u1318-\u135A\u135D-\u135F\u1380-\u138F\u13A0-\u13F5\u13F8-\u13FD\u1401-\u166C\u166F-\u167F\u1681-\u169A\u16A0-\u16EA\u16EE-\u16F8\u1700-\u170C\u170E-\u1714\u1720-\u1734\u1740-\u1753\u1760-\u176C\u176E-\u1770\u1772\u1773\u1780-\u17D3\u17D7\u17DC\u17DD\u17E0-\u17E9\u180B-\u180D\u1810-\u1819\u1820-\u1877\u1880-\u18AA\u18B0-\u18F5\u1900-\u191E\u1920-\u192B\u1930-\u193B\u1946-\u196D\u1970-\u1974\u1980-\u19AB\u19B0-\u19C9\u19D0-\u19D9\u1A00-\u1A1B\u1A20-\u1A5E\u1A60-\u1A7C\u1A7F-\u1A89\u1A90-\u1A99\u1AA7\u1AB0-\u1ABD\u1B00-\u1B4B\u1B50-\u1B59\u1B6B-\u1B73\u1B80-\u1BF3\u1C00-\u1C37\u1C40-\u1C49\u1C4D-\u1C7D\u1C80-\u1C88\u1CD0-\u1CD2\u1CD4-\u1CF9\u1D00-\u1DF9\u1DFB-\u1F15\u1F18-\u1F1D\u1F20-\u1F45\u1F48-\u1F4D\u1F50-\u1F57\u1F59\u1F5B\u1F5D\u1F5F-\u1F7D\u1F80-\u1FB4\u1FB6-\u1FBC\u1FBE\u1FC2-\u1FC4\u1FC6-\u1FCC\u1FD0-\u1FD3\u1FD6-\u1FDB\u1FE0-\u1FEC\u1FF2-\u1FF4\u1FF6-\u1FFC\u203F\u2040\u2054\u2071\u207F\u2090-\u209C\u20D0-\u20DC\u20E1\u20E5-\u20F0\u2102\u2107\u210A-\u2113\u2115\u2119-\u211D\u2124\u2126\u2128\u212A-\u212D\u212F-\u2139\u213C-\u213F\u2145-\u2149\u214E\u2160-\u2188\u2C00-\u2C2E\u2C30-\u2C5E\u2C60-\u2CE4\u2CEB-\u2CF3\u2D00-\u2D25\u2D27\u2D2D\u2D30-\u2D67\u2D6F\u2D7F-\u2D96\u2DA0-\u2DA6\u2DA8-\u2DAE\u2DB0-\u2DB6\u2DB8-\u2DBE\u2DC0-\u2DC6\u2DC8-\u2DCE\u2DD0-\u2DD6\u2DD8-\u2DDE\u2DE0-\u2DFF\u2E2F\u3005-\u3007\u3021-\u302F\u3031-\u3035\u3038-\u303C\u3041-\u3096\u3099\u309A\u309D-\u309F\u30A1-\u30FA\u30FC-\u30FF\u3105-\u312E\u3131-\u318E\u31A0-\u31BA\u31F0-\u31FF\u3400-\u4DB5\u4E00-\u9FEA\uA000-\uA48C\uA4D0-\uA4FD\uA500-\uA60C\uA610-\uA62B\uA640-\uA66F\uA674-\uA67D\uA67F-\uA6F1\uA717-\uA71F\uA722-\uA788\uA78B-\uA7AE\uA7B0-\uA7B7\uA7F7-\uA827\uA840-\uA873\uA880-\uA8C5\uA8D0-\uA8D9\uA8E0-\uA8F7\uA8FB\uA8FD\uA900-\uA92D\uA930-\uA953\uA960-\uA97C\uA980-\uA9C0\uA9CF-\uA9D9\uA9E0-\uA9FE\uAA00-\uAA36\uAA40-\uAA4D\uAA50-\uAA59\uAA60-\uAA76\uAA7A-\uAAC2\uAADB-\uAADD\uAAE0-\uAAEF\uAAF2-\uAAF6\uAB01-\uAB06\uAB09-\uAB0E\uAB11-\uAB16\uAB20-\uAB26\uAB28-\uAB2E\uAB30-\uAB5A\uAB5C-\uAB65\uAB70-\uABEA\uABEC\uABED\uABF0-\uABF9\uAC00-\uD7A3\uD7B0-\uD7C6\uD7CB-\uD7FB\uF900-\uFA6D\uFA70-\uFAD9\uFB00-\uFB06\uFB13-\uFB17\uFB1D-\uFB28\uFB2A-\uFB36\uFB38-\uFB3C\uFB3E\uFB40\uFB41\uFB43\uFB44\uFB46-\uFBB1\uFBD3-\uFD3D\uFD50-\uFD8F\uFD92-\uFDC7\uFDF0-\uFDFB\uFE00-\uFE0F\uFE20-\uFE2F\uFE33\uFE34\uFE4D-\uFE4F\uFE70-\uFE74\uFE76-\uFEFC\uFF10-\uFF19\uFF21-\uFF3A\uFF3F\uFF41-\uFF5A\uFF66-\uFFBE\uFFC2-\uFFC7\uFFCA-\uFFCF\uFFD2-\uFFD7\uFFDA-\uFFDC]|\uD800[\uDC00-\uDC0B\uDC0D-\uDC26\uDC28-\uDC3A\uDC3C\uDC3D\uDC3F-\uDC4D\uDC50-\uDC5D\uDC80-\uDCFA\uDD40-\uDD74\uDDFD\uDE80-\uDE9C\uDEA0-\uDED0\uDEE0\uDF00-\uDF1F\uDF2D-\uDF4A\uDF50-\uDF7A\uDF80-\uDF9D\uDFA0-\uDFC3\uDFC8-\uDFCF\uDFD1-\uDFD5]|\uD801[\uDC00-\uDC9D\uDCA0-\uDCA9\uDCB0-\uDCD3\uDCD8-\uDCFB\uDD00-\uDD27\uDD30-\uDD63\uDE00-\uDF36\uDF40-\uDF55\uDF60-\uDF67]|\uD802[\uDC00-\uDC05\uDC08\uDC0A-\uDC35\uDC37\uDC38\uDC3C\uDC3F-\uDC55\uDC60-\uDC76\uDC80-\uDC9E\uDCE0-\uDCF2\uDCF4\uDCF5\uDD00-\uDD15\uDD20-\uDD39\uDD80-\uDDB7\uDDBE\uDDBF\uDE00-\uDE03\uDE05\uDE06\uDE0C-\uDE13\uDE15-\uDE17\uDE19-\uDE33\uDE38-\uDE3A\uDE3F\uDE60-\uDE7C\uDE80-\uDE9C\uDEC0-\uDEC7\uDEC9-\uDEE6\uDF00-\uDF35\uDF40-\uDF55\uDF60-\uDF72\uDF80-\uDF91]|\uD803[\uDC00-\uDC48\uDC80-\uDCB2\uDCC0-\uDCF2]|\uD804[\uDC00-\uDC46\uDC66-\uDC6F\uDC7F-\uDCBA\uDCD0-\uDCE8\uDCF0-\uDCF9\uDD00-\uDD34\uDD36-\uDD3F\uDD50-\uDD73\uDD76\uDD80-\uDDC4\uDDCA-\uDDCC\uDDD0-\uDDDA\uDDDC\uDE00-\uDE11\uDE13-\uDE37\uDE3E\uDE80-\uDE86\uDE88\uDE8A-\uDE8D\uDE8F-\uDE9D\uDE9F-\uDEA8\uDEB0-\uDEEA\uDEF0-\uDEF9\uDF00-\uDF03\uDF05-\uDF0C\uDF0F\uDF10\uDF13-\uDF28\uDF2A-\uDF30\uDF32\uDF33\uDF35-\uDF39\uDF3C-\uDF44\uDF47\uDF48\uDF4B-\uDF4D\uDF50\uDF57\uDF5D-\uDF63\uDF66-\uDF6C\uDF70-\uDF74]|\uD805[\uDC00-\uDC4A\uDC50-\uDC59\uDC80-\uDCC5\uDCC7\uDCD0-\uDCD9\uDD80-\uDDB5\uDDB8-\uDDC0\uDDD8-\uDDDD\uDE00-\uDE40\uDE44\uDE50-\uDE59\uDE80-\uDEB7\uDEC0-\uDEC9\uDF00-\uDF19\uDF1D-\uDF2B\uDF30-\uDF39]|\uD806[\uDCA0-\uDCE9\uDCFF\uDE00-\uDE3E\uDE47\uDE50-\uDE83\uDE86-\uDE99\uDEC0-\uDEF8]|\uD807[\uDC00-\uDC08\uDC0A-\uDC36\uDC38-\uDC40\uDC50-\uDC59\uDC72-\uDC8F\uDC92-\uDCA7\uDCA9-\uDCB6\uDD00-\uDD06\uDD08\uDD09\uDD0B-\uDD36\uDD3A\uDD3C\uDD3D\uDD3F-\uDD47\uDD50-\uDD59]|\uD808[\uDC00-\uDF99]|\uD809[\uDC00-\uDC6E\uDC80-\uDD43]|[\uD80C\uD81C-\uD820\uD840-\uD868\uD86A-\uD86C\uD86F-\uD872\uD874-\uD879][\uDC00-\uDFFF]|\uD80D[\uDC00-\uDC2E]|\uD811[\uDC00-\uDE46]|\uD81A[\uDC00-\uDE38\uDE40-\uDE5E\uDE60-\uDE69\uDED0-\uDEED\uDEF0-\uDEF4\uDF00-\uDF36\uDF40-\uDF43\uDF50-\uDF59\uDF63-\uDF77\uDF7D-\uDF8F]|\uD81B[\uDF00-\uDF44\uDF50-\uDF7E\uDF8F-\uDF9F\uDFE0\uDFE1]|\uD821[\uDC00-\uDFEC]|\uD822[\uDC00-\uDEF2]|\uD82C[\uDC00-\uDD1E\uDD70-\uDEFB]|\uD82F[\uDC00-\uDC6A\uDC70-\uDC7C\uDC80-\uDC88\uDC90-\uDC99\uDC9D\uDC9E]|\uD834[\uDD65-\uDD69\uDD6D-\uDD72\uDD7B-\uDD82\uDD85-\uDD8B\uDDAA-\uDDAD\uDE42-\uDE44]|\uD835[\uDC00-\uDC54\uDC56-\uDC9C\uDC9E\uDC9F\uDCA2\uDCA5\uDCA6\uDCA9-\uDCAC\uDCAE-\uDCB9\uDCBB\uDCBD-\uDCC3\uDCC5-\uDD05\uDD07-\uDD0A\uDD0D-\uDD14\uDD16-\uDD1C\uDD1E-\uDD39\uDD3B-\uDD3E\uDD40-\uDD44\uDD46\uDD4A-\uDD50\uDD52-\uDEA5\uDEA8-\uDEC0\uDEC2-\uDEDA\uDEDC-\uDEFA\uDEFC-\uDF14\uDF16-\uDF34\uDF36-\uDF4E\uDF50-\uDF6E\uDF70-\uDF88\uDF8A-\uDFA8\uDFAA-\uDFC2\uDFC4-\uDFCB\uDFCE-\uDFFF]|\uD836[\uDE00-\uDE36\uDE3B-\uDE6C\uDE75\uDE84\uDE9B-\uDE9F\uDEA1-\uDEAF]|\uD838[\uDC00-\uDC06\uDC08-\uDC18\uDC1B-\uDC21\uDC23\uDC24\uDC26-\uDC2A]|\uD83A[\uDC00-\uDCC4\uDCD0-\uDCD6\uDD00-\uDD4A\uDD50-\uDD59]|\uD83B[\uDE00-\uDE03\uDE05-\uDE1F\uDE21\uDE22\uDE24\uDE27\uDE29-\uDE32\uDE34-\uDE37\uDE39\uDE3B\uDE42\uDE47\uDE49\uDE4B\uDE4D-\uDE4F\uDE51\uDE52\uDE54\uDE57\uDE59\uDE5B\uDE5D\uDE5F\uDE61\uDE62\uDE64\uDE67-\uDE6A\uDE6C-\uDE72\uDE74-\uDE77\uDE79-\uDE7C\uDE7E\uDE80-\uDE89\uDE8B-\uDE9B\uDEA1-\uDEA3\uDEA5-\uDEA9\uDEAB-\uDEBB]|\uD869[\uDC00-\uDED6\uDF00-\uDFFF]|\uD86D[\uDC00-\uDF34\uDF40-\uDFFF]|\uD86E[\uDC00-\uDC1D\uDC20-\uDFFF]|\uD873[\uDC00-\uDEA1\uDEB0-\uDFFF]|\uD87A[\uDC00-\uDFE0]|\uD87E[\uDC00-\uDE1D]|\uDB40[\uDD00-\uDDEF]/,
+var Pr = /[\u1680\u2000-\u200A\u202F\u205F\u3000]/,
+    Vr = /[\xAA\xB5\xBA\xC0-\xD6\xD8-\xF6\xF8-\u02C1\u02C6-\u02D1\u02E0-\u02E4\u02EC\u02EE\u0370-\u0374\u0376\u0377\u037A-\u037D\u037F\u0386\u0388-\u038A\u038C\u038E-\u03A1\u03A3-\u03F5\u03F7-\u0481\u048A-\u052F\u0531-\u0556\u0559\u0561-\u0587\u05D0-\u05EA\u05F0-\u05F2\u0620-\u064A\u066E\u066F\u0671-\u06D3\u06D5\u06E5\u06E6\u06EE\u06EF\u06FA-\u06FC\u06FF\u0710\u0712-\u072F\u074D-\u07A5\u07B1\u07CA-\u07EA\u07F4\u07F5\u07FA\u0800-\u0815\u081A\u0824\u0828\u0840-\u0858\u0860-\u086A\u08A0-\u08B4\u08B6-\u08BD\u0904-\u0939\u093D\u0950\u0958-\u0961\u0971-\u0980\u0985-\u098C\u098F\u0990\u0993-\u09A8\u09AA-\u09B0\u09B2\u09B6-\u09B9\u09BD\u09CE\u09DC\u09DD\u09DF-\u09E1\u09F0\u09F1\u09FC\u0A05-\u0A0A\u0A0F\u0A10\u0A13-\u0A28\u0A2A-\u0A30\u0A32\u0A33\u0A35\u0A36\u0A38\u0A39\u0A59-\u0A5C\u0A5E\u0A72-\u0A74\u0A85-\u0A8D\u0A8F-\u0A91\u0A93-\u0AA8\u0AAA-\u0AB0\u0AB2\u0AB3\u0AB5-\u0AB9\u0ABD\u0AD0\u0AE0\u0AE1\u0AF9\u0B05-\u0B0C\u0B0F\u0B10\u0B13-\u0B28\u0B2A-\u0B30\u0B32\u0B33\u0B35-\u0B39\u0B3D\u0B5C\u0B5D\u0B5F-\u0B61\u0B71\u0B83\u0B85-\u0B8A\u0B8E-\u0B90\u0B92-\u0B95\u0B99\u0B9A\u0B9C\u0B9E\u0B9F\u0BA3\u0BA4\u0BA8-\u0BAA\u0BAE-\u0BB9\u0BD0\u0C05-\u0C0C\u0C0E-\u0C10\u0C12-\u0C28\u0C2A-\u0C39\u0C3D\u0C58-\u0C5A\u0C60\u0C61\u0C80\u0C85-\u0C8C\u0C8E-\u0C90\u0C92-\u0CA8\u0CAA-\u0CB3\u0CB5-\u0CB9\u0CBD\u0CDE\u0CE0\u0CE1\u0CF1\u0CF2\u0D05-\u0D0C\u0D0E-\u0D10\u0D12-\u0D3A\u0D3D\u0D4E\u0D54-\u0D56\u0D5F-\u0D61\u0D7A-\u0D7F\u0D85-\u0D96\u0D9A-\u0DB1\u0DB3-\u0DBB\u0DBD\u0DC0-\u0DC6\u0E01-\u0E30\u0E32\u0E33\u0E40-\u0E46\u0E81\u0E82\u0E84\u0E87\u0E88\u0E8A\u0E8D\u0E94-\u0E97\u0E99-\u0E9F\u0EA1-\u0EA3\u0EA5\u0EA7\u0EAA\u0EAB\u0EAD-\u0EB0\u0EB2\u0EB3\u0EBD\u0EC0-\u0EC4\u0EC6\u0EDC-\u0EDF\u0F00\u0F40-\u0F47\u0F49-\u0F6C\u0F88-\u0F8C\u1000-\u102A\u103F\u1050-\u1055\u105A-\u105D\u1061\u1065\u1066\u106E-\u1070\u1075-\u1081\u108E\u10A0-\u10C5\u10C7\u10CD\u10D0-\u10FA\u10FC-\u1248\u124A-\u124D\u1250-\u1256\u1258\u125A-\u125D\u1260-\u1288\u128A-\u128D\u1290-\u12B0\u12B2-\u12B5\u12B8-\u12BE\u12C0\u12C2-\u12C5\u12C8-\u12D6\u12D8-\u1310\u1312-\u1315\u1318-\u135A\u1380-\u138F\u13A0-\u13F5\u13F8-\u13FD\u1401-\u166C\u166F-\u167F\u1681-\u169A\u16A0-\u16EA\u16EE-\u16F8\u1700-\u170C\u170E-\u1711\u1720-\u1731\u1740-\u1751\u1760-\u176C\u176E-\u1770\u1780-\u17B3\u17D7\u17DC\u1820-\u1877\u1880-\u1884\u1887-\u18A8\u18AA\u18B0-\u18F5\u1900-\u191E\u1950-\u196D\u1970-\u1974\u1980-\u19AB\u19B0-\u19C9\u1A00-\u1A16\u1A20-\u1A54\u1AA7\u1B05-\u1B33\u1B45-\u1B4B\u1B83-\u1BA0\u1BAE\u1BAF\u1BBA-\u1BE5\u1C00-\u1C23\u1C4D-\u1C4F\u1C5A-\u1C7D\u1C80-\u1C88\u1CE9-\u1CEC\u1CEE-\u1CF1\u1CF5\u1CF6\u1D00-\u1DBF\u1E00-\u1F15\u1F18-\u1F1D\u1F20-\u1F45\u1F48-\u1F4D\u1F50-\u1F57\u1F59\u1F5B\u1F5D\u1F5F-\u1F7D\u1F80-\u1FB4\u1FB6-\u1FBC\u1FBE\u1FC2-\u1FC4\u1FC6-\u1FCC\u1FD0-\u1FD3\u1FD6-\u1FDB\u1FE0-\u1FEC\u1FF2-\u1FF4\u1FF6-\u1FFC\u2071\u207F\u2090-\u209C\u2102\u2107\u210A-\u2113\u2115\u2119-\u211D\u2124\u2126\u2128\u212A-\u212D\u212F-\u2139\u213C-\u213F\u2145-\u2149\u214E\u2160-\u2188\u2C00-\u2C2E\u2C30-\u2C5E\u2C60-\u2CE4\u2CEB-\u2CEE\u2CF2\u2CF3\u2D00-\u2D25\u2D27\u2D2D\u2D30-\u2D67\u2D6F\u2D80-\u2D96\u2DA0-\u2DA6\u2DA8-\u2DAE\u2DB0-\u2DB6\u2DB8-\u2DBE\u2DC0-\u2DC6\u2DC8-\u2DCE\u2DD0-\u2DD6\u2DD8-\u2DDE\u2E2F\u3005-\u3007\u3021-\u3029\u3031-\u3035\u3038-\u303C\u3041-\u3096\u309D-\u309F\u30A1-\u30FA\u30FC-\u30FF\u3105-\u312E\u3131-\u318E\u31A0-\u31BA\u31F0-\u31FF\u3400-\u4DB5\u4E00-\u9FEA\uA000-\uA48C\uA4D0-\uA4FD\uA500-\uA60C\uA610-\uA61F\uA62A\uA62B\uA640-\uA66E\uA67F-\uA69D\uA6A0-\uA6EF\uA717-\uA71F\uA722-\uA788\uA78B-\uA7AE\uA7B0-\uA7B7\uA7F7-\uA801\uA803-\uA805\uA807-\uA80A\uA80C-\uA822\uA840-\uA873\uA882-\uA8B3\uA8F2-\uA8F7\uA8FB\uA8FD\uA90A-\uA925\uA930-\uA946\uA960-\uA97C\uA984-\uA9B2\uA9CF\uA9E0-\uA9E4\uA9E6-\uA9EF\uA9FA-\uA9FE\uAA00-\uAA28\uAA40-\uAA42\uAA44-\uAA4B\uAA60-\uAA76\uAA7A\uAA7E-\uAAAF\uAAB1\uAAB5\uAAB6\uAAB9-\uAABD\uAAC0\uAAC2\uAADB-\uAADD\uAAE0-\uAAEA\uAAF2-\uAAF4\uAB01-\uAB06\uAB09-\uAB0E\uAB11-\uAB16\uAB20-\uAB26\uAB28-\uAB2E\uAB30-\uAB5A\uAB5C-\uAB65\uAB70-\uABE2\uAC00-\uD7A3\uD7B0-\uD7C6\uD7CB-\uD7FB\uF900-\uFA6D\uFA70-\uFAD9\uFB00-\uFB06\uFB13-\uFB17\uFB1D\uFB1F-\uFB28\uFB2A-\uFB36\uFB38-\uFB3C\uFB3E\uFB40\uFB41\uFB43\uFB44\uFB46-\uFBB1\uFBD3-\uFD3D\uFD50-\uFD8F\uFD92-\uFDC7\uFDF0-\uFDFB\uFE70-\uFE74\uFE76-\uFEFC\uFF21-\uFF3A\uFF41-\uFF5A\uFF66-\uFFBE\uFFC2-\uFFC7\uFFCA-\uFFCF\uFFD2-\uFFD7\uFFDA-\uFFDC]|\uD800[\uDC00-\uDC0B\uDC0D-\uDC26\uDC28-\uDC3A\uDC3C\uDC3D\uDC3F-\uDC4D\uDC50-\uDC5D\uDC80-\uDCFA\uDD40-\uDD74\uDE80-\uDE9C\uDEA0-\uDED0\uDF00-\uDF1F\uDF2D-\uDF4A\uDF50-\uDF75\uDF80-\uDF9D\uDFA0-\uDFC3\uDFC8-\uDFCF\uDFD1-\uDFD5]|\uD801[\uDC00-\uDC9D\uDCB0-\uDCD3\uDCD8-\uDCFB\uDD00-\uDD27\uDD30-\uDD63\uDE00-\uDF36\uDF40-\uDF55\uDF60-\uDF67]|\uD802[\uDC00-\uDC05\uDC08\uDC0A-\uDC35\uDC37\uDC38\uDC3C\uDC3F-\uDC55\uDC60-\uDC76\uDC80-\uDC9E\uDCE0-\uDCF2\uDCF4\uDCF5\uDD00-\uDD15\uDD20-\uDD39\uDD80-\uDDB7\uDDBE\uDDBF\uDE00\uDE10-\uDE13\uDE15-\uDE17\uDE19-\uDE33\uDE60-\uDE7C\uDE80-\uDE9C\uDEC0-\uDEC7\uDEC9-\uDEE4\uDF00-\uDF35\uDF40-\uDF55\uDF60-\uDF72\uDF80-\uDF91]|\uD803[\uDC00-\uDC48\uDC80-\uDCB2\uDCC0-\uDCF2]|\uD804[\uDC03-\uDC37\uDC83-\uDCAF\uDCD0-\uDCE8\uDD03-\uDD26\uDD50-\uDD72\uDD76\uDD83-\uDDB2\uDDC1-\uDDC4\uDDDA\uDDDC\uDE00-\uDE11\uDE13-\uDE2B\uDE80-\uDE86\uDE88\uDE8A-\uDE8D\uDE8F-\uDE9D\uDE9F-\uDEA8\uDEB0-\uDEDE\uDF05-\uDF0C\uDF0F\uDF10\uDF13-\uDF28\uDF2A-\uDF30\uDF32\uDF33\uDF35-\uDF39\uDF3D\uDF50\uDF5D-\uDF61]|\uD805[\uDC00-\uDC34\uDC47-\uDC4A\uDC80-\uDCAF\uDCC4\uDCC5\uDCC7\uDD80-\uDDAE\uDDD8-\uDDDB\uDE00-\uDE2F\uDE44\uDE80-\uDEAA\uDF00-\uDF19]|\uD806[\uDCA0-\uDCDF\uDCFF\uDE00\uDE0B-\uDE32\uDE3A\uDE50\uDE5C-\uDE83\uDE86-\uDE89\uDEC0-\uDEF8]|\uD807[\uDC00-\uDC08\uDC0A-\uDC2E\uDC40\uDC72-\uDC8F\uDD00-\uDD06\uDD08\uDD09\uDD0B-\uDD30\uDD46]|\uD808[\uDC00-\uDF99]|\uD809[\uDC00-\uDC6E\uDC80-\uDD43]|[\uD80C\uD81C-\uD820\uD840-\uD868\uD86A-\uD86C\uD86F-\uD872\uD874-\uD879][\uDC00-\uDFFF]|\uD80D[\uDC00-\uDC2E]|\uD811[\uDC00-\uDE46]|\uD81A[\uDC00-\uDE38\uDE40-\uDE5E\uDED0-\uDEED\uDF00-\uDF2F\uDF40-\uDF43\uDF63-\uDF77\uDF7D-\uDF8F]|\uD81B[\uDF00-\uDF44\uDF50\uDF93-\uDF9F\uDFE0\uDFE1]|\uD821[\uDC00-\uDFEC]|\uD822[\uDC00-\uDEF2]|\uD82C[\uDC00-\uDD1E\uDD70-\uDEFB]|\uD82F[\uDC00-\uDC6A\uDC70-\uDC7C\uDC80-\uDC88\uDC90-\uDC99]|\uD835[\uDC00-\uDC54\uDC56-\uDC9C\uDC9E\uDC9F\uDCA2\uDCA5\uDCA6\uDCA9-\uDCAC\uDCAE-\uDCB9\uDCBB\uDCBD-\uDCC3\uDCC5-\uDD05\uDD07-\uDD0A\uDD0D-\uDD14\uDD16-\uDD1C\uDD1E-\uDD39\uDD3B-\uDD3E\uDD40-\uDD44\uDD46\uDD4A-\uDD50\uDD52-\uDEA5\uDEA8-\uDEC0\uDEC2-\uDEDA\uDEDC-\uDEFA\uDEFC-\uDF14\uDF16-\uDF34\uDF36-\uDF4E\uDF50-\uDF6E\uDF70-\uDF88\uDF8A-\uDFA8\uDFAA-\uDFC2\uDFC4-\uDFCB]|\uD83A[\uDC00-\uDCC4\uDD00-\uDD43]|\uD83B[\uDE00-\uDE03\uDE05-\uDE1F\uDE21\uDE22\uDE24\uDE27\uDE29-\uDE32\uDE34-\uDE37\uDE39\uDE3B\uDE42\uDE47\uDE49\uDE4B\uDE4D-\uDE4F\uDE51\uDE52\uDE54\uDE57\uDE59\uDE5B\uDE5D\uDE5F\uDE61\uDE62\uDE64\uDE67-\uDE6A\uDE6C-\uDE72\uDE74-\uDE77\uDE79-\uDE7C\uDE7E\uDE80-\uDE89\uDE8B-\uDE9B\uDEA1-\uDEA3\uDEA5-\uDEA9\uDEAB-\uDEBB]|\uD869[\uDC00-\uDED6\uDF00-\uDFFF]|\uD86D[\uDC00-\uDF34\uDF40-\uDFFF]|\uD86E[\uDC00-\uDC1D\uDC20-\uDFFF]|\uD873[\uDC00-\uDEA1\uDEB0-\uDFFF]|\uD87A[\uDC00-\uDFE0]|\uD87E[\uDC00-\uDE1D]/,
+    Ir = /[\xAA\xB5\xBA\xC0-\xD6\xD8-\xF6\xF8-\u02C1\u02C6-\u02D1\u02E0-\u02E4\u02EC\u02EE\u0300-\u0374\u0376\u0377\u037A-\u037D\u037F\u0386\u0388-\u038A\u038C\u038E-\u03A1\u03A3-\u03F5\u03F7-\u0481\u0483-\u0487\u048A-\u052F\u0531-\u0556\u0559\u0561-\u0587\u0591-\u05BD\u05BF\u05C1\u05C2\u05C4\u05C5\u05C7\u05D0-\u05EA\u05F0-\u05F2\u0610-\u061A\u0620-\u0669\u066E-\u06D3\u06D5-\u06DC\u06DF-\u06E8\u06EA-\u06FC\u06FF\u0710-\u074A\u074D-\u07B1\u07C0-\u07F5\u07FA\u0800-\u082D\u0840-\u085B\u0860-\u086A\u08A0-\u08B4\u08B6-\u08BD\u08D4-\u08E1\u08E3-\u0963\u0966-\u096F\u0971-\u0983\u0985-\u098C\u098F\u0990\u0993-\u09A8\u09AA-\u09B0\u09B2\u09B6-\u09B9\u09BC-\u09C4\u09C7\u09C8\u09CB-\u09CE\u09D7\u09DC\u09DD\u09DF-\u09E3\u09E6-\u09F1\u09FC\u0A01-\u0A03\u0A05-\u0A0A\u0A0F\u0A10\u0A13-\u0A28\u0A2A-\u0A30\u0A32\u0A33\u0A35\u0A36\u0A38\u0A39\u0A3C\u0A3E-\u0A42\u0A47\u0A48\u0A4B-\u0A4D\u0A51\u0A59-\u0A5C\u0A5E\u0A66-\u0A75\u0A81-\u0A83\u0A85-\u0A8D\u0A8F-\u0A91\u0A93-\u0AA8\u0AAA-\u0AB0\u0AB2\u0AB3\u0AB5-\u0AB9\u0ABC-\u0AC5\u0AC7-\u0AC9\u0ACB-\u0ACD\u0AD0\u0AE0-\u0AE3\u0AE6-\u0AEF\u0AF9-\u0AFF\u0B01-\u0B03\u0B05-\u0B0C\u0B0F\u0B10\u0B13-\u0B28\u0B2A-\u0B30\u0B32\u0B33\u0B35-\u0B39\u0B3C-\u0B44\u0B47\u0B48\u0B4B-\u0B4D\u0B56\u0B57\u0B5C\u0B5D\u0B5F-\u0B63\u0B66-\u0B6F\u0B71\u0B82\u0B83\u0B85-\u0B8A\u0B8E-\u0B90\u0B92-\u0B95\u0B99\u0B9A\u0B9C\u0B9E\u0B9F\u0BA3\u0BA4\u0BA8-\u0BAA\u0BAE-\u0BB9\u0BBE-\u0BC2\u0BC6-\u0BC8\u0BCA-\u0BCD\u0BD0\u0BD7\u0BE6-\u0BEF\u0C00-\u0C03\u0C05-\u0C0C\u0C0E-\u0C10\u0C12-\u0C28\u0C2A-\u0C39\u0C3D-\u0C44\u0C46-\u0C48\u0C4A-\u0C4D\u0C55\u0C56\u0C58-\u0C5A\u0C60-\u0C63\u0C66-\u0C6F\u0C80-\u0C83\u0C85-\u0C8C\u0C8E-\u0C90\u0C92-\u0CA8\u0CAA-\u0CB3\u0CB5-\u0CB9\u0CBC-\u0CC4\u0CC6-\u0CC8\u0CCA-\u0CCD\u0CD5\u0CD6\u0CDE\u0CE0-\u0CE3\u0CE6-\u0CEF\u0CF1\u0CF2\u0D00-\u0D03\u0D05-\u0D0C\u0D0E-\u0D10\u0D12-\u0D44\u0D46-\u0D48\u0D4A-\u0D4E\u0D54-\u0D57\u0D5F-\u0D63\u0D66-\u0D6F\u0D7A-\u0D7F\u0D82\u0D83\u0D85-\u0D96\u0D9A-\u0DB1\u0DB3-\u0DBB\u0DBD\u0DC0-\u0DC6\u0DCA\u0DCF-\u0DD4\u0DD6\u0DD8-\u0DDF\u0DE6-\u0DEF\u0DF2\u0DF3\u0E01-\u0E3A\u0E40-\u0E4E\u0E50-\u0E59\u0E81\u0E82\u0E84\u0E87\u0E88\u0E8A\u0E8D\u0E94-\u0E97\u0E99-\u0E9F\u0EA1-\u0EA3\u0EA5\u0EA7\u0EAA\u0EAB\u0EAD-\u0EB9\u0EBB-\u0EBD\u0EC0-\u0EC4\u0EC6\u0EC8-\u0ECD\u0ED0-\u0ED9\u0EDC-\u0EDF\u0F00\u0F18\u0F19\u0F20-\u0F29\u0F35\u0F37\u0F39\u0F3E-\u0F47\u0F49-\u0F6C\u0F71-\u0F84\u0F86-\u0F97\u0F99-\u0FBC\u0FC6\u1000-\u1049\u1050-\u109D\u10A0-\u10C5\u10C7\u10CD\u10D0-\u10FA\u10FC-\u1248\u124A-\u124D\u1250-\u1256\u1258\u125A-\u125D\u1260-\u1288\u128A-\u128D\u1290-\u12B0\u12B2-\u12B5\u12B8-\u12BE\u12C0\u12C2-\u12C5\u12C8-\u12D6\u12D8-\u1310\u1312-\u1315\u1318-\u135A\u135D-\u135F\u1380-\u138F\u13A0-\u13F5\u13F8-\u13FD\u1401-\u166C\u166F-\u167F\u1681-\u169A\u16A0-\u16EA\u16EE-\u16F8\u1700-\u170C\u170E-\u1714\u1720-\u1734\u1740-\u1753\u1760-\u176C\u176E-\u1770\u1772\u1773\u1780-\u17D3\u17D7\u17DC\u17DD\u17E0-\u17E9\u180B-\u180D\u1810-\u1819\u1820-\u1877\u1880-\u18AA\u18B0-\u18F5\u1900-\u191E\u1920-\u192B\u1930-\u193B\u1946-\u196D\u1970-\u1974\u1980-\u19AB\u19B0-\u19C9\u19D0-\u19D9\u1A00-\u1A1B\u1A20-\u1A5E\u1A60-\u1A7C\u1A7F-\u1A89\u1A90-\u1A99\u1AA7\u1AB0-\u1ABD\u1B00-\u1B4B\u1B50-\u1B59\u1B6B-\u1B73\u1B80-\u1BF3\u1C00-\u1C37\u1C40-\u1C49\u1C4D-\u1C7D\u1C80-\u1C88\u1CD0-\u1CD2\u1CD4-\u1CF9\u1D00-\u1DF9\u1DFB-\u1F15\u1F18-\u1F1D\u1F20-\u1F45\u1F48-\u1F4D\u1F50-\u1F57\u1F59\u1F5B\u1F5D\u1F5F-\u1F7D\u1F80-\u1FB4\u1FB6-\u1FBC\u1FBE\u1FC2-\u1FC4\u1FC6-\u1FCC\u1FD0-\u1FD3\u1FD6-\u1FDB\u1FE0-\u1FEC\u1FF2-\u1FF4\u1FF6-\u1FFC\u203F\u2040\u2054\u2071\u207F\u2090-\u209C\u20D0-\u20DC\u20E1\u20E5-\u20F0\u2102\u2107\u210A-\u2113\u2115\u2119-\u211D\u2124\u2126\u2128\u212A-\u212D\u212F-\u2139\u213C-\u213F\u2145-\u2149\u214E\u2160-\u2188\u2C00-\u2C2E\u2C30-\u2C5E\u2C60-\u2CE4\u2CEB-\u2CF3\u2D00-\u2D25\u2D27\u2D2D\u2D30-\u2D67\u2D6F\u2D7F-\u2D96\u2DA0-\u2DA6\u2DA8-\u2DAE\u2DB0-\u2DB6\u2DB8-\u2DBE\u2DC0-\u2DC6\u2DC8-\u2DCE\u2DD0-\u2DD6\u2DD8-\u2DDE\u2DE0-\u2DFF\u2E2F\u3005-\u3007\u3021-\u302F\u3031-\u3035\u3038-\u303C\u3041-\u3096\u3099\u309A\u309D-\u309F\u30A1-\u30FA\u30FC-\u30FF\u3105-\u312E\u3131-\u318E\u31A0-\u31BA\u31F0-\u31FF\u3400-\u4DB5\u4E00-\u9FEA\uA000-\uA48C\uA4D0-\uA4FD\uA500-\uA60C\uA610-\uA62B\uA640-\uA66F\uA674-\uA67D\uA67F-\uA6F1\uA717-\uA71F\uA722-\uA788\uA78B-\uA7AE\uA7B0-\uA7B7\uA7F7-\uA827\uA840-\uA873\uA880-\uA8C5\uA8D0-\uA8D9\uA8E0-\uA8F7\uA8FB\uA8FD\uA900-\uA92D\uA930-\uA953\uA960-\uA97C\uA980-\uA9C0\uA9CF-\uA9D9\uA9E0-\uA9FE\uAA00-\uAA36\uAA40-\uAA4D\uAA50-\uAA59\uAA60-\uAA76\uAA7A-\uAAC2\uAADB-\uAADD\uAAE0-\uAAEF\uAAF2-\uAAF6\uAB01-\uAB06\uAB09-\uAB0E\uAB11-\uAB16\uAB20-\uAB26\uAB28-\uAB2E\uAB30-\uAB5A\uAB5C-\uAB65\uAB70-\uABEA\uABEC\uABED\uABF0-\uABF9\uAC00-\uD7A3\uD7B0-\uD7C6\uD7CB-\uD7FB\uF900-\uFA6D\uFA70-\uFAD9\uFB00-\uFB06\uFB13-\uFB17\uFB1D-\uFB28\uFB2A-\uFB36\uFB38-\uFB3C\uFB3E\uFB40\uFB41\uFB43\uFB44\uFB46-\uFBB1\uFBD3-\uFD3D\uFD50-\uFD8F\uFD92-\uFDC7\uFDF0-\uFDFB\uFE00-\uFE0F\uFE20-\uFE2F\uFE33\uFE34\uFE4D-\uFE4F\uFE70-\uFE74\uFE76-\uFEFC\uFF10-\uFF19\uFF21-\uFF3A\uFF3F\uFF41-\uFF5A\uFF66-\uFFBE\uFFC2-\uFFC7\uFFCA-\uFFCF\uFFD2-\uFFD7\uFFDA-\uFFDC]|\uD800[\uDC00-\uDC0B\uDC0D-\uDC26\uDC28-\uDC3A\uDC3C\uDC3D\uDC3F-\uDC4D\uDC50-\uDC5D\uDC80-\uDCFA\uDD40-\uDD74\uDDFD\uDE80-\uDE9C\uDEA0-\uDED0\uDEE0\uDF00-\uDF1F\uDF2D-\uDF4A\uDF50-\uDF7A\uDF80-\uDF9D\uDFA0-\uDFC3\uDFC8-\uDFCF\uDFD1-\uDFD5]|\uD801[\uDC00-\uDC9D\uDCA0-\uDCA9\uDCB0-\uDCD3\uDCD8-\uDCFB\uDD00-\uDD27\uDD30-\uDD63\uDE00-\uDF36\uDF40-\uDF55\uDF60-\uDF67]|\uD802[\uDC00-\uDC05\uDC08\uDC0A-\uDC35\uDC37\uDC38\uDC3C\uDC3F-\uDC55\uDC60-\uDC76\uDC80-\uDC9E\uDCE0-\uDCF2\uDCF4\uDCF5\uDD00-\uDD15\uDD20-\uDD39\uDD80-\uDDB7\uDDBE\uDDBF\uDE00-\uDE03\uDE05\uDE06\uDE0C-\uDE13\uDE15-\uDE17\uDE19-\uDE33\uDE38-\uDE3A\uDE3F\uDE60-\uDE7C\uDE80-\uDE9C\uDEC0-\uDEC7\uDEC9-\uDEE6\uDF00-\uDF35\uDF40-\uDF55\uDF60-\uDF72\uDF80-\uDF91]|\uD803[\uDC00-\uDC48\uDC80-\uDCB2\uDCC0-\uDCF2]|\uD804[\uDC00-\uDC46\uDC66-\uDC6F\uDC7F-\uDCBA\uDCD0-\uDCE8\uDCF0-\uDCF9\uDD00-\uDD34\uDD36-\uDD3F\uDD50-\uDD73\uDD76\uDD80-\uDDC4\uDDCA-\uDDCC\uDDD0-\uDDDA\uDDDC\uDE00-\uDE11\uDE13-\uDE37\uDE3E\uDE80-\uDE86\uDE88\uDE8A-\uDE8D\uDE8F-\uDE9D\uDE9F-\uDEA8\uDEB0-\uDEEA\uDEF0-\uDEF9\uDF00-\uDF03\uDF05-\uDF0C\uDF0F\uDF10\uDF13-\uDF28\uDF2A-\uDF30\uDF32\uDF33\uDF35-\uDF39\uDF3C-\uDF44\uDF47\uDF48\uDF4B-\uDF4D\uDF50\uDF57\uDF5D-\uDF63\uDF66-\uDF6C\uDF70-\uDF74]|\uD805[\uDC00-\uDC4A\uDC50-\uDC59\uDC80-\uDCC5\uDCC7\uDCD0-\uDCD9\uDD80-\uDDB5\uDDB8-\uDDC0\uDDD8-\uDDDD\uDE00-\uDE40\uDE44\uDE50-\uDE59\uDE80-\uDEB7\uDEC0-\uDEC9\uDF00-\uDF19\uDF1D-\uDF2B\uDF30-\uDF39]|\uD806[\uDCA0-\uDCE9\uDCFF\uDE00-\uDE3E\uDE47\uDE50-\uDE83\uDE86-\uDE99\uDEC0-\uDEF8]|\uD807[\uDC00-\uDC08\uDC0A-\uDC36\uDC38-\uDC40\uDC50-\uDC59\uDC72-\uDC8F\uDC92-\uDCA7\uDCA9-\uDCB6\uDD00-\uDD06\uDD08\uDD09\uDD0B-\uDD36\uDD3A\uDD3C\uDD3D\uDD3F-\uDD47\uDD50-\uDD59]|\uD808[\uDC00-\uDF99]|\uD809[\uDC00-\uDC6E\uDC80-\uDD43]|[\uD80C\uD81C-\uD820\uD840-\uD868\uD86A-\uD86C\uD86F-\uD872\uD874-\uD879][\uDC00-\uDFFF]|\uD80D[\uDC00-\uDC2E]|\uD811[\uDC00-\uDE46]|\uD81A[\uDC00-\uDE38\uDE40-\uDE5E\uDE60-\uDE69\uDED0-\uDEED\uDEF0-\uDEF4\uDF00-\uDF36\uDF40-\uDF43\uDF50-\uDF59\uDF63-\uDF77\uDF7D-\uDF8F]|\uD81B[\uDF00-\uDF44\uDF50-\uDF7E\uDF8F-\uDF9F\uDFE0\uDFE1]|\uD821[\uDC00-\uDFEC]|\uD822[\uDC00-\uDEF2]|\uD82C[\uDC00-\uDD1E\uDD70-\uDEFB]|\uD82F[\uDC00-\uDC6A\uDC70-\uDC7C\uDC80-\uDC88\uDC90-\uDC99\uDC9D\uDC9E]|\uD834[\uDD65-\uDD69\uDD6D-\uDD72\uDD7B-\uDD82\uDD85-\uDD8B\uDDAA-\uDDAD\uDE42-\uDE44]|\uD835[\uDC00-\uDC54\uDC56-\uDC9C\uDC9E\uDC9F\uDCA2\uDCA5\uDCA6\uDCA9-\uDCAC\uDCAE-\uDCB9\uDCBB\uDCBD-\uDCC3\uDCC5-\uDD05\uDD07-\uDD0A\uDD0D-\uDD14\uDD16-\uDD1C\uDD1E-\uDD39\uDD3B-\uDD3E\uDD40-\uDD44\uDD46\uDD4A-\uDD50\uDD52-\uDEA5\uDEA8-\uDEC0\uDEC2-\uDEDA\uDEDC-\uDEFA\uDEFC-\uDF14\uDF16-\uDF34\uDF36-\uDF4E\uDF50-\uDF6E\uDF70-\uDF88\uDF8A-\uDFA8\uDFAA-\uDFC2\uDFC4-\uDFCB\uDFCE-\uDFFF]|\uD836[\uDE00-\uDE36\uDE3B-\uDE6C\uDE75\uDE84\uDE9B-\uDE9F\uDEA1-\uDEAF]|\uD838[\uDC00-\uDC06\uDC08-\uDC18\uDC1B-\uDC21\uDC23\uDC24\uDC26-\uDC2A]|\uD83A[\uDC00-\uDCC4\uDCD0-\uDCD6\uDD00-\uDD4A\uDD50-\uDD59]|\uD83B[\uDE00-\uDE03\uDE05-\uDE1F\uDE21\uDE22\uDE24\uDE27\uDE29-\uDE32\uDE34-\uDE37\uDE39\uDE3B\uDE42\uDE47\uDE49\uDE4B\uDE4D-\uDE4F\uDE51\uDE52\uDE54\uDE57\uDE59\uDE5B\uDE5D\uDE5F\uDE61\uDE62\uDE64\uDE67-\uDE6A\uDE6C-\uDE72\uDE74-\uDE77\uDE79-\uDE7C\uDE7E\uDE80-\uDE89\uDE8B-\uDE9B\uDEA1-\uDEA3\uDEA5-\uDEA9\uDEAB-\uDEBB]|\uD869[\uDC00-\uDED6\uDF00-\uDFFF]|\uD86D[\uDC00-\uDF34\uDF40-\uDFFF]|\uD86E[\uDC00-\uDC1D\uDC20-\uDFFF]|\uD873[\uDC00-\uDEA1\uDEB0-\uDFFF]|\uD87A[\uDC00-\uDFE0]|\uD87E[\uDC00-\uDE1D]|\uDB40[\uDD00-\uDDEF]/,
     Re = {
-        Space_Separator: Mr,
-        ID_Start: Pr,
-        ID_Continue: Vr
+        Space_Separator: Pr,
+        ID_Start: Vr,
+        ID_Continue: Ir
     },
     x = {
         isSpaceSeparator(t) {
             return typeof t == "string" && Re.Space_Separator.test(t)
         },
         isIdStartChar(t) {
             return typeof t == "string" && (t >= "a" && t <= "z" || t >= "A" && t <= "Z" || t === "$" || t === "_" || Re.ID_Start.test(t))
@@ -284,51 +284,51 @@
             return typeof t == "string" && /[0-9]/.test(t)
         },
         isHexDigit(t) {
             return typeof t == "string" && /[0-9A-Fa-f]/.test(t)
         }
     };
 let Ke, U, K, me, W, I, R, ut, le;
-var Ir = function(e, r) {
+var Hr = function(e, r) {
     Ke = String(e), U = "start", K = [], me = 0, W = 1, I = 0, R = void 0, ut = void 0, le = void 0;
-    do R = Hr(), Gr[U](); while (R.type !== "eof");
-    return typeof r == "function" ? jt({
+    do R = zr(), Wr[U](); while (R.type !== "eof");
+    return typeof r == "function" ? Rt({
         "": le
     }, "", r) : le
 };
 
-function jt(t, e, r) {
+function Rt(t, e, r) {
     const n = t[e];
     if (n != null && typeof n == "object")
         for (const u in n) {
-            const o = jt(n, u, r);
+            const o = Rt(n, u, r);
             o === void 0 ? delete n[u] : n[u] = o
         }
     return r.call(t, e, n)
 }
 let m, v, De, z, w;
 
-function Hr() {
+function zr() {
     for (m = "default", v = "", De = !1, z = 1;;) {
         w = G();
-        const t = Rt[m]();
+        const t = Lt[m]();
         if (t) return t
     }
 }
 
 function G() {
     if (Ke[me]) return String.fromCodePoint(Ke.codePointAt(me))
 }
 
 function y() {
     const t = G();
     return t === `
 ` ? (W++, I = 0) : t ? I += t.length : I++, t && (me += t.length), t
 }
-const Rt = {
+const Lt = {
     default () {
         switch (w) {
             case "	":
             case "\v":
             case "\f":
             case " ":
             case " ":
@@ -346,15 +346,15 @@
             case void 0:
                 return y(), O("eof")
         }
         if (x.isSpaceSeparator(w)) {
             y();
             return
         }
-        return Rt[U]()
+        return Lt[U]()
     },
     comment() {
         switch (w) {
             case "*":
                 y(), m = "multiLineComment";
                 return;
             case "/":
@@ -622,15 +622,15 @@
             return
         }
         return O("numeric", z * Number(v))
     },
     string() {
         switch (w) {
             case "\\":
-                y(), v += zr();
+                y(), v += Kr();
                 return;
             case '"':
                 if (De) return y(), O("string", v);
                 v += y();
                 return;
             case "'":
                 if (!De) return y(), O("string", v);
@@ -638,15 +638,15 @@
                 return;
             case `
 `:
             case "\r":
                 throw T(y());
             case "\u2028":
             case "\u2029":
-                Wr(w);
+                Jr(w);
                 break;
             case void 0:
                 throw T(y())
         }
         v += y()
     },
     start() {
@@ -723,15 +723,15 @@
 function J(t) {
     for (const e of t) {
         if (G() !== e) throw T(y());
         y()
     }
 }
 
-function zr() {
+function Kr() {
     switch (G()) {
         case "b":
             return y(), "\b";
         case "f":
             return y(), "\f";
         case "n":
             return y(), `
@@ -742,15 +742,15 @@
             return y(), "	";
         case "v":
             return y(), "\v";
         case "0":
             if (y(), x.isDigit(G())) throw T(y());
             return "\0";
         case "x":
-            return y(), Kr();
+            return y(), Gr();
         case "u":
             return y(), Ge();
         case `
 `:
         case "\u2028":
         case "\u2029":
             return y(), "";
@@ -769,15 +769,15 @@
             throw T(y());
         case void 0:
             throw T(y())
     }
     return y()
 }
 
-function Kr() {
+function Gr() {
     let t = "",
         e = G();
     if (!x.isHexDigit(e) || (t += y(), e = G(), !x.isHexDigit(e))) throw T(y());
     return t += y(), String.fromCodePoint(parseInt(t, 16))
 }
 
 function Ge() {
@@ -786,15 +786,15 @@
     for (; e-- > 0;) {
         const r = G();
         if (!x.isHexDigit(r)) throw T(y());
         t += y()
     }
     return String.fromCodePoint(parseInt(t, 16))
 }
-const Gr = {
+const Wr = {
     start() {
         if (R.type === "eof") throw q();
         Le()
     },
     beforePropertyName() {
         switch (R.type) {
             case "identifier":
@@ -882,30 +882,30 @@
 function Ce() {
     K.pop();
     const t = K[K.length - 1];
     t == null ? U = "end" : Array.isArray(t) ? U = "afterArrayValue" : U = "afterPropertyValue"
 }
 
 function T(t) {
-    return we(t === void 0 ? `JSON5: invalid end of input at ${W}:${I}` : `JSON5: invalid character '${Lt(t)}' at ${W}:${I}`)
+    return we(t === void 0 ? `JSON5: invalid end of input at ${W}:${I}` : `JSON5: invalid character '${kt(t)}' at ${W}:${I}`)
 }
 
 function q() {
     return we(`JSON5: invalid end of input at ${W}:${I}`)
 }
 
 function ct() {
     return I -= 5, we(`JSON5: invalid identifier character at ${W}:${I}`)
 }
 
-function Wr(t) {
-    console.warn(`JSON5: '${Lt(t)}' in strings is not valid ECMAScript; consider escaping`)
+function Jr(t) {
+    console.warn(`JSON5: '${kt(t)}' in strings is not valid ECMAScript; consider escaping`)
 }
 
-function Lt(t) {
+function kt(t) {
     const e = {
         "'": "\\'",
         '"': '\\"',
         "\\": "\\\\",
         "\b": "\\b",
         "\f": "\\f",
         "\n": "\\n",
@@ -924,15 +924,15 @@
     return t
 }
 
 function we(t) {
     const e = new SyntaxError(t);
     return e.lineNumber = W, e.columnNumber = I, e
 }
-var Jr = function(e, r, n) {
+var qr = function(e, r, n) {
     const u = [];
     let o = "",
         a, i, c = "",
         s;
     if (r != null && typeof r == "object" && !Array.isArray(r) && (n = r.space, s = r.quote, r = r.replacer), typeof r == "function") i = r;
     else if (Array.isArray(r)) {
         a = [];
@@ -953,15 +953,15 @@
             case !0:
                 return "true";
             case !1:
                 return "false"
         }
         if (typeof D == "string") return C(D);
         if (typeof D == "number") return String(D);
-        if (typeof D == "object") return Array.isArray(D) ? d(D) : g(D)
+        if (typeof D == "object") return Array.isArray(D) ? F(D) : g(D)
     }
 
     function C(p) {
         const l = {
                 "'": .1,
                 '"': .2
             },
@@ -1014,15 +1014,15 @@
         let l = o;
         o = o + c;
         let D = a || Object.keys(p),
             h = [];
         for (const E of D) {
             const S = f(E, p);
             if (S !== void 0) {
-                let j = F(E) + ":";
+                let j = d(E) + ":";
                 c !== "" && (j += " "), j += S, h.push(j)
             }
         }
         let A;
         if (h.length === 0) A = "{}";
         else {
             let E;
@@ -1034,24 +1034,24 @@
 ` + o + E + `,
 ` + l + "}"
             }
         }
         return u.pop(), o = l, A
     }
 
-    function F(p) {
+    function d(p) {
         if (p.length === 0) return C(p);
         const l = String.fromCodePoint(p.codePointAt(0));
         if (!x.isIdStartChar(l)) return C(p);
         for (let D = l.length; D < p.length; D++)
             if (!x.isIdContinueChar(String.fromCodePoint(p.codePointAt(D)))) return C(p);
         return p
     }
 
-    function d(p) {
+    function F(p) {
         if (u.indexOf(p) >= 0) throw TypeError("Converting circular structure to JSON5");
         u.push(p);
         let l = o;
         o = o + c;
         let D = [];
         for (let A = 0; A < p.length; A++) {
             const E = f(String(A), p);
@@ -1067,28 +1067,28 @@
             h = `[
 ` + o + E + `,
 ` + l + "]"
         }
         return u.pop(), o = l, h
     }
 };
-const qr = {
-    parse: Ir,
-    stringify: Jr
+const Xr = {
+    parse: Hr,
+    stringify: qr
 };
-var Xr = qr;
+var Yr = Xr;
 
 function ce() {
     const t = {};
     return t.promise = new Promise(function(e, r) {
         t.resolve = e, t.reject = r
     }), t
 }
 
-function Yr(t, e) {
+function Qr(t, e) {
     let n = 0;
     const u = {},
         o = [],
         a = {};
     let i = 1;
     const c = /^wslink_bin[\d]+$/,
         s = /^(rpc|publish|system):(\w+(?:\.\w+)*):(?:\d+)$/,
@@ -1101,32 +1101,32 @@
             method: "wslink.binary.attachment",
             args: [l]
         })), e.ws.send(a[l], {
             binary: !0
         }), delete a[l])
     }
 
-    function F(l) {
-        l && (Array.isArray(l) ? l.forEach(D => F(D)) : l.constructor === Object ? Object.keys(l).forEach(D => F(l[D])) : c.test(l) && g(l))
+    function d(l) {
+        l && (Array.isArray(l) ? l.forEach(D => d(D)) : l.constructor === Object ? Object.keys(l).forEach(D => d(l[D])) : c.test(l) && g(l))
     }
 
-    function d(l) {
+    function F(l) {
         const D = o.findIndex(h => h.key === l);
         if (D !== -1) {
             const h = o[D].data;
             return o.splice(D, 1), h
         }
         return console.error("Binary attachment key found without matching attachment"), null
     }
 
     function p(l) {
         for (let D in l)
             if (typeof l[D] == "string" && c.test(l[D])) {
                 const h = l[D],
-                    A = d(h);
+                    A = F(h);
                 A !== null && (l[D] = A)
             } else typeof l[D] == "object" && p(l[D])
     }
     t.onconnect = l => {
         const D = ce(),
             h = "system:c0:0";
         return u[h] = D, e.ws.send(JSON.stringify({
@@ -1144,15 +1144,15 @@
             const E = `rpc:${C}:${n++}`;
             u[E] = A, JSON.stringify({
                 wslink: "1.0",
                 id: E,
                 method: l,
                 args: D,
                 kwargs: h
-            }), Object.keys(a).length && (F(D), F(h)), e.ws.send(JSON.stringify({
+            }), Object.keys(a).length && (d(D), d(h)), e.ws.send(JSON.stringify({
                 wslink: "1.0",
                 id: E,
                 method: l,
                 args: D,
                 kwargs: h
             }))
         } else A.reject({
@@ -1202,15 +1202,15 @@
                 if (o[h].data === null) {
                     o[h].data = l.data, D = !0;
                     break
                 } D || console.error("Missing header for received binary message")
         } else {
             let D;
             try {
-                D = Xr.parse(l.data)
+                D = Yr.parse(l.data)
             } catch {
                 console.error("Malformed message: ", l.data)
             }
             if (!D) return;
             if (!D.id) {
                 D.method === "wslink.binary.attachment" && D.args.forEach(h => {
                     o.push({
@@ -1223,15 +1223,15 @@
             if (D.error) {
                 o.length = 0;
                 const h = u[D.id];
                 h ? h.reject(D.error) : console.error("Server error:", D.error)
             } else {
                 if (D.result && o.length > 0)
                     if (typeof D.result == "string" && c.test(D.result)) {
-                        const A = d(D.result);
+                        const A = F(D.result);
                         A !== null && (D.result = A)
                     } else p(D.result);
                 const h = s.exec(D.id);
                 if (h) {
                     const A = h[1];
                     if (A === "rpc") {
                         const E = u[D.id];
@@ -1257,63 +1257,63 @@
             delete u[D.id]
         }
     }, t.addAttachment = l => {
         const D = `wslink_bin${i}`;
         return a[D] = l, i++, D
     }
 }
-const Qr = {
+const Zr = {
     secret: "wslink-secret",
     ws: null
 };
 
-function kt(t, e, r = {}) {
-    Object.assign(e, Qr, r), b.destroy(t, e), b.isA(t, e, "Session"), Yr(t, e)
+function _t(t, e, r = {}) {
+    Object.assign(e, Zr, r), b.destroy(t, e), b.isA(t, e, "Session"), Qr(t, e)
 }
-const Zr = b.newInstance(kt),
-    en = {
-        newInstance: Zr,
-        extend: kt
+const en = b.newInstance(_t),
+    tn = {
+        newInstance: en,
+        extend: _t
     },
-    _t = "wslink-secret";
+    Ut = "wslink-secret";
 
-function tn(t) {
+function rn(t) {
     var e = t.indexOf(":"),
         r = t.substring(0, e);
     if (r === "ws" || r === "wss") return {
         type: "websocket",
         url: t
     };
     throw new Error(`Unknown protocol (${r}) for url (${t}).  Unable to create transport object.`)
 }
 
-function rn(t, e) {
+function nn(t, e) {
     t.connect = () => {
         if (!e.urls) return null;
         var n = [].concat(e.urls),
             u = [];
         for (let o = 0; o < n.length; o += 1) {
             const a = n[o];
             try {
-                const i = tn(a);
+                const i = rn(a);
                 u.push(i)
             } catch (i) {
                 return console.error(i), t.fireConnectionError(t, i), null
             }
         }
         if (e.connection) {
             if (e.connection.url !== u[0].url) e.connection.close();
             else if (e.connection.readyState === 0 || e.connection.readyState === 1) return e.session
         }
         try {
             e.connection = new WebSocket(u[0].url)
         } catch (o) {
             return console.error(o), t.fireConnectionError(t, o), null
         }
-        return e.connection.binaryType = "blob", e.secret || (e.secret = _t), e.session = en.newInstance({
+        return e.connection.binaryType = "blob", e.secret || (e.secret = Ut), e.session = tn.newInstance({
             ws: e.connection,
             secret: e.secret
         }), e.connection.onopen = o => {
             e.session && e.session.onconnect(o).then(() => {
                 t.fireConnectionReady(t)
             }, a => {
                 console.error("Connection error", a), t.fireConnectionError(t, a)
@@ -1328,92 +1328,92 @@
     }, t.getSession = () => e.session, t.getUrl = () => e.connection ? e.connection.url : void 0;
 
     function r(n = 10) {
         e.session && n > 0 && e.session.call("application.exit.later", [n]), e.connection && e.connection.close(), e.connection = null
     }
     t.destroy = b.chain(r, t.destroy)
 }
-const nn = {
-    secret: _t,
+const un = {
+    secret: Ut,
     connection: null,
     session: null,
     retry: !1
 };
 
-function Ut(t, e, r = {}) {
-    Object.assign(e, nn, r), b.destroy(t, e), b.event(t, e, "ConnectionReady"), b.event(t, e, "ConnectionClose"), b.event(t, e, "ConnectionError"), b.isA(t, e, "WebsocketConnection"), rn(t, e)
+function $t(t, e, r = {}) {
+    Object.assign(e, un, r), b.destroy(t, e), b.event(t, e, "ConnectionReady"), b.event(t, e, "ConnectionClose"), b.event(t, e, "ConnectionError"), b.isA(t, e, "WebsocketConnection"), nn(t, e)
 }
-const un = b.newInstance(Ut),
-    on = {
-        newInstance: un,
-        extend: Ut
+const on = b.newInstance($t),
+    an = {
+        newInstance: on,
+        extend: $t
     };
 
 function ke(t) {
     return t.sessionURL && (t.sessionURL = t.sessionURL.replaceAll("USE_HOSTNAME", window.location.hostname), t.sessionURL = t.sessionURL.replaceAll("USE_HOST", window.location.host)), t
 }
 
-function $t(t, e = window.location.pathname) {
+function Nt(t, e = window.location.pathname) {
     if (e.endsWith(".html") || e.endsWith(".htm")) {
         const r = e.split("/");
         r.pop(), e = r.join("/")
     }
     for (; e.length > 0 && e[e.length - 1] === "/";) e = e.substring(0, e.length - 1);
     return e.length === 0 ? t : `${e}${t}`
 }
-const an = `${window.location.protocol}//${window.location.hostname}:${window.location.port}${$t("/paraview/")}`,
-    sn = `${window.location.protocol==="https:"?"wss:":"ws:"}//${window.location.hostname}:${window.location.port}${$t("/ws")}`;
+const sn = `${window.location.protocol}//${window.location.hostname}:${window.location.port}${Nt("/paraview/")}`,
+    cn = `${window.location.protocol==="https:"?"wss:":"ws:"}//${window.location.hostname}:${window.location.port}${Nt("/ws")}`;
 
 function _e(t, e) {
-    const r = on.newInstance({
+    const r = an.newInstance({
         urls: e.config.sessionURL,
         secret: e.config.secret,
         retry: e.config.retry
     });
     return e.subscriptions.push(r.onConnectionReady(t.readyForwarder)), e.subscriptions.push(r.onConnectionError(t.errorForwarder)), e.subscriptions.push(r.onConnectionClose(t.closeForwarder)), e.gc.push(r), r.connect()
 }
 
-function cn(t, e) {
+function fn(t, e) {
     let r = null;
     e.gc = [], t.readyForwarder = u => {
         r = u.getSession(), t.fireConnectionReady(u)
     }, t.errorForwarder = (u, o) => {
         t.fireConnectionError(u, o)
     }, t.closeForwarder = (u, o) => {
         t.fireConnectionClose(u, o)
     }, t.connect = () => {
         if (e.configDecorator && (e.config = e.configDecorator(e.config)), e.config = ke(e.config), e.config.sessionURL) r = _e(t, e);
         else {
-            const u = Nr.newInstance({
-                endPoint: e.config.sessionManagerURL || an
+            const u = Mr.newInstance({
+                endPoint: e.config.sessionManagerURL || sn
             });
             e.subscriptions.push(u.onProcessReady(o => {
                 e.configDecorator ? e.config = e.configDecorator(Object.assign({}, e.config, o)) : e.config = Object.assign({}, e.config, o), e.config = ke(e.config), r = _e(t, e)
             })), e.subscriptions.push(u.onError(o => {
-                o && o.response && o.response.error ? t.errorForwarder(o, o.response.error) : (e.config.sessionURL = sn, e.config = ke(e.config), r = _e(t, e))
+                o && o.response && o.response.error ? t.errorForwarder(o, o.response.error) : (e.config.sessionURL = cn, e.config = ke(e.config), r = _e(t, e))
             })), u.start(e.config), e.gc.push(u)
         }
     }, t.getSession = () => r;
 
     function n() {
         for (r && r.close(), r = null; e.gc.length;) e.gc.pop().destroy()
     }
     t.destroy = b.chain(n, t.destroy)
 }
-const fn = {
+const Dn = {
     config: {}
 };
 
-function Nt(t, e, r = {}) {
-    Object.assign(e, fn, r), b.destroy(t, e), b.event(t, e, "ConnectionReady"), b.event(t, e, "ConnectionClose"), b.event(t, e, "ConnectionError"), b.isA(t, e, "SmartConnect"), b.get(t, e, ["config", "configDecorator"]), b.set(t, e, ["configDecorator"]), cn(t, e)
+function Mt(t, e, r = {}) {
+    Object.assign(e, Dn, r), b.destroy(t, e), b.event(t, e, "ConnectionReady"), b.event(t, e, "ConnectionClose"), b.event(t, e, "ConnectionError"), b.isA(t, e, "SmartConnect"), b.get(t, e, ["config", "configDecorator"]), b.set(t, e, ["configDecorator"]), fn(t, e)
 }
-const Dn = b.newInstance(Nt),
-    ln = {
-        newInstance: Dn,
-        extend: Nt
+const ln = b.newInstance(Mt),
+    pn = {
+        newInstance: ln,
+        extend: Mt
     };
 
 function ee(t) {
     return ee = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(e) {
         return typeof e
     } : function(e) {
         return e && typeof Symbol == "function" && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
@@ -1425,58 +1425,58 @@
         value: r,
         enumerable: !0,
         configurable: !0,
         writable: !0
     }) : t[e] = r, t
 }
 
-function pn(t) {
+function yn(t) {
     if (Array.isArray(t)) return ze(t)
 }
 
-function yn(t) {
+function gn(t) {
     if (typeof Symbol < "u" && t[Symbol.iterator] != null || t["@@iterator"] != null) return Array.from(t)
 }
 
-function gn() {
+function Cn() {
     throw new TypeError(`Invalid attempt to spread non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
 }
 
-function Mt(t) {
-    return pn(t) || yn(t) || Tt(t) || gn()
+function Pt(t) {
+    return yn(t) || gn(t) || xt(t) || Cn()
 }
 
 function ye(t, e) {
     return ye = Object.setPrototypeOf || function(n, u) {
         return n.__proto__ = u, n
     }, ye(t, e)
 }
 
-function Cn() {
+function hn() {
     if (typeof Reflect > "u" || !Reflect.construct || Reflect.construct.sham) return !1;
     if (typeof Proxy == "function") return !0;
     try {
         return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], function() {})), !0
     } catch {
         return !1
     }
 }
 
 function pe(t, e, r) {
-    return Cn() ? pe = Reflect.construct : pe = function(u, o, a) {
+    return hn() ? pe = Reflect.construct : pe = function(u, o, a) {
         var i = [null];
         i.push.apply(i, o);
         var c = Function.bind.apply(u, i),
             s = new c;
         return a && ye(s, a.prototype), s
     }, pe.apply(null, arguments)
 }
 var fe = typeof globalThis < "u" ? globalThis : typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : {},
-    hn = function t(e, r) {
+    dn = function t(e, r) {
         if (e === r) return !0;
         if (e && r && typeof e == "object" && typeof r == "object") {
             if (e.constructor !== r.constructor) return !1;
             var n, u, o;
             if (Array.isArray(e)) {
                 if (n = e.length, n != r.length) return !1;
                 for (u = n; u-- !== 0;)
@@ -1494,38 +1494,38 @@
                 if (!t(e[a], r[a])) return !1
             }
             return !0
         }
         return e !== e && r !== r
     },
     ft = Object.prototype.toString,
-    Pt = function(e) {
+    Vt = function(e) {
         var r = ft.call(e),
             n = r === "[object Arguments]";
         return n || (n = r !== "[object Array]" && e !== null && typeof e == "object" && typeof e.length == "number" && e.length >= 0 && ft.call(e.callee) === "[object Function]"), n
     },
     Ue, Dt;
 
 function Fn() {
     if (Dt) return Ue;
     Dt = 1;
     var t;
     if (!Object.keys) {
         var e = Object.prototype.hasOwnProperty,
             r = Object.prototype.toString,
-            n = Pt,
+            n = Vt,
             u = Object.prototype.propertyIsEnumerable,
             o = !u.call({
                 toString: null
             }, "toString"),
             a = u.call(function() {}, "prototype"),
             i = ["toString", "toLocaleString", "valueOf", "hasOwnProperty", "isPrototypeOf", "propertyIsEnumerable", "constructor"],
             c = function(g) {
-                var F = g.constructor;
-                return F && F.prototype === g
+                var d = g.constructor;
+                return d && d.prototype === g
             },
             s = {
                 $applicationCache: !0,
                 $console: !0,
                 $external: !0,
                 $frame: !0,
                 $frameElement: !0,
@@ -1565,56 +1565,56 @@
                 if (typeof window > "u" || !f) return c(g);
                 try {
                     return c(g)
                 } catch {
                     return !1
                 }
             };
-        t = function(F) {
-            var d = F !== null && typeof F == "object",
-                p = r.call(F) === "[object Function]",
-                l = n(F),
-                D = d && r.call(F) === "[object String]",
+        t = function(d) {
+            var F = d !== null && typeof d == "object",
+                p = r.call(d) === "[object Function]",
+                l = n(d),
+                D = F && r.call(d) === "[object String]",
                 h = [];
-            if (!d && !p && !l) throw new TypeError("Object.keys called on a non-object");
+            if (!F && !p && !l) throw new TypeError("Object.keys called on a non-object");
             var A = a && p;
-            if (D && F.length > 0 && !e.call(F, 0))
-                for (var E = 0; E < F.length; ++E) h.push(String(E));
-            if (l && F.length > 0)
-                for (var S = 0; S < F.length; ++S) h.push(String(S));
+            if (D && d.length > 0 && !e.call(d, 0))
+                for (var E = 0; E < d.length; ++E) h.push(String(E));
+            if (l && d.length > 0)
+                for (var S = 0; S < d.length; ++S) h.push(String(S));
             else
-                for (var j in F) !(A && j === "prototype") && e.call(F, j) && h.push(String(j));
+                for (var j in d) !(A && j === "prototype") && e.call(d, j) && h.push(String(j));
             if (o)
-                for (var M = C(F), P = 0; P < i.length; ++P) !(M && i[P] === "constructor") && e.call(F, i[P]) && h.push(i[P]);
+                for (var M = C(d), P = 0; P < i.length; ++P) !(M && i[P] === "constructor") && e.call(d, i[P]) && h.push(i[P]);
             return h
         }
     }
     return Ue = t, Ue
 }
-var dn = Array.prototype.slice,
-    En = Pt,
+var En = Array.prototype.slice,
+    An = Vt,
     lt = Object.keys,
     Ee = lt ? function(e) {
         return lt(e)
     } : Fn(),
     pt = Object.keys;
 Ee.shim = function() {
     if (Object.keys) {
         var e = function() {
             var r = Object.keys(arguments);
             return r && r.length === arguments.length
         }(1, 2);
         e || (Object.keys = function(n) {
-            return En(n) ? pt(dn.call(n)) : pt(n)
+            return An(n) ? pt(En.call(n)) : pt(n)
         })
     } else Object.keys = Ee;
     return Object.keys || Ee
 };
-var An = Ee,
-    vn = function() {
+var vn = Ee,
+    mn = function() {
         if (typeof Symbol != "function" || typeof Object.getOwnPropertySymbols != "function") return !1;
         if (typeof Symbol.iterator == "symbol") return !0;
         var e = {},
             r = Symbol("test"),
             n = Object(r);
         if (typeof r == "string" || Object.prototype.toString.call(r) !== "[object Symbol]" || Object.prototype.toString.call(n) !== "[object Symbol]") return !1;
         var u = 42;
@@ -1626,75 +1626,75 @@
         if (typeof Object.getOwnPropertyDescriptor == "function") {
             var a = Object.getOwnPropertyDescriptor(e, r);
             if (a.value !== u || a.enumerable !== !0) return !1
         }
         return !0
     },
     yt = typeof Symbol < "u" && Symbol,
-    mn = vn,
-    wn = function() {
-        return typeof yt != "function" || typeof Symbol != "function" || typeof yt("foo") != "symbol" || typeof Symbol("bar") != "symbol" ? !1 : mn()
+    wn = mn,
+    Bn = function() {
+        return typeof yt != "function" || typeof Symbol != "function" || typeof yt("foo") != "symbol" || typeof Symbol("bar") != "symbol" ? !1 : wn()
     },
-    Bn = "Function.prototype.bind called on incompatible ",
+    Sn = "Function.prototype.bind called on incompatible ",
     $e = Array.prototype.slice,
-    Sn = Object.prototype.toString,
-    bn = "[object Function]",
-    On = function(e) {
+    bn = Object.prototype.toString,
+    On = "[object Function]",
+    Tn = function(e) {
         var r = this;
-        if (typeof r != "function" || Sn.call(r) !== bn) throw new TypeError(Bn + r);
+        if (typeof r != "function" || bn.call(r) !== On) throw new TypeError(Sn + r);
         for (var n = $e.call(arguments, 1), u, o = function() {
                 if (this instanceof u) {
                     var f = r.apply(this, n.concat($e.call(arguments)));
                     return Object(f) === f ? f : this
                 } else return r.apply(e, n.concat($e.call(arguments)))
             }, a = Math.max(0, r.length - n.length), i = [], c = 0; c < a; c++) i.push("$" + c);
         if (u = Function("binder", "return function (" + i.join(",") + "){ return binder.apply(this,arguments); }")(o), r.prototype) {
             var s = function() {};
             s.prototype = r.prototype, u.prototype = new s, s.prototype = null
         }
         return u
     },
-    Tn = On,
-    Vt = Function.prototype.bind || Tn,
-    xn = Vt,
-    jn = xn.call(Function.call, Object.prototype.hasOwnProperty),
+    xn = Tn,
+    It = Function.prototype.bind || xn,
+    jn = It,
+    Rn = jn.call(Function.call, Object.prototype.hasOwnProperty),
     B, ae = SyntaxError,
-    It = Function,
+    Ht = Function,
     ue = TypeError,
     Ne = function(t) {
         try {
-            return It('"use strict"; return (' + t + ").constructor;")()
+            return Ht('"use strict"; return (' + t + ").constructor;")()
         } catch {}
     },
     Q = Object.getOwnPropertyDescriptor;
 if (Q) try {
     Q({}, "")
 } catch {
     Q = null
 }
 var Me = function() {
         throw new ue
     },
-    Rn = Q ? function() {
+    Ln = Q ? function() {
         try {
             return arguments.callee, Me
         } catch {
             try {
                 return Q(arguments, "callee").get
             } catch {
                 return Me
             }
         }
     }() : Me,
-    re = wn(),
+    re = Bn(),
     H = Object.getPrototypeOf || function(t) {
         return t.__proto__
     },
     ne = {},
-    Ln = typeof Uint8Array > "u" ? B : H(Uint8Array),
+    kn = typeof Uint8Array > "u" ? B : H(Uint8Array),
     Z = {
         "%AggregateError%": typeof AggregateError > "u" ? B : AggregateError,
         "%Array%": Array,
         "%ArrayBuffer%": typeof ArrayBuffer > "u" ? B : ArrayBuffer,
         "%ArrayIteratorPrototype%": re ? H([][Symbol.iterator]()) : B,
         "%AsyncFromSyncIteratorPrototype%": B,
         "%AsyncFunction%": ne,
@@ -1714,15 +1714,15 @@
         "%encodeURIComponent%": encodeURIComponent,
         "%Error%": Error,
         "%eval%": eval,
         "%EvalError%": EvalError,
         "%Float32Array%": typeof Float32Array > "u" ? B : Float32Array,
         "%Float64Array%": typeof Float64Array > "u" ? B : Float64Array,
         "%FinalizationRegistry%": typeof FinalizationRegistry > "u" ? B : FinalizationRegistry,
-        "%Function%": It,
+        "%Function%": Ht,
         "%GeneratorFunction%": ne,
         "%Int8Array%": typeof Int8Array > "u" ? B : Int8Array,
         "%Int16Array%": typeof Int16Array > "u" ? B : Int16Array,
         "%Int32Array%": typeof Int32Array > "u" ? B : Int32Array,
         "%isFinite%": isFinite,
         "%isNaN%": isNaN,
         "%IteratorPrototype%": re ? H(H([][Symbol.iterator]())) : B,
@@ -1743,33 +1743,33 @@
         "%Set%": typeof Set > "u" ? B : Set,
         "%SetIteratorPrototype%": typeof Set > "u" || !re ? B : H(new Set()[Symbol.iterator]()),
         "%SharedArrayBuffer%": typeof SharedArrayBuffer > "u" ? B : SharedArrayBuffer,
         "%String%": String,
         "%StringIteratorPrototype%": re ? H("" [Symbol.iterator]()) : B,
         "%Symbol%": re ? Symbol : B,
         "%SyntaxError%": ae,
-        "%ThrowTypeError%": Rn,
-        "%TypedArray%": Ln,
+        "%ThrowTypeError%": Ln,
+        "%TypedArray%": kn,
         "%TypeError%": ue,
         "%Uint8Array%": typeof Uint8Array > "u" ? B : Uint8Array,
         "%Uint8ClampedArray%": typeof Uint8ClampedArray > "u" ? B : Uint8ClampedArray,
         "%Uint16Array%": typeof Uint16Array > "u" ? B : Uint16Array,
         "%Uint32Array%": typeof Uint32Array > "u" ? B : Uint32Array,
         "%URIError%": URIError,
         "%WeakMap%": typeof WeakMap > "u" ? B : WeakMap,
         "%WeakRef%": typeof WeakRef > "u" ? B : WeakRef,
         "%WeakSet%": typeof WeakSet > "u" ? B : WeakSet
     };
 try {
     null.error
 } catch (t) {
-    var kn = H(H(t));
-    Z["%Error.prototype%"] = kn
+    var _n = H(H(t));
+    Z["%Error.prototype%"] = _n
 }
-var _n = function t(e) {
+var Un = function t(e) {
         var r;
         if (e === "%AsyncFunction%") r = Ne("async function () {}");
         else if (e === "%GeneratorFunction%") r = Ne("function* () {}");
         else if (e === "%AsyncGeneratorFunction%") r = Ne("async function* () {}");
         else if (e === "%AsyncGenerator%") {
             var n = t("%AsyncGeneratorFunction%");
             n && (r = n.prototype)
@@ -1828,64 +1828,64 @@
         "%Uint8ClampedArrayPrototype%": ["Uint8ClampedArray", "prototype"],
         "%Uint16ArrayPrototype%": ["Uint16Array", "prototype"],
         "%Uint32ArrayPrototype%": ["Uint32Array", "prototype"],
         "%URIErrorPrototype%": ["URIError", "prototype"],
         "%WeakMapPrototype%": ["WeakMap", "prototype"],
         "%WeakSetPrototype%": ["WeakSet", "prototype"]
     },
-    ge = Vt,
-    Se = jn,
-    Un = ge.call(Function.call, Array.prototype.concat),
-    $n = ge.call(Function.apply, Array.prototype.splice),
+    ge = It,
+    Se = Rn,
+    $n = ge.call(Function.call, Array.prototype.concat),
+    Nn = ge.call(Function.apply, Array.prototype.splice),
     Ct = ge.call(Function.call, String.prototype.replace),
     be = ge.call(Function.call, String.prototype.slice),
-    Nn = ge.call(Function.call, RegExp.prototype.exec),
-    Mn = /[^%.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|%$))/g,
-    Pn = /\\(\\)?/g,
-    Vn = function(e) {
+    Mn = ge.call(Function.call, RegExp.prototype.exec),
+    Pn = /[^%.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|%$))/g,
+    Vn = /\\(\\)?/g,
+    In = function(e) {
         var r = be(e, 0, 1),
             n = be(e, -1);
         if (r === "%" && n !== "%") throw new ae("invalid intrinsic syntax, expected closing `%`");
         if (n === "%" && r !== "%") throw new ae("invalid intrinsic syntax, expected opening `%`");
         var u = [];
-        return Ct(e, Mn, function(o, a, i, c) {
-            u[u.length] = i ? Ct(c, Pn, "$1") : a || o
+        return Ct(e, Pn, function(o, a, i, c) {
+            u[u.length] = i ? Ct(c, Vn, "$1") : a || o
         }), u
     },
-    In = function(e, r) {
+    Hn = function(e, r) {
         var n = e,
             u;
         if (Se(gt, n) && (u = gt[n], n = "%" + u[0] + "%"), Se(Z, n)) {
             var o = Z[n];
-            if (o === ne && (o = _n(n)), typeof o > "u" && !r) throw new ue("intrinsic " + e + " exists, but is not available. Please file an issue!");
+            if (o === ne && (o = Un(n)), typeof o > "u" && !r) throw new ue("intrinsic " + e + " exists, but is not available. Please file an issue!");
             return {
                 alias: u,
                 name: n,
                 value: o
             }
         }
         throw new ae("intrinsic " + e + " does not exist!")
     },
-    Hn = function(e, r) {
+    zn = function(e, r) {
         if (typeof e != "string" || e.length === 0) throw new ue("intrinsic name must be a non-empty string");
         if (arguments.length > 1 && typeof r != "boolean") throw new ue('"allowMissing" argument must be a boolean');
-        if (Nn(/^%?[^%]*%?$/, e) === null) throw new ae("`%` may not be present anywhere but at the beginning and end of the intrinsic name");
-        var n = Vn(e),
+        if (Mn(/^%?[^%]*%?$/, e) === null) throw new ae("`%` may not be present anywhere but at the beginning and end of the intrinsic name");
+        var n = In(e),
             u = n.length > 0 ? n[0] : "",
-            o = In("%" + u + "%", r),
+            o = Hn("%" + u + "%", r),
             a = o.name,
             i = o.value,
             c = !1,
             s = o.alias;
-        s && (u = s[0], $n(n, Un([0, 1], s)));
+        s && (u = s[0], Nn(n, $n([0, 1], s)));
         for (var f = 1, C = !0; f < n.length; f += 1) {
             var g = n[f],
-                F = be(g, 0, 1),
-                d = be(g, -1);
-            if ((F === '"' || F === "'" || F === "`" || d === '"' || d === "'" || d === "`") && F !== d) throw new ae("property names with quotes must have matching quotes");
+                d = be(g, 0, 1),
+                F = be(g, -1);
+            if ((d === '"' || d === "'" || d === "`" || F === '"' || F === "'" || F === "`") && d !== F) throw new ae("property names with quotes must have matching quotes");
             if ((g === "constructor" || !C) && (c = !0), u += "." + g, a = "%" + u + "%", Se(Z, a)) i = Z[a];
             else if (i != null) {
                 if (!(g in i)) {
                     if (!r) throw new ue("base intrinsic for " + e + " exists, but the property is not available.");
                     return
                 }
                 if (Q && f + 1 >= n.length) {
@@ -1893,16 +1893,16 @@
                     C = !!p, C && "get" in p && !("originalValue" in p.get) ? i = p.get : i = i[g]
                 } else C = Se(i, g), i = i[g];
                 C && !c && (Z[a] = i)
             }
         }
         return i
     },
-    zn = Hn,
-    We = zn("%Object.defineProperty%", !0),
+    Kn = zn,
+    We = Kn("%Object.defineProperty%", !0),
     Je = function() {
         if (We) try {
             return We({}, "a", {
                 value: 1
             }), !0
         } catch {
             return !1
@@ -1915,202 +1915,202 @@
         return We([], "length", {
             value: 1
         }).length !== 1
     } catch {
         return !0
     }
 };
-var Kn = Je,
-    Gn = An,
-    Wn = typeof Symbol == "function" && typeof Symbol("foo") == "symbol",
-    Jn = Object.prototype.toString,
-    qn = Array.prototype.concat,
-    Ht = Object.defineProperty,
-    Xn = function(t) {
-        return typeof t == "function" && Jn.call(t) === "[object Function]"
-    },
-    Yn = Kn(),
-    zt = Ht && Yn,
-    Qn = function(t, e, r, n) {
-        e in t && (!Xn(n) || !n()) || (zt ? Ht(t, e, {
+var Gn = Je,
+    Wn = vn,
+    Jn = typeof Symbol == "function" && typeof Symbol("foo") == "symbol",
+    qn = Object.prototype.toString,
+    Xn = Array.prototype.concat,
+    zt = Object.defineProperty,
+    Yn = function(t) {
+        return typeof t == "function" && qn.call(t) === "[object Function]"
+    },
+    Qn = Gn(),
+    Kt = zt && Qn,
+    Zn = function(t, e, r, n) {
+        e in t && (!Yn(n) || !n()) || (Kt ? zt(t, e, {
             configurable: !0,
             enumerable: !1,
             value: r,
             writable: !0
         }) : t[e] = r)
     },
-    Kt = function(t, e) {
+    Gt = function(t, e) {
         var r = arguments.length > 2 ? arguments[2] : {},
-            n = Gn(e);
-        Wn && (n = qn.call(n, Object.getOwnPropertySymbols(e)));
-        for (var u = 0; u < n.length; u += 1) Qn(t, n[u], e[n[u]], r[n[u]])
+            n = Wn(e);
+        Jn && (n = Xn.call(n, Object.getOwnPropertySymbols(e)));
+        for (var u = 0; u < n.length; u += 1) Zn(t, n[u], e[n[u]], r[n[u]])
     };
-Kt.supportsDescriptors = !!zt;
-var Gt = Kt,
+Gt.supportsDescriptors = !!Kt;
+var Wt = Gt,
     Oe = {},
     Pe = {
         get exports() {
             return Oe
         },
         set exports(t) {
             Oe = t
         }
     };
 typeof self < "u" ? Pe.exports = self : typeof window < "u" ? Pe.exports = window : Pe.exports = Function("return this")();
-var Zn = Oe,
-    Wt = function() {
-        return typeof fe != "object" || !fe || fe.Math !== Math || fe.Array !== Array ? Zn : fe
+var eu = Oe,
+    Jt = function() {
+        return typeof fe != "object" || !fe || fe.Math !== Math || fe.Array !== Array ? eu : fe
     },
-    eu = Gt,
     tu = Wt,
-    ru = function() {
-        var e = tu();
-        if (eu.supportsDescriptors) {
+    ru = Jt,
+    nu = function() {
+        var e = ru();
+        if (tu.supportsDescriptors) {
             var r = Object.getOwnPropertyDescriptor(e, "globalThis");
             (!r || r.configurable && (r.enumerable || !r.writable || globalThis !== e)) && Object.defineProperty(e, "globalThis", {
                 configurable: !0,
                 enumerable: !1,
                 value: e,
                 writable: !0
             })
         } else(typeof globalThis != "object" || globalThis !== e) && (e.globalThis = e);
         return e
     },
-    nu = Gt,
-    uu = Oe,
-    Jt = Wt,
-    ou = ru,
-    au = Jt(),
-    qt = function() {
-        return au
+    uu = Wt,
+    ou = Oe,
+    qt = Jt,
+    au = nu,
+    iu = qt(),
+    Xt = function() {
+        return iu
     };
-nu(qt, {
-    getPolyfill: Jt,
-    implementation: uu,
-    shim: ou
+uu(Xt, {
+    getPolyfill: qt,
+    implementation: ou,
+    shim: au
 });
-var iu = qt;
+var su = Xt;
 
 function ht(t, e) {
     var r = Object.keys(t);
     if (Object.getOwnPropertySymbols) {
         var n = Object.getOwnPropertySymbols(t);
         e && (n = n.filter(function(u) {
             return Object.getOwnPropertyDescriptor(t, u).enumerable
         })), r.push.apply(r, n)
     }
     return r
 }
 
-function su(t) {
+function cu(t) {
     for (var e = 1; e < arguments.length; e++) {
         var r = arguments[e] != null ? arguments[e] : {};
         e % 2 ? ht(Object(r), !0).forEach(function(n) {
             Be(t, n, r[n])
         }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(t, Object.getOwnPropertyDescriptors(r)) : ht(Object(r)).forEach(function(n) {
             Object.defineProperty(t, n, Object.getOwnPropertyDescriptor(r, n))
         })
     }
     return t
 }
-var V = iu(),
-    Xt = {
+var V = su(),
+    Yt = {
         vtkObject: function() {
             return null
         }
     };
 
 function Y(t) {
     if (t == null || t.isA) return t;
     if (!t.vtkClass) return V.console && V.console.error && V.console.error("Invalid VTK object"), null;
-    var e = Xt[t.vtkClass];
+    var e = Yt[t.vtkClass];
     if (!e) return V.console && V.console.error && V.console.error("No vtk class found for Object of type ".concat(t.vtkClass)), null;
-    var r = su({}, t);
+    var r = cu({}, t);
     Object.keys(r).forEach(function(u) {
         r[u] && ee(r[u]) === "object" && r[u].vtkClass && (r[u] = Y(r[u]))
     });
     var n = e(r);
     return n && n.modified && n.modified(), n
 }
 
-function cu(t, e) {
-    Xt[t] = e
+function fu(t, e) {
+    Yt[t] = e
 }
-Y.register = cu;
+Y.register = fu;
 
-function fu(t, e) {
+function Du(t, e) {
     if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
 }
 
-function Ft(t, e) {
+function dt(t, e) {
     for (var r = 0; r < e.length; r++) {
         var n = e[r];
         n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(t, n.key, n)
     }
 }
 
-function Du(t, e, r) {
-    return e && Ft(t.prototype, e), r && Ft(t, r), Object.defineProperty(t, "prototype", {
+function lu(t, e, r) {
+    return e && dt(t.prototype, e), r && dt(t, r), Object.defineProperty(t, "prototype", {
         writable: !1
     }), t
 }
 
 function te(t) {
     return te = Object.setPrototypeOf ? Object.getPrototypeOf : function(r) {
         return r.__proto__ || Object.getPrototypeOf(r)
     }, te(t)
 }
 
-function lu(t, e) {
+function pu(t, e) {
     for (; !Object.prototype.hasOwnProperty.call(t, e) && (t = te(t), t !== null););
     return t
 }
 
 function Ae() {
     return typeof Reflect < "u" && Reflect.get ? Ae = Reflect.get : Ae = function(e, r, n) {
-        var u = lu(e, r);
+        var u = pu(e, r);
         if (u) {
             var o = Object.getOwnPropertyDescriptor(u, r);
             return o.get ? o.get.call(arguments.length < 3 ? e : n) : o.value
         }
     }, Ae.apply(this, arguments)
 }
 
-function pu(t, e) {
+function yu(t, e) {
     if (typeof e != "function" && e !== null) throw new TypeError("Super expression must either be null or a function");
     t.prototype = Object.create(e && e.prototype, {
         constructor: {
             value: t,
             writable: !0,
             configurable: !0
         }
     }), Object.defineProperty(t, "prototype", {
         writable: !1
     }), e && ye(t, e)
 }
 
-function yu(t) {
+function gu(t) {
     if (t === void 0) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
     return t
 }
 
-function gu(t, e) {
+function Cu(t, e) {
     if (e && (ee(e) === "object" || typeof e == "function")) return e;
     if (e !== void 0) throw new TypeError("Derived constructors may only return object or undefined");
-    return yu(t)
+    return gu(t)
 }
 
-function Cu(t) {
+function hu(t) {
     return Function.toString.call(t).indexOf("[native code]") !== -1
 }
 
 function qe(t) {
     var e = typeof Map == "function" ? new Map : void 0;
     return qe = function(n) {
-        if (n === null || !Cu(n)) return n;
+        if (n === null || !hu(n)) return n;
         if (typeof n != "function") throw new TypeError("Super expression must either be null or a function");
         if (typeof e < "u") {
             if (e.has(n)) return e.get(n);
             e.set(n, u)
         }
 
         function u() {
@@ -2123,122 +2123,122 @@
                 writable: !0,
                 configurable: !0
             }
         }), ye(u, n)
     }, qe(t)
 }
 
-function hu(t) {
+function du(t) {
     var e = Fu();
     return function() {
         var n = te(t),
             u;
         if (e) {
             var o = te(this).constructor;
             u = Reflect.construct(n, arguments, o)
         } else u = n.apply(this, arguments);
-        return gu(this, u)
+        return Cu(this, u)
     }
 }
 
 function Fu() {
     if (typeof Reflect > "u" || !Reflect.construct || Reflect.construct.sham) return !1;
     if (typeof Proxy == "function") return !0;
     try {
         return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], function() {})), !0
     } catch {
         return !1
     }
 }
 var Ve = function(t) {
-    pu(r, t);
-    var e = hu(r);
+    yu(r, t);
+    var e = du(r);
 
     function r() {
-        return fu(this, r), e.apply(this, arguments)
+        return Du(this, r), e.apply(this, arguments)
     }
-    return Du(r, [{
+    return lu(r, [{
         key: "push",
         value: function() {
             for (var u = 0; u < arguments.length; u++) this.includes(arguments[u]) || Ae(te(r.prototype), "push", this).call(this, arguments[u]);
             return this.length
         }
     }]), r
 }(qe(Array));
 
-function dt(t, e) {
+function Ft(t, e) {
     var r = Object.keys(t);
     if (Object.getOwnPropertySymbols) {
         var n = Object.getOwnPropertySymbols(t);
         e && (n = n.filter(function(u) {
             return Object.getOwnPropertyDescriptor(t, u).enumerable
         })), r.push.apply(r, n)
     }
     return r
 }
 
 function Te(t) {
     for (var e = 1; e < arguments.length; e++) {
         var r = arguments[e] != null ? arguments[e] : {};
-        e % 2 ? dt(Object(r), !0).forEach(function(n) {
+        e % 2 ? Ft(Object(r), !0).forEach(function(n) {
             Be(t, n, r[n])
-        }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(t, Object.getOwnPropertyDescriptors(r)) : dt(Object(r)).forEach(function(n) {
+        }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(t, Object.getOwnPropertyDescriptors(r)) : Ft(Object(r)).forEach(function(n) {
             Object.defineProperty(t, n, Object.getOwnPropertyDescriptor(r, n))
         })
     }
     return t
 }
 var Xe = 0,
-    du = Symbol("void");
+    Eu = Symbol("void");
 
-function Eu() {
+function Au() {
     return Xe
 }
-var Yt = {};
+var Qt = {};
 
 function X() {}
-var Au = ["log", "debug", "info", "warn", "error", "time", "timeEnd", "group", "groupEnd"];
-Au.forEach(function(t) {
-    Yt[t] = X
+var vu = ["log", "debug", "info", "warn", "error", "time", "timeEnd", "group", "groupEnd"];
+vu.forEach(function(t) {
+    Qt[t] = X
 });
-V.console = console.hasOwnProperty("log") ? console : Yt;
+V.console = console.hasOwnProperty("log") ? console : Qt;
 var N = {
     debug: X,
     error: V.console.error || X,
     info: V.console.info || X,
     log: V.console.log || X,
     warn: V.console.warn || X
 };
 
-function vu(t, e) {
+function mu(t, e) {
     N[t] && (N[t] = e || X)
 }
 
-function mu() {
+function wu() {
     N.log.apply(N, arguments)
 }
 
-function wu() {
+function Bu() {
     N.info.apply(N, arguments)
 }
 
 function Ye() {
     N.debug.apply(N, arguments)
 }
 
 function L() {
     N.error.apply(N, arguments)
 }
 
-function Qt() {
+function Zt() {
     N.warn.apply(N, arguments)
 }
 var Et = {};
 
-function Bu(t) {
+function Su(t) {
     Et[t] || (N.error(t), Et[t] = !0)
 }
 var $ = Object.create(null);
 $.Float32Array = Float32Array;
 $.Float64Array = Float64Array;
 $.Uint8Array = Uint8Array;
 $.Int8Array = Int8Array;
@@ -2247,89 +2247,89 @@
 $.Uint32Array = Uint32Array;
 $.Int32Array = Int32Array;
 $.Uint8ClampedArray = Uint8ClampedArray;
 try {
     $.BigInt64Array = BigInt64Array, $.BigUint64Array = BigUint64Array
 } catch {}
 
-function Su(t) {
+function bu(t) {
     for (var e = arguments.length, r = new Array(e > 1 ? e - 1 : 0), n = 1; n < e; n++) r[n - 1] = arguments[n];
     return pe($[t] || Float64Array, r)
 }
 
-function bu(t) {
+function Ou(t) {
     for (var e, r = arguments.length, n = new Array(r > 1 ? r - 1 : 0), u = 1; u < r; u++) n[u - 1] = arguments[u];
     return (e = $[t] || Float64Array).from.apply(e, n)
 }
 
 function ot(t) {
     return t.charAt(0).toUpperCase() + t.slice(1)
 }
 
 function _(t) {
     return ot(t[0] === "_" ? t.slice(1) : t)
 }
 
-function Ou(t) {
+function Tu(t) {
     return t.charAt(0).toLowerCase() + t.slice(1)
 }
 
-function Tu(t) {
+function xu(t) {
     for (var e = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 2, r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : 1e3, n = ["TB", "GB", "MB", "KB"], u = Number(t), o = "B"; u > r;) u /= r, o = n.pop();
     return "".concat(u.toFixed(e), " ").concat(o)
 }
 
-function xu(t) {
+function ju(t) {
     for (var e = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : " ", r = [], n = t; n > 1e3;) r.push("000".concat(n % 1e3).slice(-3)), n = Math.floor(n / 1e3);
     return n > 0 && r.push(n), r.reverse(), r.join(e)
 }
 
-function Zt(t) {
+function er(t) {
     Object.keys(t).forEach(function(e) {
         Array.isArray(t[e]) && (t[e] = [].concat(t[e]))
     })
 }
 
-function ju(t, e) {
+function Ru(t, e) {
     if (t === e) return !0;
     if (Array.isArray(t) && Array.isArray(e)) {
         if (t.length !== e.length) return !1;
         for (var r = 0; r < t.length; r++)
             if (t[r] !== e[r]) return !1;
         return !0
     }
     return !1
 }
 
-function Ru(t, e) {
+function Lu(t, e) {
     return Object.keys(t).find(function(r) {
         return t[r] === e
     })
 }
 
-function er(t) {
+function tr(t) {
     return t && t.isA ? t.getState() : t
 }
 
-function tr(t) {
+function rr(t) {
     setTimeout(t, 0)
 }
 
-function Lu(t, e) {
+function ku(t, e) {
     var r = performance.now();
     t.finally(function() {
         var n = performance.now() - r;
         e(n)
     })
 }
 
-function ku() {
+function _u() {
     var t = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {},
         e = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : {};
-    Zt(e);
+    er(e);
     var r = [];
     if (Number.isInteger(e.mtime) || (e.mtime = ++Xe), !("classHierarchy" in e)) e.classHierarchy = new Ve("vtkObject");
     else if (!(e.classHierarchy instanceof Ve)) {
         for (var n = new Ve, u = 0; u < e.classHierarchy.length; u++) n.push(e.classHierarchy[u]);
         e.classHierarchy = n
     }
 
@@ -2371,15 +2371,15 @@
     }, t.set = function() {
         var i = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {},
             c = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !1,
             s = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : !1,
             f = !1;
         return Object.keys(i).forEach(function(C) {
             var g = s ? null : t["set".concat(ot(C))];
-            g && Array.isArray(i[C]) && g.length > 1 ? f = g.apply(void 0, Mt(i[C])) || f : g ? f = g(i[C]) || f : (["mtime"].indexOf(C) === -1 && !c && Qt("Warning: Set value to model directly ".concat(C, ", ").concat(i[C])), f = e[C] !== i[C] || f, e[C] = i[C])
+            g && Array.isArray(i[C]) && g.length > 1 ? f = g.apply(void 0, Pt(i[C])) || f : g ? f = g(i[C]) || f : (["mtime"].indexOf(C) === -1 && !c && Zt("Warning: Set value to model directly ".concat(C, ", ").concat(i[C])), f = e[C] !== i[C] || f, e[C] = i[C])
         }), f
     }, t.get = function() {
         for (var i = arguments.length, c = new Array(i), s = 0; s < i; s++) c[s] = arguments[s];
         if (!c.length) return e;
         var f = {};
         return c.forEach(function(C) {
             f[C] = e[C]
@@ -2394,55 +2394,55 @@
         }), e.deleted = !0
     }, t.getState = function() {
         if (e.deleted) return null;
         var i = Te(Te({}, e), {}, {
             vtkClass: t.getClassName()
         });
         Object.keys(i).forEach(function(s) {
-            i[s] === null || i[s] === void 0 || s[0] === "_" ? delete i[s] : i[s].isA ? i[s] = i[s].getState() : Array.isArray(i[s]) && (i[s] = i[s].map(er))
+            i[s] === null || i[s] === void 0 || s[0] === "_" ? delete i[s] : i[s].isA ? i[s] = i[s].getState() : Array.isArray(i[s]) && (i[s] = i[s].map(tr))
         });
         var c = {};
         return Object.keys(i).sort().forEach(function(s) {
             c[s] = i[s]
         }), c.mtime && delete c.mtime, c
     }, t.shallowCopy = function(i) {
         var c = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !1;
         if (i.getClassName() !== t.getClassName()) throw new Error("Cannot ShallowCopy ".concat(i.getClassName(), " into ").concat(t.getClassName()));
         var s = i.get(),
             f = Object.keys(e).sort(),
             C = Object.keys(s).sort();
         C.forEach(function(g) {
-            var F = f.indexOf(g);
-            F === -1 ? c && Ye("add ".concat(g, " in shallowCopy")) : f.splice(F, 1), e[g] = s[g]
+            var d = f.indexOf(g);
+            d === -1 ? c && Ye("add ".concat(g, " in shallowCopy")) : f.splice(d, 1), e[g] = s[g]
         }), f.length && c && Ye("Untouched keys: ".concat(f.join(", "))), t.modified()
     }, t.toJSON = function() {
         return t.getState()
     }, t
 }
-var _u = {
+var Uu = {
     object: function(e, r, n) {
         return function() {
             return Te({}, r[n.name])
         }
     }
 };
 
 function je(t, e, r) {
     r.forEach(function(n) {
         if (ee(n) === "object") {
-            var u = _u[n.type];
+            var u = Uu[n.type];
             u ? t["get".concat(_(n.name))] = u(t, e, n) : t["get".concat(_(n.name))] = function() {
                 return e[n.name]
             }
         } else t["get".concat(_(n))] = function() {
             return e[n]
         }
     })
 }
-var Uu = {
+var $u = {
     enum: function(e, r, n) {
         return function(u) {
             if (typeof u == "string") {
                 if (n.enum[u] !== void 0) return r[n.name] !== n.enum[u] ? (r[n.name] = n.enum[u], e.modified(), !0) : !1;
                 throw L("Set Enum with invalid argument ".concat(n, ", ").concat(u)), new RangeError("Set Enum with invalid string argument")
             }
             if (typeof u == "number") {
@@ -2455,55 +2455,55 @@
                 return !1
             }
             throw L("Set Enum with invalid argument (String/Number) ".concat(n, ", ").concat(u)), new TypeError("Set Enum with invalid argument (String/Number)")
         }
     },
     object: function(e, r, n) {
         return function(u) {
-            return hn(r[n.name], u) ? !1 : (r[n.name] = u, e.modified(), !0)
+            return dn(r[n.name], u) ? !1 : (r[n.name] = u, e.modified(), !0)
         }
     }
 };
 
 function At(t) {
     if (ee(t) === "object") {
-        var e = Uu[t.type];
+        var e = $u[t.type];
         if (e) return function(r, n) {
             return e(r, n, t)
         };
         throw L("No setter for field ".concat(t)), new TypeError("No setter for field")
     }
     return function(n, u) {
         return function(a) {
             return u.deleted ? (L("instance deleted - cannot call any method"), !1) : u[t] !== a ? (u[t] = a, n.modified(), !0) : !1
         }
     }
 }
 
-function rr(t, e, r) {
+function nr(t, e, r) {
     r.forEach(function(n) {
         ee(n) === "object" ? t["set".concat(_(n.name))] = At(n)(t, e) : t["set".concat(_(n))] = At(n)(t, e)
     })
 }
 
-function nr(t, e, r) {
-    je(t, e, r), rr(t, e, r)
+function ur(t, e, r) {
+    je(t, e, r), nr(t, e, r)
 }
 
-function ur(t, e, r) {
+function or(t, e, r) {
     r.forEach(function(n) {
         t["get".concat(_(n))] = function() {
             return e[n] ? Array.from(e[n]) : e[n]
         }, t["get".concat(_(n), "ByReference")] = function() {
             return e[n]
         }
     })
 }
 
-function or(t, e, r, n) {
+function ar(t, e, r, n) {
     var u = arguments.length > 4 && arguments[4] !== void 0 ? arguments[4] : void 0;
     r.forEach(function(o) {
         if (e[o] && n && e[o].length !== n) throw new RangeError("Invalid initial number of values for array (".concat(o, ")"));
         t["set".concat(_(o))] = function() {
             if (e.deleted) return L("instance deleted - cannot call any method"), !1;
             for (var a = arguments.length, i = new Array(a), c = 0; c < a; c++) i[c] = arguments[c];
             var s = i,
@@ -2524,147 +2524,147 @@
             a.forEach(function(c, s) {
                 i[s] = c
             })
         }
     })
 }
 
-function $u(t, e, r, n) {
+function Nu(t, e, r, n) {
     var u = arguments.length > 4 && arguments[4] !== void 0 ? arguments[4] : void 0;
-    ur(t, e, r), or(t, e, r, n, u)
+    or(t, e, r), ar(t, e, r, n, u)
 }
 
-function Nu(t, e, r) {
+function Mu(t, e, r) {
     for (var n = 0; n < r.length; n++) {
         var u = r[n];
         e[u] !== void 0 && (e["_".concat(u)] = e[u], delete e[u])
     }
 }
 
-function Mu(t, e, r, n) {
+function Pu(t, e, r, n) {
     e.inputData ? e.inputData = e.inputData.map(Y) : e.inputData = [], e.inputConnection ? e.inputConnection = e.inputConnection.map(Y) : e.inputConnection = [], e.output ? e.output = e.output.map(Y) : e.output = [], e.inputArrayToProcess ? e.inputArrayToProcess = e.inputArrayToProcess.map(Y) : e.inputArrayToProcess = [], e.numberOfInputs = r;
 
-    function u(d) {
+    function u(F) {
         var p = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0;
         if (e.deleted) {
             L("instance deleted - cannot call any method");
             return
         }
         if (p >= e.numberOfInputs) {
             L("algorithm ".concat(t.getClassName(), " only has ").concat(e.numberOfInputs, " input ports. To add more input ports, use addInputData()"));
             return
-        }(e.inputData[p] !== d || e.inputConnection[p]) && (e.inputData[p] = d, e.inputConnection[p] = null, t.modified && t.modified())
+        }(e.inputData[p] !== F || e.inputConnection[p]) && (e.inputData[p] = F, e.inputConnection[p] = null, t.modified && t.modified())
     }
 
     function o() {
-        var d = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
-        return e.inputConnection[d] && (e.inputData[d] = e.inputConnection[d]()), e.inputData[d]
+        var F = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
+        return e.inputConnection[F] && (e.inputData[F] = e.inputConnection[F]()), e.inputData[F]
     }
 
-    function a(d) {
+    function a(F) {
         var p = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0;
         if (e.deleted) {
             L("instance deleted - cannot call any method");
             return
         }
         if (p >= e.numberOfInputs) {
             var l = "algorithm ".concat(t.getClassName(), " only has ");
             l += "".concat(e.numberOfInputs), l += " input ports. To add more input ports, use addInputConnection()", L(l);
             return
         }
-        e.inputData[p] = null, e.inputConnection[p] = d
+        e.inputData[p] = null, e.inputConnection[p] = F
     }
 
     function i() {
-        var d = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
-        return e.inputConnection[d]
+        var F = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
+        return e.inputConnection[F]
     }
 
     function c() {
-        for (var d = e.numberOfInputs; d && !e.inputData[d - 1] && !e.inputConnection[d - 1];) d--;
-        return d === e.numberOfInputs && e.numberOfInputs++, d
+        for (var F = e.numberOfInputs; F && !e.inputData[F - 1] && !e.inputConnection[F - 1];) F--;
+        return F === e.numberOfInputs && e.numberOfInputs++, F
     }
 
-    function s(d) {
+    function s(F) {
         if (e.deleted) {
             L("instance deleted - cannot call any method");
             return
         }
-        a(d, c())
+        a(F, c())
     }
 
-    function f(d) {
+    function f(F) {
         if (e.deleted) {
             L("instance deleted - cannot call any method");
             return
         }
-        u(d, c())
+        u(F, c())
     }
 
     function C() {
-        var d = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
-        return e.deleted ? (L("instance deleted - cannot call any method"), null) : (t.shouldUpdate() && t.update(), e.output[d])
+        var F = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
+        return e.deleted ? (L("instance deleted - cannot call any method"), null) : (t.shouldUpdate() && t.update(), e.output[F])
     }
     t.shouldUpdate = function() {
-        for (var d = t.getMTime(), p = 1 / 0, l = n; l--;) {
+        for (var F = t.getMTime(), p = 1 / 0, l = n; l--;) {
             if (!e.output[l] || e.output[l].isDeleted()) return !0;
             var D = e.output[l].getMTime();
-            if (D < d) return !0;
+            if (D < F) return !0;
             D < p && (p = D)
         }
         for (l = e.numberOfInputs; l--;) {
             var h, A;
             if ((h = e.inputConnection[l]) !== null && h !== void 0 && h.filter.shouldUpdate() || ((A = t.getInputData(l)) === null || A === void 0 ? void 0 : A.getMTime()) > p) return !0
         }
         return !1
     };
 
     function g() {
-        var d = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0,
+        var F = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0,
             p = function() {
-                return C(d)
+                return C(F)
             };
         return p.filter = t, p
     }
     if (e.numberOfInputs) {
-        for (var F = e.numberOfInputs; F--;) e.inputData.push(null), e.inputConnection.push(null);
+        for (var d = e.numberOfInputs; d--;) e.inputData.push(null), e.inputConnection.push(null);
         t.setInputData = u, t.setInputConnection = a, t.addInputData = f, t.addInputConnection = s, t.getInputData = o, t.getInputConnection = i
     }
     n && (t.getOutputData = C, t.getOutputPort = g), t.update = function() {
-        var d = [];
+        var F = [];
         if (e.numberOfInputs)
-            for (var p = 0; p < e.numberOfInputs;) d[p] = t.getInputData(p), p++;
-        t.shouldUpdate() && t.requestData && t.requestData(d, e.output)
+            for (var p = 0; p < e.numberOfInputs;) F[p] = t.getInputData(p), p++;
+        t.shouldUpdate() && t.requestData && t.requestData(F, e.output)
     }, t.getNumberOfInputPorts = function() {
         return e.numberOfInputs
     }, t.getNumberOfOutputPorts = function() {
         return n || e.output.length
-    }, t.getInputArrayToProcess = function(d) {
-        var p = e.inputArrayToProcess[d],
-            l = e.inputData[d];
+    }, t.getInputArrayToProcess = function(F) {
+        var p = e.inputArrayToProcess[F],
+            l = e.inputData[F];
         return p && l ? l["get".concat(p.fieldAssociation)]().getArray(p.arrayName) : null
-    }, t.setInputArrayToProcess = function(d, p, l) {
-        for (var D = arguments.length > 3 && arguments[3] !== void 0 ? arguments[3] : "Scalars"; e.inputArrayToProcess.length < d;) e.inputArrayToProcess.push(null);
-        e.inputArrayToProcess[d] = {
+    }, t.setInputArrayToProcess = function(F, p, l) {
+        for (var D = arguments.length > 3 && arguments[3] !== void 0 ? arguments[3] : "Scalars"; e.inputArrayToProcess.length < F;) e.inputArrayToProcess.push(null);
+        e.inputArrayToProcess[F] = {
             arrayName: p,
             fieldAssociation: l,
             attributeType: D
         }
     }
 }
-var ar = Symbol("Event abort");
+var ir = Symbol("Event abort");
 
-function Pu(t, e, r) {
+function Vu(t, e, r) {
     var n = [],
         u = t.delete,
         o = 1;
 
     function a(s) {
         for (var f = 0; f < n.length; ++f) {
-            var C = de(n[f], 1),
+            var C = Fe(n[f], 1),
                 g = C[0];
             if (g === s) {
                 n.splice(f, 1);
                 return
             }
         }
     }
@@ -2681,77 +2681,77 @@
     function c() {
         var s = arguments;
         if (e.deleted) {
             L("instance deleted - cannot call any method");
             return
         }
         for (var f = n.slice(), C = function(p) {
-                var l = de(f[p], 3),
+                var l = Fe(f[p], 3),
                     D = l[1],
                     h = l[2];
                 if (!D) return "continue";
                 if (h < 0) setTimeout(function() {
                     return D.apply(t, s)
                 }, 1 - h);
                 else {
                     var A = D.apply(t, s);
-                    if (A === ar) return "break"
+                    if (A === ir) return "break"
                 }
             }, g = 0; g < f.length; ++g) {
-            var F = C(g);
-            if (F !== "continue" && F === "break") break
+            var d = C(g);
+            if (d !== "continue" && d === "break") break
         }
     }
     t["invoke".concat(_(r))] = c, t["on".concat(_(r))] = function(s) {
         var f = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0;
         if (!s.apply) return console.error("Invalid callback for event ".concat(r)), null;
         if (e.deleted) return L("instance deleted - cannot call any method"), null;
         var C = o++;
-        return n.push([C, s, f]), n.sort(function(g, F) {
-            return F[2] - g[2]
+        return n.push([C, s, f]), n.sort(function(g, d) {
+            return d[2] - g[2]
         }), i(C)
     }, t.delete = function() {
         u(), n.forEach(function(s) {
-            var f = de(s, 1),
+            var f = Fe(s, 1),
                 C = f[0];
             return a(C)
         })
     }
 }
 
-function Vu(t, e) {
+function Iu(t, e) {
     var r = function() {
         var u = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {},
             o = {},
             a = {};
         return t(a, o, u), Object.freeze(a)
     };
     return e && Y.register(e, r), r
 }
 
-function Iu() {
+function Hu() {
     for (var t = arguments.length, e = new Array(t), r = 0; r < t; r++) e[r] = arguments[r];
     return function() {
         for (var n = arguments.length, u = new Array(n), o = 0; o < n; o++) u[o] = arguments[o];
         return e.filter(function(a) {
             return !!a
         }).map(function(a) {
             return a.apply(void 0, u)
         })
     }
 }
 
-function ir(t) {
+function sr(t) {
     return t && t.isA && t.isA("vtkObject")
 }
 
 function Qe(t, e) {
     var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : [],
         n = arguments.length > 3 && arguments[3] !== void 0 ? arguments[3] : [];
-    if (ir(t)) {
+    if (sr(t)) {
         if (n.indexOf(t) >= 0) return r;
         n.push(t);
         var u = e(t);
         u !== void 0 && r.push(u);
         var o = t.get();
         Object.keys(o).forEach(function(a) {
             var i = o[a];
@@ -2759,15 +2759,15 @@
                 Qe(c, e, r, n)
             }) : Qe(i, e, r, n)
         })
     }
     return r
 }
 
-function Hu(t, e, r) {
+function zu(t, e, r) {
     var n = this,
         u, o = function() {
             for (var i = arguments.length, c = new Array(i), s = 0; s < i; s++) c[s] = arguments[s];
             var f = n,
                 C = function() {
                     u = null, r || t.apply(f, c)
                 },
@@ -2775,34 +2775,34 @@
             clearTimeout(u), u = setTimeout(C, e), g && t.apply(f, c)
         };
     return o.cancel = function() {
         return clearTimeout(u)
     }, o
 }
 
-function zu(t, e) {
+function Ku(t, e) {
     var r = !1,
         n = null;
 
     function u() {
-        r = !1, n !== null && (o.apply(void 0, Mt(n)), n = null)
+        r = !1, n !== null && (o.apply(void 0, Pt(n)), n = null)
     }
 
     function o() {
         for (var a = arguments.length, i = new Array(a), c = 0; c < a; c++) i[c] = arguments[c];
         if (r) {
             n = i;
             return
         }
         r = !0, t.apply(void 0, i), setTimeout(u, e)
     }
     return o
 }
 
-function sr(t, e) {
+function cr(t, e) {
     var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : {};
     e.keystore = Object.assign(e.keystore || {}, r), t.setKey = function(n, u) {
         e.keystore[n] = u
     }, t.getKey = function(n) {
         return e.keystore[n]
     }, t.getAllKeys = function() {
         return Object.keys(e.keystore)
@@ -2810,21 +2810,21 @@
         return delete e.keystore[n]
     }, t.clearKeystore = function() {
         return t.getAllKeys().forEach(function(n) {
             return delete e.keystore[n]
         })
     }
 }
-var Ku = 1,
+var Gu = 1,
     he = "__root__";
 
-function Gu(t, e) {
-    sr(t, e);
+function Wu(t, e) {
+    cr(t, e);
     var r = t.delete;
-    e.proxyId = "".concat(Ku++), e.ui = JSON.parse(JSON.stringify(e.ui || [])), je(t, e, ["proxyId", "proxyGroup", "proxyName"]), nr(t, e, ["proxyManager"]);
+    e.proxyId = "".concat(Gu++), e.ui = JSON.parse(JSON.stringify(e.ui || [])), je(t, e, ["proxyId", "proxyGroup", "proxyName"]), ur(t, e, ["proxyManager"]);
     var n = {},
         u = {};
 
     function o(s, f) {
         u[f] || (u[f] = []);
         for (var C = u[f], g = 0; g < s.length; g++) C.push(s[g].name), n[s[g].name] = s[g], s[g].children && s[g].children.length && o(s[g].children, s[g].name)
     }
@@ -2853,43 +2853,43 @@
     }, t.gcPropertyLinks = function(s) {
         for (var f = e.propertyLinkSubscribers[s] || []; f.length;) f.pop().unbind(t)
     }, e.propertyLinkMap = {}, t.getPropertyLink = function(s) {
         var f = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !1;
         if (e.propertyLinkMap[s]) return e.propertyLinkMap[s];
         var C = null,
             g = [],
-            F = 0,
-            d = !1;
+            d = 0,
+            F = !1;
 
         function p(E) {
             var S = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !1;
-            if (d) return null;
+            if (F) return null;
             var j = [],
                 M = null;
-            for (F = g.length; F--;) {
-                var P = g[F];
+            for (d = g.length; d--;) {
+                var P = g[d];
                 P.instance === E ? M = P : j.push(P)
             }
             if (!M) return null;
             var se = M.instance["get".concat(_(M.propertyName))]();
-            if (!ju(se, C) || S) {
-                for (C = se, d = !0; j.length;) {
+            if (!Ru(se, C) || S) {
+                for (C = se, F = !0; j.length;) {
                     var it = j.pop();
                     it.instance.set(Be({}, it.propertyName, C))
                 }
-                d = !1
+                F = !1
             }
             return e.propertyLinkMap[s].persistent && (e.propertyLinkMap[s].value = se), se
         }
 
         function l(E, S) {
             var j = [];
-            for (F = g.length; F--;) {
-                var M = g[F];
-                M.instance === E && (M.propertyName === S || S === void 0) && (M.subscription.unsubscribe(), j.push(F))
+            for (d = g.length; d--;) {
+                var M = g[d];
+                M.instance === E && (M.propertyName === S || S === void 0) && (M.subscription.unsubscribe(), j.push(d))
             }
             for (; j.length;) g.splice(j.pop(), 1)
         }
 
         function D(E, S) {
             var j = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : !1,
                 M = E.onModified(p),
@@ -2914,24 +2914,24 @@
             unsubscribe: h,
             persistent: f
         };
         return e.propertyLinkMap[s] = A, A
     };
 
     function i() {
-        for (var s = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : he, f = [], C = e.proxyId, g = a(s) || [], F = 0; F < g.length; F++) {
-            var d = g[F],
-                p = t["get".concat(_(d))],
+        for (var s = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : he, f = [], C = e.proxyId, g = a(s) || [], d = 0; d < g.length; d++) {
+            var F = g[d],
+                p = t["get".concat(_(F))],
                 l = p ? p() : void 0,
                 D = {
                     id: C,
-                    name: d,
+                    name: F,
                     value: l
                 },
-                h = i(d);
+                h = i(F);
             h.length && (D.children = h), f.push(D)
         }
         return f
     }
     t.listPropertyNames = function() {
         return i().map(function(s) {
             return s.name
@@ -2958,45 +2958,45 @@
 
     function c() {
         if (e.links)
             for (var s = 0; s < e.links.length; s++) {
                 var f = e.links[s],
                     C = f.link,
                     g = f.property,
-                    F = f.persistent,
-                    d = f.updateOnBind,
+                    d = f.persistent,
+                    F = f.updateOnBind,
                     p = f.type;
                 if (p === "application") {
-                    var l = e.proxyManager.getPropertyLink(C, F);
-                    t.registerPropertyLinkForGC(l, "application"), l.bind(t, g, d)
+                    var l = e.proxyManager.getPropertyLink(C, d);
+                    t.registerPropertyLinkForGC(l, "application"), l.bind(t, g, F)
                 }
             }
     }
-    tr(c)
+    rr(c)
 }
 
-function Wu(t, e, r) {
+function Ju(t, e, r) {
     for (var n = t.delete, u = [], o = Object.keys(r), a = o.length; a--;) {
         var i = o[a],
             c = r[i],
             s = c.modelKey,
             f = c.property,
             C = c.modified,
             g = C === void 0 ? !0 : C,
-            F = _(f),
-            d = _(i);
-        t["get".concat(d)] = e[s]["get".concat(F)], t["set".concat(d)] = e[s]["set".concat(F)], g && u.push(e[s].onModified(t.modified))
+            d = _(f),
+            F = _(i);
+        t["get".concat(F)] = e[s]["get".concat(d)], t["set".concat(F)] = e[s]["set".concat(d)], g && u.push(e[s].onModified(t.modified))
     }
     t.delete = function() {
         for (; u.length;) u.pop().unsubscribe();
         n()
     }
 }
 
-function Ju(t, e) {
+function qu(t, e) {
     var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : {},
         n = arguments.length > 3 && arguments[3] !== void 0 ? arguments[3] : {};
     e.this = t;
 
     function u(c) {
         for (var s = Object.keys(c), f = s.length; f--;) {
             var C = s[f];
@@ -3017,73 +3017,73 @@
         }; a--;) i();
     o.length && je(t, e, o)
 }
 var vt = 10,
     mt = 40,
     wt = 800;
 
-function qu(t) {
+function Xu(t) {
     var e = 0,
         r = 0,
         n = 0,
         u = 0;
     return "detail" in t && (r = t.detail), "wheelDelta" in t && (r = -t.wheelDelta / 120), "wheelDeltaY" in t && (r = -t.wheelDeltaY / 120), "wheelDeltaX" in t && (e = -t.wheelDeltaX / 120), "axis" in t && t.axis === t.HORIZONTAL_AXIS && (e = r, r = 0), n = e * vt, u = r * vt, "deltaY" in t && (u = t.deltaY), "deltaX" in t && (n = t.deltaX), (n || u) && t.deltaMode && (t.deltaMode === 1 ? (n *= mt, u *= mt) : (n *= wt, u *= wt)), n && !e && (e = n < 1 ? -1 : 1), u && !r && (r = u < 1 ? -1 : 1), {
         spinX: e,
         spinY: r,
         pixelX: n,
         pixelY: u
     }
 }
 var k = {
-    algo: Mu,
+    algo: Pu,
     capitalize: ot,
-    chain: Iu,
-    debounce: Hu,
-    enumToString: Ru,
-    event: Pu,
-    EVENT_ABORT: ar,
-    formatBytesToProperUnit: Tu,
-    formatNumbersWithThousandSeparator: xu,
+    chain: Hu,
+    debounce: zu,
+    enumToString: Lu,
+    event: Vu,
+    EVENT_ABORT: ir,
+    formatBytesToProperUnit: xu,
+    formatNumbersWithThousandSeparator: ju,
     get: je,
-    getArray: ur,
-    getCurrentGlobalMTime: Eu,
-    getStateArrayMapFunc: er,
-    isVtkObject: ir,
-    keystore: sr,
-    measurePromiseExecution: Lu,
-    moveToProtected: Nu,
-    newInstance: Vu,
-    newTypedArray: Su,
-    newTypedArrayFrom: bu,
-    normalizeWheel: qu,
-    obj: ku,
-    proxy: Gu,
-    proxyPropertyMapping: Wu,
-    proxyPropertyState: Ju,
-    safeArrays: Zt,
-    set: rr,
-    setArray: or,
-    setGet: nr,
-    setGetArray: $u,
-    setImmediate: tr,
-    setLoggerFunction: vu,
-    throttle: zu,
+    getArray: or,
+    getCurrentGlobalMTime: Au,
+    getStateArrayMapFunc: tr,
+    isVtkObject: sr,
+    keystore: cr,
+    measurePromiseExecution: ku,
+    moveToProtected: Mu,
+    newInstance: Iu,
+    newTypedArray: bu,
+    newTypedArrayFrom: Ou,
+    normalizeWheel: Xu,
+    obj: _u,
+    proxy: Wu,
+    proxyPropertyMapping: Ju,
+    proxyPropertyState: qu,
+    safeArrays: er,
+    set: nr,
+    setArray: ar,
+    setGet: ur,
+    setGetArray: Nu,
+    setImmediate: rr,
+    setLoggerFunction: mu,
+    throttle: Ku,
     traverseInstanceTree: Qe,
     TYPED_ARRAYS: $,
-    uncapitalize: Ou,
-    VOID: du,
+    uncapitalize: Tu,
+    VOID: Eu,
     vtkDebugMacro: Ye,
     vtkErrorMacro: L,
-    vtkInfoMacro: wu,
-    vtkLogMacro: mu,
-    vtkOnceErrorMacro: Bu,
-    vtkWarningMacro: Qt
+    vtkInfoMacro: Bu,
+    vtkLogMacro: wu,
+    vtkOnceErrorMacro: Su,
+    vtkWarningMacro: Zt
 };
 
-function Xu(t) {
+function Yu(t) {
     return {
         subscribeToImageStream: function(r) {
             return t.subscribe("viewport.image.push.subscription", r)
         },
         unsubscribeToImageStream: function(r) {
             return t.unsubscribe(r)
         },
@@ -3143,15 +3143,15 @@
                 n = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : {},
                 u = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : !0;
             return t.call("viewport.camera.update.params", [r, n, u])
         }
     }
 }
 
-function Yu(t, e) {
+function Qu(t, e) {
     e.classHierarchy.push("vtkViewStream"), e.imageDecodingPool = [new Image, new Image], e.eventPool = [], e.nextPoolImageIndex = 0, e.urlToRevoke = [], e.activeURL = null, e.fps = [], e.lastTime = Date.now(), e.lastImageEvent = null;
 
     function r(o) {
         var a = Number(this.dataset.id);
         t.invokeImageReady(e.eventPool[a])
     }
 
@@ -3230,53 +3230,53 @@
                     }
                 }, e.decodeImage ? u(e.lastImageEvent) : t.invokeImageReady(e.lastImageEvent); e.fps.length > e.fpsWindowSize;) e.fps.shift()
         }
     }, t.delete = k.chain(function() {
         for (e.unregisterViewStream(t), t.setViewId(null); e.urlToRevoke.length;) window.URL.revokeObjectURL(e.urlToRevoke.pop())
     }, t.delete), n()
 }
-var Qu = {
+var Zu = {
     cameraUpdateRate: 30,
     decodeImage: !0,
     fpsWindowSize: 250,
     interactiveQuality: 80,
     interactiveRatio: 1,
     isAnimating: !1,
     mimeType: "image/jpeg",
     size: [-1, -1],
     stillQuality: 100,
     stillRatio: 1,
     useCameraParameters: !1,
     viewId: null
 };
 
-function cr(t, e) {
+function fr(t, e) {
     var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : {};
-    Object.assign(e, Qu, r), k.obj(t, e), k.event(t, e, "ImageReady"), k.get(t, e, ["viewId", "size", "fps", "lastImageEvent"]), k.setGet(t, e, ["camera", "cameraUpdateRate", "decodeImage", "fpsWindowSize", "interactiveQuality", "interactiveRatio", "stillQuality", "stillRatio", "useCameraParameters"]), Yu(t, e), Object.assign(t, e.sharedAPI)
+    Object.assign(e, Zu, r), k.obj(t, e), k.event(t, e, "ImageReady"), k.get(t, e, ["viewId", "size", "fps", "lastImageEvent"]), k.setGet(t, e, ["camera", "cameraUpdateRate", "decodeImage", "fpsWindowSize", "interactiveQuality", "interactiveRatio", "stillQuality", "stillRatio", "useCameraParameters"]), Qu(t, e), Object.assign(t, e.sharedAPI)
 }
-var Zu = k.newInstance(cr, "vtkViewStream"),
-    eo = {
-        newInstance: Zu,
-        extend: cr
+var eo = k.newInstance(fr, "vtkViewStream"),
+    to = {
+        newInstance: eo,
+        extend: fr
     };
 
-function to(t, e) {
+function ro(t, e) {
     e.classHierarchy.push("vtkImageStream");
 
     function r(n) {
         var u = n[0];
         if (!(!u || !u.image))
             for (var o = 0; o < e.viewStreams.length; o++) e.viewStreams[o].processMessage(u)
     }
     t.setServerAnimationFPS = function() {
         var n = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 30,
             u = !1;
         return e.serverAnimationFPS !== n && (e.serverAnimationFPS = n, u = !0), e.protocol ? (u && t.modified(), e.protocol.setServerAnimationFPS(n)) : Promise.resolve(!0)
     }, t.connect = function(n) {
-        var u = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : Xu;
+        var u = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : Yu;
         e.connected || !n || !u || (e.protocol = u(n), e.protocol.subscribeToImageStream(r).promise.then(function(o) {
             e.renderTopicSubscription = o, e.connected = !0
         }).catch(function(o) {
             e.connected = !1, console.error(o)
         }))
     }, t.disconnect = function() {
         e.protocol && e.connected && e.renderTopicSubscription && (e.protocol.unsubscribeToImageStream(e.renderTopicSubscription), e.renderTopicSubscription = null), e.connected = !1
@@ -3288,49 +3288,49 @@
         })
     }, t.createViewStream = function() {
         var n = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : "-1",
             u = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : [400, 400],
             o = t.setServerAnimationFPS,
             a = t.getServerAnimationFPS,
             i = t.unregisterViewStream,
-            c = eo.newInstance({
+            c = to.newInstance({
                 protocol: e.protocol,
                 unregisterViewStream: i,
                 sharedAPI: {
                     setServerAnimationFPS: o,
                     getServerAnimationFPS: a
                 }
             });
         return c.setViewId(n), c.setSize(u[0], u[1]), t.registerViewStream(c), c
     }, t.delete = k.chain(function() {
         for (; e.viewStreams.length;) e.viewStreams.pop().delete();
         t.disconnect()
     }, t.delete)
 }
-var ro = {
+var no = {
     viewStreams: [],
     serverAnimationFPS: -1
 };
 
-function fr(t, e) {
+function Dr(t, e) {
     var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : {};
-    Object.assign(e, ro, r), k.obj(t, e), k.get(t, e, ["serverAnimationFPS", "protocol"]), to(t, e)
+    Object.assign(e, no, r), k.obj(t, e), k.get(t, e, ["serverAnimationFPS", "protocol"]), ro(t, e)
 }
-var no = k.newInstance(fr, "vtkImageStream"),
-    uo = {
-        newInstance: no,
-        extend: fr
+var uo = k.newInstance(Dr, "vtkImageStream"),
+    oo = {
+        newInstance: uo,
+        extend: Dr
     },
     Ze = null;
 
-function oo(t) {
+function ao(t) {
     Ze = t
 }
 
-function ao(t, e) {
+function io(t, e) {
     return function() {
         for (var r = arguments.length, n = new Array(r), u = 0; u < r; u++) n[u] = arguments[u];
         return new Promise(function(o, a) {
             e(1), t.apply(void 0, n).then(function(i) {
                 e(-1), o(i)
             }, function(i) {
                 e(-1), a(i)
@@ -3339,19 +3339,19 @@
     }
 }
 
 function Bt(t, e) {
     var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : [],
         n = {};
     return Object.keys(t).forEach(function(u) {
-        r.indexOf(u) === -1 ? n[u] = ao(t[u], e) : n[u] = t[u]
+        r.indexOf(u) === -1 ? n[u] = io(t[u], e) : n[u] = t[u]
     }), n
 }
 
-function io(t, e) {
+function so(t, e) {
     e.classHierarchy.push("vtkWSLinkClient");
 
     function r() {
         t.invokeBusyChange(e.busyCount)
     }
 
     function n() {
@@ -3374,15 +3374,15 @@
                 config: u,
                 configDecorator: e.configDecorator
             }), e.smartConnect.onConnectionReady(function(c) {
                 e.connection = c, e.remote = {}, e.config = e.smartConnect.getConfig();
                 var s = c.getSession();
                 e.protocols = e.protocols || {}, Object.keys(e.protocols).forEach(function(f) {
                     e.remote[f] = Bt(e.protocols[f](s), n, e.notBusyList)
-                }), e.createImageStream && (e.imageStream = uo.newInstance(), e.imageStream.connect(s)), t.invokeConnectionReady(t), a(t)
+                }), e.createImageStream && (e.imageStream = oo.newInstance(), e.imageStream.connect(s)), t.invokeConnectionReady(t), a(t)
             }), e.smartConnect.onConnectionError(function(c) {
                 t.invokeConnectionError(c), i(c)
             }), e.smartConnect.onConnectionClose(function(c) {
                 t.invokeConnectionClose(c), i(c)
             }), e.smartConnect.connect()
         })) : Promise.reject(new Error("Need to provide SmartConnect"))
     }, t.disconnect = function() {
@@ -3390,33 +3390,33 @@
         e.connection && (e.connection.destroy(u), e.connection = null)
     }, t.registerProtocol = function(u, o) {
         e.remote[u] = Bt(o(e.connection.getSession()), n, e.notBusyList)
     }, t.unregisterProtocol = function(u) {
         delete e.remote[u]
     }
 }
-var so = {
+var co = {
     notBusyList: [],
     busyCount: 0,
     timeoutId: 0,
     notificationTimeout: 50,
     createImageStream: !0
 };
 
-function Dr(t, e) {
+function lr(t, e) {
     var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : {};
-    Object.assign(e, so, r), k.obj(t, e), k.setGet(t, e, ["protocols", "notBusyList", "createImageStream", "configDecorator"]), k.get(t, e, ["connection", "config", "remote", "imageStream"]), k.event(t, e, "BusyChange"), k.event(t, e, "ConnectionReady"), k.event(t, e, "ConnectionError"), k.event(t, e, "ConnectionClose"), io(t, e)
+    Object.assign(e, co, r), k.obj(t, e), k.setGet(t, e, ["protocols", "notBusyList", "createImageStream", "configDecorator"]), k.get(t, e, ["connection", "config", "remote", "imageStream"]), k.event(t, e, "BusyChange"), k.event(t, e, "ConnectionReady"), k.event(t, e, "ConnectionError"), k.event(t, e, "ConnectionClose"), so(t, e)
 }
-var co = k.newInstance(Dr, "vtkWSLinkClient"),
-    lr = {
-        newInstance: co,
-        extend: Dr,
-        setSmartConnectClass: oo
+var fo = k.newInstance(lr, "vtkWSLinkClient"),
+    pr = {
+        newInstance: fo,
+        extend: lr,
+        setSmartConnectClass: ao
     };
-const fo = t => ({
+const Do = t => ({
         getArray(e, r = !0) {
             return t.call("viewport.geometry.array.get", [e, r])
         },
         getViewState(e, r = !1) {
             return t.call("viewport.geometry.view.get.state", [e, r])
         },
         addViewObserver(e) {
@@ -3428,15 +3428,15 @@
         subscribeToViewChange(e) {
             return t.subscribe("viewport.geometry.view.subscription", e)
         },
         unsubscribe(e) {
             return t.unsubscribe(e)
         }
     }),
-    Do = t => ({
+    lo = t => ({
         lifeCycleUpdate(e) {
             return t.call("trame.lifecycle.update", [e])
         },
         sendError(e) {
             return t.call("trame.error.client", [e])
         },
         getState() {
@@ -3454,37 +3454,37 @@
         subscribeToActions(e) {
             return t.subscribe("trame.actions.topic", e)
         },
         unsubscribe(e) {
             return t.unsubscribe(e)
         }
     }),
-    lo = {
-        SyncView: fo,
-        Trame: Do
+    po = {
+        SyncView: Do,
+        Trame: lo
     };
-lr.setSmartConnectClass(ln);
-const po = {
+pr.setSmartConnectClass(pn);
+const yo = {
         "http:": "ws:",
         "https:": "wss:",
         "ws:": "ws:",
         "wss:": "wss:"
     },
-    yo = ["unsubscribe", "subscribeToViewChange", "subscribeToStateUpdate", "subscribeToActions", "subscribeToViewChange"];
+    go = ["unsubscribe", "subscribeToViewChange", "subscribeToStateUpdate", "subscribeToActions", "subscribeToViewChange"];
 
-function pr(t) {
+function yr(t) {
     const e = {
         ...t
     };
     if (e.sessionURL) {
         let n = e.sessionURL.toLowerCase();
         const u = window.location;
         if (n.includes("use_")) {
             const a = new URL(n);
-            a.protocol = po[u.protocol], n = a.toString()
+            a.protocol = yo[u.protocol], n = a.toString()
         }
         const o = {
             use_hostname: u.hostname,
             use_host: u.host
         };
         for (const [a, i] of Object.entries(o)) n = n.replaceAll(a, i);
         e.sessionURL = n
@@ -3493,57 +3493,57 @@
     const r = document.querySelector("html").dataset.sessionManagerUrl || e.sessionManagerURL;
     return r && (e.sessionManagerURL = r), e.useUrl ? {
         ...e,
         ...oe.extractURLParameters()
     } : e
 }
 
-function go() {
-    return lr.newInstance({
-        protocols: lo,
-        configDecorator: pr,
-        notBusyList: yo
+function Co() {
+    return pr.newInstance({
+        protocols: po,
+        configDecorator: yr,
+        notBusyList: go
     })
 }
 const et = {
-    configDecorator: pr,
-    createClient: go
+    configDecorator: yr,
+    createClient: Co
 };
 var ie = [];
 
-function Co(t) {
+function ho(t) {
     return new Promise(function(e, r) {
         if (ie.indexOf(t) === -1) {
             ie.push(t);
             var n = document.createElement("script");
             n.type = "text/javascript", n.src = t, n.onload = e, n.onerror = r, document.body.appendChild(n)
         } else e(!1)
     })
 }
 
-function ho(t) {
+function Fo(t) {
     return new Promise(function(e, r) {
         if (ie.indexOf(t) === -1) {
             ie.push(t);
             var n = document.createElement("script");
             n.type = "module", n.src = t, n.onload = e, n.onerror = r, document.body.appendChild(n)
         } else e(!1)
     })
 }
 
-function Fo(t) {
+function Eo(t) {
     return new Promise(function(e, r) {
         if (ie.indexOf(t) === -1) {
             ie.push(t);
             var n = document.createElement("link");
             n.rel = "stylesheet", n.href = t, n.onload = e, n.onerror = r, document.head.appendChild(n)
         } else e(!1)
     })
 }
-async function Eo(t, e) {
+async function Ao(t, e) {
     for (let r = 0; r < t.length; r++) await e(t[r])
 }
 
 function Ie(t, e) {
     const r = [],
         n = {};
     for (let a = 0; a < t.length; a++) {
@@ -3553,19 +3553,19 @@
             const s = c[1].serial;
             s && (n[s] || (n[s] = []), i = n[s]), [c] = c
         }
         i.push(c)
     }
     const u = r.map(e),
         o = Object.values(n);
-    for (let a = 0; a < o.length; a++) u.push(Eo(o[a], e));
+    for (let a = 0; a < o.length; a++) u.push(Ao(o[a], e));
     return Promise.all(u)
 }
-async function Ao(t) {
-    return await Ie(t.trame__styles, Fo), await Ie(t.trame__scripts, Co), await Ie(t.trame__module_scripts, ho), t.trame__favicon && (document.querySelector("link[rel=icon]").href = t.trame__favicon), t.trame__title && (document.title = t.trame__title), t.trame__vue_use.map(e => {
+async function vo(t) {
+    return await Ie(t.trame__styles, Eo), await Ie(t.trame__scripts, ho), await Ie(t.trame__module_scripts, Fo), t.trame__favicon && (document.querySelector("link[rel=icon]").href = t.trame__favicon), t.trame__title && (document.title = t.trame__title), t.trame__vue_use.map(e => {
         let r = e,
             n = [];
         Array.isArray(e) && ([r, ...n] = e);
         let u = window.eval(r);
         for (let o = 0; o < n.length; o++) {
             const a = n[o];
             a.js_eval && (n[o] = window.eval(a.js_eval))
@@ -3575,19 +3575,19 @@
             return
         }
         return [u, ...n]
     })
 }
 const tt = {};
 
-function vo(t, e) {
+function mo(t, e) {
     return t.priority - e.priority
 }
 
-function mo(t) {
+function wo(t) {
     tt.addAttachement = t
 }
 const He = 2e6,
     at = {
         priority: 0,
         async decorate(t) {
             if (t == null) return t;
@@ -3619,72 +3619,72 @@
                     content: a,
                     _filter: ["content"]
                 }
             }
             return t
         }
     },
-    yr = {
+    gr = {
         priority: 0,
         async decorate(t) {
             if (t == null || typeof t == "string") return t;
             if (t.constructor && t.constructor === FileList || t.length) {
                 const e = [];
                 for (let r = 0; r < t.length; r++) e.push(await at.decorate(t[r]));
                 return e
             }
             return t
         }
     },
-    wo = {
+    Bo = {
         priority: 0,
         async decorate(t) {
             if (t == null || typeof t == "string") return t;
             if (t.constructor && t.constructor === Object) {
                 const e = {},
                     r = Object.keys(t);
                 for (let n = 0; n < r.length; n++) {
                     const u = r[n];
-                    e[u] = t[u], e[u] = await yr.decorate(e[u]), e[u] = await at.decorate(e[u])
+                    e[u] = t[u], e[u] = await gr.decorate(e[u]), e[u] = await at.decorate(e[u])
                 }
                 return e
             }
             return t
         }
     },
-    xe = [at, yr, wo];
+    xe = [at, gr, Bo];
 
-function Bo(t) {
-    xe.push(t), xe.sort(vo)
+function So(t) {
+    xe.push(t), xe.sort(mo)
 }
 async function rt(t) {
     let e = t;
     for (let r = 0; r < xe.length; r++) {
         if (e == null) return e;
         e = await xe[r].decorate(e)
     }
     return e
 }
-class So {
+class bo {
     constructor(e) {
-        this.name = "Default trame application", this.client = e, this.subscriptions = [], this.dirtyKeys = new Set, this.state = {}, this.keyTS = {}, this.mtime = 0, this.listeners = [], this.ready = !1, this.registerDecorator = Bo;
+        this.name = "Default trame application", this.client = e, this.subscriptions = [], this.dirtyKeys = new Set, this.state = {}, this.keyTS = {}, this.mtime = 0, this.listeners = [], this.ready = !1, this.registerDecorator = So;
         const r = async n => {
             var i;
             const u = [],
                 o = Object.keys(n);
             for (let c = 0; c < o.length; c++) {
                 let s = !0;
                 const f = o[c],
                     C = n[f];
                 if ((i = C == null ? void 0 : C._filter) != null && i.length) {
                     s = !1;
                     const g = this.state[f],
-                        F = Object.keys(C);
-                    for (let d = 0; !s && d < F.length; d++) {
-                        const p = F[d];
+                        d = Object.keys(C);
+                    for (let F = 0; !s && F < d.length; F++) {
+                        const p = d[F];
                         p[0] !== "_" && (g === void 0 || g[p] !== C[p]) && (s = !0)
                     }
                 }
                 s && (u.push(f), this.state[f] = C)
             }
             this.mtime += 1;
             let a = 0;
@@ -3768,120 +3768,120 @@
             this.client.isConnected() && await this.client.getRemote().Trame.updateState(o), this.dirtyKeys.size && this.flush()
         }
         this.client.isConnected() || this._updateFromServer(this.state)
     }
 }
 const St = ["type", "key", "keyCode", "controlKey", "altKey", "shiftKey", "position", "spinX", "spinY", "pixelX", "pixelY"];
 
-function bo(t) {
+function Oo(t) {
     const e = {};
     for (let r = 0; r < St.length; r++) {
         const n = St[r];
         n in t && (e[n] = t[n])
     }
     return e
 }
-const Oo = {
-    event: bo
+const To = {
+    event: Oo
 };
 
-function gr(t, e = [], r = 1e3, n = 2) {
+function Cr(t, e = [], r = 1e3, n = 2) {
     if (t === null) return null;
     for (let u = 0; u < e.length; u++) {
         const o = Array.isArray(r) ? r[u] : r,
             a = e[u];
         if (t > o) t /= o;
         else return `${t.toFixed(n)} ${a}`
     }
     return `${t.toFixed(n)} ${r[r.length-1]}`
 }
 
-function To(t, e = 2) {
-    return gr(t, ["B", "KB", "MB", "GB", "TB", "PB"], 1024, e)
+function xo(t, e = 2) {
+    return Cr(t, ["B", "KB", "MB", "GB", "TB", "PB"], 1024, e)
 }
-const xo = {
-    number: gr,
-    bytes: To
+const jo = {
+    number: Cr,
+    bytes: xo
 };
-async function jo(t, e, r = "application/octet-stream") {
+async function Ro(t, e, r = "application/octet-stream") {
     const n = await Promise.resolve(e),
         u = new Blob([n], {
             type: r
         }),
         o = URL.createObjectURL(u),
         a = document.createElement("a");
     a.setAttribute("href", o), a.setAttribute("download", t), document.body.appendChild(a), a.click(), document.body.removeChild(a), setTimeout(() => URL.revokeObjectURL(o), 1e3)
 }
 
-function Ro(t, e = window) {
+function Lo(t, e = window) {
     let r = e;
     const n = t.endsWith("()"),
         u = (n ? t.slice(0, -2) : t).split(".");
     for (let o = 0; o < u.length; o++) r = r[u[o]];
     return n ? r() : r
 }
 
-function Cr(t) {
+function hr(t) {
     try {
         return JSON.stringify(t), t
     } catch {}
     const e = {},
         r = Object.keys(t);
     for (let n = 0; n < r.length; n++) {
         const u = r[n],
             o = t[u];
-        if (Array.isArray(o)) e[u] = o.map(Cr);
+        if (Array.isArray(o)) e[u] = o.map(hr);
         else try {
             JSON.stringify(o), e[u] = o
         } catch {
             continue
         }
     }
     return e
 }
 
-function Lo(t, e, r) {
+function ko(t, e, r) {
     const n = {
             id: t
         },
         u = e ? `${e}: ` : "";
     return Array.isArray(r) ? (n.name = `${u}[]`, r.length && (n.children = []), n) : r === null || !r ? (n.name = `${u}${r}`, n) : typeof r == "function" ? (n.name = `${u}function`, n) : typeof r == "object" ? (n.name = `${u}{}`, Object.keys(r).length && (n.children = []), n) : (n.name = `${u}${r}`, n)
 }
 
 function bt(t, e, r, n) {
-    const u = Lo(e, r, n);
-    t.push(u), u.children && hr(e, u.children, n)
+    const u = ko(e, r, n);
+    t.push(u), u.children && dr(e, u.children, n)
 }
 
-function hr(t, e, r) {
+function dr(t, e, r) {
     if (Array.isArray(r))
         for (let u = 0; u < r.length; u++) bt(e, `${t}_${u}`, null, r[u]);
     else {
         const n = Object.keys(r);
         for (let u = 0; u < n.length; u++) {
             const o = n[u];
             bt(e, `${t}_${u}`, o, r[o])
         }
     }
 }
 
-function ko(t) {
+function _o(t) {
     const e = [];
-    return hr("", e, t), e
+    return dr("", e, t), e
 }
 const Fr = {
-    download: jo,
-    get: Ro,
-    safe: Cr,
-    tree: ko,
-    vtk: Oo,
-    fmt: xo
+    download: Ro,
+    get: Lo,
+    safe: hr,
+    tree: _o,
+    vtk: To,
+    fmt: jo
 };
 
-function _o(t) {
+function Uo(t) {
     const e = {
         app: t,
         client: null,
         state: null,
         config: null,
         utils: Fr,
         refs: {}
@@ -3898,84 +3898,84 @@
         for (let a = 0; a < r.length; a++) r[a]()
     }
     return e.addConnectListener = function(i) {
         r.push(i), u() && i()
     }, e.removeConnectListener = function(i) {
         r = r.filter(c => c !== i)
     }, e.connect = async function(i) {
-        return e.client || (e.client = et.createClient()), e.state && (e.state.delete(), e.client = et.createClient()), e.client.isConnected() || await e.client.connect(i), mo(e.client.getConnection().getSession().addAttachment), e.state = new So(e.client), e.config = e.client.getConfig(), await e.state.loadState(), n = !0, o(), e.config
+        return e.client || (e.client = et.createClient()), e.state && (e.state.delete(), e.client = et.createClient()), e.client.isConnected() || await e.client.connect(i), wo(e.client.getConnection().getSession().addAttachment), e.state = new bo(e.client), e.config = e.client.getConfig(), await e.state.loadState(), n = !0, o(), e.config
     }, e.trigger = async function(i, c = [], s = {}) {
         let f = [];
         const C = {};
         if (c) {
-            const g = c.map(F => rt(F));
+            const g = c.map(d => rt(d));
             f = await Promise.all(g)
         }
         if (s) {
             const g = [],
-                F = [];
+                d = [];
             Object.entries(s).forEach(p => {
-                g.push(p[0]), F.push(rt(p[1]))
+                g.push(p[0]), d.push(rt(p[1]))
             });
-            const d = await Promise.all(F);
-            for (let p = 0; p < g.length; p++) C[g[p]] = d[p]
+            const F = await Promise.all(d);
+            for (let p = 0; p < g.length; p++) C[g[p]] = F[p]
         }
         return await e.client.getRemote().Trame.trigger(i, f, C)
     }, window.trame = e, e
 }
 const {
-    inject: dr,
-    ref: Er,
-    computed: Uo,
-    onMounted: Ar,
-    onBeforeUnmount: vr,
-    nextTick: $o,
-    customRef: No
+    inject: Er,
+    ref: Ar,
+    computed: $o,
+    onMounted: vr,
+    onBeforeUnmount: mr,
+    nextTick: No,
+    customRef: Mo
 } = window.Vue;
 
-function Mo(t, e, r) {
-    return No((n, u) => (r[e] = u, {
+function Po(t, e, r) {
+    return Mo((n, u) => (r[e] = u, {
         get() {
             return n(), t.state.get(e)
         },
         set(o) {
             t.state.set(e, o), u()
         }
     }))
 }
 
-function Po() {
-    const t = dr("trame"),
-        e = Er(0),
+function Vo() {
+    const t = Er("trame"),
+        e = Ar(0),
         r = {},
         n = {
             trame: t,
             window,
             utils: Fr,
             tts: e
         };
     t.state.getAllKeys().forEach(o => {
-        n[o] = Mo(t, o, r)
+        n[o] = Po(t, o, r)
     });
     const u = ({
         type: o,
         keys: a
     }) => {
         if (o === "dirty-state") {
             for (let i = 0; i < a.length; i++) r[a[i]]();
             a.includes("trame__favicon") && t.state.get("trame__favicon") && (document.querySelector("link[rel=icon]").href = t.state.get("trame__favicon")), a.includes("trame__title") && t.state.get("trame__title") && (document.title = t.state.get("trame__title"))
         }
     };
-    return Ar(() => {
+    return vr(() => {
         t.state.addListener(u)
-    }), vr(() => {
+    }), mr(() => {
         t.state.removeListener(u)
     }), n.trigger = (...o) => t.trigger(...o), n.set = (o, a) => t.state.set(o, a), n.get = o => n[o], n.setAll = o => t.state.update(o), n.flushState = (...o) => t.state.flush(...o), n.registerDecorator = (...o) => t.state.registerDecorator(...o), n
 }
-const Vo = {
+const Io = {
         props: {
             templateName: {
                 type: String,
                 default: "main"
             },
             urlKey: {
                 type: String,
@@ -3983,88 +3983,88 @@
             },
             useUrl: {
                 type: Boolean,
                 default: !1
             }
         },
         setup(t) {
-            const e = dr("trame"),
-                r = Er(0),
-                n = Uo(() => {
+            const e = Er("trame"),
+                r = Ar(0),
+                n = $o(() => {
                     let a = t.templateName;
                     return t.useUrl && oe.extractURLParameters()[t.urlKey] && (a = oe.extractURLParameters()[t.urlKey]), `trame-template-${a.toLowerCase()}`
                 });
             async function u() {
-                await $o(), r.value++
+                await No(), r.value++
             }
             const o = ({
                 type: a,
                 keys: i
             }) => {
                 if (a === "dirty-state")
                     for (let c = 0; c < i.length; c++) i[c].toLowerCase().replaceAll("_", "-").replaceAll("--", "-") === n.value && u()
             };
-            return Ar(() => {
+            return vr(() => {
                 e.state.addListener(o)
-            }), vr(() => {
+            }), mr(() => {
                 e.state.removeListener(o)
             }), {
                 tts: r,
                 componentName: n
             }
         },
         template: '<component :key="tts" :is="componentName" :name="componentName" />'
     },
     {
-        inject: Io,
-        ref: Fe,
-        onBeforeMount: Ho,
-        onBeforeUnmount: zo
+        inject: Ho,
+        ref: de,
+        onBeforeMount: zo,
+        onBeforeUnmount: Ko
     } = window.Vue,
-    Ko = {
+    Go = {
         props: {
             useUrl: {
                 type: Boolean,
                 default: !1
             }
         },
         setup() {
-            const t = Io("trame"),
-                e = Fe(!1),
-                r = Fe(!1),
-                n = Fe(1),
-                u = Fe(1),
+            const t = Ho("trame"),
+                e = de(!1),
+                r = de(!1),
+                n = de(1),
+                u = de(1),
                 o = [];
 
             function a(f) {
                 const C = `trame-template-${f.toLowerCase().substring(16)}`,
                     g = t.state.get(f);
                 t.app.component(C, {
                     props: ["name"],
-                    setup: Po,
+                    setup: Vo,
                     template: g
                 })
             }
             const i = ({
                 type: f,
                 keys: C
             }) => {
                 if (f === "dirty-state")
                     for (let g = 0; g < C.length; g++) {
-                        const F = C[g];
-                        F.startsWith("trame__template_") && a(F)
+                        const d = C[g];
+                        d.startsWith("trame__template_") && a(d)
                     } else f === "refresh" ? u.value++ : f === "ready" && (r.value = !0, u.value++)
             };
 
             function c(f) {
                 n.value = f, t.state && t.state.set("trame__busy", f), f === 0 && t.state.flush()
             }
 
             function s() {
-                var g, F, d;
+                var g, d, F;
                 for (; o.length;) o.pop()();
                 if (o.push(t.client.onBusyChange(c).unsubscribe), e.value = t.client.isConnected(), t.state.addListener(i), o.push(() => t.state.removeListener(i)), t.state.ready) {
                     const p = t.state.getAllKeys();
                     for (let l = 0; l < p.length; l++) {
                         const D = p[l];
                         D.startsWith("trame__template_") && a(D)
                     }
@@ -4091,76 +4091,92 @@
                         h[A] = E
                     }
                 }
                 const C = t.client.getRemote().Trame.subscribeToActions(([p]) => p.map(f));
                 o.push(() => {
                     var p, l, D;
                     return (D = (l = (p = t == null ? void 0 : t.client) == null ? void 0 : p.getRemote()) == null ? void 0 : l.Trame) == null ? void 0 : D.unsubscribe(C)
-                }), (d = (F = (g = t.client) == null ? void 0 : g.getRemote()) == null ? void 0 : F.Trame) == null || d.lifeCycleUpdate("client_connected"), window.addEventListener("beforeunload", () => {
+                }), (F = (d = (g = t.client) == null ? void 0 : g.getRemote()) == null ? void 0 : d.Trame) == null || F.lifeCycleUpdate("client_connected"), window.addEventListener("beforeunload", () => {
                     var p, l, D;
                     return (D = (l = (p = t.client) == null ? void 0 : p.getRemote()) == null ? void 0 : l.Trame) == null ? void 0 : D.lifeCycleUpdate("client_exited")
                 })
             }
-            return Ho(() => {
+            return zo(() => {
                 t.addConnectListener(s)
-            }), zo(() => {
+            }), Ko(() => {
                 var f, C, g;
                 for (t.removeConnectListener(s), (g = (C = (f = t.client) == null ? void 0 : f.getRemote()) == null ? void 0 : C.Trame) == null || g.lifeCycleUpdate("client_unmounted"); o.length;) o.pop()()
             }), {
                 connected: e,
                 ready: r,
                 busy: n,
                 refreshTS: u
             }
         },
         template: '<trame-template v-if="ready" :key="refreshTS" :use-url="useUrl" />'
     },
     {
-        unref: Go
+        unref: Wo
     } = window.Vue,
-    Wo = {
+    Jo = {
         props: ["event"],
         emits: ["exec"],
         setup(t, {
             emit: e
         }) {
             function r(n) {
-                n === void 0 ? e("exec", Go(t.event)) : e("exec", n)
+                n === void 0 ? e("exec", Wo(t.event)) : e("exec", n)
             }
             return {
                 exec: r
             }
         }
     },
     {
-        inject: Jo,
-        ref: qo,
+        inject: qo,
+        ref: Ot,
         onBeforeMount: Xo,
         onBeforeUnmount: Yo,
         watch: Qo
     } = window.Vue,
     Zo = {
         props: ["name"],
         setup(t) {
-            const e = Jo("trame"),
-                r = qo(null);
+            const e = qo("trame"),
+                r = Ot(null),
+                n = Ot(null);
+
+            function u(i, c) {
+                const s = JSON.parse(JSON.stringify(e.state.get(t.name)));
+                let f = s;
+                const C = String(i).split(".");
+                for (let g = 0; g < C.length - 1; g++) f = f[C[g]];
+                f[C.at(-1)] = c, e.state.set(t.name, s)
+            }
+
+            function o(i) {
+                e.state.set(t.name, i)
+            }
 
-            function n() {
-                const u = e.state.get(t.name);
-                u !== r.value && (r.value = u)
+            function a() {
+                const i = e.state.get(t.name);
+                n.value !== t.name && (n.value = t.name), i !== r.value && (r.value = i)
             }
-            return Qo(() => t.name, n), Xo(() => {
-                e.state.addListener(n), n()
+            return Qo(() => t.name, a), Xo(() => {
+                e.state.addListener(a), a()
             }), Yo(() => {
-                e.state.removeListener(n)
+                e.state.removeListener(a)
             }), {
-                computed: r
+                computedValue: r,
+                computedName: n,
+                updateNested: u,
+                update: o
             }
         },
-        template: '<slot :value="computed"></slot>'
+        template: '<slot :name="computedName" :update="update" :updateNested="updateNested" :value="computedValue"></slot>'
     },
     ea = {
         props: {
             message: {
                 type: String,
                 default: "Loading..."
             }
@@ -4269,38 +4285,38 @@
             removeStyle() {
                 const t = document.querySelector(`#${this.elemId}`);
                 t && t.parentNode.removeChild(t)
             }
         },
         template: '<div class="trame-style" />'
     },
-    Ot = {
-        TrameApp: Ko,
-        TrameExec: Wo,
+    Tt = {
+        TrameApp: Go,
+        TrameExec: Jo,
         TrameGetter: Zo,
         TrameLoading: ea,
         TrameReconnect: ua,
         TrameStyle: sa,
-        TrameTemplate: Vo
+        TrameTemplate: Io
     },
     ca = {
         install(t) {
-            Object.keys(Ot).forEach(e => {
-                t.component(e, Ot[e])
+            Object.keys(Tt).forEach(e => {
+                t.component(e, Tt[e])
             })
         }
     },
     {
         createApp: fa
     } = window.Vue;
 async function Da() {
     const t = fa({
         template: "<trame-app use-url />"
     });
-    let e = _o(t),
+    let e = Uo(t),
         r = et.configDecorator({
             application: "trame",
             useUrl: !0
         });
     e.addConnectListener(() => {
         e.client.onConnectionError(a => {
             var i;
@@ -4330,12 +4346,12 @@
             e.client.isConnected() && e.client.getRemote().Trame.sendError(a.join(" "))
         } catch (i) {
             u(i)
         } finally {
             u(...a)
         }
     }, window.addEventListener("error", a => console.error(`${a.type}: ${a.message}`)), t.use(ca), t.provide("trame", e);
-    const o = await Ao(e.state.state);
+    const o = await vo(e.state.state);
     for (let a = 0; a < o.length; a++) t.use(...o[a]), console.info(`Vue.use(${o[a]})`);
     t.mount("#app")
 }
 Da();
```

### Comparing `trame-client-2.7.6/trame_client/module/vue3-www/index.html` & `trame-client-2.7.7/trame_client/module/vue3-www/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         100% {
           -webkit-transform: rotate(360deg); /* Chrome, Opera 15+, Safari 3.1+ */
           -ms-transform: rotate(360deg); /* IE 9 */
           transform: rotate(360deg); /* Firefox 16+, IE 10+, Opera */
         }
       }
     </style>
-    <script type="module" crossorigin src="./assets/index-e4900adb.js"></script>
+    <script type="module" crossorigin src="./assets/index-ccad3410.js"></script>
   </head>
   <body>
     <noscript>
       <strong>We're sorry but trame built by Kitware doesn't work properly without JavaScript enabled. Please enable it to continue.</strong>
     </noscript>
     <div id="app">
       <div style="position:absolute;top:0;left:0;width:100%;height:100%;z-index:1000;">
```

### Comparing `trame-client-2.7.6/trame_client/module/vue3-www/logo.png` & `trame-client-2.7.7/trame_client/module/vue3-www/logo.png`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.6/trame_client/module/vue3-www/vue.global.js` & `trame-client-2.7.7/trame_client/module/vue3-www/vue.global.js`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.6/trame_client/resources/attributes.json` & `trame-client-2.7.7/trame_client/resources/attributes.json`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.6/trame_client/resources/vue.json` & `trame-client-2.7.7/trame_client/resources/vue.json`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.6/trame_client/ui/core.py` & `trame-client-2.7.7/trame_client/ui/core.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.6/trame_client/ui/html.py` & `trame-client-2.7.7/trame_client/ui/html.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.6/trame_client/utils/version.py` & `trame-client-2.7.7/trame_client/utils/version.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.6/trame_client/widgets/core.py` & `trame-client-2.7.7/trame_client/widgets/core.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.6/trame_client/widgets/generator.py` & `trame-client-2.7.7/trame_client/widgets/generator.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.6/trame_client/widgets/html.py` & `trame-client-2.7.7/trame_client/widgets/html.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.7.6/trame_client.egg-info/PKG-INFO` & `trame-client-2.7.7/trame_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-client
-Version: 2.7.6
+Version: 2.7.7
 Summary: Internal client of trame
 Author: Kitware Inc.
 License: MIT
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-client-2.7.6/trame_client.egg-info/SOURCES.txt` & `trame-client-2.7.7/trame_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 trame_client/module/__init__.py
 trame_client/module/vue2.py
 trame_client/module/vue3.py
 trame_client/module/vue2-www/index.html
 trame_client/module/vue2-www/logo.png
 trame_client/module/vue2-www/vue.global.js
 trame_client/module/vue2-www/css/app.0b077e70.css
-trame_client/module/vue2-www/js/app.4ae908a0.js
-trame_client/module/vue2-www/js/chunk-vendors.ec946a94.js
+trame_client/module/vue2-www/js/app.93852572.js
+trame_client/module/vue2-www/js/chunk-vendors.b42af71c.js
 trame_client/module/vue3-www/index.html
 trame_client/module/vue3-www/logo.png
 trame_client/module/vue3-www/vue.global.js
-trame_client/module/vue3-www/assets/index-e4900adb.js
+trame_client/module/vue3-www/assets/index-ccad3410.js
 trame_client/resources/attributes.json
 trame_client/resources/events.json
 trame_client/resources/vue.json
 trame_client/ui/__init__.py
 trame_client/ui/core.py
 trame_client/ui/html.py
 trame_client/utils/__init__.py
```

