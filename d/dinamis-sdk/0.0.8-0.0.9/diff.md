# Comparing `tmp/dinamis-sdk-0.0.8.tar.gz` & `tmp/dinamis-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dinamis-sdk-0.0.8.tar", last modified: Thu May 11 10:52:38 2023, max compression
+gzip compressed data, was "dinamis-sdk-0.0.9.tar", last modified: Wed May 24 07:21:08 2023, max compression
```

## Comparing `dinamis-sdk-0.0.8.tar` & `dinamis-sdk-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:52:38.651153 dinamis-sdk-0.0.8/
--rw-rw-rw-   0 root         (0) root         (0)    11340 2023-02-22 11:50:47.000000 dinamis-sdk-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      191 2023-05-11 10:52:38.651153 dinamis-sdk-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-03-28 12:19:28.000000 dinamis-sdk-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:52:38.647153 dinamis-sdk-0.0.8/dinamis_sdk/
--rw-rw-rw-   0 root         (0) root         (0)      194 2023-03-28 09:22:01.000000 dinamis-sdk-0.0.8/dinamis_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8267 2023-03-28 09:22:01.000000 dinamis-sdk-0.0.8/dinamis_sdk/auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:52:38.651153 dinamis-sdk-0.0.8/dinamis_sdk/examples/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-03-31 13:55:36.000000 dinamis-sdk-0.0.8/dinamis_sdk/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      920 2023-05-11 10:48:18.000000 dinamis-sdk-0.0.8/dinamis_sdk/examples/pyotb_ndvi_loss.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-05-11 10:48:18.000000 dinamis-sdk-0.0.8/dinamis_sdk/examples/pyotb_toa_mosaic.py
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-03-30 14:16:11.000000 dinamis-sdk-0.0.8/dinamis_sdk/examples/rio_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    16407 2023-05-03 18:09:30.000000 dinamis-sdk-0.0.8/dinamis_sdk/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     1717 2023-05-03 18:03:30.000000 dinamis-sdk-0.0.8/dinamis_sdk/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 10:52:38.647153 dinamis-sdk-0.0.8/dinamis_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      191 2023-05-11 10:52:38.000000 dinamis-sdk-0.0.8/dinamis_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2023-05-11 10:52:38.000000 dinamis-sdk-0.0.8/dinamis_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 10:52:38.000000 dinamis-sdk-0.0.8/dinamis_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 10:52:38.000000 dinamis-sdk-0.0.8/dinamis_sdk.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       54 2023-05-11 10:52:38.000000 dinamis-sdk-0.0.8/dinamis_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-11 10:52:38.000000 dinamis-sdk-0.0.8/dinamis_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 10:52:38.651153 dinamis-sdk-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-05-03 18:03:30.000000 dinamis-sdk-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:21:08.001575 dinamis-sdk-0.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)    11340 2023-02-22 11:50:47.000000 dinamis-sdk-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-24 07:21:08.001575 dinamis-sdk-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-03-28 12:19:28.000000 dinamis-sdk-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:21:07.993574 dinamis-sdk-0.0.9/dinamis_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-03-28 09:22:01.000000 dinamis-sdk-0.0.9/dinamis_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8267 2023-03-28 09:22:01.000000 dinamis-sdk-0.0.9/dinamis_sdk/auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:21:07.997574 dinamis-sdk-0.0.9/dinamis_sdk/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-03-31 13:55:36.000000 dinamis-sdk-0.0.9/dinamis_sdk/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      920 2023-05-11 10:48:18.000000 dinamis-sdk-0.0.9/dinamis_sdk/examples/pyotb_ndvi_loss.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-05-11 10:48:18.000000 dinamis-sdk-0.0.9/dinamis_sdk/examples/pyotb_toa_mosaic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-03-30 14:16:11.000000 dinamis-sdk-0.0.9/dinamis_sdk/examples/rio_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    16374 2023-05-24 07:16:26.000000 dinamis-sdk-0.0.9/dinamis_sdk/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1717 2023-05-03 18:03:30.000000 dinamis-sdk-0.0.9/dinamis_sdk/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:21:07.997574 dinamis-sdk-0.0.9/dinamis_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-24 07:21:07.000000 dinamis-sdk-0.0.9/dinamis_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2023-05-24 07:21:07.000000 dinamis-sdk-0.0.9/dinamis_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:21:07.000000 dinamis-sdk-0.0.9/dinamis_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:21:07.000000 dinamis-sdk-0.0.9/dinamis_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       54 2023-05-24 07:21:07.000000 dinamis-sdk-0.0.9/dinamis_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-24 07:21:07.000000 dinamis-sdk-0.0.9/dinamis_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 07:21:08.001575 dinamis-sdk-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-05-24 07:12:42.000000 dinamis-sdk-0.0.9/setup.py
```

### Comparing `dinamis-sdk-0.0.8/LICENSE` & `dinamis-sdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.0.8/README.md` & `dinamis-sdk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.0.8/dinamis_sdk/auth.py` & `dinamis-sdk-0.0.9/dinamis_sdk/auth.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.0.8/dinamis_sdk/examples/pyotb_ndvi_loss.py` & `dinamis-sdk-0.0.9/dinamis_sdk/examples/pyotb_ndvi_loss.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.0.8/dinamis_sdk/examples/pyotb_toa_mosaic.py` & `dinamis-sdk-0.0.9/dinamis_sdk/examples/pyotb_toa_mosaic.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.0.8/dinamis_sdk/examples/rio_metadata.py` & `dinamis-sdk-0.0.9/dinamis_sdk/examples/rio_metadata.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.0.8/dinamis_sdk/s3.py` & `dinamis-sdk-0.0.9/dinamis_sdk/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,19 +222,18 @@
         been replaced with a signed version. In addition, an "expiry"
         property is added to the Item properties indicating the earliest
         expiry time for any assets that were signed.
 
     """
     if copy:
         item = item.clone()
-    urls = {key: asset.href for key, asset in item.assets.items()}
+    urls = [asset.href for asset in item.assets.values()]
     signed_urls = sign_urls(urls=urls)
-    for key in item.assets:
-        url = urls[key]
-        item.assets[key] = signed_urls[url]
+    for key, asset in item.assets.items():
+        item.assets[key].href = signed_urls[asset.href]
     return item
 
 
 @sign.register(Asset)
 def sign_asset(asset: Asset, copy: bool = True) -> Asset:
     """Sign a PySTAC asset.
 
@@ -270,24 +269,23 @@
         HREFs for each item have been replaced with a signed version. In
         addition, an "expiry" property is added to the Item properties
         indicating the earliest expiry time for any assets that were signed.
 
     """
     if copy:
         item_collection = item_collection.clone()
-    urls = {
-        key: asset.href
+    urls = [
+        asset.href
         for item in item_collection
-        for key, asset in item.assets.items()
-    }
+        for asset in item.values()
+    ]
     signed_urls = sign_urls(urls=urls)
     for item in item_collection:
-        for key in item.assets:
-            url = item.assets[key]
-            item.assets[key].href = signed_urls[url]
+        for key, asset in item.assets.items():
+            item.assets[key].href = signed_urls[asset.href]
     return item_collection
 
 
 @sign.register(ItemSearch)
 def _search_and_sign(search: ItemSearch, copy: bool = True) -> ItemCollection:
     """Perform a PySTAC Client search, and sign the resulting item collection.
 
@@ -327,19 +325,21 @@
     if copy:
         # https://github.com/stac-utils/pystac/pull/834 fixed asset dropping
         assets = collection.assets
         collection = collection.clone()
         if assets and not collection.assets:
             collection.assets = deepcopy(assets)
 
-    urls = [collection.assets[key].href for key in collection.assets]
+    urls = [
+        collection.assets[key].href
+        for key in collection.assets
+    ]
     signed_urls = sign_urls(urls=urls)
-    for key in collection.assets:
-        url = collection.assets[key].href
-        collection.assets[key].href = signed_urls[url]
+    for key, asset in collection.assets.items():
+        collection.assets[key].href = signed_urls[asset.href]
     return collection
 
 
 @sign.register(collections.abc.Mapping)
 def sign_mapping(mapping: Mapping, copy: bool = True) -> Mapping:
     """
     Sign a mapping.
```

### Comparing `dinamis-sdk-0.0.8/dinamis_sdk/utils.py` & `dinamis-sdk-0.0.9/dinamis_sdk/utils.py`

 * *Files identical despite different names*

