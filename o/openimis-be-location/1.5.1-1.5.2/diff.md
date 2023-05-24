# Comparing `tmp/openimis-be-location-1.5.1.tar.gz` & `tmp/openimis-be-location-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-location-1.5.1.tar", last modified: Tue May 16 21:37:57 2023, max compression
+gzip compressed data, was "openimis-be-location-1.5.2.tar", last modified: Wed May 24 08:15:08 2023, max compression
```

## Comparing `openimis-be-location-1.5.1.tar` & `openimis-be-location-1.5.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:57.514262 openimis-be-location-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-16 21:37:57.514262 openimis-be-location-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:57.510262 openimis-be-location-1.5.1/location/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:57.510262 openimis-be-location-1.5.1/location/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0002_location.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0003_userdistrict.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0004_locationmutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0005_healthfacilitycatchment_healthfacilitylegalform_healthfacilitymutation_healthfacilitysublevel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0006_users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0007_auto_20211103_1046.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0008_add_enrollment_officer_gql_query_location_right.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0009_add_location_read_right.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0010_insert_create_region_location_perms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0011_auto_20230317_0924.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0012_auto_20230317_0927.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0013_auto_20230317_1534.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0014_add_missing_fields_to_django_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0015_set_managed_to_true.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15924 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/services.py
--rw-r--r--   0 runner    (1001) docker     (123)    15748 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:57.514262 openimis-be-location-1.5.1/openimis_be_location.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-16 21:37:57.000000 openimis-be-location-1.5.1/openimis_be_location.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-16 21:37:57.000000 openimis-be-location-1.5.1/openimis_be_location.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:37:57.000000 openimis-be-location-1.5.1/openimis_be_location.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-16 21:37:57.000000 openimis-be-location-1.5.1/openimis_be_location.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 21:37:57.000000 openimis-be-location-1.5.1/openimis_be_location.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:37:57.514262 openimis-be-location-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-16 21:37:55.000000 openimis-be-location-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:15:08.347416 openimis-be-location-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-24 08:15:08.347416 openimis-be-location-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:15:08.347416 openimis-be-location-1.5.2/location/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:15:08.347416 openimis-be-location-1.5.2/location/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/migrations/0002_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/migrations/0003_userdistrict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/migrations/0004_locationmutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/migrations/0005_healthfacilitycatchment_healthfacilitylegalform_healthfacilitymutation_healthfacilitysublevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/migrations/0006_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/migrations/0007_auto_20211103_1046.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/migrations/0008_add_enrollment_officer_gql_query_location_right.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/migrations/0009_add_location_read_right.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/migrations/0010_insert_create_region_location_perms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/migrations/0011_auto_20230317_0924.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/migrations/0012_auto_20230317_0927.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/migrations/0013_auto_20230317_1534.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/migrations/0014_add_missing_fields_to_django_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/migrations/0015_set_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15924 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15748 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 08:14:51.000000 openimis-be-location-1.5.2/location/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:15:08.347416 openimis-be-location-1.5.2/openimis_be_location.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-24 08:15:08.000000 openimis-be-location-1.5.2/openimis_be_location.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-24 08:15:08.000000 openimis-be-location-1.5.2/openimis_be_location.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 08:15:08.000000 openimis-be-location-1.5.2/openimis_be_location.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 08:15:08.000000 openimis-be-location-1.5.2/openimis_be_location.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 08:15:08.000000 openimis-be-location-1.5.2/openimis_be_location.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 08:15:08.347416 openimis-be-location-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-24 08:15:05.000000 openimis-be-location-1.5.2/setup.py
```

### Comparing `openimis-be-location-1.5.1/LICENSE.md` & `openimis-be-location-1.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/PKG-INFO` & `openimis-be-location-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-location
-Version: 1.5.1
+Version: 1.5.2
 Summary: The openIMIS Backend Location reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-location-1.5.1/README.md` & `openimis-be-location-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/apps.py` & `openimis-be-location-1.5.2/location/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/dataloaders.py` & `openimis-be-location-1.5.2/location/dataloaders.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/gql_mutations.py` & `openimis-be-location-1.5.2/location/gql_mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/gql_queries.py` & `openimis-be-location-1.5.2/location/gql_queries.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,39 @@
+from core.gql.custom_lookup import NotEqual
 import graphene
 import base64
 from graphene_django import DjangoObjectType
 from django.core.exceptions import PermissionDenied
 from django.utils.translation import gettext as _
 from core import prefix_filterset, filter_validity, ExtendedConnection
 from location.apps import LocationConfig
 from location.models import HealthFacilityLegalForm, Location, HealthFacilitySubLevel, HealthFacilityCatchment, \
     HealthFacility, UserDistrict, OfficerVillage
+from django.db.models import Field
 
 
 class LocationGQLType(DjangoObjectType):
     client_mutation_id = graphene.String()
+    Field.register_lookup(NotEqual)
 
     def resolve_parent(self, info):
         if not info.context.user.is_authenticated:
             raise PermissionDenied(_("unauthorized"))
         if "location_loader" in info.context.dataloaders and self.parent_id:
             return info.context.dataloaders["location_loader"].load(self.parent_id)
         return self.parent
 
     class Meta:
         model = Location
         interfaces = (graphene.relay.Node,)
         filter_fields = {
             "id": ["exact"],
             "uuid": ["exact"],
-            "code": ["exact", "istartswith", "icontains", "iexact"],
-            "name": ["exact", "istartswith", "icontains", "iexact"],
+            "code": ["exact", "istartswith", "icontains", "iexact", "ne"],
+            "name": ["exact", "istartswith", "icontains", "iexact", "ne"],
             "type": ["exact"],
             "parent__uuid": ["exact", "in"],  # can't import itself!
             "parent__parent__uuid": ["exact", "in"],  # can't import itself!
             "parent__parent__parent__uuid": ["exact", "in"],  # can't import itself!
             "parent__id": ["exact", "in"],  # can't import itself!
         }
 
@@ -42,14 +45,35 @@
         return location_mutation.mutation.client_mutation_id if location_mutation else None
 
     @classmethod
     def get_queryset(cls, queryset, info):
         return Location.get_queryset(queryset, info.context.user)
 
 
+class LocationAllGQLType(LocationGQLType):
+    class Meta:
+        model = Location
+        interfaces = (graphene.relay.Node,)
+        filter_fields = {
+            "id": ["exact"],
+            "uuid": ["exact"],
+            "code": ["exact", "istartswith", "icontains", "iexact"],
+            "name": ["exact", "istartswith", "icontains", "iexact"],
+            "type": ["exact"],
+            "parent__uuid": ["exact", "in"],  # can't import itself!
+            "parent__parent__uuid": ["exact", "in"],  # can't import itself!
+            "parent__parent__parent__uuid": ["exact", "in"],  # can't import itself!
+            "parent__id": ["exact", "in"],  # can't import itself!
+        }
+
+    @classmethod
+    def get_queryset(cls, queryset, info):
+        return Location.objects.filter(*filter_validity())
+
+
 class HealthFacilityLegalFormGQLType(DjangoObjectType):
     class Meta:
         model = HealthFacilityLegalForm
 
 
 class HealthFacilitySubLevelGQLType(DjangoObjectType):
     class Meta:
```

### Comparing `openimis-be-location-1.5.1/location/migrations/0001_initial.py` & `openimis-be-location-1.5.2/location/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/migrations/0002_location.py` & `openimis-be-location-1.5.2/location/migrations/0002_location.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/migrations/0003_userdistrict.py` & `openimis-be-location-1.5.2/location/migrations/0003_userdistrict.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/migrations/0004_locationmutation.py` & `openimis-be-location-1.5.2/location/migrations/0004_locationmutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/migrations/0005_healthfacilitycatchment_healthfacilitylegalform_healthfacilitymutation_healthfacilitysublevel.py` & `openimis-be-location-1.5.2/location/migrations/0005_healthfacilitycatchment_healthfacilitylegalform_healthfacilitymutation_healthfacilitysublevel.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/migrations/0006_users_api.py` & `openimis-be-location-1.5.2/location/migrations/0006_users_api.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/migrations/0007_auto_20211103_1046.py` & `openimis-be-location-1.5.2/location/migrations/0007_auto_20211103_1046.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/migrations/0008_add_enrollment_officer_gql_query_location_right.py` & `openimis-be-location-1.5.2/location/migrations/0008_add_enrollment_officer_gql_query_location_right.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/migrations/0009_add_location_read_right.py` & `openimis-be-location-1.5.2/location/migrations/0009_add_location_read_right.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/migrations/0010_insert_create_region_location_perms.py` & `openimis-be-location-1.5.2/location/migrations/0010_insert_create_region_location_perms.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/migrations/0011_auto_20230317_0924.py` & `openimis-be-location-1.5.2/location/migrations/0011_auto_20230317_0924.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/migrations/0013_auto_20230317_1534.py` & `openimis-be-location-1.5.2/location/migrations/0013_auto_20230317_1534.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/migrations/0014_add_missing_fields_to_django_scheme.py` & `openimis-be-location-1.5.2/location/migrations/0014_add_missing_fields_to_django_scheme.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/migrations/0015_set_managed_to_true.py` & `openimis-be-location-1.5.2/location/migrations/0015_set_managed_to_true.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/models.py` & `openimis-be-location-1.5.2/location/models.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/schema.py` & `openimis-be-location-1.5.2/location/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,18 @@
         showHistory=graphene.Boolean(),
         orderBy=graphene.List(of_type=graphene.String)
     )
     locations = OrderedDjangoFilterConnectionField(
         LocationGQLType,
         orderBy=graphene.List(of_type=graphene.String),
     )
+    locations_all = OrderedDjangoFilterConnectionField(
+        LocationAllGQLType,
+        orderBy=graphene.List(of_type=graphene.String)
+    )
     locations_str = DjangoFilterConnectionField(
         LocationGQLType,
         str=graphene.String(),
     )
     user_districts = graphene.List(
         UserDistrictGQLType
     )
@@ -36,14 +40,15 @@
                                       description="Returns list of locations assigned to a given enrolment officer.")
     health_facilities_str = DjangoFilterConnectionField(
         HealthFacilityGQLType,
         str=graphene.String(),
         region_uuid=graphene.String(),
         district_uuid=graphene.String(),
         districts_uuids=graphene.List(of_type=graphene.String),
+        ignore_location=graphene.Boolean()
     )
     validate_location_code = graphene.Field(
         graphene.Boolean,
         location_code=graphene.String(required=True),
         description="Checks that the specified location code is unique."
     )
     validate_health_facility_code = graphene.Field(
@@ -81,14 +86,20 @@
 
     def resolve_locations(self, info, **kwargs):
         # OMT-281 allow querying to anyone, with limitations in the get_queryset
         # if not info.context.user.has_perms(LocationConfig.gql_query_locations_perms):
         if info.context.user.is_anonymous:
             raise PermissionDenied(_("unauthorized"))
 
+    def resolve_locations_all(self, info, **kwargs):
+        # OMT-281 allow querying to anyone, with limitations in the get_queryset
+        # if not info.context.user.has_perms(LocationConfig.gql_query_locations_perms):
+        if info.context.user.is_anonymous:
+            raise PermissionDenied(_("unauthorized"))
+
     def resolve_locations_str(self, info, **kwargs):
         if info.context.user.is_anonymous:
             raise PermissionDenied(_("unauthorized"))
 
         queryset = Location.get_queryset(None, info.context.user)
         filters = [*filter_validity(**kwargs)]
 
@@ -111,17 +122,21 @@
         if district_uuid is not None:
             filters += [Q(location__uuid=district_uuid)]
         if district_uuids is not None:
             if None not in district_uuids:
                 filters += [Q(location__uuid__in=district_uuids)]
         if region_uuid is not None:
             filters += [Q(location__parent__uuid=region_uuid)]
-        if settings.ROW_SECURITY:
-            dist = UserDistrict.get_user_districts(info.context.user._u)
-            filters += [Q(location__id__in=[l.location_id for l in dist])]
+
+        if (kwargs.get('ignore_location') == False or kwargs.get('ignore_location') is None):
+
+          if settings.ROW_SECURITY:
+              dist = UserDistrict.get_user_districts(info.context.user._u)
+
+              filters += [Q(location__id__in=[l.location_id for l in dist])]
         return HealthFacility.objects.filter(*filters)
 
     def resolve_user_districts(self, info, **kwargs):
         if info.context.user.is_anonymous:
             raise NotImplementedError(
                 'Anonymous Users are not registered for districts')
         if not isinstance(info.context.user._u, core_models.InteractiveUser):
```

### Comparing `openimis-be-location-1.5.1/location/services.py` & `openimis-be-location-1.5.2/location/services.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/test_graphql.py` & `openimis-be-location-1.5.2/location/test_graphql.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/location/test_helpers.py` & `openimis-be-location-1.5.2/location/test_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/openimis_be_location.egg-info/PKG-INFO` & `openimis-be-location-1.5.2/openimis_be_location.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-location
-Version: 1.5.1
+Version: 1.5.2
 Summary: The openIMIS Backend Location reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-location-1.5.1/openimis_be_location.egg-info/SOURCES.txt` & `openimis-be-location-1.5.2/openimis_be_location.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.1/setup.py` & `openimis-be-location-1.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-location',
-    version='v1.5.1',
+    version='v1.5.2',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Location reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
```

