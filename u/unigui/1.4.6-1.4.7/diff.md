# Comparing `tmp/unigui-1.4.6.tar.gz` & `tmp/unigui-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.4.6.tar", last modified: Fri May 19 07:55:40 2023, max compression
+gzip compressed data, was "dist/unigui-1.4.7.tar", last modified: Wed May 24 11:14:01 2023, max compression
```

## Comparing `unigui-1.4.6.tar` & `unigui-1.4.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-19 07:55:40.000000 unigui-1.4.6/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-19 07:55:40.000000 unigui-1.4.6/unigui/
--rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.4.6/unigui/manager.py
--rw-rw-r--   0 george    (1000) george    (1000)     7900 2023-05-16 12:54:09.000000 unigui-1.4.6/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.4.6/unigui/userset.py
--rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:39.000000 unigui-1.4.6/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:49.000000 unigui-1.4.6/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.4.6/unigui/utils.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-19 07:55:40.000000 unigui-1.4.6/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-19 07:55:40.000000 unigui-1.4.6/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/css/259.f5c7cbc7.css
--rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/css/vendor.49a52e8f.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-19 07:55:40.000000 unigui-1.4.6/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-19 07:55:40.000000 unigui-1.4.6/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-19 07:55:40.000000 unigui-1.4.6/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)    42644 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/js/259.1c52f635.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/js/app.0d4bddce.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/js/vendor.3e8714c2.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-05-19 07:49:22.000000 unigui-1.4.6/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.4.6/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      585 2023-05-19 07:55:15.000000 unigui-1.4.6/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    19455 2023-05-19 07:55:40.000000 unigui-1.4.6/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-05-19 07:55:40.000000 unigui-1.4.6/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    19165 2023-05-17 15:17:52.000000 unigui-1.4.6/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.4.6/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-19 07:55:40.000000 unigui-1.4.6/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       30 2023-05-19 07:55:40.000000 unigui-1.4.6/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-05-19 07:55:40.000000 unigui-1.4.6/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    19455 2023-05-19 07:55:40.000000 unigui-1.4.6/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.4.6/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1223 2023-05-19 07:55:40.000000 unigui-1.4.6/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-05-19 07:55:40.000000 unigui-1.4.6/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-24 11:14:01.000000 unigui-1.4.7/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui/
+-rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.4.7/unigui/manager.py
+-rw-rw-r--   0 george    (1000) george    (1000)     7900 2023-05-16 12:54:09.000000 unigui-1.4.7/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.4.7/unigui/userset.py
+-rw-r--r--   0 george    (1000) george    (1000)     3654 2022-09-03 18:32:39.000000 unigui-1.4.7/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:49.000000 unigui-1.4.7/unigui/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.4.7/unigui/utils.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/css/889.c9159919.css
+-rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/css/vendor.49a52e8f.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/js/app.92f553f5.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)    42555 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/js/889.504369e0.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/js/vendor.3e8714c2.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-05-24 10:59:31.000000 unigui-1.4.7/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.4.7/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      585 2023-05-24 11:13:41.000000 unigui-1.4.7/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    19452 2023-05-24 11:14:01.000000 unigui-1.4.7/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-05-24 11:14:01.000000 unigui-1.4.7/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    19162 2023-05-24 11:05:25.000000 unigui-1.4.7/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.4.7/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       30 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    19452 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.4.7/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1223 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-05-24 11:14:01.000000 unigui-1.4.7/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.4.6/unigui/manager.py` & `unigui-1.4.7/unigui/manager.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/guielements.py` & `unigui-1.4.7/unigui/guielements.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/server.py` & `unigui-1.4.7/unigui/server.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/utils.py` & `unigui-1.4.7/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/web/favicon.ico` & `unigui-1.4.7/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/web/css/259.f5c7cbc7.css` & `unigui-1.4.7/unigui/web/css/889.c9159919.css`

 * *Files 12% similar despite different names*

```diff
@@ -1 +1 @@
-thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-6d149d62]{display:flex;justify-content:center}.custom-caption[data-v-6d149d62]{padding:5px!important}.web-camera-container[data-v-6d149d62]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-6d149d62]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-6d149d62]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-6d149d62]{opacity:1}.web-camera-container .camera-shoot[data-v-6d149d62]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-6d149d62]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-6d149d62]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-6d149d62]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-6d149d62]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-6d149d62]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-6d149d62]{animation:preload-6d149d62 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-6d149d62]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-6d149d62]:nth-child(3){animation-delay:.4s}@keyframes preload-6d149d62{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-6d149d62]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
+thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-0593ed42]{display:flex;justify-content:center}.custom-caption[data-v-0593ed42]{padding:5px!important}.web-camera-container[data-v-0593ed42]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-0593ed42]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-0593ed42]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-0593ed42]{opacity:1}.web-camera-container .camera-shoot[data-v-0593ed42]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-0593ed42]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-0593ed42]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-0593ed42]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-0593ed42]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-0593ed42]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-0593ed42]{animation:preload-0593ed42 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-0593ed42]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-0593ed42]:nth-child(3){animation-delay:.4s}@keyframes preload-0593ed42{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-0593ed42]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
```

### Comparing `unigui-1.4.6/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.4.7/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/web/icons/favicon-96x96.png` & `unigui-1.4.7/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/web/icons/favicon-16x16.png` & `unigui-1.4.7/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/web/icons/favicon-32x32.png` & `unigui-1.4.7/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/web/icons/favicon-128x128.png` & `unigui-1.4.7/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.4.7/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.4.7/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.4.7/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.4.7/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.4.7/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.4.7/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.4.7/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.4.7/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/web/js/259.1c52f635.js` & `unigui-1.4.7/unigui/web/js/889.504369e0.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [259], {
-        8259: (e, t, a) => {
+    [889], {
+        2889: (e, t, a) => {
             a.r(t), a.d(t, {
-                default: () => Jt
+                default: () => Gt
             });
             var l = a(3673),
                 s = a(2323);
             const i = (0, l._)("div", {
                 class: "q-pa-lg"
             }, null, -1);
 
@@ -110,17 +110,17 @@
                 f = `height: ${g}px; width: ${m}px`;
 
             function y(e) {
                 let t = e.minheight ? e.minheight : g,
                     a = e.minwidth ? e.minwidth : m;
                 return `height: ${t}px; width: ${a}px`
             }
-            const w = {},
-                b = {},
-                k = ["error", "progress", "warning", "info"];
+            let w = {},
+                b = {};
+            const k = ["error", "progress", "warning", "info"];
 
             function v(e) {
                 d = new WebSocket("ws://localhost:8000/ws"), d.onopen = () => e.statusConnect = !0, d.onmessage = t => {
                     p && console.log("socket message", t.data), e.processMessage(JSON.parse(t.data))
                 }, d.onerror = t => e.error(t), d.onclose = t => {
                     t.wasClean ? e.info("Connection closed and was clean.") : e.error("Connection suddenly closed!"), e.statusConnect = !1, p && console.info("close code : " + t.code + " reason: " + t.reason)
                 }, h = e
@@ -128,85 +128,81 @@
 
             function C(e) {
                 console.log("sended", e), d.send(JSON.stringify(e))
             }
             let q, S = 0;
 
             function j() {
-                for (let [e, t] of Object.entries(b)) t.expanding_height && (t.styleSize = null)
+                for (let [e, t] of Object.entries(b)) t.styleSize = null
             }
 
-            function A(e) {
-                for (var t in Object.keys(e)) delete e[t]
-            }
-
-            function z(e, t, a, l = "?") {
+            function A(e, t, a, l = "?") {
                 let s = ++S,
                     i = [e.pdata.name, e.data.name, l, t, s];
                 C(i), u[s] = a
             }
 
-            function Z() {
-                A(w), A(b)
+            function z() {
+                w = {}, b = {}
             }
 
-            function M(e, t) {
+            function Z(e, t) {
                 Object.assign(e.data, t), e.updated = t.value, e.value = t.value
             }
 
-            function $(e) {
+            function M(e) {
                 if (e.multi)
                     for (let [t, a] of e.update.entries())
                         if (a.length > 1) {
                             a.reverse();
                             let l = a.join("@"),
                                 s = b[l];
-                            M(s, e.data[t])
+                            Z(s, e.data[t])
                         } else {
                             let l = w[a[0]];
                             Object.assign(l.data, e.data[t])
                         }
                 else {
                     let t, a = e.update;
                     if (a.length > 1) {
                         a.reverse();
                         let e = a.join("@");
                         t = b[e]
                     } else t = w[a[0]];
-                    M(t, e.data), 1 == a.length && (0, c.delay)(W, 200, t)
+                    Z(t, e.data), 1 == a.length && (0, c.delay)(Q, 200, t)
                 }
             }
 
-            function D(e) {
+            function $(e) {
                 typeof e.answer == String ? h.showError() : u[e.id](e.answer), delete u[e.id]
             }
 
-            function V(e) {
+            function D(e) {
                 let t = [];
                 for (let l of e) l instanceof Array ? t.push(l) : t.push([l]);
                 let a = t.shift();
                 return t.reduce(((e, t) => e.flatMap((e => t.map((t => e instanceof Array ? [...e, t] : [e, t]))))), a)
             }
 
-            function O() {
+            function V() {
                 for (let [e, t] of Object.entries(b)) t.expanding && (t.styleSize = y(t.data));
                 (0, l.Y3)((() => {
                     requestAnimationFrame((() => {
                         requestAnimationFrame((() => {
-                            W()
+                            Q()
                         }))
                     }))
                 }))
             }
-            let Q = _.debounce(O, 200);
+            let O = _.debounce(V, 200);
 
-            function W(e) {
+            function Q(e) {
                 Array.isArray(e) && (e = null), q && (q.disconnect(), q = null), p && console.log("------------------recalc design");
-                const t = H(e),
-                    a = E(e);
+                const t = W(e),
+                    a = H(e);
                 for (let [l, s] of Object.entries(t)) {
                     let e = b[l];
                     const [t, i] = a[l];
                     let o, n = e.geom().el,
                         d = e.pdata ? e.pdata.name : e.name,
                         r = w[d];
                     for (let a of r.data.childs)
@@ -224,27 +220,27 @@
                     let c = r.data.width ? r.data.width - n.clientWidth - t : r.$el.getBoundingClientRect().right - (o ? o.geom().right : e.geom().right);
                     c /= i;
                     let h = l.startsWith("_scroll@") ? e.geom().inner.clientHeight : n.clientHeight;
                     e.styleSize = `height: ${h+s}px; width: ${n.clientWidth+c+t}px;`
                 }
             }
 
-            function H(e) {
+            function W(e) {
                 const t = h.screen.blocks;
                 let a = window.innerHeight;
                 a -= 2;
                 let l = {},
                     s = new Map,
                     i = {};
                 for (let [d, r] of Object.entries(w)) i[r.name] = r.$el.getBoundingClientRect().height;
                 let o = [];
                 for (let d of t) {
                     const e = [];
                     let t = d instanceof Array,
-                        n = t ? V(d) : [
+                        n = t ? D(d) : [
                             [d]
                         ];
                     for (let a of n) {
                         let e = 0;
                         for (let t of a) e += i[t.name] + 8;
                         o.push([e, a])
                     }
@@ -290,15 +286,15 @@
                 }
                 let n = Array.from(s.entries());
                 n.sort(((e, t) => e[0] in l || e[1] in l ? -1 : 1));
                 for (let [d, r] of n) r in l ? l[d] = l[r] : l[r] = l[d];
                 return l
             }
 
-            function E(e) {
+            function H(e) {
                 e = null;
                 const t = e ? [e] : h.screen.blocks;
                 let a = window.innerWidth - 30,
                     l = [],
                     s = {};
                 for (let n of t)
                     if (0 == l.length)
@@ -357,15 +353,15 @@
                             s[a.fullname] = [Math.floor(n / e), t[l]]
                         }
                     }
                 }
                 for (let [n, d] of o.entries()) d in s ? s[n] = s[d] : s[d] = s[n];
                 return s
             }
-            const N = (0, l.aZ)({
+            const E = (0, l.aZ)({
                 name: "menubar",
                 methods: {
                     send() {
                         C(["root", this.name])
                     }
                 },
                 props: {
@@ -375,177 +371,177 @@
                     },
                     icon: {
                         type: String,
                         default: ""
                     }
                 }
             });
-            var U = a(4260),
-                P = a(3414),
-                F = a(2035),
-                K = a(4554),
-                T = a(2350),
-                I = a(7518),
-                R = a.n(I);
-            const B = (0, U.Z)(N, [
+            var N = a(4260),
+                U = a(3414),
+                P = a(2035),
+                F = a(4554),
+                K = a(2350),
+                T = a(7518),
+                I = a.n(T);
+            const R = (0, N.Z)(E, [
                     ["render", n]
                 ]),
-                L = B;
-            R()(N, "components", {
-                QItem: P.Z,
-                QItemSection: F.Z,
-                QIcon: K.Z,
-                QItemLabel: T.Z
+                B = R;
+            I()(E, "components", {
+                QItem: U.Z,
+                QItemSection: P.Z,
+                QIcon: F.Z,
+                QItemLabel: K.Z
             });
-            const Y = {
+            const L = {
                     key: 0,
                     class: "row q-col-gutter-sm q-py-sm"
                 },
-                X = {
+                Y = {
                     class: "q-col-gutter-sm"
                 },
-                G = {
+                X = {
                     key: 0,
                     class: "column q-col-gutter-sm"
                 };
 
-            function J(e, t, a, s, i, o) {
+            function G(e, t, a, s, i, o) {
                 const n = (0, l.up)("zone", !0),
                     d = (0, l.up)("block");
-                return e.data instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", Y, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data, (e => ((0, l.wg)(), (0, l.iD)("div", X, [e instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", G, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e, (e => ((0, l.wg)(), (0, l.j4)(n, {
+                return e.data instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", L, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data, (e => ((0, l.wg)(), (0, l.iD)("div", Y, [e instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", X, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e, (e => ((0, l.wg)(), (0, l.j4)(n, {
                     data: e
                 }, null, 8, ["data"])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                     key: 1,
                     data: e
                 }, null, 8, ["data"]))])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                     key: 1,
                     data: e.data
                 }, null, 8, ["data"]))
             }
-            const ee = {
+            const J = {
                     class: "row"
                 },
-                te = {
+                ee = {
                     key: 2,
                     class: "q-ma-sm",
                     style: {
                         "font-size": "18px"
                     }
                 },
-                ae = ["data", "pdata"],
-                le = {
+                te = ["data", "pdata"],
+                ae = {
                     key: 0,
                     class: "row"
                 },
-                se = ["data", "pdata"],
-                ie = {
+                le = ["data", "pdata"],
+                se = {
                     key: 0,
                     class: "row"
                 };
 
-            function oe(e, t, a, i, o, n) {
+            function ie(e, t, a, i, o, n) {
                 const d = (0, l.up)("element"),
                     r = (0, l.up)("q-icon"),
                     c = (0, l.up)("q-scroll-area"),
                     h = (0, l.up)("q-card");
                 return (0, l.wg)(), (0, l.j4)(h, {
                     class: "my-card q-ma-xs"
                 }, {
-                    default: (0, l.w5)((() => [(0, l._)("div", ee, [e.data.logo ? ((0, l.wg)(), (0, l.j4)(d, {
+                    default: (0, l.w5)((() => [(0, l._)("div", J, [e.data.logo ? ((0, l.wg)(), (0, l.j4)(d, {
                         key: 0,
                         data: e.data.logo,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])) : e.data.icon ? ((0, l.wg)(), (0, l.j4)(r, {
                         key: 1,
                         size: "sm",
                         name: e.data.icon
-                    }, null, 8, ["name"])) : (0, l.kq)("", !0), "_" != e.name[0] ? ((0, l.wg)(), (0, l.iD)("p", te, (0, s.zw)(e.name), 1)) : (0, l.kq)("", !0), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data.top_childs, (t => ((0, l.wg)(), (0, l.j4)(d, {
+                    }, null, 8, ["name"])) : (0, l.kq)("", !0), "_" != e.name[0] ? ((0, l.wg)(), (0, l.iD)("p", ee, (0, s.zw)(e.name), 1)) : (0, l.kq)("", !0), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data.top_childs, (t => ((0, l.wg)(), (0, l.j4)(d, {
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])))), 256))]), e.data.scroll ? ((0, l.wg)(), (0, l.j4)(c, {
                         key: 0,
                         style: (0, s.j5)(e.styleSize),
                         "thumb-style": e.thumbStyle,
                         "bar-style": e.barStyle
                     }, {
                         default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data.childs, (t => ((0, l.wg)(), (0, l.iD)("div", {
                             class: "column",
                             data: t,
                             pdata: e.data
-                        }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", le, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
+                        }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", ae, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
                             class: "q-ma-xs",
                             data: t,
                             pdata: e.data
                         }, null, 8, ["data", "pdata"])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                             key: 1,
                             class: "q-ma-xs",
                             data: t,
                             pdata: e.data
-                        }, null, 8, ["data", "pdata"]))], 8, ae)))), 256))])),
+                        }, null, 8, ["data", "pdata"]))], 8, te)))), 256))])),
                         _: 1
                     }, 8, ["style", "thumb-style", "bar-style"])) : ((0, l.wg)(!0), (0, l.iD)(l.HY, {
                         key: 1
                     }, (0, l.Ko)(e.data.childs, (t => ((0, l.wg)(), (0, l.iD)("div", {
                         class: "column",
                         data: t,
                         pdata: e.data
-                    }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", ie, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
+                    }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", se, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                         key: 1,
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
-                    }, null, 8, ["data", "pdata"]))], 8, se)))), 256))])),
+                    }, null, 8, ["data", "pdata"]))], 8, le)))), 256))])),
                     _: 1
                 })
             }
-            var ne = a(8880);
-            const de = e => ((0, l.dD)("data-v-6d149d62"), e = e(), (0, l.Cn)(), e),
-                re = ["width", "height"],
-                ce = ["src"],
-                he = {
+            var oe = a(8880);
+            const ne = e => ((0, l.dD)("data-v-0593ed42"), e = e(), (0, l.Cn)(), e),
+                de = ["width", "height"],
+                re = ["src"],
+                ce = {
                     key: 16,
                     class: "web-camera-container"
                 },
-                ue = {
+                he = {
                     class: "camera-button"
                 },
-                pe = {
+                ue = {
                     key: 0
                 },
-                ge = {
+                pe = {
                     key: 1
                 },
-                me = {
+                ge = {
                     class: "camera-loading"
                 },
-                fe = de((() => (0, l._)("ul", {
+                me = ne((() => (0, l._)("ul", {
                     class: "loader-circle"
                 }, [(0, l._)("li"), (0, l._)("li"), (0, l._)("li")], -1))),
-                ye = [fe],
+                fe = [me],
+                ye = ["height"],
                 we = ["height"],
-                be = ["height"],
-                ke = {
+                be = {
                     key: 1,
                     class: "camera-shoot"
                 },
-                ve = de((() => (0, l._)("img", {
+                ke = ne((() => (0, l._)("img", {
                     src: "https://img.icons8.com/material-outlined/50/000000/camera--v2.png"
                 }, null, -1))),
-                xe = [ve],
-                Ce = {
+                ve = [ke],
+                xe = {
                     key: 2,
                     class: "camera-download"
                 };
 
-            function qe(e, t, a, i, o, n) {
+            function Ce(e, t, a, i, o, n) {
                 const d = (0, l.up)("q-icon"),
                     r = (0, l.up)("q-img"),
                     c = (0, l.up)("q-badge"),
                     h = (0, l.up)("q-select"),
                     u = (0, l.up)("q-checkbox"),
                     p = (0, l.up)("q-toggle"),
                     g = (0, l.up)("q-btn-toggle"),
@@ -558,22 +554,22 @@
                     v = (0, l.up)("q-uploader"),
                     x = (0, l.up)("cgraph"),
                     C = (0, l.up)("q-btn");
                 return "image" == e.type ? ((0, l.wg)(), (0, l.j4)(r, {
                     key: 0,
                     src: e.data.name,
                     "spinner-color": "blue",
-                    onClick: (0, ne.iM)(e.switchValue, ["stop"]),
+                    onClick: (0, oe.iM)(e.switchValue, ["stop"]),
                     fit: "cover",
                     style: (0, s.j5)(e.elemSize)
                 }, {
                     default: (0, l.w5)((() => [e.data.header ? ((0, l.wg)(), (0, l.iD)("div", {
                         key: 0,
                         class: "absolute-bottom-right text-subtitle2 custom-caption",
-                        onClick: t[0] || (t[0] = (0, ne.iM)(((...t) => e.lens && e.lens(...t)), ["stop"]))
+                        onClick: t[0] || (t[0] = (0, oe.iM)(((...t) => e.lens && e.lens(...t)), ["stop"]))
                     }, (0, s.zw)(e.data.header), 1)) : (0, l.kq)("", !0), e.value ? ((0, l.wg)(), (0, l.j4)(d, {
                         key: 1,
                         class: "absolute all-pointer-events",
                         size: "32px",
                         name: "check_circle",
                         color: "gray",
                         style: {
@@ -651,15 +647,15 @@
                     key: 7,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[5] || (t[5] = t => e.value = t),
                     label: e.name,
                     ref: "inputRef",
                     autogrow: e.data.autogrow,
                     dense: "",
-                    onKeyup: (0, ne.D2)(e.pressedEnter, ["enter"]),
+                    onKeyup: (0, oe.D2)(e.pressedEnter, ["enter"]),
                     readonly: !1 === e.data.edit
                 }, null, 8, ["modelValue", "label", "autogrow", "onKeyup", "readonly"])) : "autoedit" == e.type ? ((0, l.wg)(), (0, l.j4)(h, {
                     key: 8,
                     dense: "",
                     modelValue: e.value,
                     "onUpdate:modelValue": t[6] || (t[6] = t => e.value = t),
                     "use-input": "",
@@ -668,15 +664,15 @@
                     outlined: "",
                     "hide-bottom-space": "",
                     "fill-input": "",
                     "input-debounce": "0",
                     options: e.options,
                     onFilter: e.complete,
                     label: e.name,
-                    onKeyup: (0, ne.D2)(e.pressedEnter, ["enter"])
+                    onKeyup: (0, oe.D2)(e.pressedEnter, ["enter"])
                 }, null, 8, ["modelValue", "options", "onFilter", "label", "onKeyup"])) : "tree" == e.type || "list" == e.type ? ((0, l.wg)(), (0, l.j4)(b, {
                     key: 9,
                     style: (0, s.j5)(e.styleSize),
                     "thumb-style": e.thumbStyle,
                     "bar-style": e.barStyle
                 }, {
                     default: (0, l.w5)((() => [(0, l.Wm)(w, {
@@ -694,27 +690,27 @@
                     key: 10,
                     class: "textarea",
                     "onUpdate:modelValue": t[9] || (t[9] = t => e.value = t),
                     filled: "",
                     type: "textarea",
                     style: (0, s.j5)(e.elemSize)
                 }, null, 4)), [
-                    [ne.nr, e.value]
+                    [oe.nr, e.value]
                 ]) : "line" == e.type ? ((0, l.wg)(), (0, l.j4)(k, {
                     key: 11,
                     color: "green"
                 })) : "video" == e.type ? ((0, l.wg)(), (0, l.iD)("video", {
                     width: e.data.width,
                     height: e.data.height,
                     key: e.data.src,
                     controls: ""
                 }, [(0, l._)("source", {
                     src: e.data.src,
                     type: "video/mp4"
-                }, null, 8, ce)], 8, re)) : "gallery" == e.type ? ((0, l.wg)(), (0, l.j4)(v, {
+                }, null, 8, re)], 8, de)) : "gallery" == e.type ? ((0, l.wg)(), (0, l.j4)(v, {
                     key: 13,
                     label: e.name,
                     "auto-upload": "",
                     thumbnails: "",
                     url: "http://localhost:8000",
                     onUploaded: e.updateDom,
                     onAdded: e.onAdded,
@@ -732,53 +728,53 @@
                     ref: "uploaderRef",
                     flat: ""
                 }, null, 8, ["label", "onUploaded", "onAdded"])) : "graph" == e.type ? ((0, l.wg)(), (0, l.j4)(x, {
                     key: 15,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.elemSize
-                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, l.wg)(), (0, l.iD)("div", he, [(0, l._)("div", ue, [(0, l._)("button", {
+                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, l.wg)(), (0, l.iD)("div", ce, [(0, l._)("div", he, [(0, l._)("button", {
                     class: (0, s.C_)(["button is-rounded", {
                         "is-primary": !e.isCameraOpen,
                         "is-danger": e.isCameraOpen
                     }]),
                     type: "button",
                     onClick: t[10] || (t[10] = (...t) => e.toggleCamera && e.toggleCamera(...t))
-                }, [e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("span", ge, "Close Camera")) : ((0, l.wg)(), (0, l.iD)("span", pe, "Open Camera"))], 2)]), (0, l.wy)((0, l._)("div", me, ye, 512), [
-                    [ne.F8, e.isCameraOpen && e.isLoading]
+                }, [e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("span", pe, "Close Camera")) : ((0, l.wg)(), (0, l.iD)("span", ue, "Open Camera"))], 2)]), (0, l.wy)((0, l._)("div", ge, fe, 512), [
+                    [oe.F8, e.isCameraOpen && e.isLoading]
                 ]), e.isCameraOpen ? (0, l.wy)(((0, l.wg)(), (0, l.iD)("div", {
                     key: 0,
                     class: (0, s.C_)(["camera-box", {
                         flash: e.isShotPhoto
                     }])
                 }, [(0, l._)("div", {
                     class: (0, s.C_)(["camera-shutter", {
                         flash: e.isShotPhoto
                     }])
                 }, null, 2), (0, l.wy)((0, l._)("video", {
                     ref: "camera",
                     width: 450,
                     height: 337.5,
                     autoplay: ""
-                }, null, 8, we), [
-                    [ne.F8, !e.isPhotoTaken]
+                }, null, 8, ye), [
+                    [oe.F8, !e.isPhotoTaken]
                 ]), (0, l.wy)((0, l._)("canvas", {
                     id: "photoTaken",
                     ref: "canvas",
                     width: 450,
                     height: 337.5
-                }, null, 8, be), [
-                    [ne.F8, e.isPhotoTaken]
+                }, null, 8, we), [
+                    [oe.F8, e.isPhotoTaken]
                 ])], 2)), [
-                    [ne.F8, !e.isLoading]
-                ]) : (0, l.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, l.wg)(), (0, l.iD)("div", ke, [(0, l._)("button", {
+                    [oe.F8, !e.isLoading]
+                ]) : (0, l.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, l.wg)(), (0, l.iD)("div", be, [(0, l._)("button", {
                     class: "button",
                     type: "button",
                     onClick: t[11] || (t[11] = (...t) => e.takePhoto && e.takePhoto(...t))
-                }, xe)])) : (0, l.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("div", Ce, [(0, l.Wm)(C, {
+                }, ve)])) : (0, l.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("div", xe, [(0, l.Wm)(C, {
                     onClick: e.downloadImage,
                     label: "Send"
                 }, null, 8, ["onClick"])])) : (0, l.kq)("", !0)])) : "" != e.showname ? ((0, l.wg)(), (0, l.j4)(C, {
                     key: 17,
                     "no-caps": "",
                     label: e.name,
                     icon: e.data.icon,
@@ -787,23 +783,23 @@
                     key: 18,
                     "no-caps": "",
                     dense: "",
                     icon: e.data.icon,
                     onClick: e.sendValue
                 }, null, 8, ["icon", "onClick"]))
             }
-            const _e = {
+            const qe = {
                     key: 0
                 },
-                Se = {
+                _e = {
                     class: "row"
                 },
-                je = ["onClick"];
+                Se = ["onClick"];
 
-            function Ae(e, t, a, i, o, n) {
+            function je(e, t, a, i, o, n) {
                 const d = (0, l.up)("q-icon"),
                     r = (0, l.up)("q-input"),
                     c = (0, l.up)("q-tooltip"),
                     h = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-th"),
                     p = (0, l.up)("q-tr"),
                     g = (0, l.up)("q-checkbox"),
@@ -825,15 +821,15 @@
                     title: e.name,
                     rows: e.rows,
                     columns: e.columns,
                     selection: e.singleMode ? "single" : "multiple",
                     selected: e.selected,
                     "onUpdate:selected": t[1] || (t[1] = t => e.selected = t)
                 }, {
-                    "top-right": (0, l.w5)((() => [!1 !== e.data.tools ? ((0, l.wg)(), (0, l.iD)("div", _e, [(0, l._)("div", Se, [(0, l.Wm)(r, {
+                    "top-right": (0, l.w5)((() => [!1 !== e.data.tools ? ((0, l.wg)(), (0, l.iD)("div", qe, [(0, l._)("div", _e, [(0, l.Wm)(r, {
                         modelValue: e.search,
                         "onUpdate:modelValue": t[0] || (t[0] = t => e.search = t),
                         label: "Search",
                         dense: ""
                     }, {
                         prepend: (0, l.w5)((() => [(0, l.Wm)(d, {
                             name: "search"
@@ -992,34 +988,34 @@
                                 "onUpdate:modelValue": [e => t.row[a.name] = e, e.change],
                                 dense: "",
                                 onKeydown: e.keyInput,
                                 autofocus: ""
                             }, null, 8, ["modelValue", "onUpdate:modelValue", "onKeydown"])) : ((0, l.wg)(), (0, l.iD)("div", {
                                 key: 3,
                                 onClick: a => e.select(t.row.iiid, i)
-                            }, (0, s.zw)(t.row[a.name]), 9, je))])),
+                            }, (0, s.zw)(t.row[a.name]), 9, Se))])),
                             _: 2
                         }, 1032, ["props"])))), 128))])),
                         _: 2
                     }, 1032, ["props", "onClick"])])),
                     _: 1
                 }, 8, ["style", "filter", "title", "rows", "columns", "selection", "selected"])
             }
-            var ze = a(1959);
+            var Ae = a(1959);
 
-            function Ze(e, t) {
+            function ze(e, t) {
                 return e.length === t.length && e.every(((e, a) => e.iiid == t[a].iiid))
             }
-            const Me = (0, l.aZ)({
+            const Ze = (0, l.aZ)({
                 name: "utable",
                 setup(e) {
                     const {
                         data: t,
                         pdata: a
-                    } = (0, ze.BK)(e);
+                    } = (0, Ae.BK)(e);
                     let s = (0, l.Fl)((() => {
                             let e = [],
                                 a = t.value;
                             const l = a.headers,
                                 s = l.length,
                                 i = a.rows,
                                 o = i.length;
@@ -1033,17 +1029,17 @@
                         })),
                         i = () => {
                             let e = t.value,
                                 a = null === e.value || 0 == s.value.length ? [] : Array.isArray(e.value) ? e.value.map((e => s.value[e])) : [s.value[e.value]];
                             return a
                         },
                         o = i(),
-                        n = (0, ze.iH)(o),
-                        d = (0, ze.iH)(o),
-                        r = (0, ze.iH)(!Array.isArray(t.value.value)),
+                        n = (0, Ae.iH)(o),
+                        d = (0, Ae.iH)(o),
+                        r = (0, Ae.iH)(!Array.isArray(t.value.value)),
                         c = (e, l) => {
                             C([a.value.name, t.value.name, e, l])
                         },
                         h = (0, l.Fl)((() => r.value ? d.value.length > 0 ? d.value[0].iiid : null : d.value.map((e => e.iiid)))),
                         u = (0, l.Fl)((() => t.value.value));
                     return (0, l.YP)(s, ((e, t) => {
                         d.value = i(), n.value = d.value
@@ -1131,23 +1127,23 @@
                                         t = typeof this.data.rows[e][this.cedit];
                                     "string" != t && "number" != t || (this.selected = [this.rows[e]])
                                 }
                                 break
                         }
                     },
                     complete(e, t, a) {
-                        z(this, [e, [this.redit, this.cedit]], (e => t((() => {
+                        A(this, [e, [this.redit, this.cedit]], (e => t((() => {
                             this.options = e
                         }))))
                     },
                     append() {
                         let e = this.data.rows,
                             t = e.length,
                             a = this;
-                        z(this, [t, this.search], (function(l) {
+                        A(this, [t, this.search], (function(l) {
                             if (!Array.isArray(l)) return h.error(l);
                             p && console.log("added row", l), a.search = "", e.push(l), setTimeout((() => {
                                 let e = a.rows;
                                 a.select(e[t], 0), a.showSelected()
                             }), 100)
                         }), "+")
                     },
@@ -1181,15 +1177,15 @@
                             for (let t of this.selected) e.splice(t.iiid, 1)
                         }
                         this.selected = []
                     }
                 },
                 watch: {
                     selected(e) {
-                        Ze(this.updated, this.selected) || (this.sendMessage("=", this.value), this.updated = this.selected), this.data.show && this.showSelected()
+                        ze(this.updated, this.selected) || (this.sendMessage("=", this.value), this.updated = this.selected), this.data.show && this.showSelected()
                     }
                 },
                 computed: {
                     redit() {
                         return console.log("redit", this.editMode && this.selected.length ? this.selected[0].iiid : null), this.editMode && this.selected.length ? this.selected[0].iiid : null
                     },
                     editable() {
@@ -1210,52 +1206,52 @@
                 },
                 props: {
                     data: Object,
                     pdata: Object,
                     styleSize: String
                 }
             });
-            var $e = a(9267),
-                De = a(4842),
-                Ve = a(2165),
-                Oe = a(8870),
-                Qe = a(8186),
-                We = a(2414),
-                He = a(3884),
-                Ee = a(5735),
-                Ne = a(7208);
-            const Ue = (0, U.Z)(Me, [
-                    ["render", Ae]
+            var Me = a(9267),
+                $e = a(4842),
+                De = a(2165),
+                Ve = a(8870),
+                Oe = a(8186),
+                Qe = a(2414),
+                We = a(3884),
+                He = a(5735),
+                Ee = a(7208);
+            const Ne = (0, N.Z)(Ze, [
+                    ["render", je]
                 ]),
-                Pe = Ue;
-            R()(Me, "components", {
-                QTable: $e.Z,
-                QInput: De.Z,
-                QIcon: K.Z,
-                QBtn: Ve.Z,
-                QTooltip: Oe.Z,
-                QTr: Qe.Z,
-                QTh: We.Z,
-                QTd: He.Z,
-                QCheckbox: Ee.Z,
-                QSelect: Ne.Z
+                Ue = Ne;
+            I()(Ze, "components", {
+                QTable: Me.Z,
+                QInput: $e.Z,
+                QIcon: F.Z,
+                QBtn: De.Z,
+                QTooltip: Ve.Z,
+                QTr: Oe.Z,
+                QTh: Qe.Z,
+                QTd: We.Z,
+                QCheckbox: He.Z,
+                QSelect: Ee.Z
             });
-            const Fe = ["nodes", "edges"];
+            const Pe = ["nodes", "edges"];
 
-            function Ke(e, t, a, i, o, n) {
+            function Fe(e, t, a, i, o, n) {
                 return (0, l.wg)(), (0, l.iD)("div", {
                     nodes: e.nodes,
                     edges: e.edges,
                     style: (0, s.j5)(e.styleSize),
                     ref: "cy"
-                }, null, 12, Fe)
+                }, null, 12, Pe)
             }
-            var Te = a(2393),
-                Ie = a.n(Te);
-            const Re = Ie().stylesheet().selector("node").css({
+            var Ke = a(2393),
+                Te = a.n(Ke);
+            const Ie = Te().stylesheet().selector("node").css({
                     content: "data(id)",
                     "background-color": "#4286f4"
                 }).selector(".selected").css({
                     "background-color": "#ff5555",
                     "border-color": "#ff5555"
                 }).selector("node[label]").css({
                     label: "data(label)",
@@ -1274,45 +1270,45 @@
                 }).selector("edge[label]").css({
                     label: "data(label)",
                     "text-rotation": "autorotate",
                     "text-margin-x": "-8px",
                     "text-margin-y": "-8px",
                     color: "gray"
                 }),
-                Be = {
+                Re = {
                     animate: !0,
                     randomize: !0
                 };
 
-            function Le(e, t) {
+            function Be(e, t) {
                 if (e.length != t.length) return !0;
                 for (let a = 0; a < e.length; a++)
                     if (e[a].id != t[a].id) return !0;
                 return !1
             }
-            const Ye = (0, l.aZ)({
+            const Le = (0, l.aZ)({
                     name: "cgraph",
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
                         return {
                             cy: null,
-                            style: Re,
-                            layoutOptions: Be,
+                            style: Ie,
+                            layoutOptions: Re,
                             selectedNodes: [],
                             selectedEdges: [],
                             oldNodes: [],
                             oldEdges: []
                         }
                     },
                     mounted() {
-                        let e = Ie()({
+                        let e = Te()({
                                 container: this.$refs.cy,
                                 elements: {
                                     nodes: this.nodes,
                                     edges: this.edges
                                 },
                                 style: this.style
                             }),
@@ -1427,15 +1423,15 @@
                             }
                         },
                         data: {
                             handler(e, t) {
                                 console.log("wa gr");
                                 let a = e.value,
                                     l = !1;
-                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Le(e.nodes, this.oldNodes) && (l = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Le(e.edges, this.oldEdges) && (l = !0, this.oldEdges = e.edges), l && null != this.cy) {
+                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Be(e.nodes, this.oldNodes) && (l = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Be(e.edges, this.oldEdges) && (l = !0, this.oldEdges = e.edges), l && null != this.cy) {
                                     this.cy.json({
                                         elements: {
                                             nodes: this.nodes,
                                             edges: this.edges
                                         }
                                     });
                                     let e = this.data.method;
@@ -1452,43 +1448,43 @@
                             this.cy.style(e)
                         },
                         layoutOptions(e) {
                             this.cy.layout(e).run()
                         }
                     }
                 }),
-                Xe = (0, U.Z)(Ye, [
-                    ["render", Ke]
+                Ye = (0, N.Z)(Le, [
+                    ["render", Fe]
                 ]),
-                Ge = Xe;
+                Xe = Ye;
 
-            function Je(e, t, a, i, o, n) {
+            function Ge(e, t, a, i, o, n) {
                 const d = (0, l.up)("v-chart");
                 return (0, l.wg)(), (0, l.j4)(d, {
                     ref: "chart",
                     option: o.options,
                     style: (0, s.j5)(a.styleSize),
                     autoresize: !0,
                     onClick: n.clicked
                 }, null, 8, ["option", "style", "onClick"])
             }
-            var et = a(5512),
-                tt = a(4447),
-                at = a(1006),
-                lt = a(3526),
-                st = a(763),
-                it = a(546),
-                ot = a(6902),
-                nt = a(2826),
-                dt = a(5256),
-                rt = a(3825),
-                ct = a(8825);
-            (0, st.D)([tt.N, at.N, lt.N]), (0, st.D)([it.N, ot.N, nt.N, dt.N, rt.N]);
-            let ht = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"],
-                ut = {
+            var Je = a(5512),
+                et = a(4447),
+                tt = a(1006),
+                at = a(3526),
+                lt = a(763),
+                st = a(546),
+                it = a(6902),
+                ot = a(2826),
+                nt = a(5256),
+                dt = a(3825),
+                rt = a(8825);
+            (0, lt.D)([et.N, tt.N, at.N]), (0, lt.D)([st.N, it.N, ot.N, nt.N, dt.N]);
+            let ct = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"],
+                ht = {
                     responsive: !0,
                     maintainAspectRatio: !1,
                     legend: {
                         data: [],
                         bottom: 10
                     },
                     tooltip: {
@@ -1523,26 +1519,26 @@
                         end: 10
                     }, {
                         start: 0,
                         end: 10
                     }],
                     series: []
                 };
-            const pt = {
+            const ut = {
                     name: "linechart",
                     components: {
-                        VChart: et.ZP
+                        VChart: Je.ZP
                     },
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
-                        const e = (0, ct.Z)();
+                        const e = (0, rt.Z)();
                         return {
                             $q: e,
                             model: !1,
                             options: null
                         }
                     },
                     methods: {
@@ -1571,49 +1567,49 @@
                             let s = [];
                             for (let o = 0; o < l.length; o++) l[o] = "i" == l[o] ? -1 : parseInt(l[o]), s.push([]), o && (this.options.series.push({
                                 name: t[l[o]],
                                 type: "line",
                                 symbol: "none",
                                 sampling: "lttb",
                                 itemStyle: {
-                                    color: ht[o]
+                                    color: ct[o]
                                 },
                                 data: s[o]
                             }), this.options.legend.data.push(t[l[o]]));
                             this.options.xAxis.data = s[0];
                             let i = this.data.rows;
                             for (let o = 0; o < i.length; o++)
                                 for (let e = 0; e < l.length; e++) s[e].push(-1 == l[e] ? o : i[o][l[e]]);
                             this.$refs.chart.setOption(this.options)
                         }
                     },
                     mounted() {
-                        this.options = (0, c.cloneDeep)(ut), this.calcSeries(), this.$refs.chart.chart.on("click", this.clicked)
+                        this.options = (0, c.cloneDeep)(ht), this.calcSeries(), this.$refs.chart.chart.on("click", this.clicked)
                     },
                     watch: {}
                 },
-                gt = (0, U.Z)(pt, [
-                    ["render", Je]
+                pt = (0, N.Z)(ut, [
+                    ["render", Ge]
                 ]),
-                mt = gt;
+                gt = pt;
 
-            function ft(e) {
+            function mt(e) {
                 let t = new FormData;
                 t.append("image", e);
                 let a = new XMLHttpRequest;
                 a.open("POST", "http://localhost:8000", !0), a.onload = function() {
                     200 === this.status ? console.log(this.response) : console.error(a)
                 }, a.send(t)
             }
-            const yt = (0, l.aZ)({
+            const ft = (0, l.aZ)({
                 name: "element",
                 components: {
-                    utable: Pe,
-                    cgraph: Ge,
-                    linechart: mt
+                    utable: Ue,
+                    cgraph: Xe,
+                    linechart: gt
                 },
                 methods: {
                     log(e) {
                         console.log(e)
                     },
                     onAdded(e) {
                         0 !== e.length && (0 !== this.fileArr.length ? (this.$refs.uploaderRef.removeFile(this.fileArr[0]), this.fileArr.splice(0, 1, e[0])) : this.fileArr.push(e[0]))
@@ -1622,27 +1618,27 @@
                         C([this.pdata["name"], this.data["name"], e, t])
                     },
                     pressedEnter() {
                         "update" in this.data && this.sendMessage("->", this.value)
                     },
                     updateDom(e) {
                         let t = e.files.length;
-                        t && (this.sendMessage("=", e.files[t - 1].name), Q())
+                        t && (this.sendMessage("=", e.files[t - 1].name), O())
                     },
                     sendValue() {
                         this.sendMessage("=", this.value)
                     },
                     switchValue() {
                         this.value = !this.value
                     },
                     setValue(e) {
                         console.log(e), this.value = e
                     },
                     complete(e, t, a) {
-                        this.value = e, z(this, e, (e => t((() => {
+                        this.value = e, A(this, e, (e => t((() => {
                             this.options = e
                         }))))
                     },
                     lens() {
                         h.lens(this.data)
                     },
                     toggleCamera() {
@@ -1675,15 +1671,15 @@
                             }), e)
                         }
                         this.isPhotoTaken = !this.isPhotoTaken;
                         const e = this.$refs.canvas.getContext("2d");
                         e.drawImage(this.$refs.camera, 0, 0, 450, 337.5)
                     },
                     downloadImage() {
-                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(ft, "image/jpeg")
+                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(mt, "image/jpeg")
                     },
                     geom() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
                         e || (e = this.$el.previousElementSibling, e = "clientHeight" in e ? e : e.nextElementSibling);
                         let t = this.type;
                         const a = "docviewer" == t || "graph" == t || "linechart" == t ? e : e.querySelector("table" == t ? ".scroll" : ".q-tree"),
                             l = e.getBoundingClientRect();
@@ -1814,50 +1810,50 @@
                         p && console.log("selection changed", e, this.$refs.inputRef), Array.isArray(e) || (e = [0, 0]);
                         let t = this.$refs.inputRef.$el;
                         t.focus();
                         let a = t.getElementsByTagName("textarea");
                         0 == a.length && (a = t.getElementsByTagName("input")), a[0].setSelectionRange(e[0], e[1])
                     },
                     data(e, t) {
-                        p && console.log("data update", this.fullname, t.name), this.expanding && (this.styleSize || (this.styleSize = y(this.data), console.log(`${this.name} size changed`))), this.value = this.data.value, this.updated = this.value, b[this.fullname] = this
+                        p && console.log("data update", this.fullname, t.name), this.styleSize || (this.styleSize = y(this.data), p && console.log(`${this.name} size changed`)), this.value = this.data.value, this.updated = this.value, b[this.fullname] = this
                     }
                 }
             });
-            var wt = a(4027),
-                bt = a(9721),
-                kt = a(8886),
-                vt = a(8761),
-                xt = a(1232),
-                Ct = a(5551),
-                qt = a(5869),
-                _t = a(1745);
-            const St = (0, U.Z)(yt, [
-                    ["render", qe],
-                    ["__scopeId", "data-v-6d149d62"]
+            var yt = a(4027),
+                wt = a(9721),
+                bt = a(8886),
+                kt = a(8761),
+                vt = a(1232),
+                xt = a(5551),
+                Ct = a(5869),
+                qt = a(1745);
+            const _t = (0, N.Z)(ft, [
+                    ["render", Ce],
+                    ["__scopeId", "data-v-0593ed42"]
                 ]),
-                jt = St;
-            R()(yt, "components", {
-                QImg: wt.Z,
-                QIcon: K.Z,
-                QSelect: Ne.Z,
-                QBadge: bt.Z,
-                QCheckbox: Ee.Z,
-                QToggle: kt.Z,
-                QBtnToggle: vt.Z,
-                QInput: De.Z,
-                QScrollArea: xt.Z,
-                QTree: Ct.Z,
-                QSeparator: qt.Z,
-                QUploader: _t.Z,
-                QBtn: Ve.Z
+                St = _t;
+            I()(ft, "components", {
+                QImg: yt.Z,
+                QIcon: F.Z,
+                QSelect: Ee.Z,
+                QBadge: wt.Z,
+                QCheckbox: He.Z,
+                QToggle: bt.Z,
+                QBtnToggle: kt.Z,
+                QInput: $e.Z,
+                QScrollArea: vt.Z,
+                QTree: xt.Z,
+                QSeparator: Ct.Z,
+                QUploader: qt.Z,
+                QBtn: De.Z
             });
-            const At = (0, l.aZ)({
+            const jt = (0, l.aZ)({
                 name: "block",
                 components: {
-                    element: jt
+                    element: St
                 },
                 data() {
                     return {
                         styleSize: f,
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
@@ -1924,51 +1920,51 @@
                 },
                 watch: {
                     data(e) {
                         p && console.log("data update", this.name), this.styleSize = f, w[this.name] = this, this.expanding && (b[this.fullname] = this)
                     }
                 }
             });
-            var zt = a(151);
-            const Zt = (0, U.Z)(At, [
-                    ["render", oe]
+            var At = a(151);
+            const zt = (0, N.Z)(jt, [
+                    ["render", ie]
                 ]),
-                Mt = Zt;
-            R()(At, "components", {
-                QCard: zt.Z,
-                QIcon: K.Z,
-                QScrollArea: xt.Z
+                Zt = zt;
+            I()(jt, "components", {
+                QCard: At.Z,
+                QIcon: F.Z,
+                QScrollArea: vt.Z
             });
-            const $t = (0, l.aZ)({
+            const Mt = (0, l.aZ)({
                     name: "zone",
                     components: {
-                        block: Mt
+                        block: Zt
                     },
                     props: {
                         data: Object
                     },
                     updated(e) {
                         (0, l.Y3)((() => {
                             requestAnimationFrame((() => {
                                 requestAnimationFrame((() => {
-                                    W()
+                                    Q()
                                 }))
                             }))
                         }))
                     }
                 }),
-                Dt = (0, U.Z)($t, [
-                    ["render", J]
+                $t = (0, N.Z)(Mt, [
+                    ["render", G]
                 ]),
-                Vt = Dt,
-                Ot = {
+                Dt = $t,
+                Vt = {
                     class: "row q-gutter-sm row-md"
                 };
 
-            function Qt(e, t, a, i, o, n) {
+            function Ot(e, t, a, i, o, n) {
                 const d = (0, l.up)("block"),
                     r = (0, l.up)("q-item-label"),
                     c = (0, l.up)("q-space"),
                     h = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-card"),
                     p = (0, l.up)("q-dialog");
                 return (0, l.wg)(), (0, l.j4)(p, {
@@ -1984,32 +1980,32 @@
                             key: 0,
                             data: a.data
                         }, null, 8, ["data"])) : (0, l.kq)("", !0), (0, l.Wm)(r, {
                             class: "text-h6"
                         }, {
                             default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(a.data.text ? a.data.text : ""), 1)])),
                             _: 1
-                        }), (0, l._)("div", Ot, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
+                        }), (0, l._)("div", Vt, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
                             class: "col-md-3",
                             label: e,
                             color: a.buttons[0] == e ? "primary" : "secondary",
                             onClick: t => n.sendMessage(e)
                         }, null, 8, ["label", "color", "onClick"])))), 256))])])),
                         _: 1
                     }, 8, ["style"])])),
                     _: 1
                 }, 8, ["onHide"])
             }
-            const Wt = {
+            const Qt = {
                 props: {
                     data: Object,
                     buttons: Array
                 },
                 components: {
-                    block: Mt
+                    block: Zt
                 },
                 emits: ["ok", "hide"],
                 methods: {
                     show() {
                         this.$refs.dialog.show()
                     },
                     sendMessage(e) {
@@ -2025,46 +2021,46 @@
                         this.$emit("ok"), this.hide()
                     },
                     onCancelClick() {
                         this.hide()
                     }
                 }
             };
-            var Ht = a(5926),
-                Et = a(2025);
-            const Nt = (0, U.Z)(Wt, [
-                    ["render", Qt]
+            var Wt = a(5926),
+                Ht = a(2025);
+            const Et = (0, N.Z)(Qt, [
+                    ["render", Ot]
                 ]),
-                Ut = Nt;
-            R()(Wt, "components", {
-                QDialog: Ht.Z,
-                QCard: zt.Z,
-                QItemLabel: T.Z,
-                QSpace: Et.Z,
-                QBtn: Ve.Z
+                Nt = Et;
+            I()(Qt, "components", {
+                QDialog: Wt.Z,
+                QCard: At.Z,
+                QItemLabel: K.Z,
+                QSpace: Ht.Z,
+                QBtn: De.Z
             });
-            var Pt = !0;
-            let Ft = null;
-            const Kt = (0, l.aZ)({
+            var Ut = !0;
+            let Pt = null;
+            const Ft = (0, l.aZ)({
                 name: "MainLayout",
                 data() {
                     return {
                         leftDrawerOpen: !1,
                         menu: [],
                         tab: "",
                         localServer: !0,
                         statusConnect: !1,
                         screen: {
                             blocks: []
                         }
                     }
                 },
                 components: {
-                    menubar: L,
-                    zone: Vt
+                    menubar: B,
+                    zone: Dt
                 },
                 created() {
                     v(this)
                 },
                 unmounted() {
                     window.removeEventListener("resize", this.onResize)
                 },
@@ -2072,23 +2068,23 @@
                     toggleLeftDrawer() {
                         this.leftDrawerOpen = !this.leftDrawerOpen
                     },
                     tabclick(e) {
                         C(["root", e])
                     },
                     onResize(e) {
-                        p && console.log("window has been resized", window.innerHeight, window.innerWidth), Q()
+                        p && console.log("window has been resized", window.innerHeight, window.innerWidth), O()
                     },
                     lens(e) {
                         let t = {
                                 title: "Photo lens",
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0,
-                                component: Ut
+                                component: Nt
                             },
                             {
                                 height: a,
                                 ...l
                             } = e;
                         l.width = 750;
                         let s = {
@@ -2106,82 +2102,82 @@
                         let a = t,
                             l = {
                                 message: e,
                                 type: t,
                                 position: "top",
                                 icon: a
                             };
-                        "progress" == t ? null == Ft ? (l = {
+                        "progress" == t ? null == Pt ? (l = {
                             group: !1,
                             timeout: 0,
                             spinner: !0,
                             type: "info",
                             message: e || "Progress..",
                             position: "top",
                             color: "secondary"
-                        }, Ft = this.$q.notify(l)) : null == e ? (Ft(), Ft = null) : (l = {
+                        }, Pt = this.$q.notify(l)) : null == e ? (Pt(), Pt = null) : (l = {
                             caption: e
-                        }, Ft(l)) : ("error" == t && l.type, this.$q.notify(l))
+                        }, Pt(l)) : ("error" == t && l.type, this.$q.notify(l))
                     },
                     error(e) {
                         this.notify(e, "error")
                     },
                     info(e) {
                         this.notify(e, "info")
                     },
                     processMessage(e) {
-                        if (Pt) Pt = !1, this.menu = e[0].map((e => ({
+                        if (Ut) Ut = !1, this.menu = e[0].map((e => ({
                             name: e[0],
                             icon: e[1],
                             order: e[2]
                         }))), this.screen = e[1], this.tab = this.screen.name, p && console.log("init loading..");
-                        else if ("screen" == e.type) this.screen.name != e.name && j(), Z(), this.screen = e;
+                        else if ("screen" == e.type) this.screen.name != e.name && j(), z(), this.screen = e;
                         else if ("dialog" == e.type) {
                             let t = {
                                 title: e.name,
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0
                             };
-                            t.component = Ut, t.componentProps = {
+                            t.component = Nt, t.componentProps = {
                                 data: e.content ? e.content : e,
                                 buttons: e.buttons
                             }, this.$q.dialog(t)
-                        } else if (e.hasOwnProperty("answer")) D(e);
+                        } else if (e.hasOwnProperty("answer")) $(e);
                         else {
-                            e.update && $(e);
+                            e.update && M(e);
                             let t = !1;
                             for (let a of k) a in e && (this.notify(e[a], a), t = !0);
                             t || e.update || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
                         }
-                        Ft && !e.progress && this.notify(null, "progress")
+                        Pt && !e.progress && this.notify(null, "progress")
                     }
                 },
                 mounted() {
                     window.addEventListener("resize", this.onResize)
                 }
             });
-            var Tt = a(9214),
-                It = a(3812),
-                Rt = a(9570),
-                Bt = a(7547),
-                Lt = a(3269),
-                Yt = a(2652),
-                Xt = a(4379);
-            const Gt = (0, U.Z)(Kt, [
+            var Kt = a(9214),
+                Tt = a(3812),
+                It = a(9570),
+                Rt = a(7547),
+                Bt = a(3269),
+                Lt = a(2652),
+                Yt = a(4379);
+            const Xt = (0, N.Z)(Ft, [
                     ["render", o]
                 ]),
-                Jt = Gt;
-            R()(Kt, "components", {
-                QLayout: Tt.Z,
-                QHeader: It.Z,
-                QToolbar: Rt.Z,
-                QBtn: Ve.Z,
-                QItemLabel: T.Z,
-                QTabs: Bt.Z,
-                QTab: Lt.Z,
-                QPageContainer: Yt.Z,
-                QPage: Xt.Z
+                Gt = Xt;
+            I()(Ft, "components", {
+                QLayout: Kt.Z,
+                QHeader: Tt.Z,
+                QToolbar: It.Z,
+                QBtn: De.Z,
+                QItemLabel: K.Z,
+                QTabs: Rt.Z,
+                QTab: Bt.Z,
+                QPageContainer: Lt.Z,
+                QPage: Yt.Z
             })
         }
     }
 ]);
```

### Comparing `unigui-1.4.6/unigui/web/js/430.591e9a73.js` & `unigui-1.4.7/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/web/js/app.0d4bddce.js` & `unigui-1.4.7/unigui/web/js/app.92f553f5.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(259)]).then(r.bind(r, 8259)),
+                        component: () => Promise.all([r.e(736), r.e(889)]).then(r.bind(r, 2889)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -159,25 +159,25 @@
             })
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, n) => (r.f[n](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "283445be",
-            259: "1c52f635",
-            430: "591e9a73"
+            430: "591e9a73",
+            889: "504369e0"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
-            259: "f5c7cbc7",
-            736: "49a52e8f"
+            736: "49a52e8f",
+            889: "c9159919"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
             } catch (e) {
@@ -260,15 +260,15 @@
                 e(n, l, o, a)
             })),
             o = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                259: 1
+                889: 1
             };
             o[e] ? t.push(o[e]) : 0 !== o[e] && r[e] && t.push(o[e] = n(e).then((() => {
                 o[e] = 0
             }), (t => {
                 throw delete o[e], t
             })))
         }
```

### Comparing `unigui-1.4.6/unigui/web/js/193.283445be.js` & `unigui-1.4.7/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/web/js/vendor.3e8714c2.js` & `unigui-1.4.7/unigui/web/js/vendor.3e8714c2.js`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/unigui/web/index.html` & `unigui-1.4.7/unigui/web/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.3e8714c2.js></script><script defer src=js/app.0d4bddce.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.3e8714c2.js></script><script defer src=js/app.92f553f5.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.4.6/LICENSE` & `unigui-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.4.6/setup.py` & `unigui-1.4.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.4.6',      
+      version='1.4.7',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal app browser',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.4.6/PKG-INFO` & `unigui-1.4.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.4.6
+Version: 1.4.7
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -56,20 +56,19 @@
 
 #### Screen function prepare() syncronizes GUI elements one to another and with the program/system data. prepare() is called when the screen open/loaded. prepare() is optional. ###
 
 ### Server start ###
 tests/run_hello.py
 ```
 import unigui
-#app name, port for initial connection and upload_dir folder are optional
+#app name, the others server setting in config.py like port, upload_dir, ..
 unigui.start('Test app') 
 ```
 Unigui builds the interactive app for the code above.
 Connect a browser to localhast:8000 which are by default and will see:
-server port and ip config is in config.py file in the working directory
 
 ![image](https://github.com/Claus1/unigui/assets/1247062/5afcf4ac-b388-4237-98ff-3a92e802d44a)
 
 ### Handling events ###
 All handlers are functions which have a signature
 ```
 def handler_x(gui_object, value_x)
@@ -91,26 +90,28 @@
 | :---: | :---: | 
 | Gui object |  Object to update |
 | Gui object array or tuple |  Objects to update |
 | None | Nothing to update, Ok |
 | Error(...), Warning(...), Info(...) | Show to user info about a problem. |
 | UpdateScreen, True | Redraw whole screen |
 | Dialog(..) | Open a dialog with parameters |
+| user.set_screen(screen_name) | switch to another screen |
+| Signal(signal_name, ..) | causes indirect call screen.dispatch or/and user.dispatch handlers | 
 
 Unigui	synchronizes GUI state on frontend-end automatically after calling a handler.
 
 If a Gui object doesn't have 'changed' handler the object accepts incoming value automatically to the 'value' variable of gui object.
 
 If 'value' is not acceptable instead of returning an object possible to return Error or Warning or Info. That functions can update a object list passed after the message argument.
 
 ```
 def changed_range(_, value):
    if value < 0.5 and value > 1.0:
-       #or Error(message, _) if we want to return the previous visible value to the field
-       return Error(f‘The value of {_.name} has to be > 0.5 and < 1.0!') 
+       #or Error(message, _) if we want to return the previous visible value to the field, return gui object _ also.
+       return Error(f‘The value of {_.name} has to be > 0.5 and < 1.0!', _) 
     #accept value othewise
     _.value = value
 
 edit = Edit('Range of involving', 0.6, changed_range)
 ```
 
 ### Block details ###
@@ -248,14 +249,16 @@
 ```
 Optional type parameter can be 'toggles','list','dropdown'. Unigui automatically chooses between toogles and dropdown, if type is omitted,
 if type = 'list' then Unigui build it as vertical select list.
 
 
 ### Image. ###
 width,changed,height,header are optional, changed is called if the user select or touch the image.
+When the user click the image, a check mark is appearing on the image, showning select status of the image.
+It is usefull for image list, gallery, e.t.c
 ```
 Image(image_url, header = 'description', changed = selecting_changed, width = .., height = ..)
 ```
 
 
 ### Video. ###
 width and height are optional.
@@ -264,15 +267,14 @@
 ```
 
 ### Tree. The element for tree-like data. ###
 ```
 Tree(name, selected_item_name, changed_handler, options = {name1: parent1, name2 : None, .})
 ```
 options is a tree structure, a dictionary {item_name:parent_name}. 
-
 parent_name is None for root items. changed_handler gets item key (name) as value. 
 
 ### Table. ###
 Tables is common structure for presenting 2D data and charts. 
 Optional append, delete, update handlers are called for adding, deleting and updating rows.
 
 
@@ -409,18 +411,12 @@
 ```
 In screens and blocks sources we can access the user by call get_user()
 ```
 user = get_user()
 print(isinstance(user, Hello_user))
 ```
 
-More info about User class methods you can find in manager.py in the root dir.
+More info about User class methods you can find in manager.py in the souce dir.
 
 Examples are in tests folder.
 
-The articles about Unigui and its protocol in details:
-
-in English https://docs.google.com/document/d/1G_9Ejt9ETDoXpTCD3YkR8CW508Idk9BaMlD72tlx8bc/edit?usp=sharing
-
-in Russian https://docs.google.com/document/d/1EleilkEX-m5XOZK5S9WytIGpImAzOhz7kW3EUaeow7Q/edit?usp=sharing
-
```

### Comparing `unigui-1.4.6/README.md` & `unigui-1.4.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -44,20 +44,19 @@
 
 #### Screen function prepare() syncronizes GUI elements one to another and with the program/system data. prepare() is called when the screen open/loaded. prepare() is optional. ###
 
 ### Server start ###
 tests/run_hello.py
 ```
 import unigui
-#app name, port for initial connection and upload_dir folder are optional
+#app name, the others server setting in config.py like port, upload_dir, ..
 unigui.start('Test app') 
 ```
 Unigui builds the interactive app for the code above.
 Connect a browser to localhast:8000 which are by default and will see:
-server port and ip config is in config.py file in the working directory
 
 ![image](https://github.com/Claus1/unigui/assets/1247062/5afcf4ac-b388-4237-98ff-3a92e802d44a)
 
 ### Handling events ###
 All handlers are functions which have a signature
 ```
 def handler_x(gui_object, value_x)
@@ -79,26 +78,28 @@
 | :---: | :---: | 
 | Gui object |  Object to update |
 | Gui object array or tuple |  Objects to update |
 | None | Nothing to update, Ok |
 | Error(...), Warning(...), Info(...) | Show to user info about a problem. |
 | UpdateScreen, True | Redraw whole screen |
 | Dialog(..) | Open a dialog with parameters |
+| user.set_screen(screen_name) | switch to another screen |
+| Signal(signal_name, ..) | causes indirect call screen.dispatch or/and user.dispatch handlers | 
 
 Unigui	synchronizes GUI state on frontend-end automatically after calling a handler.
 
 If a Gui object doesn't have 'changed' handler the object accepts incoming value automatically to the 'value' variable of gui object.
 
 If 'value' is not acceptable instead of returning an object possible to return Error or Warning or Info. That functions can update a object list passed after the message argument.
 
 ```
 def changed_range(_, value):
    if value < 0.5 and value > 1.0:
-       #or Error(message, _) if we want to return the previous visible value to the field
-       return Error(f‘The value of {_.name} has to be > 0.5 and < 1.0!') 
+       #or Error(message, _) if we want to return the previous visible value to the field, return gui object _ also.
+       return Error(f‘The value of {_.name} has to be > 0.5 and < 1.0!', _) 
     #accept value othewise
     _.value = value
 
 edit = Edit('Range of involving', 0.6, changed_range)
 ```
 
 ### Block details ###
@@ -236,14 +237,16 @@
 ```
 Optional type parameter can be 'toggles','list','dropdown'. Unigui automatically chooses between toogles and dropdown, if type is omitted,
 if type = 'list' then Unigui build it as vertical select list.
 
 
 ### Image. ###
 width,changed,height,header are optional, changed is called if the user select or touch the image.
+When the user click the image, a check mark is appearing on the image, showning select status of the image.
+It is usefull for image list, gallery, e.t.c
 ```
 Image(image_url, header = 'description', changed = selecting_changed, width = .., height = ..)
 ```
 
 
 ### Video. ###
 width and height are optional.
@@ -252,15 +255,14 @@
 ```
 
 ### Tree. The element for tree-like data. ###
 ```
 Tree(name, selected_item_name, changed_handler, options = {name1: parent1, name2 : None, .})
 ```
 options is a tree structure, a dictionary {item_name:parent_name}. 
-
 parent_name is None for root items. changed_handler gets item key (name) as value. 
 
 ### Table. ###
 Tables is common structure for presenting 2D data and charts. 
 Optional append, delete, update handlers are called for adding, deleting and updating rows.
 
 
@@ -397,16 +399,10 @@
 ```
 In screens and blocks sources we can access the user by call get_user()
 ```
 user = get_user()
 print(isinstance(user, Hello_user))
 ```
 
-More info about User class methods you can find in manager.py in the root dir.
+More info about User class methods you can find in manager.py in the souce dir.
 
 Examples are in tests folder.
-
-The articles about Unigui and its protocol in details:
-
-in English https://docs.google.com/document/d/1G_9Ejt9ETDoXpTCD3YkR8CW508Idk9BaMlD72tlx8bc/edit?usp=sharing
-
-in Russian https://docs.google.com/document/d/1EleilkEX-m5XOZK5S9WytIGpImAzOhz7kW3EUaeow7Q/edit?usp=sharing
```

### Comparing `unigui-1.4.6/unigui.egg-info/PKG-INFO` & `unigui-1.4.7/unigui.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.4.6
+Version: 1.4.7
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -56,20 +56,19 @@
 
 #### Screen function prepare() syncronizes GUI elements one to another and with the program/system data. prepare() is called when the screen open/loaded. prepare() is optional. ###
 
 ### Server start ###
 tests/run_hello.py
 ```
 import unigui
-#app name, port for initial connection and upload_dir folder are optional
+#app name, the others server setting in config.py like port, upload_dir, ..
 unigui.start('Test app') 
 ```
 Unigui builds the interactive app for the code above.
 Connect a browser to localhast:8000 which are by default and will see:
-server port and ip config is in config.py file in the working directory
 
 ![image](https://github.com/Claus1/unigui/assets/1247062/5afcf4ac-b388-4237-98ff-3a92e802d44a)
 
 ### Handling events ###
 All handlers are functions which have a signature
 ```
 def handler_x(gui_object, value_x)
@@ -91,26 +90,28 @@
 | :---: | :---: | 
 | Gui object |  Object to update |
 | Gui object array or tuple |  Objects to update |
 | None | Nothing to update, Ok |
 | Error(...), Warning(...), Info(...) | Show to user info about a problem. |
 | UpdateScreen, True | Redraw whole screen |
 | Dialog(..) | Open a dialog with parameters |
+| user.set_screen(screen_name) | switch to another screen |
+| Signal(signal_name, ..) | causes indirect call screen.dispatch or/and user.dispatch handlers | 
 
 Unigui	synchronizes GUI state on frontend-end automatically after calling a handler.
 
 If a Gui object doesn't have 'changed' handler the object accepts incoming value automatically to the 'value' variable of gui object.
 
 If 'value' is not acceptable instead of returning an object possible to return Error or Warning or Info. That functions can update a object list passed after the message argument.
 
 ```
 def changed_range(_, value):
    if value < 0.5 and value > 1.0:
-       #or Error(message, _) if we want to return the previous visible value to the field
-       return Error(f‘The value of {_.name} has to be > 0.5 and < 1.0!') 
+       #or Error(message, _) if we want to return the previous visible value to the field, return gui object _ also.
+       return Error(f‘The value of {_.name} has to be > 0.5 and < 1.0!', _) 
     #accept value othewise
     _.value = value
 
 edit = Edit('Range of involving', 0.6, changed_range)
 ```
 
 ### Block details ###
@@ -248,14 +249,16 @@
 ```
 Optional type parameter can be 'toggles','list','dropdown'. Unigui automatically chooses between toogles and dropdown, if type is omitted,
 if type = 'list' then Unigui build it as vertical select list.
 
 
 ### Image. ###
 width,changed,height,header are optional, changed is called if the user select or touch the image.
+When the user click the image, a check mark is appearing on the image, showning select status of the image.
+It is usefull for image list, gallery, e.t.c
 ```
 Image(image_url, header = 'description', changed = selecting_changed, width = .., height = ..)
 ```
 
 
 ### Video. ###
 width and height are optional.
@@ -264,15 +267,14 @@
 ```
 
 ### Tree. The element for tree-like data. ###
 ```
 Tree(name, selected_item_name, changed_handler, options = {name1: parent1, name2 : None, .})
 ```
 options is a tree structure, a dictionary {item_name:parent_name}. 
-
 parent_name is None for root items. changed_handler gets item key (name) as value. 
 
 ### Table. ###
 Tables is common structure for presenting 2D data and charts. 
 Optional append, delete, update handlers are called for adding, deleting and updating rows.
 
 
@@ -409,18 +411,12 @@
 ```
 In screens and blocks sources we can access the user by call get_user()
 ```
 user = get_user()
 print(isinstance(user, Hello_user))
 ```
 
-More info about User class methods you can find in manager.py in the root dir.
+More info about User class methods you can find in manager.py in the souce dir.
 
 Examples are in tests folder.
 
-The articles about Unigui and its protocol in details:
-
-in English https://docs.google.com/document/d/1G_9Ejt9ETDoXpTCD3YkR8CW508Idk9BaMlD72tlx8bc/edit?usp=sharing
-
-in Russian https://docs.google.com/document/d/1EleilkEX-m5XOZK5S9WytIGpImAzOhz7kW3EUaeow7Q/edit?usp=sharing
-
```

### Comparing `unigui-1.4.6/unigui.egg-info/SOURCES.txt` & `unigui-1.4.7/unigui.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/259.f5c7cbc7.css
+unigui/web/css/889.c9159919.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.49a52e8f.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -28,11 +28,11 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.283445be.js
-unigui/web/js/259.1c52f635.js
 unigui/web/js/430.591e9a73.js
-unigui/web/js/app.0d4bddce.js
+unigui/web/js/889.504369e0.js
+unigui/web/js/app.92f553f5.js
 unigui/web/js/vendor.3e8714c2.js
```

