# Comparing `tmp/edc_notification-0.3.8-py3-none-any.whl.zip` & `tmp/edc_notification-0.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,14 @@
-Zip file size: 44250 bytes, number of entries: 45
+Zip file size: 44824 bytes, number of entries: 47
 -rw-r--r--  2.0 unx      318 b- defN 21-Feb-08 16:20 edc_notification/__init__.py
 -rw-r--r--  2.0 unx      360 b- defN 21-Feb-08 16:20 edc_notification/admin.py
 -rw-r--r--  2.0 unx      177 b- defN 21-May-14 21:40 edc_notification/admin_site.py
 -rw-r--r--  2.0 unx     1162 b- defN 21-Feb-08 16:20 edc_notification/apps.py
+-rw-r--r--  2.0 unx      217 b- defN 21-Sep-09 00:28 edc_notification/auth_objects.py
+-rw-r--r--  2.0 unx      272 b- defN 21-Sep-09 00:28 edc_notification/auths.py
 -rw-r--r--  2.0 unx       39 b- defN 21-Apr-11 22:58 edc_notification/constants.py
 -rw-r--r--  2.0 unx      613 b- defN 21-Feb-08 16:20 edc_notification/decorators.py
 -rw-r--r--  2.0 unx     5779 b- defN 21-Feb-08 16:20 edc_notification/mailing_list_manager.py
 -rw-r--r--  2.0 unx     2160 b- defN 21-Feb-08 16:20 edc_notification/modeladmin_mixins.py
 -rw-r--r--  2.0 unx      882 b- defN 21-Feb-08 16:20 edc_notification/models.py
 -rw-r--r--  2.0 unx     2078 b- defN 21-Feb-08 16:20 edc_notification/signals.py
 -rw-r--r--  2.0 unx     8219 b- defN 21-Apr-11 22:58 edc_notification/site_notifications.py
@@ -32,16 +34,16 @@
 -rw-r--r--  2.0 unx      365 b- defN 21-Apr-11 22:58 edc_notification/notification/updated_model_notification.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Mar-04 23:21 edc_notification/tests/__init__.py
 -rw-r--r--  2.0 unx      486 b- defN 21-Feb-08 16:20 edc_notification/tests/admin.py
 -rw-r--r--  2.0 unx     1124 b- defN 20-Mar-04 23:21 edc_notification/tests/models.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Feb-08 16:20 edc_notification/tests/tests/__init__.py
 -rw-r--r--  2.0 unx     3350 b- defN 21-Feb-08 16:20 edc_notification/tests/tests/test_admin_mixin.py
 -rw-r--r--  2.0 unx     6076 b- defN 21-Feb-08 16:20 edc_notification/tests/tests/test_mailing_list.py
--rw-r--r--  2.0 unx    22808 b- defN 21-Apr-11 22:58 edc_notification/tests/tests/test_notification.py
+-rw-r--r--  2.0 unx    22763 b- defN 21-Sep-09 00:28 edc_notification/tests/tests/test_notification.py
 -rw-r--r--  2.0 unx     2266 b- defN 21-May-15 16:33 edc_notification/tests/tests/test_sms.py
--rw-r--r--  2.0 unx       37 b- defN 21-Aug-18 19:02 edc_notification-0.3.8.dist-info/AUTHORS
--rw-r--r--  2.0 unx    35149 b- defN 21-Aug-18 19:02 edc_notification-0.3.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1587 b- defN 21-Aug-18 19:02 edc_notification-0.3.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Aug-18 19:02 edc_notification-0.3.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 21-Aug-18 19:02 edc_notification-0.3.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4354 b- defN 21-Aug-18 19:02 edc_notification-0.3.8.dist-info/RECORD
-45 files, 132177 bytes uncompressed, 37056 bytes compressed:  72.0%
+-rw-r--r--  2.0 unx       37 b- defN 21-Sep-09 00:28 edc_notification-0.3.9.dist-info/AUTHORS
+-rw-r--r--  2.0 unx    35149 b- defN 21-Sep-09 00:28 edc_notification-0.3.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1587 b- defN 21-Sep-09 00:28 edc_notification-0.3.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Sep-09 00:28 edc_notification-0.3.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 21-Sep-09 00:28 edc_notification-0.3.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4523 b- defN 21-Sep-09 00:28 edc_notification-0.3.9.dist-info/RECORD
+47 files, 132790 bytes uncompressed, 37364 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -6,14 +6,20 @@
 
 Filename: edc_notification/admin_site.py
 Comment: 
 
 Filename: edc_notification/apps.py
 Comment: 
 
+Filename: edc_notification/auth_objects.py
+Comment: 
+
+Filename: edc_notification/auths.py
+Comment: 
+
 Filename: edc_notification/constants.py
 Comment: 
 
 Filename: edc_notification/decorators.py
 Comment: 
 
 Filename: edc_notification/mailing_list_manager.py
@@ -111,26 +117,26 @@
 
 Filename: edc_notification/tests/tests/test_notification.py
 Comment: 
 
 Filename: edc_notification/tests/tests/test_sms.py
 Comment: 
 
-Filename: edc_notification-0.3.8.dist-info/AUTHORS
+Filename: edc_notification-0.3.9.dist-info/AUTHORS
 Comment: 
 
-Filename: edc_notification-0.3.8.dist-info/LICENSE
+Filename: edc_notification-0.3.9.dist-info/LICENSE
 Comment: 
 
-Filename: edc_notification-0.3.8.dist-info/METADATA
+Filename: edc_notification-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: edc_notification-0.3.8.dist-info/WHEEL
+Filename: edc_notification-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: edc_notification-0.3.8.dist-info/top_level.txt
+Filename: edc_notification-0.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: edc_notification-0.3.8.dist-info/RECORD
+Filename: edc_notification-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## edc_notification/tests/tests/test_notification.py

```diff
@@ -2,15 +2,15 @@
 from unittest.mock import patch
 
 from django.conf import settings
 from django.contrib.auth.models import User
 from django.core import mail
 from django.core.exceptions import ObjectDoesNotExist
 from django.core.management.color import color_style
-from django.test import TestCase, tag
+from django.test import TestCase
 from django.test.utils import override_settings
 from edc_utils import get_utcnow
 
 from edc_notification.constants import CREATE, UPDATE
 
 from ...decorators import RegisterNotificationError, register
 from ...models import Notification as NotificationModel
@@ -28,15 +28,14 @@
     site_notifications,
 )
 from ..models import AE, AnyModel, Condition, Death
 
 style = color_style()
 
 
-@tag("22")
 class TestNotification(TestCase):
     def setUp(self):
         Condition.objects.create()
         Condition.objects.create(name="arthritis")
 
     def test_register(self):
 
@@ -462,15 +461,14 @@
         death.report_datetime = get_utcnow()
         death.save()
         self.assertEqual(len(mail.outbox), 2)
 
         death.delete()
         self.assertEqual(len(mail.outbox), 2)
 
-    @tag("11")
     @override_settings(EDC_PROTOCOL_PROJECT_NAME="Mashi Trial")
     def test_model_notification_mail_subject(self):
 
         site_notifications._registry = {}
         site_notifications.update_notification_list()
 
         @register()
@@ -594,15 +592,14 @@
         self.assertRaises(
             ObjectDoesNotExist,
             NotificationModel.objects.get,
             name=DeathNotification2.name,
             enabled=True,
         )
 
-    @tag("1")
     def test_graded_event_grade3_as_test_email_message(self):
 
         site_notifications._registry = {}
         site_notifications.update_notification_list()
 
         @register()
         class G3EventNotification(GradedEventNotification):
```

## Comparing `edc_notification-0.3.8.dist-info/LICENSE` & `edc_notification-0.3.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edc_notification-0.3.8.dist-info/METADATA` & `edc_notification-0.3.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-notification
-Version: 0.3.8
+Version: 0.3.9
 Summary: Simple notification classes for clinic/edc
 Home-page: http://github.com/clinicedc/edc-notification
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: edc notification
 Platform: UNKNOWN
```

## Comparing `edc_notification-0.3.8.dist-info/RECORD` & `edc_notification-0.3.9.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 edc_notification/__init__.py,sha256=PADKXnS482L8EEJtGbISOJ4z9QzZK1pw5XmMR1_z-tY,318
 edc_notification/admin.py,sha256=xv_FNRRVp3buXRJSgqumNtLte72kdiMxV5rmNpPOJOs,360
 edc_notification/admin_site.py,sha256=4HuE70pTqNSLf9bSfskgi3W6A9VAD4LvOfO3GazVcOs,177
 edc_notification/apps.py,sha256=7OVGCXqZccsoE1wQs63nk8iPCF2DmiuQ8ZGJ-s3DyiQ,1162
+edc_notification/auth_objects.py,sha256=ABR8wOd-ZKY2JVq1Vi69aGOzhngvu55wEa8a-fYDVjo,217
+edc_notification/auths.py,sha256=AuXGxXIMA94CkDWZybm2BR4UHYySJbOZQun4McgXm-s,272
 edc_notification/constants.py,sha256=nZizX4z8bsJVIqQ5aExyu5uNKomSh36qcm55HFTkYSo,39
 edc_notification/decorators.py,sha256=OmLOW_jwsviyT9oGFS7q7SyAlx_u6vvY6vMtLHCRMkc,613
 edc_notification/mailing_list_manager.py,sha256=6EqPSFnFdIim6trBLTbPO-AIdcmLwgIt4MvyJtcfufU,5779
 edc_notification/modeladmin_mixins.py,sha256=CwdYDDEV9UzRB-mM4aOYp08RKlLER_wBTeo98A1mTdA,2160
 edc_notification/models.py,sha256=w_SmBXhDZ73XzQwv8yCkNMzONKePAHxUI2EnRs1S7HE,882
 edc_notification/signals.py,sha256=LwEZpK8hQ7tbrHNVnW6XdvxbTpErU48lrs86QemaX4Q,2078
 edc_notification/site_notifications.py,sha256=2PfMDCOtsn2eiPwsBOWeLzTcUpSnMzqupT0OMJI0vfc,8219
@@ -31,15 +33,15 @@
 edc_notification/notification/updated_model_notification.py,sha256=unrWByQek76_504nO3ginpkns-SCLec0hHvGU1JVkAk,365
 edc_notification/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 edc_notification/tests/admin.py,sha256=E8JFRvbT9ROIkBwB8HpBZgpzm8NpQ0fMq4ks4OTZm0Y,486
 edc_notification/tests/models.py,sha256=4i2mSIh3ONKiw3nnlunMKSIGAlDK-k0fGL8cZgXZ8bw,1124
 edc_notification/tests/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 edc_notification/tests/tests/test_admin_mixin.py,sha256=kkhPtEAvioRTll-r8iSnIsPRmX2Y3HThC1I6Hbyw68M,3350
 edc_notification/tests/tests/test_mailing_list.py,sha256=e23bPsjKVnw_xAMJA3zCHOaYhIobffe4YQgaVpVj1ns,6076
-edc_notification/tests/tests/test_notification.py,sha256=2auEQIYkFrW2cgkFsY-1K7mSHC_l6Ags9pLGbgai1u0,22808
+edc_notification/tests/tests/test_notification.py,sha256=yTOsmP8BNh2rOixfWpyv4bw4NzQWToHhQ1L_BPR32wU,22763
 edc_notification/tests/tests/test_sms.py,sha256=3e2IBljHNM03_jHpcv9A8q8D0DcpFPuG0AccB8V14EI,2266
-edc_notification-0.3.8.dist-info/AUTHORS,sha256=bASVS-K7ZNbIK4-9QOpuBM4CAkpiE5g8DKv7rSqST5g,37
-edc_notification-0.3.8.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-edc_notification-0.3.8.dist-info/METADATA,sha256=nZU9RSPDJdhyFrQOUKBbkWxe6U1r0L89slPwt-G7eBs,1587
-edc_notification-0.3.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-edc_notification-0.3.8.dist-info/top_level.txt,sha256=dezLTByR3IMxa6YvpkNwEgjTmRl9Xpg_oeSbsmN0WX0,17
-edc_notification-0.3.8.dist-info/RECORD,,
+edc_notification-0.3.9.dist-info/AUTHORS,sha256=bASVS-K7ZNbIK4-9QOpuBM4CAkpiE5g8DKv7rSqST5g,37
+edc_notification-0.3.9.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+edc_notification-0.3.9.dist-info/METADATA,sha256=SX3nUkVaeeawgTV6CURnGN_sOXM1TcBeFV8r6_hQBnc,1587
+edc_notification-0.3.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+edc_notification-0.3.9.dist-info/top_level.txt,sha256=dezLTByR3IMxa6YvpkNwEgjTmRl9Xpg_oeSbsmN0WX0,17
+edc_notification-0.3.9.dist-info/RECORD,,
```

