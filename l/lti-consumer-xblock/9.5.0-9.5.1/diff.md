# Comparing `tmp/lti-consumer-xblock-9.5.0.tar.gz` & `tmp/lti-consumer-xblock-9.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lti-consumer-xblock-9.5.0.tar", last modified: Mon May 15 20:31:54 2023, max compression
+gzip compressed data, was "lti-consumer-xblock-9.5.1.tar", last modified: Fri May 19 20:26:56 2023, max compression
```

## Comparing `lti-consumer-xblock-9.5.0.tar` & `lti-consumer-xblock-9.5.1.tar`

### file list

```diff
@@ -1,246 +1,246 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (122)    14454 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13670 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.693691 lti-consumer-xblock-9.5.0/lti_consumer/
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      672 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     6551 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/data.py
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.693691 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15317 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.693691 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/contrib/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5551 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/contrib/django.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.693691 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/contrib/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/contrib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/contrib/tests/test_django.py
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5976 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.693691 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14154 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/tests/test_oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.697691 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/ags.py
--rw-r--r--   0 runner    (1001) docker     (122)     3083 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    34236 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.697691 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.697691 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)      388 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      554 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3887 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10557 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/key_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/nprs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.697691 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.697691 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/extensions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.697691 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)     9875 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/test_ags.py
--rw-r--r--   0 runner    (1001) docker     (122)    42504 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/test_deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)    10270 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/test_key_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/test_nrps.py
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    72133 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/lti_xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.701691 lti-consumer-xblock-9.5.0/lti_consumer/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0002_ltiagslineitem.py
--rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0003_ltiagsscore.py
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0004_keyset_mgmt_to_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0005_migrate_keyset_to_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0007_ltidlcontentitem.py
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0008_fix_uuid_backfill.py
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0009_backfill-empty-string-config-id.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0012_rename_courseeditltifieldsenabledflag_model.py
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0013_auto_20210712_1352.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0014_adds_external_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0015_add_additional_1p3_fields.py
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32021 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/outcomes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.701691 lti-consumer-xblock-9.5.0/lti_consumer/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11593 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/plugin/compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)    35442 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/plugin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.685691 lti-consumer-xblock-9.5.0/lti_consumer/public/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.685691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.701691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ar/
--rw-r--r--   0 runner    (1001) docker     (122)    22730 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ar/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.701691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/en/
--rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/en/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.701691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/es_419/
--rw-r--r--   0 runner    (1001) docker     (122)    23422 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/es_419/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.701691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/fr/
--rw-r--r--   0 runner    (1001) docker     (122)    21751 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/fr/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.701691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/he/
--rw-r--r--   0 runner    (1001) docker     (122)    20445 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/he/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.701691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/hi/
--rw-r--r--   0 runner    (1001) docker     (122)     3735 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/hi/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.701691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/it/
--rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/it/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.701691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ja/
--rw-r--r--   0 runner    (1001) docker     (122)    17362 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ja/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ko/
--rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ko/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/pt_BR/
--rw-r--r--   0 runner    (1001) docker     (122)     4601 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/pt_BR/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/pt_PT/
--rw-r--r--   0 runner    (1001) docker     (122)    13621 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/pt_PT/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ru/
--rw-r--r--   0 runner    (1001) docker     (122)     3772 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ru/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/zh_CN/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/signals/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/signals/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/static/css/student.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/static/js/
--rw-r--r--   0 runner    (1001) docker     (122)    12186 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/static/js/xblock_lti_consumer.js
--rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/static/js/xblock_studio_view.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/static/sass/
--rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/static/sass/student.scss
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/dl_response_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/dl_response_saved.html
--rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/render_dl_content.html
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/render_html.html
--rw-r--r--   0 runner    (1001) docker     (122)      890 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/render_image.html
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/render_link.html
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/render_lti_resource_link.html
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_1p3_launch.html
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_1p3_permission_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_1p3_studio.html
--rw-r--r--   0 runner    (1001) docker     (122)      364 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_iframe.html
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_launch.html
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_launch_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_proctoring_start_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      519 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_start_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/html/student.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/templates/xml/
--rw-r--r--   0 runner    (1001) docker     (122)      798 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templates/xml/outcome_service_response.xml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.705691 lti-consumer-xblock-9.5.0/lti_consumer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      780 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templatetags/get_dl_lti_launch_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/templatetags/lti_sanitize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.709691 lti-consumer-xblock-9.5.0/lti_consumer/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.709691 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.709691 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11758 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/test_proctoring.py
--rw-r--r--   0 runner    (1001) docker     (122)    25574 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)    38579 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/test_views_lti_ags.py
--rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)    10559 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
--rw-r--r--   0 runner    (1001) docker     (122)    26379 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)    84733 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_lti_xblock.py
--rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    16718 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_outcomes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/track.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.709691 lti-consumer-xblock-9.5.0/lti_consumer/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.709691 lti-consumer-xblock-9.5.0/lti_consumer/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10252 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/ar/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/ar/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.709691 lti-consumer-xblock-9.5.0/lti_consumer/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/en/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/en/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.709691 lti-consumer-xblock-9.5.0/lti_consumer/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    20799 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/es_419/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26467 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/es_419/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.709691 lti-consumer-xblock-9.5.0/lti_consumer/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    18761 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/fr/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25340 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/fr/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/lti_consumer/translations/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9166 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/he/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/lti_consumer/translations/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9608 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/he/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    21499 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/he/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/hi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/lti_consumer/translations/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/hi/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16407 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/hi/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/lti_consumer/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9838 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/lti_consumer/translations/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/ko_KR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16477 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16884 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10221 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18852 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/lti_consumer/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/ru/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16547 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/ru/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     1987 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.689691 lti-consumer-xblock-9.5.0/lti_consumer/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/lti_consumer/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/zh_CN/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16458 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)    10931 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/lti_consumer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/lti_consumer_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14454 2023-05-15 20:31:54.000000 lti-consumer-xblock-9.5.0/lti_consumer_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7644 2023-05-15 20:31:54.000000 lti-consumer-xblock-9.5.0/lti_consumer_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-05-15 20:31:54.000000 lti-consumer-xblock-9.5.0/lti_consumer_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-05-15 20:31:54.000000 lti-consumer-xblock-9.5.0/lti_consumer_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-15 20:31:54.000000 lti-consumer-xblock-9.5.0/lti_consumer_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-15 20:31:54.000000 lti-consumer-xblock-9.5.0/lti_consumer_xblock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 20:31:54.713692 lti-consumer-xblock-9.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-15 20:31:54.717692 lti-consumer-xblock-9.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-05-15 20:31:50.000000 lti-consumer-xblock-9.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.955956 lti-consumer-xblock-9.5.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)    14454 2023-05-19 20:26:56.955956 lti-consumer-xblock-9.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13670 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.923956 lti-consumer-xblock-9.5.1/lti_consumer/
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      672 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6551 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.927956 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15317 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.927956 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/contrib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5551 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/contrib/django.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.927956 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/contrib/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/contrib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/contrib/tests/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5976 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.927956 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14154 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/tests/test_oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.931956 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3081 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35146 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.931956 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.935956 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/extensions/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/extensions/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)      388 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/extensions/rest_framework/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      554 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3887 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/extensions/rest_framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10557 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/key_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/nprs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.935956 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.935956 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.935956 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9875 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/test_ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44438 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/test_deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10270 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/test_key_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/test_nrps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    72133 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/lti_xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.943956 lti-consumer-xblock-9.5.1/lti_consumer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/migrations/0002_ltiagslineitem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/migrations/0003_ltiagsscore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/migrations/0004_keyset_mgmt_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/migrations/0005_migrate_keyset_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/migrations/0007_ltidlcontentitem.py
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/migrations/0008_fix_uuid_backfill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/migrations/0009_backfill-empty-string-config-id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/migrations/0012_rename_courseeditltifieldsenabledflag_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/migrations/0013_auto_20210712_1352.py
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/migrations/0014_adds_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/migrations/0015_add_additional_1p3_fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32021 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/outcomes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.943956 lti-consumer-xblock-9.5.1/lti_consumer/plugin/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11593 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/plugin/compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/plugin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35475 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/plugin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.907956 lti-consumer-xblock-9.5.1/lti_consumer/public/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.907956 lti-consumer-xblock-9.5.1/lti_consumer/public/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.911956 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.943956 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/ar/
+-rw-r--r--   0 runner    (1001) docker     (122)    22730 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/ar/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.943956 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/en/
+-rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/en/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.943956 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/es_419/
+-rw-r--r--   0 runner    (1001) docker     (122)    23422 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/es_419/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.943956 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/fr/
+-rw-r--r--   0 runner    (1001) docker     (122)    21751 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/fr/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.943956 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/he/
+-rw-r--r--   0 runner    (1001) docker     (122)    20445 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/he/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.943956 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/hi/
+-rw-r--r--   0 runner    (1001) docker     (122)     3735 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/hi/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.943956 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/it/
+-rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/it/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.943956 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/ja/
+-rw-r--r--   0 runner    (1001) docker     (122)    17362 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/ja/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.943956 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/ko/
+-rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/ko/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.943956 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/pt_BR/
+-rw-r--r--   0 runner    (1001) docker     (122)     4601 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/pt_BR/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.943956 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/pt_PT/
+-rw-r--r--   0 runner    (1001) docker     (122)    13621 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/pt_PT/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.943956 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/ru/
+-rw-r--r--   0 runner    (1001) docker     (122)     3772 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/ru/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.943956 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/zh_CN/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.943956 lti-consumer-xblock-9.5.1/lti_consumer/signals/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/signals/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.911956 lti-consumer-xblock-9.5.1/lti_consumer/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.943956 lti-consumer-xblock-9.5.1/lti_consumer/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/static/css/student.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.943956 lti-consumer-xblock-9.5.1/lti_consumer/static/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    12186 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/static/js/xblock_lti_consumer.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/static/js/xblock_studio_view.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.943956 lti-consumer-xblock-9.5.1/lti_consumer/static/sass/
+-rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/static/sass/student.scss
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.911956 lti-consumer-xblock-9.5.1/lti_consumer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.947956 lti-consumer-xblock-9.5.1/lti_consumer/templates/html/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.947956 lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti-dl/
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti-dl/dl_response_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti-dl/dl_response_saved.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti-dl/render_dl_content.html
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti-dl/render_html.html
+-rw-r--r--   0 runner    (1001) docker     (122)      890 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti-dl/render_image.html
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti-dl/render_link.html
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti-dl/render_lti_resource_link.html
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti_1p3_launch.html
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti_1p3_permission_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti_1p3_studio.html
+-rw-r--r--   0 runner    (1001) docker     (122)      364 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti_iframe.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti_launch.html
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti_launch_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti_proctoring_start_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti_start_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/templates/html/student.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.947956 lti-consumer-xblock-9.5.1/lti_consumer/templates/xml/
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/templates/xml/outcome_service_response.xml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.947956 lti-consumer-xblock-9.5.1/lti_consumer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      780 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/templatetags/get_dl_lti_launch_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/templatetags/lti_sanitize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.947956 lti-consumer-xblock-9.5.1/lti_consumer/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.947956 lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.951956 lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/plugin/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11758 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/plugin/test_proctoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25574 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/plugin/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38579 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/plugin/test_views_lti_ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10559 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26379 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    84733 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/test_lti_xblock.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16718 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/test_outcomes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/track.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.951956 lti-consumer-xblock-9.5.1/lti_consumer/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.911956 lti-consumer-xblock-9.5.1/lti_consumer/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.951956 lti-consumer-xblock-9.5.1/lti_consumer/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10252 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/ar/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/ar/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.915956 lti-consumer-xblock-9.5.1/lti_consumer/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.951956 lti-consumer-xblock-9.5.1/lti_consumer/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/en/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/en/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.915956 lti-consumer-xblock-9.5.1/lti_consumer/translations/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.951956 lti-consumer-xblock-9.5.1/lti_consumer/translations/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    20799 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/es_419/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26467 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/es_419/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.915956 lti-consumer-xblock-9.5.1/lti_consumer/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.951956 lti-consumer-xblock-9.5.1/lti_consumer/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    18761 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/fr/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25340 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/fr/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.915956 lti-consumer-xblock-9.5.1/lti_consumer/translations/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.951956 lti-consumer-xblock-9.5.1/lti_consumer/translations/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9166 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.915956 lti-consumer-xblock-9.5.1/lti_consumer/translations/he/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.951956 lti-consumer-xblock-9.5.1/lti_consumer/translations/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9608 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/he/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    21499 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/he/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.915956 lti-consumer-xblock-9.5.1/lti_consumer/translations/hi/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.951956 lti-consumer-xblock-9.5.1/lti_consumer/translations/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/hi/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16407 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/hi/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.915956 lti-consumer-xblock-9.5.1/lti_consumer/translations/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.951956 lti-consumer-xblock-9.5.1/lti_consumer/translations/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9838 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.915956 lti-consumer-xblock-9.5.1/lti_consumer/translations/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.951956 lti-consumer-xblock-9.5.1/lti_consumer/translations/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/ko_KR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16477 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.919956 lti-consumer-xblock-9.5.1/lti_consumer/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.951956 lti-consumer-xblock-9.5.1/lti_consumer/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16884 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.919956 lti-consumer-xblock-9.5.1/lti_consumer/translations/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.951956 lti-consumer-xblock-9.5.1/lti_consumer/translations/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10221 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18852 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.919956 lti-consumer-xblock-9.5.1/lti_consumer/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.955956 lti-consumer-xblock-9.5.1/lti_consumer/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/ru/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16547 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/ru/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1987 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.919956 lti-consumer-xblock-9.5.1/lti_consumer/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.955956 lti-consumer-xblock-9.5.1/lti_consumer/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/zh_CN/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16458 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)    10931 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/lti_consumer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.955956 lti-consumer-xblock-9.5.1/lti_consumer_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14454 2023-05-19 20:26:56.000000 lti-consumer-xblock-9.5.1/lti_consumer_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7644 2023-05-19 20:26:56.000000 lti-consumer-xblock-9.5.1/lti_consumer_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-05-19 20:26:56.000000 lti-consumer-xblock-9.5.1/lti_consumer_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-05-19 20:26:56.000000 lti-consumer-xblock-9.5.1/lti_consumer_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-19 20:26:56.000000 lti-consumer-xblock-9.5.1/lti_consumer_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-19 20:26:56.000000 lti-consumer-xblock-9.5.1/lti_consumer_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 20:26:56.955956 lti-consumer-xblock-9.5.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-19 20:26:56.955956 lti-consumer-xblock-9.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-05-19 20:26:52.000000 lti-consumer-xblock-9.5.1/setup.py
```

### Comparing `lti-consumer-xblock-9.5.0/LICENSE` & `lti-consumer-xblock-9.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/NOTICE` & `lti-consumer-xblock-9.5.1/NOTICE`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/PKG-INFO` & `lti-consumer-xblock-9.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lti-consumer-xblock
-Version: 9.5.0
+Version: 9.5.1
 Summary: This XBlock implements the consumer side of the LTI specification.
 Home-page: https://github.com/openedx/xblock-lti-consumer
 Author: Open edX project
 Author-email: oscm@edx.org
 Keywords: lti consumer xblock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `lti-consumer-xblock-9.5.0/README.rst` & `lti-consumer-xblock-9.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/admin.py` & `lti-consumer-xblock-9.5.1/lti_consumer/admin.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/api.py` & `lti-consumer-xblock-9.5.1/lti_consumer/api.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/apps.py` & `lti-consumer-xblock-9.5.1/lti_consumer/apps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/data.py` & `lti-consumer-xblock-9.5.1/lti_consumer/data.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/filters.py` & `lti-consumer-xblock-9.5.1/lti_consumer/filters.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/forms.py` & `lti-consumer-xblock-9.5.1/lti_consumer/forms.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/consumer.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/contrib/django.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/contrib/django.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/contrib/tests/test_django.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/contrib/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/oauth.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/oauth.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/tests/test_consumer.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p1/tests/test_oauth.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p1/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/ags.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/constants.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,19 +61,17 @@
     'https://purl.imsglobal.org/spec/lti-ags/scope/lineitem.readonly',
     'https://purl.imsglobal.org/spec/lti-ags/scope/lineitem',
     'https://purl.imsglobal.org/spec/lti-ags/scope/result.readonly',
     'https://purl.imsglobal.org/spec/lti-ags/scope/score',
 
     # LTI-NRPS Scopes
     'https://purl.imsglobal.org/spec/lti-nrps/scope/contextmembership.readonly',
-
-    # ACS Scope
-    'https://purl.imsglobal.org/spec/lti-ap/scope/control.all',
 ]
 
+LTI_1P3_ACS_SCOPE = 'https://purl.imsglobal.org/spec/lti-ap/scope/control.all'
 
 LTI_DEEP_LINKING_ACCEPTED_TYPES = [
     'ltiResourceLink',
     'link',
     'html',
     'image',
     # TODO: implement "file" support,
```

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/consumer.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from . import constants, exceptions
 from .constants import (
     LTI_1P3_ROLE_MAP,
     LTI_BASE_MESSAGE,
     LTI_1P3_ACCESS_TOKEN_REQUIRED_CLAIMS,
     LTI_1P3_ACCESS_TOKEN_SCOPES,
+    LTI_1P3_ACS_SCOPE,
     LTI_1P3_CONTEXT_TYPE,
     LTI_PROCTORING_DATA_KEYS,
 )
 from .key_handlers import ToolKeyHandler, PlatformKeyHandler
 from .ags import LtiAgs
 from .deep_linking import LtiDeepLinking
 from .nprs import LtiNrps
@@ -27,14 +28,15 @@
 log = logging.getLogger(__name__)
 
 
 class LtiConsumer1p3:
     """
     LTI 1.3 Consumer Implementation
     """
+
     def __init__(
             self,
             iss,
             lti_oidc_url,
             lti_launch_url,
             client_id,
             deployment_id,
@@ -403,14 +405,27 @@
 
     def get_public_keyset(self):
         """
         Export Public JWK
         """
         return self.key_handler.get_public_jwk()
 
+    def _check_if_scope_is_valid(self, scope):
+        """
+        Helper function to return the list of valid scopes present in the
+        request to the access token endpoint.
+        """
+        # Currently there are no scopes, because there is no use for
+        # these access tokens until a tool needs to access the LMS.
+        # LTI Advantage extensions make use of this.
+        # TODO: Make this function should only return the NRPS and AGS scopes if those features are enabled.
+        if scope in LTI_1P3_ACCESS_TOKEN_SCOPES:
+            return True
+        return False
+
     def access_token(self, token_request_data):
         """
         Validate request and return JWT access token.
 
         This complies to IMS Security Framework and accepts a JWT
         as a secret for the client credentials grant.
         See this section:
@@ -450,21 +465,22 @@
         self.tool_jwt.validate_and_decode(
             token_request_data['client_assertion']
         )
 
         # Check scopes and only return valid and supported ones
         valid_scopes = []
         requested_scopes = token_request_data['scope'].split(' ')
-
         for scope in requested_scopes:
-            # Currently there are no scopes, because there is no use for
-            # these access tokens until a tool needs to access the LMS.
-            # LTI Advantage extensions make use of this.
-            if scope in LTI_1P3_ACCESS_TOKEN_SCOPES:
+            if self._check_if_scope_is_valid(scope):
                 valid_scopes.append(scope)
+            else:
+                log.warning(
+                    f'Scope: {scope} found in the request is not a valid '
+                    f'LTI 1.3 access token or ACS scope'
+                )
 
         # Scopes are space separated as described in
         # https://tools.ietf.org/html/rfc6749
         scopes_str = " ".join(valid_scopes)
 
         # This response is compliant with RFC 6749
         # https://tools.ietf.org/html/rfc6749#section-4.4.3
@@ -540,14 +556,15 @@
     the following LTI Advantage Services:
 
     * Assignments and Grades Service (LTI-AGS): Allows tools to
       retrieve and send back grades into the platform.
       Note: this is a partial implementation with read-only LineItems.
       Reference spec: https://www.imsglobal.org/spec/lti-ags/v2p0
     """
+
     def __init__(self, *args, **kwargs):
         """
         Override parent class and set up required LTI Advantage variables.
         """
         super().__init__(*args, **kwargs)
 
         # LTI Advantage services
@@ -752,14 +769,15 @@
     This consumer currently only supports the "Assessment Proctoring Messages" and the proctoring assessment flow.
     It does not currently support the Assessment Control Service.
 
     The LtiProctoringConsumer requires necessary context to work properly, including data like attempt_number,
     resource_link, etc. This information is provided to the consumer through the set_proctoring_data method, which
     is called from the consuming context to pass in necessary data.
     """
+
     def __init__(
         self,
         iss,
         lti_oidc_url,
         lti_launch_url,
         client_id,
         deployment_id,
@@ -873,14 +891,23 @@
         self.set_extra_claim(proctoring_claims)
 
         if self.proctoring_data.get("assessment_control_url"):
             self.set_extra_claim(self.get_assessment_control_claim())
 
         return super().generate_launch_request(preflight_response)
 
+    def _check_if_scope_is_valid(self, scope):
+        """
+        Override of Lti1p3Consumer's _check_if_scope_is_valid
+        that accounts for the ACS scope for proctoring.
+        """
+        if scope in (LTI_1P3_ACCESS_TOKEN_SCOPES, LTI_1P3_ACS_SCOPE):
+            return True
+        return False
+
     def check_and_decode_token(self, token):
         """
         Decodes a Tool JWT token and validates OAuth and LTI Proctoring Services specificatin related claims. Returns a
         dictionary representation of key proctoring claims in the Tool JWT token.
 
         Arguments:
             * token (string): a JWT
```

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/deep_linking.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/exceptions.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/exceptions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/extensions/rest_framework/utils.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/extensions/rest_framework/utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/key_handlers.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/key_handlers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/nprs.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/nprs.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/test_ags.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/test_ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/test_consumer.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/test_consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,20 +35,34 @@
 NONCE = "1234"
 STATE = "ABCD"
 # Consider storing a fixed key
 RSA_KEY_ID = "1"
 RSA_KEY = RSA.generate(2048).export_key('PEM')
 
 
+def _generate_token_request_data(token, scope):
+    """
+    Helper function to generate requests to the access_token endpoint
+    """
+    return {
+        # We don't actually care about these 2 first values
+        "grant_type": "client_credentials",
+        "client_assertion_type": "urn:ietf:params:oauth:client-assertion-type:jwt-bearer",
+        "client_assertion": token,
+        "scope": scope,
+    }
+
+
 # Test classes
 @ddt.ddt
 class TestLti1p3Consumer(TestCase):
     """
     Unit tests for LtiConsumer1p3
     """
+
     def setUp(self):
         super().setUp()
 
         # Set up consumer
         self.lti_consumer = LtiConsumer1p3(
             iss=ISS,
             lti_oidc_url=OIDC_URL,
@@ -538,26 +552,39 @@
         with self.assertRaises(exceptions.MissingRequiredClaim):
             self.lti_consumer.access_token({})
 
     def test_access_token_invalid_jwt(self):
         """
         Check if access token with invalid request data raises.
         """
-        request_data = {
-            "grant_type": "client_credentials",
-            "client_assertion_type": "urn:ietf:params:oauth:client-assertion-type:jwt-bearer",
-            # This should be a valid JWT
-            "client_assertion": "invalid-jwt",
-            # Scope can be empty
-            "scope": "",
-        }
+        request_data = _generate_token_request_data("invalid_jwt", "")
 
         with self.assertRaises(exceptions.MalformedJwtToken):
             self.lti_consumer.access_token(request_data)
 
+    def test_access_token_no_acs(self):
+        """
+        Check that ACS does not work for the access token in the
+        default LTI 1.3 consumer
+        """
+        # Generate a dummy, but valid JWT
+        token = self.lti_consumer.key_handler.encode_and_sign(
+            {
+                "test": "test"
+            },
+            expiration=1000
+        )
+
+        request_data = _generate_token_request_data(token, "https://purl.imsglobal.org/spec/lti-ap/scope/control.all")
+
+        response = self.lti_consumer.access_token(request_data)
+
+        # Check no ACS scope present in returned token
+        self.assertEqual(response.get('scope'), '')
+
     def test_access_token(self):
         """
         Check if a valid access token is returned.
 
         Since we're using the same key for both tool and
         platform here, we can make use of the internal
         _decode_token to check validity.
@@ -566,23 +593,15 @@
         token = self.lti_consumer.key_handler.encode_and_sign(
             {
                 "test": "test"
             },
             expiration=1000
         )
 
-        request_data = {
-            # We don't actually care about these 2 first values
-            "grant_type": "client_credentials",
-            "client_assertion_type": "urn:ietf:params:oauth:client-assertion-type:jwt-bearer",
-            # This should be a valid JWT
-            "client_assertion": token,
-            # Scope can be empty
-            "scope": "",
-        }
+        request_data = _generate_token_request_data(token, "")
 
         response = self.lti_consumer.access_token(request_data)
 
         # Check response contents
         self.assertIn('access_token', response)
         self.assertEqual(response.get('token_type'), 'bearer')
         self.assertEqual(response.get('expires_in'), 3600)
@@ -652,14 +671,15 @@
 
 
 @ddt.ddt
 class TestLtiAdvantageConsumer(TestCase):
     """
     Unit tests for LtiAdvantageConsumer
     """
+
     def setUp(self):
         super().setUp()
 
         # Set up consumer
         self.lti_consumer = LtiAdvantageConsumer(
             iss=ISS,
             lti_oidc_url=OIDC_URL,
@@ -895,14 +915,15 @@
 
 
 @ddt.ddt
 class TestLtiProctoringConsumer(TestCase):
     """
     Unit tests for LtiProctoringConsumer
     """
+
     def setUp(self):
         super().setUp()
 
         # Set up consumer
         self.lti_consumer = LtiProctoringConsumer(
             iss=ISS,
             lti_oidc_url=OIDC_URL,
@@ -1162,14 +1183,54 @@
             message=start_assessment_response,
             expiration=3600
         )
 
         with self.assertRaises(MissingRequiredClaim):
             self.lti_consumer.check_and_decode_token(encoded_token)
 
+    def test_access_token_no_valid_scopes(self):
+        """
+        Ensure that the no scopes are returned in the access token if the request scopes are invalid
+        """
+        # Generate a dummy, but valid JWT
+        token = self.lti_consumer.key_handler.encode_and_sign(
+            {
+                "test": "test"
+            },
+            expiration=1000
+        )
+
+        # This should be a valid JWT w/ the ACS scope
+        request_data = _generate_token_request_data(token, "invalid_scope")
+
+        response = self.lti_consumer.access_token(request_data)
+
+        # Check that the response has the ACS scope
+        self.assertEqual(response.get('scope'), "")
+
+    def test_access_token(self):
+        """
+        Ensure that the ACS scope is added based on the request to the access token endpoint
+        """
+        # Generate a dummy, but valid JWT
+        token = self.lti_consumer.key_handler.encode_and_sign(
+            {
+                "test": "test"
+            },
+            expiration=1000
+        )
+
+        # This should be a valid JWT w/ the ACS scope
+        request_data = _generate_token_request_data(token, "https://purl.imsglobal.org/spec/lti-ap/scope/control.all")
+
+        response = self.lti_consumer.access_token(request_data)
+
+        # Check that the response has the ACS scope
+        self.assertEqual(response.get('scope'), "https://purl.imsglobal.org/spec/lti-ap/scope/control.all")
+
     def test_valid_check_and_decode_token(self):
         """
         Ensures that a valid LtiStartAssessment JWT is validated successfully.
         """
         self.lti_consumer.set_proctoring_data(
             attempt_number="attempt_number",
             session_data="session_data",
```

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/test_deep_linking.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/test_deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/test_key_handlers.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/test_key_handlers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_1p3/tests/test_nrps.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_1p3/tests/test_nrps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/lti_xblock.py` & `lti-consumer-xblock-9.5.1/lti_consumer/lti_xblock.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0001_initial.py` & `lti-consumer-xblock-9.5.1/lti_consumer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0002_ltiagslineitem.py` & `lti-consumer-xblock-9.5.1/lti_consumer/migrations/0002_ltiagslineitem.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0003_ltiagsscore.py` & `lti-consumer-xblock-9.5.1/lti_consumer/migrations/0003_ltiagsscore.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0004_keyset_mgmt_to_model.py` & `lti-consumer-xblock-9.5.1/lti_consumer/migrations/0004_keyset_mgmt_to_model.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0005_migrate_keyset_to_model.py` & `lti-consumer-xblock-9.5.1/lti_consumer/migrations/0005_migrate_keyset_to_model.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py` & `lti-consumer-xblock-9.5.1/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0007_ltidlcontentitem.py` & `lti-consumer-xblock-9.5.1/lti_consumer/migrations/0007_ltidlcontentitem.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0008_fix_uuid_backfill.py` & `lti-consumer-xblock-9.5.1/lti_consumer/migrations/0008_fix_uuid_backfill.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0009_backfill-empty-string-config-id.py` & `lti-consumer-xblock-9.5.1/lti_consumer/migrations/0009_backfill-empty-string-config-id.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py` & `lti-consumer-xblock-9.5.1/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py` & `lti-consumer-xblock-9.5.1/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0013_auto_20210712_1352.py` & `lti-consumer-xblock-9.5.1/lti_consumer/migrations/0013_auto_20210712_1352.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0014_adds_external_id.py` & `lti-consumer-xblock-9.5.1/lti_consumer/migrations/0014_adds_external_id.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0015_add_additional_1p3_fields.py` & `lti-consumer-xblock-9.5.1/lti_consumer/migrations/0015_add_additional_1p3_fields.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py` & `lti-consumer-xblock-9.5.1/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py` & `lti-consumer-xblock-9.5.1/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/models.py` & `lti-consumer-xblock-9.5.1/lti_consumer/models.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/outcomes.py` & `lti-consumer-xblock-9.5.1/lti_consumer/outcomes.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/plugin/compat.py` & `lti-consumer-xblock-9.5.1/lti_consumer/plugin/compat.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/plugin/urls.py` & `lti-consumer-xblock-9.5.1/lti_consumer/plugin/urls.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/plugin/views.py` & `lti-consumer-xblock-9.5.1/lti_consumer/plugin/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -773,15 +773,15 @@
 
     launch_data_key = get_cache_key(**common_cache_key_arguments, key="launch_data")
     launch_data = get_data_from_cache(launch_data_key)
     if not launch_data:
         log.warning(
             f'There was a cache miss trying to fetch the launch data during an LTI 1.3 proctoring StartAssessment '
             f'launch when using the cache key {launch_data_key}. The LtiConfiguration config_id is '
-            f'{lti_config.config_id}.'
+            f'{lti_config.config_id} the user_id is {request.user.id}.'
         )
         return render(request, 'html/lti_proctoring_start_error.html', status=HTTP_400_BAD_REQUEST)
 
     session_data_key = get_cache_key(**common_cache_key_arguments, key="session_data")
     session_data = get_data_from_cache(session_data_key)
 
     lti_consumer.set_proctoring_data(
```

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ar/text.js` & `lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/ar/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/en/text.js` & `lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/en/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/es_419/text.js` & `lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/es_419/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/fr/text.js` & `lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/fr/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/he/text.js` & `lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/he/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/hi/text.js` & `lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/hi/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/it/text.js` & `lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/it/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ja/text.js` & `lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/ja/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ko/text.js` & `lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/ko/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/pt_BR/text.js` & `lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/pt_BR/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/pt_PT/text.js` & `lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/pt_PT/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/ru/text.js` & `lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/ru/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/public/js/translations/zh_CN/text.js` & `lti-consumer-xblock-9.5.1/lti_consumer/public/js/translations/zh_CN/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/signals/signals.py` & `lti-consumer-xblock-9.5.1/lti_consumer/signals/signals.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/static/css/student.css` & `lti-consumer-xblock-9.5.1/lti_consumer/static/css/student.css`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/static/js/xblock_lti_consumer.js` & `lti-consumer-xblock-9.5.1/lti_consumer/static/js/xblock_lti_consumer.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/static/js/xblock_studio_view.js` & `lti-consumer-xblock-9.5.1/lti_consumer/static/js/xblock_studio_view.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/static/sass/student.scss` & `lti-consumer-xblock-9.5.1/lti_consumer/static/sass/student.scss`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/render_dl_content.html` & `lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti-dl/render_dl_content.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/render_image.html` & `lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti-dl/render_image.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti-dl/render_link.html` & `lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti-dl/render_link.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_1p3_launch.html` & `lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti_1p3_launch.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_1p3_studio.html` & `lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti_1p3_studio.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_launch.html` & `lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti_launch.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/templates/html/lti_start_assessment.html` & `lti-consumer-xblock-9.5.1/lti_consumer/templates/html/lti_start_assessment.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/templates/html/student.html` & `lti-consumer-xblock-9.5.1/lti_consumer/templates/html/student.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/templates/xml/outcome_service_response.xml` & `lti-consumer-xblock-9.5.1/lti_consumer/templates/xml/outcome_service_response.xml`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/templatetags/get_dl_lti_launch_url.py` & `lti-consumer-xblock-9.5.1/lti_consumer/templatetags/get_dl_lti_launch_url.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/templatetags/lti_sanitize.py` & `lti-consumer-xblock-9.5.1/lti_consumer/templatetags/lti_sanitize.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/tests/test_utils.py` & `lti-consumer-xblock-9.5.1/lti_consumer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/test_proctoring.py` & `lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/plugin/test_proctoring.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/test_views.py` & `lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/plugin/test_views.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/test_views_lti_ags.py` & `lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/plugin/test_views_lti_ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py` & `lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py` & `lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_api.py` & `lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_filters.py` & `lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/test_filters.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_lti_xblock.py` & `lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/test_lti_xblock.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_models.py` & `lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_outcomes.py` & `lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_signals.py` & `lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/test_signals.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/tests/unit/test_utils.py` & `lti-consumer-xblock-9.5.1/lti_consumer/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/ar/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/ar/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/ar/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/ar/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/en/LC_MESSAGES/django.po` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/en/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/en/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/es_419/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/es_419/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/es_419/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/es_419/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/fr/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/fr/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/fr/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/fr/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/he/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/he/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/he/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/he/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/hi/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/hi/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/ru/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/ru/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/ru/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/ru/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/settings.py` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/settings.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.5.1/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer/utils.py` & `lti-consumer-xblock-9.5.1/lti_consumer/utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer_xblock.egg-info/PKG-INFO` & `lti-consumer-xblock-9.5.1/lti_consumer_xblock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lti-consumer-xblock
-Version: 9.5.0
+Version: 9.5.1
 Summary: This XBlock implements the consumer side of the LTI specification.
 Home-page: https://github.com/openedx/xblock-lti-consumer
 Author: Open edX project
 Author-email: oscm@edx.org
 Keywords: lti consumer xblock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `lti-consumer-xblock-9.5.0/lti_consumer_xblock.egg-info/SOURCES.txt` & `lti-consumer-xblock-9.5.1/lti_consumer_xblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.5.0/setup.py` & `lti-consumer-xblock-9.5.1/setup.py`

 * *Files identical despite different names*
