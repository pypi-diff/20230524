# Comparing `tmp/odoo14_addon_crm_rest_api-14.0.1.0.1-py3-none-any.whl.zip` & `tmp/odoo14_addon_crm_rest_api-14.0.1.0.1.dev1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 3586 bytes, number of entries: 10
--rw-r--r--  2.0 unx       96 b- defN 23-May-24 15:12 odoo/addons/crm_rest_api/README.rst
--rw-r--r--  2.0 unx       23 b- defN 23-May-24 15:12 odoo/addons/crm_rest_api/__init__.py
--rw-r--r--  2.0 unx      516 b- defN 23-May-24 15:14 odoo/addons/crm_rest_api/__manifest__.py
--rw-r--r--  2.0 unx       32 b- defN 23-May-24 15:12 odoo/addons/crm_rest_api/services/__init__.py
--rw-r--r--  2.0 unx      995 b- defN 23-May-24 15:13 odoo/addons/crm_rest_api/services/crm_lead_services.py
--rw-r--r--  2.0 unx      235 b- defN 23-May-24 15:13 odoo/addons/crm_rest_api/services/schemas.py
--rw-r--r--  2.0 unx      556 b- defN 23-May-24 15:17 odoo14_addon_crm_rest_api-14.0.1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-24 15:17 odoo14_addon_crm_rest_api-14.0.1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-May-24 15:17 odoo14_addon_crm_rest_api-14.0.1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      975 b- defN 23-May-24 15:17 odoo14_addon_crm_rest_api-14.0.1.0.1.dist-info/RECORD
-10 files, 3525 bytes uncompressed, 1856 bytes compressed:  47.3%
+Zip file size: 3637 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       96 b- defN 23-May-03 12:41 odoo/addons/crm_rest_api/README.rst
+-rw-r--r--  2.0 unx       23 b- defN 23-May-03 12:41 odoo/addons/crm_rest_api/__init__.py
+-rw-r--r--  2.0 unx      516 b- defN 23-May-03 13:36 odoo/addons/crm_rest_api/__manifest__.py
+-rw-r--r--  2.0 unx       32 b- defN 23-May-03 12:41 odoo/addons/crm_rest_api/services/__init__.py
+-rw-r--r--  2.0 unx      952 b- defN 23-May-03 12:41 odoo/addons/crm_rest_api/services/crm_lead_services.py
+-rw-r--r--  2.0 unx      235 b- defN 23-May-08 14:04 odoo/addons/crm_rest_api/services/schemas.py
+-rw-r--r--  2.0 unx      605 b- defN 23-May-08 14:10 odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-08 14:10 odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-May-08 14:10 odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      995 b- defN 23-May-08 14:10 odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/RECORD
+10 files, 3551 bytes uncompressed, 1867 bytes compressed:  47.4%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: odoo/addons/crm_rest_api/services/crm_lead_services.py
 Comment: 
 
 Filename: odoo/addons/crm_rest_api/services/schemas.py
 Comment: 
 
-Filename: odoo14_addon_crm_rest_api-14.0.1.0.1.dist-info/METADATA
+Filename: odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_crm_rest_api-14.0.1.0.1.dist-info/WHEEL
+Filename: odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_crm_rest_api-14.0.1.0.1.dist-info/top_level.txt
+Filename: odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_crm_rest_api-14.0.1.0.1.dist-info/RECORD
+Filename: odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/crm_rest_api/__manifest__.py

```diff
@@ -5,15 +5,15 @@
     'summary': """
         Expose CRM Lead on the Rest API""",
 
     'author': "Coopdevs Treball SCCL",
     'website': "",
 
     'category': 'api',
-    'version': '14.0.1.0.1',
+    'version': '14.0.1.0.0',
 
     # any module necessary for this one to work correctly
     'depends': [
         'base',
         'base_rest',
         'base_rest_base_structure',
         'crm',
```

## odoo/addons/crm_rest_api/services/crm_lead_services.py

```diff
@@ -25,13 +25,11 @@
             content_type="application/json"
         )
 
     def _validator_create(self):
         return schemas.S_CRM_LEAD_CREATE
 
     def _prepare_create(self, params):
-        create_dict = {
-            'type': 'opportunity'
-        }
+        create_dict = {}
         for key in params:
             create_dict[key] = params[key]
         return create_dict
```

## Comparing `odoo14_addon_crm_rest_api-14.0.1.0.1.dist-info/METADATA` & `odoo14_addon_crm_rest_api-14.0.1.0.1.dev1.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-crm-rest-api
-Version: 14.0.1.0.1
+Version: 14.0.1.0.1.dev1
 Summary: Expose CRM Lead on the Rest API
-Home-page: 
+Home-page: UNKNOWN
 Author: Coopdevs Treball SCCL
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
 Requires-Python: >=3.6
 Requires-Dist: odoo14-addon-base-rest
 Requires-Dist: odoo14-addon-base-rest-base-structure
 Requires-Dist: odoo14-addon-component
 Requires-Dist: odoo (<14.1dev,>=14.0a)
 
 ========================
 CRM rest api
 ========================
 
 Expose crm lead on the rest api
+
+
```

