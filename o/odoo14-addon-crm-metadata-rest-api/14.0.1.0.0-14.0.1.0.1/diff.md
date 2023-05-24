# Comparing `tmp/odoo14_addon_crm_metadata_rest_api-14.0.1.0.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_crm_metadata_rest_api-14.0.1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 3751 bytes, number of entries: 10
--rwxr-xr-x  2.0 unx      146 b- defN 23-May-03 12:41 odoo/addons/crm_metadata_rest_api/README.rst
--rwxr-xr-x  2.0 unx       23 b- defN 23-May-03 12:41 odoo/addons/crm_metadata_rest_api/__init__.py
--rwxr-xr-x  2.0 unx      484 b- defN 23-May-03 13:35 odoo/addons/crm_metadata_rest_api/__manifest__.py
--rwxr-xr-x  2.0 unx       32 b- defN 23-May-03 12:41 odoo/addons/crm_metadata_rest_api/services/__init__.py
--rwxr-xr-x  2.0 unx      911 b- defN 23-May-03 12:41 odoo/addons/crm_metadata_rest_api/services/crm_lead_services.py
--rwxr-xr-x  2.0 unx      314 b- defN 23-May-03 12:41 odoo/addons/crm_metadata_rest_api/services/schemas.py
--rw-r--r--  2.0 unx      616 b- defN 23-May-03 14:11 odoo14_addon_crm_metadata_rest_api-14.0.1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-03 14:11 odoo14_addon_crm_metadata_rest_api-14.0.1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-May-03 14:11 odoo14_addon_crm_metadata_rest_api-14.0.1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1066 b- defN 23-May-03 14:11 odoo14_addon_crm_metadata_rest_api-14.0.1.0.0.dist-info/RECORD
-10 files, 3689 bytes uncompressed, 1841 bytes compressed:  50.1%
+Zip file size: 3733 bytes, number of entries: 10
+-rwxr-xr-x  2.0 unx      146 b- defN 23-May-24 15:12 odoo/addons/crm_metadata_rest_api/README.rst
+-rwxr-xr-x  2.0 unx       23 b- defN 23-May-24 15:12 odoo/addons/crm_metadata_rest_api/__init__.py
+-rwxr-xr-x  2.0 unx      484 b- defN 23-May-24 15:13 odoo/addons/crm_metadata_rest_api/__manifest__.py
+-rwxr-xr-x  2.0 unx       32 b- defN 23-May-24 15:12 odoo/addons/crm_metadata_rest_api/services/__init__.py
+-rwxr-xr-x  2.0 unx      951 b- defN 23-May-24 15:13 odoo/addons/crm_metadata_rest_api/services/crm_lead_services.py
+-rwxr-xr-x  2.0 unx      314 b- defN 23-May-24 15:12 odoo/addons/crm_metadata_rest_api/services/schemas.py
+-rw-r--r--  2.0 unx      572 b- defN 23-May-24 15:17 odoo14_addon_crm_metadata_rest_api-14.0.1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-24 15:17 odoo14_addon_crm_metadata_rest_api-14.0.1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-May-24 15:17 odoo14_addon_crm_metadata_rest_api-14.0.1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1066 b- defN 23-May-24 15:17 odoo14_addon_crm_metadata_rest_api-14.0.1.0.1.dist-info/RECORD
+10 files, 3685 bytes uncompressed, 1823 bytes compressed:  50.5%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: odoo/addons/crm_metadata_rest_api/services/crm_lead_services.py
 Comment: 
 
 Filename: odoo/addons/crm_metadata_rest_api/services/schemas.py
 Comment: 
 
-Filename: odoo14_addon_crm_metadata_rest_api-14.0.1.0.0.dist-info/METADATA
+Filename: odoo14_addon_crm_metadata_rest_api-14.0.1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_crm_metadata_rest_api-14.0.1.0.0.dist-info/WHEEL
+Filename: odoo14_addon_crm_metadata_rest_api-14.0.1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_crm_metadata_rest_api-14.0.1.0.0.dist-info/top_level.txt
+Filename: odoo14_addon_crm_metadata_rest_api-14.0.1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_crm_metadata_rest_api-14.0.1.0.0.dist-info/RECORD
+Filename: odoo14_addon_crm_metadata_rest_api-14.0.1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/crm_metadata_rest_api/__manifest__.py

```diff
@@ -5,15 +5,15 @@
     'summary': """
         Expose CRM Metadata on the Rest API""",
 
     'author': "Coopdevs Treball SCCL",
     'website': "",
 
     'category': 'api',
-    'version': '14.0.1.0.0',
+    'version': '14.0.1.0.1',
 
     # any module necessary for this one to work correctly
     'depends': [
         'base',
         'crm_metadata',
         'crm_rest_api'
     ],
```

## odoo/addons/crm_metadata_rest_api/services/crm_lead_services.py

```diff
@@ -19,8 +19,9 @@
                 line
                 for line in form_metadatas
             ]
             crm_metadata_lines = self.env["crm.lead.metadata.line"].create(
                 crm_metadata_lines_args)
             create_dict['metadata_line_ids'] = [
                 (6, 0, [line.id for line in crm_metadata_lines])]
+            create_dict.pop('metadata')
         return create_dict
```

## Comparing `odoo14_addon_crm_metadata_rest_api-14.0.1.0.0.dist-info/METADATA` & `odoo14_addon_crm_metadata_rest_api-14.0.1.0.1.dist-info/METADATA`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-crm-metadata-rest-api
-Version: 14.0.1.0.0
+Version: 14.0.1.0.1
 Summary: Expose CRM Metadata on the Rest API
-Home-page: UNKNOWN
+Home-page: 
 Author: Coopdevs Treball SCCL
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
 Requires-Python: >=3.6
 Requires-Dist: odoo14-addon-crm-metadata
 Requires-Dist: odoo14-addon-crm-rest-api
 Requires-Dist: odoo (<14.1dev,>=14.0a)
 
 ========================
 CRM metadata rest api
 ========================
 
 Expose relationship between crm lead and it's metadatada on the rest api
-
-
```

## Comparing `odoo14_addon_crm_metadata_rest_api-14.0.1.0.0.dist-info/RECORD` & `odoo14_addon_crm_metadata_rest_api-14.0.1.0.1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 odoo/addons/crm_metadata_rest_api/README.rst,sha256=DvbD63tEN89Nk3TUJBQVhpPF5cL1CMXdJT5kbvLfOWg,146
 odoo/addons/crm_metadata_rest_api/__init__.py,sha256=qksdRxAxHhEXpY0NZlTEolhxFILjRI5o7J0O4UrAE04,23
-odoo/addons/crm_metadata_rest_api/__manifest__.py,sha256=JRCizWI8lW8cWyNCGmZL_Tss2kUkZtbvP2AWaEGLZzQ,484
+odoo/addons/crm_metadata_rest_api/__manifest__.py,sha256=dOQAEA8gNR9cepT14R1jSNq6hlYxpJMfsMBqAW_uTkw,484
 odoo/addons/crm_metadata_rest_api/services/__init__.py,sha256=gyXaE_NlVgF1KawzsiRb0DeYYTT13kmL4Ya1LgcRg5c,32
-odoo/addons/crm_metadata_rest_api/services/crm_lead_services.py,sha256=faCwYuAG0Byu3ef1aonpYjhaXdWBlQhNFLsvwEO29gw,911
+odoo/addons/crm_metadata_rest_api/services/crm_lead_services.py,sha256=nwGWouvj1sETHhGJatsvizkO7QUdfPIH_i7OHlShP9o,951
 odoo/addons/crm_metadata_rest_api/services/schemas.py,sha256=9VEyt5XaHTZk6z1CnaKwXHKaVTWN8047TvlIDZtWE4k,314
-odoo14_addon_crm_metadata_rest_api-14.0.1.0.0.dist-info/METADATA,sha256=6c6Ne-mIDpchhNWTkMstM_BfSvyTEmMYXnCyAd_uQrg,616
-odoo14_addon_crm_metadata_rest_api-14.0.1.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-odoo14_addon_crm_metadata_rest_api-14.0.1.0.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_crm_metadata_rest_api-14.0.1.0.0.dist-info/RECORD,,
+odoo14_addon_crm_metadata_rest_api-14.0.1.0.1.dist-info/METADATA,sha256=ndCSYcKZj3b0HVMQ9vK_il7cb0dC_3QCBUhYK94JMV4,572
+odoo14_addon_crm_metadata_rest_api-14.0.1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+odoo14_addon_crm_metadata_rest_api-14.0.1.0.1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_crm_metadata_rest_api-14.0.1.0.1.dist-info/RECORD,,
```

