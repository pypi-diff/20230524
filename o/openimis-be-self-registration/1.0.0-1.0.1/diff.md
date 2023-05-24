# Comparing `tmp/openimis-be-self-registration-1.0.0.tar.gz` & `tmp/openimis-be-self-registration-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-self-registration-1.0.0.tar", last modified: Mon Nov 21 14:29:52 2022, max compression
+gzip compressed data, was "openimis-be-self-registration-1.0.1.tar", last modified: Wed May 24 06:45:19 2023, max compression
```

## Comparing `openimis-be-self-registration-1.0.0.tar` & `openimis-be-self-registration-1.0.1.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-21 14:29:52.902172 openimis-be-self-registration-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1852 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)       36 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      693 2022-11-21 14:29:52.902172 openimis-be-self-registration-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      152 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-21 14:29:52.898172 openimis-be-self-registration-1.0.0/openimis_be_self_registration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      693 2022-11-21 14:29:52.000000 openimis-be-self-registration-1.0.0/openimis_be_self_registration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1749 2022-11-21 14:29:52.000000 openimis-be-self-registration-1.0.0/openimis_be_self_registration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-21 14:29:52.000000 openimis-be-self-registration-1.0.0/openimis_be_self_registration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      205 2022-11-21 14:29:52.000000 openimis-be-self-registration-1.0.0/openimis_be_self_registration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2022-11-21 14:29:52.000000 openimis-be-self-registration-1.0.0/openimis_be_self_registration.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-21 14:29:52.898172 openimis-be-self-registration-1.0.0/self_registration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      213 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)    15418 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-21 14:29:52.902172 openimis-be-self-registration-1.0.0/self_registration/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)      893 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      436 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/0002_auto_20210526_1618.py
--rw-r--r--   0 runner    (1001) docker     (122)      882 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/0003_notice.py
--rw-r--r--   0 runner    (1001) docker     (122)      849 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/0004_otp.py
--rw-r--r--   0 runner    (1001) docker     (122)      598 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/0005_auto_20210530_2156.py
--rw-r--r--   0 runner    (1001) docker     (122)     1137 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/0006_healthfacilitycoordinate.py
--rw-r--r--   0 runner    (1001) docker     (122)      959 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/0007_voucherpayment.py
--rw-r--r--   0 runner    (1001) docker     (122)      446 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/0008_voucherpayment_vocher_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     1346 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/0009_auto_20210617_2217.py
--rw-r--r--   0 runner    (1001) docker     (122)      434 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/0010_auto_20210623_0809.py
--rw-r--r--   0 runner    (1001) docker     (122)      434 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/0011_auto_20210623_0809.py
--rw-r--r--   0 runner    (1001) docker     (122)     1299 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/0012_auto_20210623_2016.py
--rw-r--r--   0 runner    (1001) docker     (122)      603 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/0013_auto_20210623_2131.py
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/0014_auto_20210627_0808.py
--rw-r--r--   0 runner    (1001) docker     (122)      778 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/0015_auto_20210704_2249.py
--rw-r--r--   0 runner    (1001) docker     (122)     1965 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/0016_auto_20210707_2310.py
--rw-r--r--   0 runner    (1001) docker     (122)     1017 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/0017_auto_20210710_1255.py
--rw-r--r--   0 runner    (1001) docker     (122)      850 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/0018_auto_20210712_1431.py
--rw-r--r--   0 runner    (1001) docker     (122)      996 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/0019_auto_20210715_0721.py
--rw-r--r--   0 runner    (1001) docker     (122)     1160 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/0020_auto_20210715_0732.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5163 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/models.py
--rw-r--r--   0 runner    (1001) docker     (122)    15332 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/test.py
--rw-r--r--   0 runner    (1001) docker     (122)       63 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)      121 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      465 2022-11-21 14:29:40.000000 openimis-be-self-registration-1.0.0/self_registration/views.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-21 14:29:52.906172 openimis-be-self-registration-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2022-11-21 14:29:49.000000 openimis-be-self-registration-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:45:19.417637 openimis-be-self-registration-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-24 06:45:19.417637 openimis-be-self-registration-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:45:19.413637 openimis-be-self-registration-1.0.1/openimis_be_self_registration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-24 06:45:19.000000 openimis-be-self-registration-1.0.1/openimis_be_self_registration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-24 06:45:19.000000 openimis-be-self-registration-1.0.1/openimis_be_self_registration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 06:45:19.000000 openimis-be-self-registration-1.0.1/openimis_be_self_registration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-24 06:45:19.000000 openimis-be-self-registration-1.0.1/openimis_be_self_registration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 06:45:19.000000 openimis-be-self-registration-1.0.1/openimis_be_self_registration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:45:19.413637 openimis-be-self-registration-1.0.1/self_registration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16591 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:45:19.417637 openimis-be-self-registration-1.0.1/self_registration/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0002_auto_20210526_1618.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0003_notice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0004_otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0005_auto_20210530_2156.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0006_healthfacilitycoordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0007_voucherpayment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0008_voucherpayment_vocher_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0009_auto_20210617_2217.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0010_auto_20210623_0809.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0011_auto_20210623_0809.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0012_auto_20210623_2016.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0013_auto_20210623_2131.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0014_auto_20210627_0808.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0015_auto_20210704_2249.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0016_auto_20210707_2310.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0017_auto_20210710_1255.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0018_auto_20210712_1431.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0019_auto_20210715_0721.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0020_auto_20210715_0732.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/0021_alter_voucherpayment_vocher_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18567 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-24 06:45:03.000000 openimis-be-self-registration-1.0.1/self_registration/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 06:45:19.417637 openimis-be-self-registration-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-24 06:45:17.000000 openimis-be-self-registration-1.0.1/setup.py
```

### Comparing `openimis-be-self-registration-1.0.0/LICENSE.md` & `openimis-be-self-registration-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-self-registration-1.0.0/PKG-INFO` & `openimis-be-self-registration-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-self-registration
-Version: 1.0.0
+Version: 1.0.1
 Summary: The openIMIS self registration reference module.
 Home-page: https://openimis.org/
 Author: Tinker Technology
 Author-email: info@tinker.com.np
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-self-registration-1.0.0/openimis_be_self_registration.egg-info/PKG-INFO` & `openimis-be-self-registration-1.0.1/openimis_be_self_registration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-self-registration
-Version: 1.0.0
+Version: 1.0.1
 Summary: The openIMIS self registration reference module.
 Home-page: https://openimis.org/
 Author: Tinker Technology
 Author-email: info@tinker.com.np
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-self-registration-1.0.0/openimis_be_self_registration.egg-info/SOURCES.txt` & `openimis-be-self-registration-1.0.1/openimis_be_self_registration.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,8 +34,9 @@
 self_registration/migrations/0014_auto_20210627_0808.py
 self_registration/migrations/0015_auto_20210704_2249.py
 self_registration/migrations/0016_auto_20210707_2310.py
 self_registration/migrations/0017_auto_20210710_1255.py
 self_registration/migrations/0018_auto_20210712_1431.py
 self_registration/migrations/0019_auto_20210715_0721.py
 self_registration/migrations/0020_auto_20210715_0732.py
+self_registration/migrations/0021_alter_voucherpayment_vocher_id.py
 self_registration/migrations/__init__.py
```

### Comparing `openimis-be-self-registration-1.0.0/self_registration/gql_mutations.py` & `openimis-be-self-registration-1.0.1/self_registration/gql_mutations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 import base64
 from django.core.files.base import ContentFile
 
 import graphene
 from core.schema import OpenIMISMutation
 from graphql import GraphQLError
 from insuree.schema import InsureeGQLType
+from .apps import SelfRegistrationConfig
 from .models import ChfidTempInsuree
-
-def dfprint(i):
-    print(i)
-    pass
+from django.utils.translation import gettext as _
+from django.core.exceptions import PermissionDenied
 
 
 # format base64 id string
 def fbis64(inp):
     if not inp:
         return inp
-    dfprint('fbis64')
     # NoticeGQLType:38
     # 
     bstr = base64.b64decode(inp)
     sstr = bstr.decode('utf-8')
     istrs = sstr.split(':')
     istr = istrs[1]
-    dfprint([bstr, sstr, istr])
     return istr
 
 
 from .models import Notice, VoucherPayment, Feedback, Config
 from graphene_django import DjangoObjectType
 from graphene import Connection, Int
 from insuree import models as insuree_models
@@ -38,18 +35,21 @@
     class Meta:
         abstract = True
 
     total_count = Int()
     edge_count = Int()
 
     def resolve_total_count(root, info, **kwargs):
-        print(root.length)
+        if not info.context.user.is_authenticated:
+            raise PermissionDenied(_("unauthorized"))
         return root.length
 
     def resolve_edge_count(root, info, **kwargs):
+        if not info.context.user.is_authenticated:
+            raise PermissionDenied(_("unauthorized"))
         return len(root.edges)
 
 
 class VoucherPaymentType(DjangoObjectType):
     class Meta:
         model = VoucherPayment
         fields = ['voucher']
@@ -68,20 +68,23 @@
         phone = graphene.String()
 
     ok = graphene.Boolean()
 
     # @classmethod
     def mutate(self, info, file, insureeCHFID, email, phone):
         files = info.context.FILES
-        print(files)
         insuree_obj = insuree_models.Insuree.objects.filter(chf_id=insureeCHFID).first()
-        print(insuree_obj.pk)
         instance = Profile.objects.filter(insuree_id=insuree_obj.pk).first()
         if not instance:
+            if not info.context.user.has_perms(SelfRegistrationConfig.gql_mutation_add_profile_perms):
+                raise PermissionDenied(_("unauthorized"))
             instance = Profile()
+        else:
+            if not info.context.user.has_perms(SelfRegistrationConfig.gql_mutation_update_profile_perms):
+                raise PermissionDenied(_("unauthorized"))
         instance.photo = files.get('file') if files.get('file') else instance.photo
         instance.email = email if email else instance.email
         instance.phone = phone if phone else instance.phone
         instance.save()
         return CreateOrUpdateProfileMutation(ok=True)
 
 
@@ -95,14 +98,16 @@
         file = graphene.List(graphene.String)
         insuree = graphene.String()
 
     ok = graphene.Boolean()
 
     # @classmethod
     def mutate(self, info, file, insuree):
+        if not info.context.user.has_perms(SelfRegistrationConfig.gql_mutation_add_voucher_perms):
+            raise PermissionDenied(_("unauthorized"))
         files = info.context.FILES
         insuree_obj = insuree_models.Insuree.objects.filter(chf_id=insuree).first()
         VoucherPayment.objects.create(voucher=files.get('file'), insuree=insuree_obj)
         Notification.objects.create(insuree=insuree_obj, message="Your Submission has been saved thank you",
                                     chf_id=insuree)
         return CreateVoucherPaymentMutation(ok=True)
 
@@ -138,15 +143,16 @@
         mobile_number = graphene.String(required=True)
         queries = graphene.String(required=True)
 
     feedback = graphene.Field(FeedbackAppGQLType)
 
     @classmethod
     def mutate(cls, root, info, **kwargs):
-        print(kwargs)
+        if not info.context.user.has_perms(SelfRegistrationConfig.gql_mutation_add_feedback_perms):
+            raise PermissionDenied(_("unauthorized"))
         feedback = Feedback.objects.create(**kwargs)
         return CreateFeedbackMutation(feedback=feedback)
 
 
 class CreateNoticeMutation(OpenIMISMutation):  # graphene.relay.ClientIDMutation):
     class Input:
         title = graphene.String(required=True)
@@ -154,15 +160,16 @@
         client_mutation_id = graphene.String()
         client_mutation_label = graphene.String()
 
     notice = graphene.Field(NoticeType)
 
     @classmethod
     def mutate_and_get_payload(cls, root, info, **input):
-        print('CreateNoticeMutation mutate')
+        if not info.context.user.has_perms(SelfRegistrationConfig.gql_mutation_add_notification_perms):
+            raise PermissionDenied(_("unauthorized"))
         data = input
         if "client_mutation_id" in data:
             data.pop('client_mutation_id')
         if "client_mutation_label" in data:
             data.pop('client_mutation_label')
         notice = Notice.objects.create(title=input['title'], description=input['description'])
         return CreateNoticeMutation(notice=notice)
@@ -176,36 +183,39 @@
         title = graphene.String(required=False, )
         description = graphene.String(required=True)
         client_mutation_id = graphene.String()
         client_mutation_label = graphene.String()
 
     @classmethod
     def mutate_and_get_payload(cls, root, info, **input):
-        dfprint('UpdateNoticeMutation mutate')
+        if not info.context.user.has_perms(SelfRegistrationConfig.gql_mutation_update_notification_perms):
+            raise PermissionDenied(_("unauthorized"))
         data = input
         if "client_mutation_id" in data:
             data.pop('client_mutation_id')
         if "client_mutation_label" in data:
             data.pop('client_mutation_label')
         try:
-            notice = Notice.objects.filter(pk=fbis64(input['id']))  # ;dfprint(notice)
+            notice = Notice.objects.filter(pk=fbis64(input['id']))
             notice.update(title=input['title'], description=input['description'])
             return UpdateNoticeMutation(notice=notice)
         except:
             return GraphQLError('The notice you are updating might not exist anymore')
 
 
 class DeleteNoticeMutation(graphene.Mutation):
     class Arguments:
         id = graphene.Int(required=True)
 
     notice = graphene.Field(NoticeType)
 
     @classmethod
     def mutate(self, info, cls, id):
+        if not info.context.user.has_perms(SelfRegistrationConfig.gql_mutation_delete_notification_perms):
+            raise PermissionDenied(_("unauthorized"))
         try:
             notice = Notice.objects.filter(pk=id).first()
             notice.active = False  # soft_delete
             notice.save()
             return DeleteNoticeMutation(notice=notice)
         except:
             return GraphQLError('The notice you are deleting might not exist anymore')
@@ -220,18 +230,18 @@
 class CreateTempRegInsureeMutation(graphene.Mutation):
     class Arguments:
         json = graphene.JSONString()
     ok = graphene.Boolean()
 
     @classmethod
     def mutate(self, info, cls, **kwargs):
-        dfprint(kwargs)
+        if not info.context.user.has_perms(SelfRegistrationConfig.gql_mutation_add_insuree_reg_perms):
+            raise PermissionDenied(_("unauthorized"))
         inp_json = kwargs['json']
         str_json = json.dumps(inp_json)  # stringify json to save imp_json.get("Isurees"]
-        dfprint(str_json)
         jantu = inp_json.get("Insurees")[0]
         phone_number=jantu.get("Phone")
         
         tempReg=None
         tempReg=InsureeTempReg.objects.filter(phone_number=phone_number).first()
         if tempReg:
             tempReg.json = str_json
@@ -279,15 +289,14 @@
             "audit_user_id": 1,
             "is_offline": True,
             # "confirmation_no" : None,
             # "confirmation_type_id": None,
 
         }
         family_create["head_insuree_id"] = insuree_.id
-        print('familty-save-after', family_create)
         family = insuree_models.Family.objects.create(**family_create)
         family_id = family.id
     return family_id
 
 def process_b64photo_write(args):
     photo = args.get('b64photo')
     save_path=args.get('save_path')
@@ -304,18 +313,16 @@
         os.makedirs(save_path, exist_ok=True)
         img_fullpath=os.path.join(save_path, img_name)
         image_result = open(img_fullpath, 'wb')
         final_image = image_result.write(image_data)
     return img_name
 
 def process_photo(args):
-    dfprint('process_photo')
     insuree_save = args.get('insuree_save')
     photo = insuree_save.get('B64Photo')  # dbg_tmp_insuree_photo()
-    # print( insuree_models.__dict__ )
 
     save_path=""
     img_name=""
     if photo:  # and False:        
         cfg = Config.objects.filter(key='InsureeImageDir').first()
         if cfg:
             save_path = cfg.value
@@ -361,15 +368,14 @@
         # "validity_from" : "2020-01-01",
         "card_issued": False,
         "audit_user_id": 1,
         'photo_id': photo_id,
         # "audit_user_id" : 1,
     }
     insuree_create["family_id"] = family_id
-    dfprint(insuree_create)
     modelInsuree = insuree_models.Insuree.objects.create(**insuree_create)
     return modelInsuree.pk
     pass
 
 
 """
 mutation {
@@ -394,20 +400,20 @@
         status_message = graphene.String()
 
     ok = graphene.Boolean()
     message = graphene.String()
 
     @classmethod
     def mutate(self, info, cls, **kwargs):
-        dfprint('CreateInsureeMutation mutate')
+        if not info.context.user.has_perms(SelfRegistrationConfig.gql_mutation_add_insuree_perms):
+            raise PermissionDenied(_("unauthorized"))
         message = ""
         try:
             pk = kwargs['id']  # access Arguments #13 testing
             temp_insuree = InsureeTempReg.objects.filter(pk=pk).first()
-            print('kwargs----------',kwargs)
             if kwargs.get('is_hold'):
                 temp_insuree.is_hold = True
                 temp_insuree.status_message = kwargs.get('status_message')
                 temp_insuree.save()
             if kwargs.get('is_rejected'):
                 temp_insuree.is_rejected = True
                 temp_insuree.status_message = kwargs.get('status_message')
@@ -443,14 +449,13 @@
                             temp_insuree.save()
 
                     # everything ok, then approved flag changed
                     temp_insuree.is_approved = True
                     temp_insuree.status_message = kwargs.get('statusMessage')
                     temp_insuree.save()
         except Exception as e:
-            print(e)
             import traceback
             traceback.print_exc()
             return CreateInsureeMutation(ok=False, message=message)
             # raise
         return CreateInsureeMutation(ok=True)
```

### Comparing `openimis-be-self-registration-1.0.0/self_registration/migrations/0001_initial.py` & `openimis-be-self-registration-1.0.1/self_registration/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-self-registration-1.0.0/self_registration/migrations/0003_notice.py` & `openimis-be-self-registration-1.0.1/self_registration/migrations/0003_notice.py`

 * *Files identical despite different names*

### Comparing `openimis-be-self-registration-1.0.0/self_registration/migrations/0004_otp.py` & `openimis-be-self-registration-1.0.1/self_registration/migrations/0004_otp.py`

 * *Files identical despite different names*

### Comparing `openimis-be-self-registration-1.0.0/self_registration/migrations/0005_auto_20210530_2156.py` & `openimis-be-self-registration-1.0.1/self_registration/migrations/0005_auto_20210530_2156.py`

 * *Files identical despite different names*

### Comparing `openimis-be-self-registration-1.0.0/self_registration/migrations/0006_healthfacilitycoordinate.py` & `openimis-be-self-registration-1.0.1/self_registration/migrations/0006_healthfacilitycoordinate.py`

 * *Files identical despite different names*

### Comparing `openimis-be-self-registration-1.0.0/self_registration/migrations/0007_voucherpayment.py` & `openimis-be-self-registration-1.0.1/self_registration/migrations/0007_voucherpayment.py`

 * *Files identical despite different names*

### Comparing `openimis-be-self-registration-1.0.0/self_registration/migrations/0009_auto_20210617_2217.py` & `openimis-be-self-registration-1.0.1/self_registration/migrations/0009_auto_20210617_2217.py`

 * *Files identical despite different names*

### Comparing `openimis-be-self-registration-1.0.0/self_registration/migrations/0012_auto_20210623_2016.py` & `openimis-be-self-registration-1.0.1/self_registration/migrations/0012_auto_20210623_2016.py`

 * *Files identical despite different names*

### Comparing `openimis-be-self-registration-1.0.0/self_registration/migrations/0013_auto_20210623_2131.py` & `openimis-be-self-registration-1.0.1/self_registration/migrations/0013_auto_20210623_2131.py`

 * *Files identical despite different names*

### Comparing `openimis-be-self-registration-1.0.0/self_registration/migrations/0014_auto_20210627_0808.py` & `openimis-be-self-registration-1.0.1/self_registration/migrations/0014_auto_20210627_0808.py`

 * *Files identical despite different names*

### Comparing `openimis-be-self-registration-1.0.0/self_registration/migrations/0015_auto_20210704_2249.py` & `openimis-be-self-registration-1.0.1/self_registration/migrations/0015_auto_20210704_2249.py`

 * *Files identical despite different names*

### Comparing `openimis-be-self-registration-1.0.0/self_registration/migrations/0016_auto_20210707_2310.py` & `openimis-be-self-registration-1.0.1/self_registration/migrations/0016_auto_20210707_2310.py`

 * *Files identical despite different names*

### Comparing `openimis-be-self-registration-1.0.0/self_registration/migrations/0017_auto_20210710_1255.py` & `openimis-be-self-registration-1.0.1/self_registration/migrations/0017_auto_20210710_1255.py`

 * *Files identical despite different names*

### Comparing `openimis-be-self-registration-1.0.0/self_registration/migrations/0018_auto_20210712_1431.py` & `openimis-be-self-registration-1.0.1/self_registration/migrations/0018_auto_20210712_1431.py`

 * *Files identical despite different names*

### Comparing `openimis-be-self-registration-1.0.0/self_registration/migrations/0019_auto_20210715_0721.py` & `openimis-be-self-registration-1.0.1/self_registration/migrations/0019_auto_20210715_0721.py`

 * *Files identical despite different names*

### Comparing `openimis-be-self-registration-1.0.0/self_registration/migrations/0020_auto_20210715_0732.py` & `openimis-be-self-registration-1.0.1/self_registration/migrations/0020_auto_20210715_0732.py`

 * *Files identical despite different names*

### Comparing `openimis-be-self-registration-1.0.0/self_registration/models.py` & `openimis-be-self-registration-1.0.1/self_registration/models.py`

 * *Files identical despite different names*

### Comparing `openimis-be-self-registration-1.0.0/self_registration/test.py` & `openimis-be-self-registration-1.0.1/self_registration/test.py`

 * *Files identical despite different names*

### Comparing `openimis-be-self-registration-1.0.0/setup.py` & `openimis-be-self-registration-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-self-registration',
-    version='v1.0.0',
+    version='v1.0.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS self registration reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Tinker Technology',
```

