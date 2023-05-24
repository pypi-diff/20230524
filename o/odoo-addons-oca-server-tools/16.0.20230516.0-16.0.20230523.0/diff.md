# Comparing `tmp/odoo_addons_oca_server_tools-16.0.20230516.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_server_tools-16.0.20230523.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1618 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1815 b- defN 23-May-17 07:09 odoo_addons_oca_server_tools-16.0.20230516.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-17 07:09 odoo_addons_oca_server_tools-16.0.20230516.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-17 07:09 odoo_addons_oca_server_tools-16.0.20230516.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      421 b- defN 23-May-17 07:09 odoo_addons_oca_server_tools-16.0.20230516.0.dist-info/RECORD
-4 files, 2329 bytes uncompressed, 788 bytes compressed:  66.2%
+Zip file size: 1625 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1879 b- defN 23-May-24 05:04 odoo_addons_oca_server_tools-16.0.20230523.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-24 05:04 odoo_addons_oca_server_tools-16.0.20230523.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-24 05:04 odoo_addons_oca_server_tools-16.0.20230523.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      421 b- defN 23-May-24 05:04 odoo_addons_oca_server_tools-16.0.20230523.0.dist-info/RECORD
+4 files, 2393 bytes uncompressed, 795 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_server_tools-16.0.20230516.0.dist-info/METADATA
+Filename: odoo_addons_oca_server_tools-16.0.20230523.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_server_tools-16.0.20230516.0.dist-info/WHEEL
+Filename: odoo_addons_oca_server_tools-16.0.20230523.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_server_tools-16.0.20230516.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_server_tools-16.0.20230523.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_server_tools-16.0.20230516.0.dist-info/RECORD
+Filename: odoo_addons_oca_server_tools-16.0.20230523.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_server_tools-16.0.20230516.0.dist-info/METADATA` & `odoo_addons_oca_server_tools-16.0.20230523.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-server-tools
-Version: 16.0.20230516.0
+Version: 16.0.20230523.0
 Summary: Meta package for oca-server-tools Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
+Requires-Dist: odoo-addon-attachment-queue (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-attachment-unindex-content (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-auditlog (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-cron-exclusion (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-exception (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-fontawesome (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-m2m-custom-field (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-search-fuzzy (<16.1dev,>=16.0dev)
```

