# Comparing `tmp/openedx-ledger-0.4.0.tar.gz` & `tmp/openedx-ledger-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-ledger-0.4.0.tar", last modified: Wed May 17 18:07:20 2023, max compression
+gzip compressed data, was "openedx-ledger-0.4.1.tar", last modified: Wed May 24 15:52:21 2023, max compression
```

## Comparing `openedx-ledger-0.4.0.tar` & `openedx-ledger-0.4.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 18:07:20.899044 openedx-ledger-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8581 2023-05-17 18:07:20.899044 openedx-ledger-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 18:07:20.887044 openedx-ledger-0.4.0/openedx_ledger/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3884 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5326 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 18:07:20.895044 openedx-ledger-0.4.0/openedx_ledger/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     6005 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py
--rw-r--r--   0 runner    (1001) docker     (122)     4294 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/migrations/0003_field_updates_20230216_1605.py
--rw-r--r--   0 runner    (1001) docker     (122)      638 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py
--rw-r--r--   0 runner    (1001) docker     (122)    12708 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/migrations/0005_help_text_and_more_indices.py
--rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/migrations/0006_auto_20230404_1744.py
--rw-r--r--   0 runner    (1001) docker     (122)      468 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/migrations/0007_alter_externalfulfillmentprovider_name.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15756 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 18:07:20.895044 openedx-ledger-0.4.0/openedx_ledger/signals/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      246 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/signals/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 18:07:20.883043 openedx-ledger-0.4.0/openedx_ledger/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 18:07:20.895044 openedx-ledger-0.4.0/openedx_ledger/templates/edx_ledger/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 18:07:20.895044 openedx-ledger-0.4.0/openedx_ledger/templates/edx_ledger/admin/
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/templates/edx_ledger/base.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 18:07:20.899044 openedx-ledger-0.4.0/openedx_ledger/test_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/test_utils/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/openedx_ledger/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 18:07:20.891044 openedx-ledger-0.4.0/openedx_ledger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8581 2023-05-17 18:07:20.000000 openedx-ledger-0.4.0/openedx_ledger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-05-17 18:07:20.000000 openedx-ledger-0.4.0/openedx_ledger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 18:07:20.000000 openedx-ledger-0.4.0/openedx_ledger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 18:07:20.000000 openedx-ledger-0.4.0/openedx_ledger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      197 2023-05-17 18:07:20.000000 openedx-ledger-0.4.0/openedx_ledger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-17 18:07:20.000000 openedx-ledger-0.4.0/openedx_ledger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 18:07:20.899044 openedx-ledger-0.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-17 18:07:20.899044 openedx-ledger-0.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5100 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 18:07:20.899044 openedx-ledger-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2209 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     7880 2023-05-17 18:07:15.000000 openedx-ledger-0.4.0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.979185 openedx-ledger-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8581 2023-05-24 15:52:21.979185 openedx-ledger-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.975185 openedx-ledger-0.4.1/openedx_ledger/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3884 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5394 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.975185 openedx-ledger-0.4.1/openedx_ledger/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6005 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4294 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/migrations/0003_field_updates_20230216_1605.py
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12708 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/migrations/0005_help_text_and_more_indices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/migrations/0006_auto_20230404_1744.py
+-rw-r--r--   0 runner    (1001) docker     (122)      468 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/migrations/0007_alter_externalfulfillmentprovider_name.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15825 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.975185 openedx-ledger-0.4.1/openedx_ledger/signals/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/signals/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.971185 openedx-ledger-0.4.1/openedx_ledger/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.975185 openedx-ledger-0.4.1/openedx_ledger/templates/edx_ledger/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.979185 openedx-ledger-0.4.1/openedx_ledger/templates/edx_ledger/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/templates/edx_ledger/base.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.979185 openedx-ledger-0.4.1/openedx_ledger/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/test_utils/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/openedx_ledger/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.975185 openedx-ledger-0.4.1/openedx_ledger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8581 2023-05-24 15:52:21.000000 openedx-ledger-0.4.1/openedx_ledger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-05-24 15:52:21.000000 openedx-ledger-0.4.1/openedx_ledger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 15:52:21.000000 openedx-ledger-0.4.1/openedx_ledger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 15:52:21.000000 openedx-ledger-0.4.1/openedx_ledger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-05-24 15:52:21.000000 openedx-ledger-0.4.1/openedx_ledger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-24 15:52:21.000000 openedx-ledger-0.4.1/openedx_ledger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.979185 openedx-ledger-0.4.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-24 15:52:21.979185 openedx-ledger-0.4.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5100 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:52:21.979185 openedx-ledger-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7504 2023-05-24 15:52:17.000000 openedx-ledger-0.4.1/tests/test_models.py
```

### Comparing `openedx-ledger-0.4.0/CHANGELOG.rst` & `openedx-ledger-0.4.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.0/LICENSE.txt` & `openedx-ledger-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.0/PKG-INFO` & `openedx-ledger-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-ledger
-Version: 0.4.0
+Version: 0.4.1
 Summary: Records transactions against a ledger, denominated in units of value.
 Home-page: https://github.com/openedx/openedx-ledger
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `openedx-ledger-0.4.0/README.rst` & `openedx-ledger-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.0/openedx_ledger/admin.py` & `openedx-ledger-0.4.1/openedx_ledger/admin.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.0/openedx_ledger/api.py` & `openedx-ledger-0.4.1/openedx_ledger/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     lms_user_id=None,
     content_key=None,
     subsidy_access_policy_uuid=None,
     state=models.TransactionStateChoices.CREATED,
     **metadata
 ):
     """
-    Create a transaction.
+    Create a pending transaction.
 
     Args:
         ledger (openedx_ledger.models.Ledger): The ledger to which the transaction should be added.
         quantity (int): Negative value representing the desired quantity of the new Transaction.
         idempotency_key (str): The idempotency_key of the new Transaction.
         lms_user_id (int, Optional):
             The lms_user_id representing the learner who is enrolling. Skip if this does not represent a policy
@@ -89,14 +89,15 @@
         reversal, _ = models.Reversal.objects.get_or_create(
             transaction=transaction,
             idempotency_key=idempotency_key,
             defaults={
                 'quantity': transaction.quantity * -1,
                 'metadata': metadata,
             },
+            state=models.TransactionStateChoices.COMMITTED,
         )
         TRANSACTION_REVERSED.send(sender=models.Reversal, reversal=reversal)
         return reversal
 
 
 def create_ledger(unit=None, idempotency_key=None, subsidy_uuid=None, initial_deposit=None, **metadata):
     """
```

### Comparing `openedx-ledger-0.4.0/openedx_ledger/migrations/0001_initial.py` & `openedx-ledger-0.4.1/openedx_ledger/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.0/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py` & `openedx-ledger-0.4.1/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.0/openedx_ledger/migrations/0003_field_updates_20230216_1605.py` & `openedx-ledger-0.4.1/openedx_ledger/migrations/0003_field_updates_20230216_1605.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.0/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py` & `openedx-ledger-0.4.1/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.0/openedx_ledger/migrations/0005_help_text_and_more_indices.py` & `openedx-ledger-0.4.1/openedx_ledger/migrations/0005_help_text_and_more_indices.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.0/openedx_ledger/migrations/0006_auto_20230404_1744.py` & `openedx-ledger-0.4.1/openedx_ledger/migrations/0006_auto_20230404_1744.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.0/openedx_ledger/models.py` & `openedx-ledger-0.4.1/openedx_ledger/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,16 @@
             agg = agg.aggregate(total_quantity=Coalesce(models.Sum('row_total'), 0))
             return agg['total_quantity']
 
     def balance(self, committed_only=False):
         """
         Calculate the current balance of the ledger.
 
+        TODO: propagate committed_only down into the reversals too.
+
         Args:
             committed_only (boolean): If true, computes balance only for `committed` transations.  Defaults to False.
 
         Returns:
             int: The total balance of non-failed transactions in this ledger.
         """
         if committed_only:
```

### Comparing `openedx-ledger-0.4.0/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html` & `openedx-ledger-0.4.1/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.0/openedx_ledger/templates/edx_ledger/base.html` & `openedx-ledger-0.4.1/openedx_ledger/templates/edx_ledger/base.html`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.0/openedx_ledger/test_utils/factories.py` & `openedx-ledger-0.4.1/openedx_ledger/test_utils/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     Test factory for the `Transaction` model.
     """
     class Meta:
         model = Transaction
 
     uuid = factory.LazyFunction(uuid4)
     idempotency_key = factory.LazyFunction(uuid4)
-    state = TransactionStateChoices.CREATED
+    state = TransactionStateChoices.COMMITTED
     quantity = factory.Faker("random_int", min=-100000, max=-100)
     ledger = factory.Iterator(Ledger.objects.all())
     lms_user_id = factory.Faker("random_int", min=1, max=1000)
 
 
 class ExternalFulfillmentProviderFactory(factory.django.DjangoModelFactory):
     """
@@ -74,9 +74,9 @@
     """
     class Meta:
         model = Reversal
 
     uuid = factory.LazyFunction(uuid4)
     transaction = factory.Iterator(Transaction.objects.all())
     idempotency_key = factory.LazyFunction(uuid4)
-    state = TransactionStateChoices.CREATED
+    state = TransactionStateChoices.COMMITTED
     quantity = factory.Faker("random_int", min=100, max=10000)
```

### Comparing `openedx-ledger-0.4.0/openedx_ledger/utils.py` & `openedx-ledger-0.4.1/openedx_ledger/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.0/openedx_ledger/views.py` & `openedx-ledger-0.4.1/openedx_ledger/views.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.0/openedx_ledger.egg-info/PKG-INFO` & `openedx-ledger-0.4.1/openedx_ledger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-ledger
-Version: 0.4.0
+Version: 0.4.1
 Summary: Records transactions against a ledger, denominated in units of value.
 Home-page: https://github.com/openedx/openedx-ledger
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `openedx-ledger-0.4.0/openedx_ledger.egg-info/SOURCES.txt` & `openedx-ledger-0.4.1/openedx_ledger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.0/requirements/constraints.txt` & `openedx-ledger-0.4.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.0/setup.py` & `openedx-ledger-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.4.0/tests/test_api.py` & `openedx-ledger-0.4.1/tests/test_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 Tests for the openedx_ledger Python API.
 """
 import pytest
 
 from openedx_ledger import api
-from openedx_ledger.models import UnitChoices
+from openedx_ledger.models import TransactionStateChoices, UnitChoices
 
 
 @pytest.mark.django_db
 def test_create_ledger_happy_path():
     ledger = api.create_ledger(unit=UnitChoices.USD_CENTS, idempotency_key='my-happy-ledger')
     assert ledger.balance() == 0
 
-    api.create_transaction(ledger, quantity=5000, idempotency_key='tx-1')
+    api.create_transaction(ledger, quantity=5000, idempotency_key='tx-1', state=TransactionStateChoices.CREATED)
     assert ledger.balance() == 5000
 
-    tx_2 = api.create_transaction(ledger, quantity=5000, idempotency_key='tx-2')
+    tx_2 = api.create_transaction(ledger, quantity=5000, idempotency_key='tx-2', state=TransactionStateChoices.CREATED)
     assert ledger.balance() == 10000
 
     api.reverse_full_transaction(tx_2, idempotency_key='reversal-1')
     assert ledger.balance() == 5000
 
     other_ledger = api.create_ledger(unit=UnitChoices.USD_CENTS, idempotency_key='my-happy-ledger')
     assert ledger == other_ledger
@@ -30,30 +30,30 @@
     ledger = api.create_ledger(unit=UnitChoices.USD_CENTS, idempotency_key='my-other-ledger')
     assert ledger.balance() == 0
 
     with pytest.raises(
         api.LedgerBalanceExceeded,
         match="A Transaction was not created because it would exceed the ledger balance."
     ):
-        api.create_transaction(ledger, quantity=-1, idempotency_key='tx-1')
+        api.create_transaction(ledger, quantity=-1, idempotency_key='tx-1', state=TransactionStateChoices.CREATED)
 
-    api.create_transaction(ledger, quantity=999, idempotency_key='tx-2')
+    api.create_transaction(ledger, quantity=999, idempotency_key='tx-2', state=TransactionStateChoices.CREATED)
     with pytest.raises(
         api.LedgerBalanceExceeded,
         match="A Transaction was not created because it would exceed the ledger balance."
     ):
-        api.create_transaction(ledger, quantity=-1000, idempotency_key='tx-3')
+        api.create_transaction(ledger, quantity=-1000, idempotency_key='tx-3', state=TransactionStateChoices.CREATED)
 
 
 @pytest.mark.django_db
 def test_multiple_reversals():
     ledger = api.create_ledger(unit=UnitChoices.USD_CENTS, idempotency_key='my-other-ledger')
     assert ledger.balance() == 0
 
-    tx_1 = api.create_transaction(ledger, quantity=5000, idempotency_key='tx-1')
+    tx_1 = api.create_transaction(ledger, quantity=5000, idempotency_key='tx-1', state=TransactionStateChoices.CREATED)
     assert ledger.balance() == 5000
 
     reversal = api.reverse_full_transaction(tx_1, idempotency_key='reversal-1')
     assert ledger.balance() == 0
 
     with pytest.raises(Exception):
         api.reverse_full_transaction(tx_1, idempotency_key='reversal-2')
```

### Comparing `openedx-ledger-0.4.0/tests/test_models.py` & `openedx-ledger-0.4.1/tests/test_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,42 +20,59 @@
 
     def setUp(self):
         super().setUp()
         self.ledger = LedgerFactory()
         self.initial_transaction = TransactionFactory(
             ledger=self.ledger,
             quantity=100,
-            state=models.TransactionStateChoices.COMMITTED,
         )
         self.transaction_2 = TransactionFactory(
             ledger=self.ledger, lms_user_id=1, content_key="course-v1:edX+test+course.1", quantity=-10
         )
         self.transaction_3 = TransactionFactory(
             ledger=self.ledger, lms_user_id=1, content_key="course-v1:edX+test+course.2", quantity=-10
         )
         self.transaction_4 = TransactionFactory(
             ledger=self.ledger, lms_user_id=2, content_key="course-v1:edX+test+course.2", quantity=-10
         )
         self.reversal_1 = ReversalFactory(
             transaction=self.transaction_4,
             quantity=10,
         )
+        self.transaction_5 = TransactionFactory(
+            ledger=self.ledger,
+            lms_user_id=3,
+            content_key="course-v1:edX+test+course.3",
+            quantity=-10,
+            state=models.TransactionStateChoices.PENDING,
+        )
 
     def test_balance(self):
         """
-        Test Ledger.balance().
+        Test ``Ledger.balance()``.
+
+        ``committed_only`` is implicitly False.
         """
         result = self.ledger.balance()
+        assert result == 100 - 10 - 10 - 10 + 10 - 10
+
+    def test_balance_committed_only(self):
+        """
+        Test ``Ledger.balance(committed_only=True)``.
+
+        One of the setUp transactions is still pending.
+        """
+        result = self.ledger.balance(committed_only=True)
         assert result == 100 - 10 - 10 - 10 + 10
 
     @ddt.data(
         # Test calculating the balance of the entire ledger.
         {
             "transaction_filters": {},
-            "expected_balance": 100 - 10 - 10 - 10 + 10,
+            "expected_balance": 100 - 10 - 10 - 10 + 10 - 10,
         },
         # Test calculating the balance of a user subset.
         {
             "transaction_filters": {"lms_user_id": 1},
             "expected_balance": -10 - 10,
         },
         # Test calculating the balance of a user subset, reversal case.
@@ -93,37 +110,18 @@
         _ = TransactionFactory(
             ledger=self.ledger,
             lms_user_id=2,
             content_key="course-v1:edX+test+course.2",
             quantity=-55,
             state=models.TransactionStateChoices.FAILED,
         )
-        expected_balance = 100 - 10 - 10 - 10 + 10
+        expected_balance = 100 - 10 - 10 - 10 + 10 - 10
 
         self.assertEqual(self.ledger.balance(), expected_balance)
 
-    def test_balance_committed_only(self):
-        """
-        When balance() specifies `committed_only=True`, only committed transactions
-        should be included in the balance calculation.
-        """
-        # all the non-initial transactions from setUp() are only in the `created` state
-        self.assertEqual(self.ledger.balance(committed_only=True), self.initial_transaction.quantity)
-
-        committed_transaction = TransactionFactory(
-            ledger=self.ledger,
-            lms_user_id=2,
-            content_key="course-v1:edX+test+course.2",
-            quantity=-31,
-            state=models.TransactionStateChoices.COMMITTED,
-        )
-
-        expected_committed_balance = self.initial_transaction.quantity + committed_transaction.quantity
-        self.assertEqual(self.ledger.balance(committed_only=True), expected_committed_balance)
-
     def test_idempotency_key_is_generated(self):
         """
         Tests that Ledger.save() will create an idempotency_key
         if none exists.
         """
         my_ledger = LedgerFactory(idempotency_key=None)
         my_ledger.save()
@@ -195,29 +193,28 @@
             name='My provider',
             slug='my-provider',
         )
         cls.ledger = LedgerFactory()
         cls.initial_transaction = TransactionFactory(
             ledger=cls.ledger,
             quantity=100,
-            state=models.TransactionStateChoices.COMMITTED,
         )
 
     def test_simple_provider_stuff(self):
         """
         Test we can str() these.
         """
         self.assertIn('my-provider', str(self.provider))
         self.assertIn('My provider', str(self.provider))
 
     def test_external_reference(self):
         """
         Test that we can create an external transaction reference.
         """
-        transaction = TransactionFactory.create(
+        transaction = TransactionFactory(
             ledger=self.ledger,
         )
         external_id = str(uuid.uuid4())
         external_reference = models.ExternalTransactionReference.objects.create(
             transaction=transaction,
             external_fulfillment_provider=self.provider,
             external_reference_id=external_id,
```

