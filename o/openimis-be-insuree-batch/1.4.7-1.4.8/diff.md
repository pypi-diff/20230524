# Comparing `tmp/openimis-be-insuree_batch-1.4.7.tar.gz` & `tmp/openimis-be-insuree_batch-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-insuree_batch-1.4.7.tar", last modified: Sun Sep 25 19:57:27 2022, max compression
+gzip compressed data, was "openimis-be-insuree_batch-1.4.8.tar", last modified: Wed May 24 06:40:58 2023, max compression
```

## Comparing `openimis-be-insuree_batch-1.4.7.tar` & `openimis-be-insuree_batch-1.4.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 19:57:27.195888 openimis-be-insuree_batch-1.4.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-09-25 19:57:18.000000 openimis-be-insuree_batch-1.4.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-09-25 19:57:18.000000 openimis-be-insuree_batch-1.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-09-25 19:57:27.195888 openimis-be-insuree_batch-1.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-09-25 19:57:18.000000 openimis-be-insuree_batch-1.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 19:57:27.191887 openimis-be-insuree_batch-1.4.7/insuree_batch/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-09-25 19:57:18.000000 openimis-be-insuree_batch-1.4.7/insuree_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-09-25 19:57:18.000000 openimis-be-insuree_batch-1.4.7/insuree_batch/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-09-25 19:57:18.000000 openimis-be-insuree_batch-1.4.7/insuree_batch/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 19:57:27.191887 openimis-be-insuree_batch-1.4.7/insuree_batch/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-09-25 19:57:18.000000 openimis-be-insuree_batch-1.4.7/insuree_batch/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-09-25 19:57:18.000000 openimis-be-insuree_batch-1.4.7/insuree_batch/migrations/0002_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-25 19:57:18.000000 openimis-be-insuree_batch-1.4.7/insuree_batch/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-09-25 19:57:18.000000 openimis-be-insuree_batch-1.4.7/insuree_batch/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     5761 2022-09-25 19:57:18.000000 openimis-be-insuree_batch-1.4.7/insuree_batch/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)    10137 2022-09-25 19:57:18.000000 openimis-be-insuree_batch-1.4.7/insuree_batch/services.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 19:57:27.187888 openimis-be-insuree_batch-1.4.7/insuree_batch/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 19:57:27.195888 openimis-be-insuree_batch-1.4.7/insuree_batch/templates/insuree_batch/
--rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-09-25 19:57:18.000000 openimis-be-insuree_batch-1.4.7/insuree_batch/templates/insuree_batch/batch_qr.html
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-09-25 19:57:18.000000 openimis-be-insuree_batch-1.4.7/insuree_batch/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4931 2022-09-25 19:57:18.000000 openimis-be-insuree_batch-1.4.7/insuree_batch/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-09-25 19:57:18.000000 openimis-be-insuree_batch-1.4.7/insuree_batch/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     2000 2022-09-25 19:57:18.000000 openimis-be-insuree_batch-1.4.7/insuree_batch/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 19:57:27.195888 openimis-be-insuree_batch-1.4.7/openimis_be_insuree_batch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-09-25 19:57:27.000000 openimis-be-insuree_batch-1.4.7/openimis_be_insuree_batch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-09-25 19:57:27.000000 openimis-be-insuree_batch-1.4.7/openimis_be_insuree_batch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-25 19:57:27.000000 openimis-be-insuree_batch-1.4.7/openimis_be_insuree_batch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-09-25 19:57:27.000000 openimis-be-insuree_batch-1.4.7/openimis_be_insuree_batch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-25 19:57:27.000000 openimis-be-insuree_batch-1.4.7/openimis_be_insuree_batch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-25 19:57:27.195888 openimis-be-insuree_batch-1.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-09-25 19:57:18.000000 openimis-be-insuree_batch-1.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:40:58.874785 openimis-be-insuree_batch-1.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-24 06:40:44.000000 openimis-be-insuree_batch-1.4.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-24 06:40:44.000000 openimis-be-insuree_batch-1.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-24 06:40:58.874785 openimis-be-insuree_batch-1.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-24 06:40:44.000000 openimis-be-insuree_batch-1.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:40:58.870785 openimis-be-insuree_batch-1.4.8/insuree_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-24 06:40:44.000000 openimis-be-insuree_batch-1.4.8/insuree_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-24 06:40:44.000000 openimis-be-insuree_batch-1.4.8/insuree_batch/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-24 06:40:44.000000 openimis-be-insuree_batch-1.4.8/insuree_batch/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:40:58.874785 openimis-be-insuree_batch-1.4.8/insuree_batch/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-24 06:40:44.000000 openimis-be-insuree_batch-1.4.8/insuree_batch/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-24 06:40:44.000000 openimis-be-insuree_batch-1.4.8/insuree_batch/migrations/0002_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 06:40:44.000000 openimis-be-insuree_batch-1.4.8/insuree_batch/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-24 06:40:44.000000 openimis-be-insuree_batch-1.4.8/insuree_batch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-24 06:40:44.000000 openimis-be-insuree_batch-1.4.8/insuree_batch/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-05-24 06:40:44.000000 openimis-be-insuree_batch-1.4.8/insuree_batch/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:40:58.870785 openimis-be-insuree_batch-1.4.8/insuree_batch/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:40:58.874785 openimis-be-insuree_batch-1.4.8/insuree_batch/templates/insuree_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-24 06:40:44.000000 openimis-be-insuree_batch-1.4.8/insuree_batch/templates/insuree_batch/batch_qr.html
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-24 06:40:44.000000 openimis-be-insuree_batch-1.4.8/insuree_batch/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-24 06:40:44.000000 openimis-be-insuree_batch-1.4.8/insuree_batch/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-24 06:40:44.000000 openimis-be-insuree_batch-1.4.8/insuree_batch/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-24 06:40:44.000000 openimis-be-insuree_batch-1.4.8/insuree_batch/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:40:58.874785 openimis-be-insuree_batch-1.4.8/openimis_be_insuree_batch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-24 06:40:58.000000 openimis-be-insuree_batch-1.4.8/openimis_be_insuree_batch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-24 06:40:58.000000 openimis-be-insuree_batch-1.4.8/openimis_be_insuree_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 06:40:58.000000 openimis-be-insuree_batch-1.4.8/openimis_be_insuree_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-24 06:40:58.000000 openimis-be-insuree_batch-1.4.8/openimis_be_insuree_batch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-24 06:40:58.000000 openimis-be-insuree_batch-1.4.8/openimis_be_insuree_batch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 06:40:58.874785 openimis-be-insuree_batch-1.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-24 06:40:44.000000 openimis-be-insuree_batch-1.4.8/setup.py
```

### Comparing `openimis-be-insuree_batch-1.4.7/LICENSE.md` & `openimis-be-insuree_batch-1.4.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree_batch-1.4.7/PKG-INFO` & `openimis-be-insuree_batch-1.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-insuree_batch
-Version: 1.4.7
+Version: 1.4.8
 Summary: The openIMIS Backend Insuree Batch reference module.
 Home-page: https://openimis.org/
 Author: Eric Darchis
 Author-email: edarchis@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-insuree_batch-1.4.7/README.md` & `openimis-be-insuree_batch-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree_batch-1.4.7/insuree_batch/apps.py` & `openimis-be-insuree_batch-1.4.8/insuree_batch/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree_batch-1.4.7/insuree_batch/migrations/0001_initial.py` & `openimis-be-insuree_batch-1.4.8/insuree_batch/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree_batch-1.4.7/insuree_batch/migrations/0002_initial.py` & `openimis-be-insuree_batch-1.4.8/insuree_batch/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree_batch-1.4.7/insuree_batch/models.py` & `openimis-be-insuree_batch-1.4.8/insuree_batch/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,20 @@
 from core import models as core_models
 from django.db import models
 from location import models as location_models
 
 
 class InsureeBatch(core_models.UUIDModel):
     location = models.ForeignKey(
-        location_models.Location, models.DO_NOTHING,
-        db_column='LocationId', blank=True, null=True)
+        "location.Location",
+        models.DO_NOTHING,
+        db_column="LocationId",
+        blank=True,
+        null=True,
+    )
     audit_user_id = models.IntegerField(db_column='AuditUserID')
     run_date = fields.DateTimeField(db_column='RunDate', auto_now_add=True)
     archived = models.BooleanField(default=False)
     comment = models.TextField(blank=True, null=True)
 
 
 class BatchInsureeNumber(core_models.UUIDModel):
```

### Comparing `openimis-be-insuree_batch-1.4.7/insuree_batch/schema.py` & `openimis-be-insuree_batch-1.4.8/insuree_batch/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import graphene
 from django.core.exceptions import PermissionDenied, ValidationError
-from django.db import connection
 from core import prefix_filterset, ExtendedConnection
 from core.schema import OpenIMISMutation, OrderedDjangoFilterConnectionField
-from graphene import ObjectType
 from django.urls import reverse
 from graphene_django import DjangoObjectType
-from graphene_django.filter import DjangoFilterConnectionField
 from django.contrib.auth.models import AnonymousUser
 
 from location.models import Location
 from location.schema import LocationGQLType
 from .models import InsureeBatch, BatchInsureeNumber, InsureeBatchMutation
 from .apps import InsureeBatchConfig
 from django.utils.translation import gettext as _
@@ -21,15 +18,17 @@
 
 logger = logging.getLogger(__file__)
 
 
 class InsureeBatchGQLType(DjangoObjectType):
     print_url = graphene.Field(graphene.String)
     export_url = graphene.Field(
-        graphene.String, dry_run=graphene.Boolean(), count=graphene.Int()
+        graphene.String,
+        dry_run=graphene.Boolean(),
+        count=graphene.Int()
     )
     nb_generated = graphene.Field(graphene.Int)
     nb_printed = graphene.Field(graphene.Int)
 
     def resolve_nb_generated(self, info):
         return self.insuree_numbers.count()
 
@@ -72,33 +71,44 @@
         connection_class = ExtendedConnection
 
 
 class Query(graphene.ObjectType):
     insuree_batches = OrderedDjangoFilterConnectionField(
         InsureeBatchGQLType,
         client_mutation_id=graphene.String(),
+        location=graphene.Int(),
         orderBy=graphene.List(of_type=graphene.String),
     )
 
     batch_insuree_numbers = OrderedDjangoFilterConnectionField(
         InsureeBatchGQLType, orderBy=graphene.List(of_type=graphene.String)
     )
 
-    def resolve_insuree_batches(self, info, client_mutation_id=None, **kwargs):
+    def resolve_insuree_batches(
+            self,
+            info,
+            client_mutation_id=None,
+            location=None,
+            **kwargs
+    ):
         if not info.context.user.has_perms(
             InsureeBatchConfig.gql_query_batch_runs_perms
         ):
             raise PermissionDenied(_("unauthorized"))
+        queryset = InsureeBatch.objects.all()
         if client_mutation_id:
-            queryset = InsureeBatch.objects.filter(
+            queryset = queryset.filter(
                 Q(mutations__mutation__client_mutation_id=client_mutation_id)
             )
-        else:
-            queryset = InsureeBatch.objects
-
+        elif location is not None:
+            queryset = queryset.filter(
+                Q(location__in=Location.objects.parents(location))
+                | Q(location__id=location)
+                | Q(location__isnull=True)
+            )
         return queryset
 
     def resolve_batch_insuree_numbers(self, info, **kwargs):
         if not info.context.user.has_perms(
             InsureeBatchConfig.gql_query_batch_runs_perms
         ):
             raise PermissionDenied(_("unauthorized"))
```

### Comparing `openimis-be-insuree_batch-1.4.7/insuree_batch/services.py` & `openimis-be-insuree_batch-1.4.8/insuree_batch/services.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,31 +53,36 @@
     if length is None or modulo is None:
         logging.warning("The settings do not specify an insuree number length. This normally means that they are not "
                         "validated by openIMIS. However, this doesn't make sense when generating insuree numbers. "
                         "We are using 9 and 7 as default values but you should configure these in the settings")
         length = 9
         modulo = 7
     modulo_len = len(str(modulo))
-
     if location:
+        digital_code = extract_digits_from_code(location.code)
         try:
-            main_number = int(location.code) * (10 ** (length - modulo_len - get_location_id_len(location.type))) \
+            main_number = digital_code * (10 ** (length - modulo_len - get_location_id_len(location.type))) \
                           + get_random(length - get_location_id_len(location.type) - modulo_len)
         except ValueError:
             logger.error("Computing a QR code with a location that is not numeric will fail its modulo")
             raise
     else:
         main_number = get_random(length - modulo_len)
     checksum = main_number % modulo
     # generates "%010d" that is then formatted with the actual insuree number. This confuses the IDE => noinspection
     padded_main = f"%0{length - modulo_len}d" % main_number
     padded_checksum = f"%0{modulo_len}d" % checksum
     return f"{padded_main}{padded_checksum}"
 
 
+def extract_digits_from_code(raw_code: str) -> int:
+    digital_code = [x for x in raw_code if x.isdigit()]
+    return int("".join(digital_code))
+
+
 def get_random(length):
     return random.randint(10 ** (length - 1), (10 ** length) - 1)
 
 
 @lru_cache(maxsize=None)
 def get_location_id_len(location_type):
     """
@@ -97,15 +102,15 @@
         csv_file_path = os.path.join(tmp_dir_name, "index.csv")
         with open(csv_file_path, 'w') as f:
             # create the csv writer
             writer = csv.writer(f)
             writer.writerow([
                 "InsureeNum", "OtherNames", "LastName", "DateOfBirth", "Gender", "Phone", "EffectiveDate",
                 "ValidityDate", "VillageCode", "VillageName", "WardCode", "WardName", "DistrictCode", "DistrictName",
-                "RegionCode", "RegionName", "Filename", "Error"
+                "RegionCode", "RegionName", "Filename", "Error", "EnrollmentDate",
             ])
             files_to_zip = [(csv_file_path, "index.csv")]
             zip_file_path = tempfile.NamedTemporaryFile("wb", prefix="insuree_export", suffix=".zip", delete=False)
 
             for insuree in to_export:
                 from core import datetimedelta
                 latest_policy = insuree\
@@ -146,15 +151,17 @@
                     ward.code,
                     ward.name,
                     district.code,
                     district.name,
                     region.code,
                     region.name,
                     f"{insuree.chf_id}.jpg" if photo_filename else None,
-                    ""
+                    "",
+                    latest_policy.enrollment_date.strftime('%d/%m/%Y')
+                    if latest_policy and latest_policy.enrollment_date else None,
                 ]
 
                 if photo_filename:
                     if insuree.photo.photo:
                         with open(photo_filename, "wb") as photo_file:
                             photo_bytes = insuree.photo.photo.encode("utf-8")
                             decoded_photo = base64.decodebytes(photo_bytes)
@@ -180,16 +187,16 @@
                                     photo_root_path,
                                     re.sub(r"Images([/\\\\])", "", insuree_photo_folder),
                                     insuree.photo.filename)
                             try:
                                 shutil.copyfile(full_path, photo_filename)
                                 files_to_zip.append((photo_filename, f"{insuree.chf_id}.jpg"))
                             except Exception as exc:
-                                row_to_write[-2] = ""
-                                row_to_write[-1] = f"Could not copy file {full_path}: {exc}"
+                                row_to_write[-3] = ""
+                                row_to_write[-2] = f"Could not copy file {full_path}: {exc}"
                     else:
                         logger.warning("Photo was identified but neither base64 photo nor filename")
                 writer.writerow(row_to_write)
         if not dry_run:
             BatchInsureeNumber.objects\
                 .filter(insuree_number__in=[i.chf_id for i in to_export])\
                 .update(print_date=datetime.now())
```

### Comparing `openimis-be-insuree_batch-1.4.7/insuree_batch/templates/insuree_batch/batch_qr.html` & `openimis-be-insuree_batch-1.4.8/insuree_batch/templates/insuree_batch/batch_qr.html`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree_batch-1.4.7/insuree_batch/tests.py` & `openimis-be-insuree_batch-1.4.8/insuree_batch/tests.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import random
 from django.test import TestCase, override_settings
 
 from core.models import Officer
+from .models import InsureeBatch
 from insuree.apps import InsureeConfig
 from insuree.services import validate_insuree_number
 from insuree.test_helpers import create_test_insuree, create_test_photo
 from location.models import Location
 from location.test_helpers import create_test_location
+from .test_helpers import create_test_batch
 from .services import get_random, generate_insuree_number, generate_insuree_numbers, get_insurees_to_export, \
     export_insurees, get_location_id_len
 
 
 class InsureeBatchTest(TestCase):
     def setUp(self) -> None:
         self.test_location = create_test_location("D", valid=True, custom_props={"code": "99"})
@@ -104,7 +106,16 @@
         zip_file = export_insurees(batch=batch)
         self.assertIsNotNone(zip_file)
         # TODO check the zip file in depth
 
         for insuree in insurees:
             insuree.delete()
         batch.delete()
+
+    def test_fetch_batches(self):
+        test_region = create_test_location('R', custom_props={"code": "71"})
+        test_district = create_test_location('D', custom_props={"code": "23"})
+        create_test_batch(test_region)
+        create_test_batch(test_district)
+        queryset = InsureeBatch.objects.filter(location=test_region.id)
+        self.assertIsNotNone(queryset)
+        self.assertEqual(len(queryset), 1)
```

### Comparing `openimis-be-insuree_batch-1.4.7/insuree_batch/views.py` & `openimis-be-insuree_batch-1.4.8/insuree_batch/views.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree_batch-1.4.7/openimis_be_insuree_batch.egg-info/PKG-INFO` & `openimis-be-insuree_batch-1.4.8/openimis_be_insuree_batch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-insuree-batch
-Version: 1.4.7
+Version: 1.4.8
 Summary: The openIMIS Backend Insuree Batch reference module.
 Home-page: https://openimis.org/
 Author: Eric Darchis
 Author-email: edarchis@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-insuree_batch-1.4.7/openimis_be_insuree_batch.egg-info/SOURCES.txt` & `openimis-be-insuree_batch-1.4.8/openimis_be_insuree_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree_batch-1.4.7/setup.py` & `openimis-be-insuree_batch-1.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="openimis-be-insuree_batch",
-    version="1.4.7",
+    version="1.4.8",
     packages=find_packages(),
     include_package_data=True,
     license="GNU AGPL v3",
     description="The openIMIS Backend Insuree Batch reference module.",
     # long_description=README,
     url="https://openimis.org/",
     author="Eric Darchis",
```

