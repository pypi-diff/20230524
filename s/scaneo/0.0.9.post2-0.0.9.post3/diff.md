# Comparing `tmp/scaneo-0.0.9.post2.tar.gz` & `tmp/scaneo-0.0.9.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaneo-0.0.9.post2.tar", max compression
+gzip compressed data, was "scaneo-0.0.9.post3.tar", max compression
```

## Comparing `scaneo-0.0.9.post2.tar` & `scaneo-0.0.9.post3.tar`

### file list

```diff
@@ -1,70 +1,76 @@
--rw-r--r--   0        0        0     6199 2023-05-24 09:26:01.616553 scaneo-0.0.9.post2/README.md
--rw-r--r--   0        0        0      347 2023-05-24 12:36:09.517226 scaneo-0.0.9.post2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 09:29:06.132298 scaneo-0.0.9.post2/scaneo/__init__.py
--rw-r--r--   0        0        0      990 2023-05-24 12:36:00.709196 scaneo-0.0.9.post2/scaneo/api.py
--rw-r--r--   0        0        0      584 2023-05-24 12:31:10.176185 scaneo-0.0.9.post2/scaneo/main.py
--rw-r--r--   0        0        0     7056 2023-05-24 11:13:45.790816 scaneo-0.0.9.post2/scaneo/ui/_app/immutable/chunks/index.6dba6488.js
--rw-r--r--   0        0        0     2836 2023-05-24 11:13:45.790816 scaneo-0.0.9.post2/scaneo/ui/_app/immutable/chunks/singletons.1df1af67.js
--rw-r--r--   0        0        0      238 2023-05-24 11:13:45.790816 scaneo-0.0.9.post2/scaneo/ui/_app/immutable/chunks/stores.a2dd7dd6.js
--rw-r--r--   0        0        0     5722 2023-05-24 11:13:45.790816 scaneo-0.0.9.post2/scaneo/ui/_app/immutable/entry/app.77ddf75f.js
--rw-r--r--   0        0        0    23876 2023-05-24 11:13:45.790816 scaneo-0.0.9.post2/scaneo/ui/_app/immutable/entry/start.8814d3e0.js
--rw-r--r--   0        0        0      719 2023-05-24 11:13:45.790816 scaneo-0.0.9.post2/scaneo/ui/_app/immutable/nodes/0.663a3db5.js
--rw-r--r--   0        0        0      800 2023-05-24 11:13:45.790816 scaneo-0.0.9.post2/scaneo/ui/_app/immutable/nodes/1.86013cb7.js
--rw-r--r--   0        0        0     1328 2023-05-24 11:13:45.790816 scaneo-0.0.9.post2/scaneo/ui/_app/immutable/nodes/2.35154476.js
--rw-r--r--   0        0        0      372 2023-05-24 11:13:45.790816 scaneo-0.0.9.post2/scaneo/ui/_app/immutable/nodes/3.cb33ee2b.js
--rw-r--r--   0        0        0       27 2023-05-24 11:13:45.790816 scaneo-0.0.9.post2/scaneo/ui/_app/version.json
--rw-r--r--   0        0        0     7056 2023-05-24 12:36:09.517226 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/index.6dba6488.js
--rw-r--r--   0        0        0     2836 2023-05-24 12:14:25.943839 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/singletons.1df1af67.js
--rw-r--r--   0        0        0     2838 2023-05-24 12:34:55.796976 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/singletons.36580b7a.js
--rw-r--r--   0        0        0     2838 2023-05-24 12:31:51.180333 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/singletons.4ffcfa45.js
--rw-r--r--   0        0        0     2838 2023-05-24 12:36:09.517226 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/singletons.7210d6da.js
--rw-r--r--   0        0        0     2838 2023-05-24 12:14:59.847912 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/singletons.76776748.js
--rw-r--r--   0        0        0     2836 2023-05-24 12:32:47.980534 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/singletons.8ca8a18c.js
--rw-r--r--   0        0        0     2838 2023-05-24 12:17:37.064518 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/singletons.a1fc90ce.js
--rw-r--r--   0        0        0      238 2023-05-24 12:32:47.980534 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/stores.24647ac6.js
--rw-r--r--   0        0        0      238 2023-05-24 12:14:59.847912 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/stores.6bb331f9.js
--rw-r--r--   0        0        0      238 2023-05-24 12:14:25.943839 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/stores.a2dd7dd6.js
--rw-r--r--   0        0        0      238 2023-05-24 12:34:55.796976 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/stores.c0d9e12d.js
--rw-r--r--   0        0        0      238 2023-05-24 12:31:51.180333 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/stores.dd0e8ee4.js
--rw-r--r--   0        0        0      238 2023-05-24 12:36:09.517226 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/stores.ebd8fd52.js
--rw-r--r--   0        0        0      238 2023-05-24 12:17:37.064518 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/stores.ebfb6cb3.js
--rw-r--r--   0        0        0     5722 2023-05-24 12:34:55.796976 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/app.11edd54e.js
--rw-r--r--   0        0        0     5722 2023-05-24 12:31:51.180333 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/app.19a98a41.js
--rw-r--r--   0        0        0     5722 2023-05-24 12:32:47.980534 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/app.6cae644b.js
--rw-r--r--   0        0        0     5722 2023-05-24 12:14:25.943839 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/app.77ddf75f.js
--rw-r--r--   0        0        0     5722 2023-05-24 12:14:59.847912 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/app.9fea0e15.js
--rw-r--r--   0        0        0     5722 2023-05-24 12:17:37.064518 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/app.f45b1117.js
--rw-r--r--   0        0        0     5722 2023-05-24 12:36:09.517226 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/app.f61a80e5.js
--rw-r--r--   0        0        0    23876 2023-05-24 12:32:47.980534 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/start.215451c5.js
--rw-r--r--   0        0        0    23876 2023-05-24 12:34:55.796976 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/start.2fa5423d.js
--rw-r--r--   0        0        0    23876 2023-05-24 12:17:37.064518 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/start.31eba02c.js
--rw-r--r--   0        0        0    23876 2023-05-24 12:14:25.951839 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/start.8814d3e0.js
--rw-r--r--   0        0        0    23876 2023-05-24 12:36:09.517226 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/start.9cce7b47.js
--rw-r--r--   0        0        0    23876 2023-05-24 12:14:59.847912 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/start.a5a82fbc.js
--rw-r--r--   0        0        0    23876 2023-05-24 12:31:51.180333 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/start.f2579792.js
--rw-r--r--   0        0        0      719 2023-05-24 12:14:25.951839 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/0.663a3db5.js
--rw-r--r--   0        0        0      676 2023-05-24 12:36:09.517226 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/0.6e67e459.js
--rw-r--r--   0        0        0      800 2023-05-24 12:34:55.796976 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/1.519d840f.js
--rw-r--r--   0        0        0      800 2023-05-24 12:17:37.064518 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/1.5cf77ad0.js
--rw-r--r--   0        0        0      800 2023-05-24 12:36:09.517226 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/1.7a4b92ca.js
--rw-r--r--   0        0        0      800 2023-05-24 12:14:25.951839 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/1.86013cb7.js
--rw-r--r--   0        0        0      800 2023-05-24 12:14:59.847912 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/1.917eb664.js
--rw-r--r--   0        0        0      800 2023-05-24 12:31:51.180333 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/1.a0346c75.js
--rw-r--r--   0        0        0      800 2023-05-24 12:32:47.980534 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/1.f89a0772.js
--rw-r--r--   0        0        0     1269 2023-05-24 12:31:51.180333 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/2.0f870bcf.js
--rw-r--r--   0        0        0     1328 2023-05-24 12:14:25.951839 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/2.35154476.js
--rw-r--r--   0        0        0     1269 2023-05-24 12:36:09.517226 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/2.b937115c.js
--rw-r--r--   0        0        0     1269 2023-05-24 12:17:37.064518 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/2.cef09f18.js
--rw-r--r--   0        0        0     1269 2023-05-24 12:34:55.800976 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/2.d76a8d27.js
--rw-r--r--   0        0        0     1269 2023-05-24 12:32:47.980534 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/2.da635a22.js
--rw-r--r--   0        0        0     1269 2023-05-24 12:14:59.847912 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/2.eb1e05c8.js
--rw-r--r--   0        0        0      372 2023-05-24 12:36:09.517226 scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/3.cb33ee2b.js
--rw-r--r--   0        0        0       27 2023-05-24 12:36:09.517226 scaneo-0.0.9.post2/scaneo/ui/build/_app/version.json
--rw-r--r--   0        0        0     1571 2023-05-24 12:36:09.517226 scaneo-0.0.9.post2/scaneo/ui/build/favicon.png
--rw-r--r--   0        0        0     1575 2023-05-24 12:36:09.517226 scaneo-0.0.9.post2/scaneo/ui/build/index.html
--rw-r--r--   0        0        0     1364 2023-05-24 12:36:09.517226 scaneo-0.0.9.post2/scaneo/ui/build/kk.html
--rw-r--r--   0        0        0     1571 2023-05-24 11:13:45.790816 scaneo-0.0.9.post2/scaneo/ui/favicon.png
--rw-r--r--   0        0        0     1571 2023-05-24 12:34:37.332913 scaneo-0.0.9.post2/scaneo/ui/index.html
--rw-r--r--   0        0        0     1363 2023-05-24 11:13:45.790816 scaneo-0.0.9.post2/scaneo/ui/kk.html
--rw-r--r--   0        0        0     7260 1970-01-01 00:00:00.000000 scaneo-0.0.9.post2/setup.py
--rw-r--r--   0        0        0     6585 1970-01-01 00:00:00.000000 scaneo-0.0.9.post2/PKG-INFO
+-rw-r--r--   0        0        0     6199 2023-05-24 09:26:01.616553 scaneo-0.0.9.post3/README.md
+-rw-r--r--   0        0        0      347 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 09:29:06.132298 scaneo-0.0.9.post3/scaneo/__init__.py
+-rw-r--r--   0        0        0     1037 2023-05-24 12:36:44.461343 scaneo-0.0.9.post3/scaneo/api.py
+-rw-r--r--   0        0        0      584 2023-05-24 12:31:10.176185 scaneo-0.0.9.post3/scaneo/main.py
+-rw-r--r--   0        0        0     7056 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/_app/immutable/chunks/index.6dba6488.js
+-rw-r--r--   0        0        0     2836 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/_app/immutable/chunks/singletons.1df1af67.js
+-rw-r--r--   0        0        0      238 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/_app/immutable/chunks/stores.a2dd7dd6.js
+-rw-r--r--   0        0        0     5722 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/_app/immutable/entry/app.77ddf75f.js
+-rw-r--r--   0        0        0    23876 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/_app/immutable/entry/start.8814d3e0.js
+-rw-r--r--   0        0        0      719 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/_app/immutable/nodes/0.663a3db5.js
+-rw-r--r--   0        0        0      800 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/_app/immutable/nodes/1.86013cb7.js
+-rw-r--r--   0        0        0     1328 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/_app/immutable/nodes/2.35154476.js
+-rw-r--r--   0        0        0      372 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/_app/immutable/nodes/3.cb33ee2b.js
+-rw-r--r--   0        0        0       27 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/_app/version.json
+-rw-r--r--   0        0        0     7056 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/index.6dba6488.js
+-rw-r--r--   0        0        0     2836 2023-05-24 12:14:25.943839 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.1df1af67.js
+-rw-r--r--   0        0        0     2836 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.2ddc59bf.js
+-rw-r--r--   0        0        0     2838 2023-05-24 12:34:55.796976 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.36580b7a.js
+-rw-r--r--   0        0        0     2838 2023-05-24 12:31:51.180333 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.4ffcfa45.js
+-rw-r--r--   0        0        0     2838 2023-05-24 12:36:09.517226 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.7210d6da.js
+-rw-r--r--   0        0        0     2838 2023-05-24 12:14:59.847912 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.76776748.js
+-rw-r--r--   0        0        0     2836 2023-05-24 12:32:47.980534 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.8ca8a18c.js
+-rw-r--r--   0        0        0     2838 2023-05-24 12:17:37.064518 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.a1fc90ce.js
+-rw-r--r--   0        0        0      238 2023-05-24 12:32:47.980534 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/stores.24647ac6.js
+-rw-r--r--   0        0        0      238 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/stores.6a2effc3.js
+-rw-r--r--   0        0        0      238 2023-05-24 12:14:59.847912 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/stores.6bb331f9.js
+-rw-r--r--   0        0        0      238 2023-05-24 12:14:25.943839 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/stores.a2dd7dd6.js
+-rw-r--r--   0        0        0      238 2023-05-24 12:34:55.796976 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/stores.c0d9e12d.js
+-rw-r--r--   0        0        0      238 2023-05-24 12:31:51.180333 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/stores.dd0e8ee4.js
+-rw-r--r--   0        0        0      238 2023-05-24 12:36:09.517226 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/stores.ebd8fd52.js
+-rw-r--r--   0        0        0      238 2023-05-24 12:17:37.064518 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/stores.ebfb6cb3.js
+-rw-r--r--   0        0        0     5722 2023-05-24 12:34:55.796976 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.11edd54e.js
+-rw-r--r--   0        0        0     5722 2023-05-24 12:31:51.180333 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.19a98a41.js
+-rw-r--r--   0        0        0     5722 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.450412c1.js
+-rw-r--r--   0        0        0     5722 2023-05-24 12:32:47.980534 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.6cae644b.js
+-rw-r--r--   0        0        0     5722 2023-05-24 12:14:25.943839 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.77ddf75f.js
+-rw-r--r--   0        0        0     5722 2023-05-24 12:14:59.847912 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.9fea0e15.js
+-rw-r--r--   0        0        0     5722 2023-05-24 12:17:37.064518 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.f45b1117.js
+-rw-r--r--   0        0        0     5722 2023-05-24 12:36:09.517226 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.f61a80e5.js
+-rw-r--r--   0        0        0    23876 2023-05-24 12:32:47.980534 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.215451c5.js
+-rw-r--r--   0        0        0    23876 2023-05-24 12:34:55.796976 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.2fa5423d.js
+-rw-r--r--   0        0        0    23876 2023-05-24 12:17:37.064518 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.31eba02c.js
+-rw-r--r--   0        0        0    23876 2023-05-24 12:14:25.951839 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.8814d3e0.js
+-rw-r--r--   0        0        0    23876 2023-05-24 12:36:09.517226 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.9cce7b47.js
+-rw-r--r--   0        0        0    23876 2023-05-24 12:14:59.847912 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.a5a82fbc.js
+-rw-r--r--   0        0        0    23876 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.aca2ebd3.js
+-rw-r--r--   0        0        0    23876 2023-05-24 12:31:51.180333 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.f2579792.js
+-rw-r--r--   0        0        0      719 2023-05-24 12:14:25.951839 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/0.663a3db5.js
+-rw-r--r--   0        0        0      676 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/0.6e67e459.js
+-rw-r--r--   0        0        0      800 2023-05-24 12:34:55.796976 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.519d840f.js
+-rw-r--r--   0        0        0      800 2023-05-24 12:17:37.064518 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.5cf77ad0.js
+-rw-r--r--   0        0        0      800 2023-05-24 12:36:09.517226 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.7a4b92ca.js
+-rw-r--r--   0        0        0      800 2023-05-24 12:14:25.951839 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.86013cb7.js
+-rw-r--r--   0        0        0      800 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.8a8831ee.js
+-rw-r--r--   0        0        0      800 2023-05-24 12:14:59.847912 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.917eb664.js
+-rw-r--r--   0        0        0      800 2023-05-24 12:31:51.180333 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.a0346c75.js
+-rw-r--r--   0        0        0      800 2023-05-24 12:32:47.980534 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.f89a0772.js
+-rw-r--r--   0        0        0     1269 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.0e7d4a8f.js
+-rw-r--r--   0        0        0     1269 2023-05-24 12:31:51.180333 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.0f870bcf.js
+-rw-r--r--   0        0        0     1328 2023-05-24 12:14:25.951839 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.35154476.js
+-rw-r--r--   0        0        0     1269 2023-05-24 12:36:09.517226 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.b937115c.js
+-rw-r--r--   0        0        0     1269 2023-05-24 12:17:37.064518 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.cef09f18.js
+-rw-r--r--   0        0        0     1269 2023-05-24 12:34:55.800976 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.d76a8d27.js
+-rw-r--r--   0        0        0     1269 2023-05-24 12:32:47.980534 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.da635a22.js
+-rw-r--r--   0        0        0     1269 2023-05-24 12:14:59.847912 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.eb1e05c8.js
+-rw-r--r--   0        0        0      372 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/3.cb33ee2b.js
+-rw-r--r--   0        0        0       27 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/_app/version.json
+-rw-r--r--   0        0        0     1571 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/favicon.png
+-rw-r--r--   0        0        0     1574 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/index.html
+-rw-r--r--   0        0        0     1363 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/kk.html
+-rw-r--r--   0        0        0     1571 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/favicon.png
+-rw-r--r--   0        0        0     1571 2023-05-24 12:34:37.332913 scaneo-0.0.9.post3/scaneo/ui/index.html
+-rw-r--r--   0        0        0     1363 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/kk.html
+-rw-r--r--   0        0        0     7260 1970-01-01 00:00:00.000000 scaneo-0.0.9.post3/setup.py
+-rw-r--r--   0        0        0     6585 1970-01-01 00:00:00.000000 scaneo-0.0.9.post3/PKG-INFO
```

### Comparing `scaneo-0.0.9.post2/README.md` & `scaneo-0.0.9.post3/README.md`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/api.py` & `scaneo-0.0.9.post3/scaneo/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,8 +30,10 @@
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--port", type=int, default=8000)
     parser.add_argument("--host", type=str, default="localhost")
     parser.add_argument("--reload", action="store_true", default=False)
     args = parser.parse_args()
     os.chdir(current_dir)
+    print(os.getcwd())
+    print(os.listdir())
     uvicorn.run("api:app", host=args.host, port=args.port, reload=args.reload)
```

### Comparing `scaneo-0.0.9.post2/scaneo/main.py` & `scaneo-0.0.9.post3/scaneo/main.py`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/_app/immutable/chunks/index.6dba6488.js` & `scaneo-0.0.9.post3/scaneo/ui/_app/immutable/chunks/index.6dba6488.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/_app/immutable/chunks/singletons.1df1af67.js` & `scaneo-0.0.9.post3/scaneo/ui/_app/immutable/chunks/singletons.1df1af67.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/_app/immutable/entry/app.77ddf75f.js` & `scaneo-0.0.9.post3/scaneo/ui/_app/immutable/entry/app.77ddf75f.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/_app/immutable/entry/start.8814d3e0.js` & `scaneo-0.0.9.post3/scaneo/ui/_app/immutable/entry/start.8814d3e0.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/_app/immutable/nodes/0.663a3db5.js` & `scaneo-0.0.9.post3/scaneo/ui/_app/immutable/nodes/0.663a3db5.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/_app/immutable/nodes/1.86013cb7.js` & `scaneo-0.0.9.post3/scaneo/ui/_app/immutable/nodes/1.86013cb7.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/_app/immutable/nodes/2.35154476.js` & `scaneo-0.0.9.post3/scaneo/ui/_app/immutable/nodes/2.35154476.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/index.6dba6488.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/index.6dba6488.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/singletons.1df1af67.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.1df1af67.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/singletons.36580b7a.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.36580b7a.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/singletons.4ffcfa45.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.4ffcfa45.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/singletons.7210d6da.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.7210d6da.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/singletons.76776748.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.76776748.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/singletons.8ca8a18c.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.8ca8a18c.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/chunks/singletons.a1fc90ce.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.a1fc90ce.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/app.11edd54e.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.11edd54e.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/app.19a98a41.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.19a98a41.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/app.6cae644b.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.6cae644b.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/app.77ddf75f.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.77ddf75f.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/app.9fea0e15.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.9fea0e15.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/app.f45b1117.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.f45b1117.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/app.f61a80e5.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.f61a80e5.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/start.215451c5.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.215451c5.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/start.2fa5423d.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.2fa5423d.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/start.31eba02c.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.31eba02c.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/start.8814d3e0.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.8814d3e0.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/start.9cce7b47.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.9cce7b47.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/start.a5a82fbc.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.a5a82fbc.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/entry/start.f2579792.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.f2579792.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/0.663a3db5.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/0.663a3db5.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/0.6e67e459.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/0.6e67e459.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/1.519d840f.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.519d840f.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/1.5cf77ad0.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.5cf77ad0.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/1.7a4b92ca.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.7a4b92ca.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/1.86013cb7.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.86013cb7.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/1.917eb664.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.917eb664.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/1.a0346c75.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.a0346c75.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/1.f89a0772.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.f89a0772.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/2.0f870bcf.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.0f870bcf.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/2.35154476.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.35154476.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/2.b937115c.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.b937115c.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/2.cef09f18.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.cef09f18.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/2.d76a8d27.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.d76a8d27.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/2.da635a22.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.da635a22.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/_app/immutable/nodes/2.eb1e05c8.js` & `scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.eb1e05c8.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/favicon.png` & `scaneo-0.0.9.post3/scaneo/ui/build/favicon.png`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/index.html` & `scaneo-0.0.9.post3/scaneo/ui/build/kk.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 <!DOCTYPE html>
 <html lang="en">
 	<head>
 		<meta charset="utf-8" />
 		<link rel="icon" href="./favicon.png" />
 		<meta name="viewport" content="width=device-width" />
 		<meta http-equiv="content-security-policy" content="">
-		<link rel="modulepreload" href="./_app/immutable/entry/start.9cce7b47.js">
+		<link rel="modulepreload" href="./_app/immutable/entry/start.aca2ebd3.js">
 		<link rel="modulepreload" href="./_app/immutable/chunks/index.6dba6488.js">
-		<link rel="modulepreload" href="./_app/immutable/chunks/singletons.7210d6da.js">
-		<link rel="modulepreload" href="./_app/immutable/entry/app.f61a80e5.js">
+		<link rel="modulepreload" href="./_app/immutable/chunks/singletons.2ddc59bf.js">
+		<link rel="modulepreload" href="./_app/immutable/entry/app.450412c1.js">
 		<link rel="modulepreload" href="./_app/immutable/nodes/0.6e67e459.js">
-		<link rel="modulepreload" href="./_app/immutable/nodes/2.b937115c.js">
-		<link rel="modulepreload" href="./_app/immutable/chunks/stores.ebd8fd52.js">
+		<link rel="modulepreload" href="./_app/immutable/nodes/3.cb33ee2b.js">
 	</head>
 	<body data-sveltekit-preload-data="hover">
 		<div style="display: contents">
 
 
-<h1>Welcome to SvelteKit</h1>
-<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
-<a href="/kk">hola</a>
+<p>hola</p>
 
 
 			
 			<script>
 				{
-					__sveltekit_17885f5 = {
+					__sveltekit_rgg8pi = {
 						base: new URL(".", location).pathname.slice(0, -1),
 						env: {"PUBLIC_API_URL":""}
 					};
 
 					const element = document.currentScript.parentElement;
 
 					const data = [null,null];
 
 					Promise.all([
-						import("./_app/immutable/entry/start.9cce7b47.js"),
-						import("./_app/immutable/entry/app.f61a80e5.js")
+						import("./_app/immutable/entry/start.aca2ebd3.js"),
+						import("./_app/immutable/entry/app.450412c1.js")
 					]).then(([kit, app]) => {
 						kit.start(app, element, {
-							node_ids: [0, 2],
+							node_ids: [0, 3],
 							data,
 							form: null,
 							error: null
 						});
 					});
 				}
 			</script>
```

#### html2text {}

```diff
@@ -3,11 +3,8 @@
 
 
 
 
 
 
 
-
-****** Welcome to SvelteKit ******
-Visit kit.svelte.dev to read the documentation
 hola
```

### Comparing `scaneo-0.0.9.post2/scaneo/ui/build/kk.html` & `scaneo-0.0.9.post3/scaneo/ui/build/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 <!DOCTYPE html>
 <html lang="en">
 	<head>
 		<meta charset="utf-8" />
 		<link rel="icon" href="./favicon.png" />
 		<meta name="viewport" content="width=device-width" />
 		<meta http-equiv="content-security-policy" content="">
-		<link rel="modulepreload" href="./_app/immutable/entry/start.9cce7b47.js">
+		<link rel="modulepreload" href="./_app/immutable/entry/start.aca2ebd3.js">
 		<link rel="modulepreload" href="./_app/immutable/chunks/index.6dba6488.js">
-		<link rel="modulepreload" href="./_app/immutable/chunks/singletons.7210d6da.js">
-		<link rel="modulepreload" href="./_app/immutable/entry/app.f61a80e5.js">
+		<link rel="modulepreload" href="./_app/immutable/chunks/singletons.2ddc59bf.js">
+		<link rel="modulepreload" href="./_app/immutable/entry/app.450412c1.js">
 		<link rel="modulepreload" href="./_app/immutable/nodes/0.6e67e459.js">
-		<link rel="modulepreload" href="./_app/immutable/nodes/3.cb33ee2b.js">
+		<link rel="modulepreload" href="./_app/immutable/nodes/2.0e7d4a8f.js">
+		<link rel="modulepreload" href="./_app/immutable/chunks/stores.6a2effc3.js">
 	</head>
 	<body data-sveltekit-preload-data="hover">
 		<div style="display: contents">
 
 
-<p>hola</p>
+<h1>Welcome to SvelteKit</h1>
+<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
+<a href="/kk">hola</a>
 
 
 			
 			<script>
 				{
-					__sveltekit_17885f5 = {
+					__sveltekit_rgg8pi = {
 						base: new URL(".", location).pathname.slice(0, -1),
 						env: {"PUBLIC_API_URL":""}
 					};
 
 					const element = document.currentScript.parentElement;
 
 					const data = [null,null];
 
 					Promise.all([
-						import("./_app/immutable/entry/start.9cce7b47.js"),
-						import("./_app/immutable/entry/app.f61a80e5.js")
+						import("./_app/immutable/entry/start.aca2ebd3.js"),
+						import("./_app/immutable/entry/app.450412c1.js")
 					]).then(([kit, app]) => {
 						kit.start(app, element, {
-							node_ids: [0, 3],
+							node_ids: [0, 2],
 							data,
 							form: null,
 							error: null
 						});
 					});
 				}
 			</script>
```

#### html2text {}

```diff
@@ -3,8 +3,11 @@
 
 
 
 
 
 
 
+
+****** Welcome to SvelteKit ******
+Visit kit.svelte.dev to read the documentation
 hola
```

### Comparing `scaneo-0.0.9.post2/scaneo/ui/favicon.png` & `scaneo-0.0.9.post3/scaneo/ui/favicon.png`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/index.html` & `scaneo-0.0.9.post3/scaneo/ui/index.html`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/scaneo/ui/kk.html` & `scaneo-0.0.9.post3/scaneo/ui/kk.html`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post2/setup.py` & `scaneo-0.0.9.post3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             'ui/build/_app/immutable/nodes/*']}
 
 entry_points = \
 {'console_scripts': ['scaneo = scaneo.main:app']}
 
 setup_kwargs = {
     'name': 'scaneo',
-    'version': '0.0.9.post2',
+    'version': '0.0.9.post3',
     'description': '',
     'long_description': "# scan-new\n\n\n\n## Getting started\n\nTo make it easy for you to get started with GitLab, here's a list of recommended next steps.\n\nAlready a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!\n\n## Add your files\n\n- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files\n- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:\n\n```\ncd existing_repo\ngit remote add origin https://gitlab.com/earthpulse/scan-new.git\ngit branch -M main\ngit push -uf origin main\n```\n\n## Integrate with your tools\n\n- [ ] [Set up project integrations](https://gitlab.com/earthpulse/scan-new/-/settings/integrations)\n\n## Collaborate with your team\n\n- [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)\n- [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)\n- [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)\n- [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)\n- [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)\n\n## Test and Deploy\n\nUse the built-in continuous integration in GitLab.\n\n- [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)\n- [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)\n- [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)\n- [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)\n- [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)\n\n***\n\n# Editing this README\n\nWhen you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.\n\n## Suggestions for a good README\nEvery project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.\n\n## Name\nChoose a self-explaining name for your project.\n\n## Description\nLet people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.\n\n## Badges\nOn some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.\n\n## Visuals\nDepending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.\n\n## Installation\nWithin a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.\n\n## Usage\nUse examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.\n\n## Support\nTell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.\n\n## Roadmap\nIf you have ideas for releases in the future, it is a good idea to list them in the README.\n\n## Contributing\nState if you are open to contributions and what your requirements are for accepting them.\n\nFor people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.\n\nYou can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.\n\n## Authors and acknowledgment\nShow your appreciation to those who have contributed to the project.\n\n## License\nFor open source projects, say how it is licensed.\n\n## Project status\nIf you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.\n",
     'author': 'Juan Sensio',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `scaneo-0.0.9.post2/PKG-INFO` & `scaneo-0.0.9.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scaneo
-Version: 0.0.9.post2
+Version: 0.0.9.post3
 Summary: 
 Author: Juan Sensio
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

