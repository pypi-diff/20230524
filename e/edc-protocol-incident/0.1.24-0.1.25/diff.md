# Comparing `tmp/edc-protocol-incident-0.1.24.tar.gz` & `tmp/edc-protocol-incident-0.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-protocol-incident-0.1.24.tar", last modified: Fri Dec  9 18:44:07 2022, max compression
+gzip compressed data, was "edc-protocol-incident-0.1.25.tar", last modified: Wed May 24 16:57:42 2023, max compression
```

## Comparing `edc-protocol-incident-0.1.24.tar` & `edc-protocol-incident-0.1.25.tar`

### file list

```diff
@@ -1,101 +1,100 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-12-09 18:44:07.256208 edc-protocol-incident-0.1.24/
--rw-r--r--   0 erikvw     (501) staff       (20)      123 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-09-10 21:37:33.000000 edc-protocol-incident-0.1.24/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-12-09 18:44:07.239002 edc-protocol-incident-0.1.24/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-12-09 18:44:07.243360 edc-protocol-incident-0.1.24/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1914 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.24/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-06-01 17:50:51.000000 edc-protocol-incident-0.1.24/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-09-15 02:06:07.000000 edc-protocol-incident-0.1.24/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 00:41:59.000000 edc-protocol-incident-0.1.24/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)       37 2021-09-10 21:37:33.000000 edc-protocol-incident-0.1.24/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 17:50:51.000000 edc-protocol-incident-0.1.24/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-09-09 17:06:27.000000 edc-protocol-incident-0.1.24/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 17:50:51.000000 edc-protocol-incident-0.1.24/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     2117 2022-12-09 18:44:07.256298 edc-protocol-incident-0.1.24/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1232 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        7 2022-10-04 02:54:16.000000 edc-protocol-incident-0.1.24/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-10 00:41:59.000000 edc-protocol-incident-0.1.24/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-12-09 18:44:07.245698 edc-protocol-incident-0.1.24/edc_protocol_incident/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1333 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-12-09 18:44:07.247339 edc-protocol-incident-0.1.24/edc_protocol_incident/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2593 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/admin/protocol_deviation_violation_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      476 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/admin/protocol_incident_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      193 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      244 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      892 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1637 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)      430 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      358 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-12-09 18:44:07.248063 edc-protocol-incident-0.1.24/edc_protocol_incident/form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)      182 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1660 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/form_validators/mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1645 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/form_validators/protocol_deviation_violation_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1555 2022-10-04 02:54:16.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/form_validators/protocol_incident_form_validator.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-12-09 18:44:07.248624 edc-protocol-incident-0.1.24/edc_protocol_incident/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      135 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      992 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/forms/protocol_deviation_violation_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      794 2022-10-04 02:54:16.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/forms/protocol_incident_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1552 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-12-09 18:44:07.252351 edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    31950 2022-09-29 19:42:41.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)    73010 2022-09-29 19:42:41.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0001_squashed_0015_auto_20220927_0401.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2356 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0002_auto_20210911_2036.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1182 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0003_auto_20211104_1456.py
--rw-r--r--   0 erikvw     (501) staff       (20)      720 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0004_alter_protocoldeviationviolation_violation.py
--rw-r--r--   0 erikvw     (501) staff       (20)    26980 2022-09-29 19:42:41.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0005_protocolincident_historicalprotocolincident_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2622 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0006_protocolincidents_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1456 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0007_auto_20220704_1841.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1087 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0008_alter_historicalprotocoldeviationviolation_action_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1218 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0009_auto_20220826_0258.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1092 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0010_auto_20220826_0322.py
--rw-r--r--   0 erikvw     (501) staff       (20)      784 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0011_auto_20220826_0406.py
--rw-r--r--   0 erikvw     (501) staff       (20)      868 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0012_auto_20220913_2139.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2208 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0013_auto_20220927_0349.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1381 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0014_auto_20220927_0400.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1180 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0015_auto_20220927_0401.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1891 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0016_historicalprotocolincident_reasons_withdrawn_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      691 2022-12-09 18:43:58.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0017_alter_historicalprotocolincident_reasons_withdrawn_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-12-09 18:44:07.252830 edc-protocol-incident-0.1.24/edc_protocol_incident/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      170 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4117 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/model_mixins/protocol_deviation_violation_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3944 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/model_mixins/protocol_incident_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3888 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/modeladmin_mixins.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-12-09 18:44:07.253483 edc-protocol-incident-0.1.24/edc_protocol_incident/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      178 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      773 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/models/list_models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1018 2022-09-29 19:42:41.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/models/protocol_deviation_violation.py
--rw-r--r--   0 erikvw     (501) staff       (20)      946 2022-09-29 19:42:41.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/models/protocol_incident.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-12-09 18:44:07.253644 edc-protocol-incident-0.1.24/edc_protocol_incident/pdf_reports/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/pdf_reports/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-12-09 18:44:07.254351 edc-protocol-incident-0.1.24/edc_protocol_incident/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      608 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/tests/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-12-09 18:44:07.255637 edc-protocol-incident-0.1.24/edc_protocol_incident/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1895 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)       73 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-12-09 18:44:07.256061 edc-protocol-incident-0.1.24/edc_protocol_incident/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5901 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/tests/tests/test_protocol_incident.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9323 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/tests/tests/test_protocol_violation.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1638 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/tests/visit_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)      220 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.24/edc_protocol_incident/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-12-09 18:44:07.246856 edc-protocol-incident-0.1.24/edc_protocol_incident.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     2117 2022-12-09 18:44:07.000000 edc-protocol-incident-0.1.24/edc_protocol_incident.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     3979 2022-12-09 18:44:07.000000 edc-protocol-incident-0.1.24/edc_protocol_incident.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-12-09 18:44:07.000000 edc-protocol-incident-0.1.24/edc_protocol_incident.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-27 01:17:18.000000 edc-protocol-incident-0.1.24/edc_protocol_incident.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2022-12-09 18:44:07.000000 edc-protocol-incident-0.1.24/edc_protocol_incident.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1630 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.24/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1128 2022-09-28 03:06:58.000000 edc-protocol-incident-0.1.24/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1201 2022-12-09 18:44:07.256616 edc-protocol-incident-0.1.24/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.412697 edc-protocol-incident-0.1.25/
+-rw-r--r--   0 erikvw     (501) staff       (20)      123 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-09-10 21:37:33.000000 edc-protocol-incident-0.1.25/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.396960 edc-protocol-incident-0.1.25/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.401040 edc-protocol-incident-0.1.25/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-06-01 17:50:51.000000 edc-protocol-incident-0.1.25/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 00:41:59.000000 edc-protocol-incident-0.1.25/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)       37 2021-09-10 21:37:33.000000 edc-protocol-incident-0.1.25/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 17:50:51.000000 edc-protocol-incident-0.1.25/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-09-09 17:06:27.000000 edc-protocol-incident-0.1.25/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 17:50:51.000000 edc-protocol-incident-0.1.25/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     2168 2023-05-24 16:57:42.412809 edc-protocol-incident-0.1.25/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1232 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-10 00:41:59.000000 edc-protocol-incident-0.1.25/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.403135 edc-protocol-incident-0.1.25/edc_protocol_incident/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1331 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.404349 edc-protocol-incident-0.1.25/edc_protocol_incident/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2592 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/admin/protocol_deviation_violation_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      475 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/admin/protocol_incident_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      193 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      244 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      892 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1637 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      430 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      358 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.404954 edc-protocol-incident-0.1.25/edc_protocol_incident/form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)      182 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1660 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/form_validators/mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1645 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/form_validators/protocol_deviation_violation_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1554 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/form_validators/protocol_incident_form_validator.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.405387 edc-protocol-incident-0.1.25/edc_protocol_incident/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      135 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      992 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/forms/protocol_deviation_violation_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      794 2022-10-04 02:54:16.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/forms/protocol_incident_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1552 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.408300 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    31949 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    73009 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0001_squashed_0015_auto_20220927_0401.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2355 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0002_auto_20210911_2036.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1181 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0003_auto_20211104_1456.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      719 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0004_alter_protocoldeviationviolation_violation.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    26979 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0005_protocolincident_historicalprotocolincident_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2621 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0006_protocolincidents_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1455 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0007_auto_20220704_1841.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1086 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0008_alter_historicalprotocoldeviationviolation_action_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1217 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0009_auto_20220826_0258.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1091 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0010_auto_20220826_0322.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      783 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0011_auto_20220826_0406.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      867 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0012_auto_20220913_2139.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2207 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0013_auto_20220927_0349.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1380 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0014_auto_20220927_0400.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1179 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0015_auto_20220927_0401.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1890 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0016_historicalprotocolincident_reasons_withdrawn_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      690 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0017_alter_historicalprotocolincident_reasons_withdrawn_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.408701 edc-protocol-incident-0.1.25/edc_protocol_incident/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      170 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4116 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/model_mixins/protocol_deviation_violation_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3943 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/model_mixins/protocol_incident_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3887 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/modeladmin_mixins.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.409386 edc-protocol-incident-0.1.25/edc_protocol_incident/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      178 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      773 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/models/list_models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1018 2022-09-29 19:42:41.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/models/protocol_deviation_violation.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      946 2022-09-29 19:42:41.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/models/protocol_incident.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.409585 edc-protocol-incident-0.1.25/edc_protocol_incident/pdf_reports/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/pdf_reports/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.410536 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      606 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.411890 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1895 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)       73 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.412510 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5901 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/tests/test_protocol_incident.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9323 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/tests/test_protocol_violation.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1638 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/visit_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      220 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.404007 edc-protocol-incident-0.1.25/edc_protocol_incident.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2168 2023-05-24 16:57:42.000000 edc-protocol-incident-0.1.25/edc_protocol_incident.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     3971 2023-05-24 16:57:42.000000 edc-protocol-incident-0.1.25/edc_protocol_incident.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 16:57:42.000000 edc-protocol-incident-0.1.25/edc_protocol_incident.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-27 01:17:18.000000 edc-protocol-incident-0.1.25/edc_protocol_incident.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2023-05-24 16:57:42.000000 edc-protocol-incident-0.1.25/edc_protocol_incident.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1788 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1128 2022-09-28 03:06:58.000000 edc-protocol-incident-0.1.25/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1241 2023-05-24 16:57:42.413132 edc-protocol-incident-0.1.25/setup.cfg
```

### Comparing `edc-protocol-incident-0.1.24/.github/workflows/build.yml` & `edc-protocol-incident-0.1.25/.github/workflows/build.yml`

 * *Files 18% similar despite different names*

```diff
@@ -7,19 +7,20 @@
   build:
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.10']
-        django-version: ['4.1', 'dev']
-
+        python-version: ['3.10', '3.11']
+        django-version: ['4.1', '4.2', 'dev']
+        exclude:
+          - python-version: '3.10'
+            django-version: 'dev'
     services:
-
       mysql:
         image: mysql:latest
         env:
           MYSQL_DATABASE: mysql
           MYSQL_ROOT_PASSWORD: mysql
         ports:
           - 3306:3306
@@ -28,28 +29,27 @@
     steps:
       - name: Install pycups and words dependency
         run: |
           sudo sed -i 's/azure\.//' /etc/apt/sources.list
           sudo apt-get -y update
           sudo apt-get install libcups2-dev wamerican
 
-      - uses: actions/checkout@v2
-
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Get pip cache dir
         id: pip-cache
         run: |
-          echo "::set-output name=dir::$(pip cache dir)"
+          echo "dir=$(pip cache dir)" >>$GITHUB_OUTPUT
 
       - name: Cache
-        uses: actions/cache@v2
+        uses: actions/cache@v3
         with:
           path: ${{ steps.pip-cache.outputs.dir }}
           key:
             ${{ matrix.python-version }}-v1-${{ hashFiles('**/setup.py') }}-${{ hashFiles('**/tox.ini') }}
           restore-keys: |
             ${{ matrix.python-version }}-v1-
 
@@ -61,11 +61,11 @@
 
       - name: Tox tests
         run: |
           tox -v
         env:
           DJANGO: ${{ matrix.django-version }}
 
-      - name: Upload coverage
-        uses: codecov/codecov-action@v1
+      - name: Upload coverage to Codecov
+        uses: codecov/codecov-action@v3
         with:
           name: Python ${{ matrix.python-version }}
```

### Comparing `edc-protocol-incident-0.1.24/.gitignore` & `edc-protocol-incident-0.1.25/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.24/.pre-commit-config.yaml` & `edc-protocol-incident-0.1.25/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 ---
 exclude: tests/etc/user-*
 
 repos:
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.4
+    rev: 1.7.5
     hooks:
       - id: bandit
         args:
           - "-x *test*.py"
 
   - repo: https://github.com/psf/black
-    rev: 22.6.0
+    rev: 23.3.0
     hooks:
       - id: black
-        language_version: python3.9
+        language_version: python3.10
 
   - repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
       - id: flake8
         args:
           - "--config=setup.cfg"
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: requirements-txt-fixer
         files: requirements/.*\.txt$
       - id: trailing-whitespace
       - id: check-added-large-files
       - id: fix-byte-order-marker
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
       - id: detect-private-key
 
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.27.1
+    rev: v1.31.0
     hooks:
       - id: yamllint
         args:
           - "--strict"
```

### Comparing `edc-protocol-incident-0.1.24/LICENSE` & `edc-protocol-incident-0.1.25/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.24/PKG-INFO` & `edc-protocol-incident-0.1.25/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: edc-protocol-incident
-Version: 0.1.24
+Version: 0.1.25
 Summary: Classes for protocol incident (violations/deviations) in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-protocol-incident
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc protocol incident violations deviations,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |codecov| |downloads|
```

### Comparing `edc-protocol-incident-0.1.24/README.rst` & `edc-protocol-incident-0.1.25/README.rst`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/action_items.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/action_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     PROTOCOL_DEVIATION_VIOLATION_ACTION,
     PROTOCOL_INCIDENT_ACTION,
     WITHDRAWN,
 )
 
 
 class ProtocolDeviationViolationAction(ActionWithNotification):
-
     reference_model = None  # "my_app.protocolincident"
     admin_site_name = None  # "my_app_admin"
 
     name = PROTOCOL_DEVIATION_VIOLATION_ACTION
     display_name = "Submit Protocol Deviation / Violation Report"
     notification_display_name = "Protocol Deviation / Violation Report"
     parent_action_names = []
@@ -22,15 +21,14 @@
     priority = HIGH_PRIORITY
 
     def close_action_item_on_save(self):
         return self.reference_obj.report_status == CLOSED
 
 
 class ProtocolIncidentAction(ActionWithNotification):
-
     reference_model = None  # "my_app.protocolincident"
     admin_site_name = None  # "my_app"
 
     name = PROTOCOL_INCIDENT_ACTION
     display_name = "Submit Protocol Incident Report"
     notification_display_name = "Protocol Incident Report"
     parent_action_names = []
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/admin/protocol_deviation_violation_admin.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/admin/protocol_deviation_violation_admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from ..admin_site import edc_protocol_incident_admin
 from ..forms import ProtocolDeviationViolationForm
 from ..models import ProtocolDeviationViolation
 
 
 @admin.register(ProtocolDeviationViolation, site=edc_protocol_incident_admin)
 class ProtocolDeviationViolationAdmin(ModelAdminSubjectDashboardMixin, SimpleHistoryAdmin):
-
     form = ProtocolDeviationViolationForm
 
     fieldsets = (
         (
             None,
             {
                 "fields": (
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/auth_objects.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/auth_objects.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/auths.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/auths.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/form_validators/mixins.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/form_validators/mixins.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/form_validators/protocol_deviation_violation_form_validator.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/form_validators/protocol_deviation_violation_form_validator.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/form_validators/protocol_incident_form_validator.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/form_validators/protocol_incident_form_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from .mixins import IncidentFormvalidatorMixin
 
 
 class ProtocolIncidentFormValidator(
     IncidentFormvalidatorMixin, PrnFormValidatorMixin, FormValidator
 ):
     def clean(self):
-
         self.required_if(YES, field="safety_impact", field_required="safety_impact_details")
 
         self.required_if(
             YES,
             field="study_outcomes_impact",
             field_required="study_outcomes_impact_details",
         )
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/forms/protocol_deviation_violation_form.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/forms/protocol_deviation_violation_form.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/forms/protocol_incident_form.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/forms/protocol_incident_form.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/list_data.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/list_data.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0001_initial.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import edc_utils.date
 import simple_history.models
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         ("sites", "0002_alter_domain_unique"),
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ("edc_action_item", "0028_auto_20210203_0706"),
     ]
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0001_squashed_0015_auto_20220927_0401.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0001_squashed_0015_auto_20220927_0401.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import edc_utils.date
 import simple_history.models
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     replaces = [
         ("edc_protocol_incident", "0001_initial"),
         ("edc_protocol_incident", "0002_auto_20210911_2036"),
         ("edc_protocol_incident", "0003_auto_20211104_1456"),
         ("edc_protocol_incident", "0004_alter_protocoldeviationviolation_violation"),
         ("edc_protocol_incident", "0005_protocolincident_historicalprotocolincident_and_more"),
         ("edc_protocol_incident", "0006_protocolincidents_and_more"),
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0002_auto_20210911_2036.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0002_auto_20210911_2036.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.6 on 2021-09-11 17:36
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("edc_protocol_incident", "0001_initial"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="historicalprotocoldeviationviolation",
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0003_auto_20211104_1456.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0003_auto_20211104_1456.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.2.7 on 2021-11-04 11:56
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("edc_protocol_incident", "0002_auto_20210911_2036"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="historicalprotocoldeviationviolation",
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0004_alter_protocoldeviationviolation_violation.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0004_alter_protocoldeviationviolation_violation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 4.0.4 on 2022-06-02 01:53
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("edc_protocol_incident", "0003_auto_20211104_1456"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="protocoldeviationviolation",
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0005_protocolincident_historicalprotocolincident_and_more.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0005_protocolincident_historicalprotocolincident_and_more.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import edc_utils.date
 import simple_history.models
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("edc_action_item", "0028_auto_20210203_0706"),
         ("sites", "0002_alter_domain_unique"),
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ("edc_protocol_incident", "0004_alter_protocoldeviationviolation_violation"),
     ]
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0006_protocolincidents_and_more.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0006_protocolincidents_and_more.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 4.0.5 on 2022-06-25 20:57
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         (
             "edc_protocol_incident",
             "0005_protocolincident_historicalprotocolincident_and_more",
         ),
     ]
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0007_auto_20220704_1841.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0007_auto_20220704_1841.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.13 on 2022-07-04 15:41
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("edc_protocol_incident", "0006_protocolincidents_and_more"),
     ]
 
     operations = [
         migrations.AlterModelOptions(
             name="historicalprotocoldeviationviolation",
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0008_alter_historicalprotocoldeviationviolation_action_identifier_and_more.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0009_auto_20220826_0258.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-# Generated by Django 4.0.7 on 2022-08-23 13:24
+# Generated by Django 3.2.13 on 2022-08-25 23:58
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ("edc_protocol_incident", "0007_auto_20220704_1841"),
+        (
+            "edc_protocol_incident",
+            "0008_alter_historicalprotocoldeviationviolation_action_identifier_and_more",
+        ),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="historicalprotocoldeviationviolation",
             name="action_identifier",
-            field=models.CharField(blank=True, db_index=True, max_length=50),
+            field=models.CharField(blank=True, db_index=True, max_length=50, null=True),
         ),
         migrations.AlterField(
             model_name="historicalprotocolincident",
             name="action_identifier",
-            field=models.CharField(blank=True, db_index=True, max_length=50),
+            field=models.CharField(blank=True, db_index=True, max_length=50, null=True),
         ),
         migrations.AlterField(
             model_name="protocoldeviationviolation",
             name="action_identifier",
-            field=models.CharField(blank=True, max_length=50, unique=True),
+            field=models.CharField(blank=True, max_length=50, null=True, unique=True),
         ),
         migrations.AlterField(
             model_name="protocolincident",
             name="action_identifier",
-            field=models.CharField(blank=True, max_length=50, unique=True),
+            field=models.CharField(blank=True, max_length=50, null=True, unique=True),
         ),
     ]
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0009_auto_20220826_0258.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0008_alter_historicalprotocoldeviationviolation_action_identifier_and_more.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,32 @@
-# Generated by Django 3.2.13 on 2022-08-25 23:58
+# Generated by Django 4.0.7 on 2022-08-23 13:24
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        (
-            "edc_protocol_incident",
-            "0008_alter_historicalprotocoldeviationviolation_action_identifier_and_more",
-        ),
+        ("edc_protocol_incident", "0007_auto_20220704_1841"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="historicalprotocoldeviationviolation",
             name="action_identifier",
-            field=models.CharField(blank=True, db_index=True, max_length=50, null=True),
+            field=models.CharField(blank=True, db_index=True, max_length=50),
         ),
         migrations.AlterField(
             model_name="historicalprotocolincident",
             name="action_identifier",
-            field=models.CharField(blank=True, db_index=True, max_length=50, null=True),
+            field=models.CharField(blank=True, db_index=True, max_length=50),
         ),
         migrations.AlterField(
             model_name="protocoldeviationviolation",
             name="action_identifier",
-            field=models.CharField(blank=True, max_length=50, null=True, unique=True),
+            field=models.CharField(blank=True, max_length=50, unique=True),
         ),
         migrations.AlterField(
             model_name="protocolincident",
             name="action_identifier",
-            field=models.CharField(blank=True, max_length=50, null=True, unique=True),
+            field=models.CharField(blank=True, max_length=50, unique=True),
         ),
     ]
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0010_auto_20220826_0322.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0010_auto_20220826_0322.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.13 on 2022-08-26 00:22
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("edc_protocol_incident", "0009_auto_20220826_0258"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="historicalprotocoldeviationviolation",
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0011_auto_20220826_0406.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0011_auto_20220826_0406.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.13 on 2022-08-26 01:06
 
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("edc_protocol_incident", "0010_auto_20220826_0322"),
     ]
 
     operations = [
         migrations.RemoveField(
             model_name="historicalprotocoldeviationviolation",
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0012_auto_20220913_2139.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0012_auto_20220913_2139.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.13 on 2022-09-13 18:39
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("edc_protocol_incident", "0011_auto_20220826_0406"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="actionsrequired",
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0013_auto_20220927_0349.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0013_auto_20220927_0349.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.13 on 2022-09-27 00:49
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("edc_protocol_incident", "0012_auto_20220913_2139"),
     ]
 
     operations = [
         migrations.RemoveIndex(
             model_name="actionsrequired",
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0014_auto_20220927_0400.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0014_auto_20220927_0400.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.13 on 2022-09-27 01:00
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("edc_protocol_incident", "0013_auto_20220927_0349"),
     ]
 
     operations = [
         migrations.RemoveIndex(
             model_name="protocolviolations",
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0015_auto_20220927_0401.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0015_auto_20220927_0401.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.13 on 2022-09-27 01:01
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("edc_protocol_incident", "0014_auto_20220927_0400"),
     ]
 
     operations = [
         migrations.RemoveIndex(
             model_name="protocolviolations",
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0016_historicalprotocolincident_reasons_withdrawn_and_more.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0016_historicalprotocolincident_reasons_withdrawn_and_more.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 4.1.2 on 2022-11-30 21:52
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("edc_protocol_incident", "0001_squashed_0015_auto_20220927_0401"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="historicalprotocolincident",
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/migrations/0017_alter_historicalprotocolincident_reasons_withdrawn_and_more.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0017_alter_historicalprotocolincident_reasons_withdrawn_and_more.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 4.1.2 on 2022-11-30 22:38
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         (
             "edc_protocol_incident",
             "0016_historicalprotocolincident_reasons_withdrawn_and_more",
         ),
     ]
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/model_mixins/protocol_deviation_violation_model_mixin.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/model_mixins/protocol_deviation_violation_model_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from edc_utils import get_utcnow
 
 from ..choices import DEVIATION_VIOLATION
 from ..models import ActionsRequired, ProtocolViolations
 
 
 class ProtocolDeviationViolationModelMixin(models.Model):
-
     report_datetime = models.DateTimeField(
         verbose_name="Report Date and Time", default=get_utcnow
     )
 
     short_description = models.CharField(
         verbose_name="Provide a short description of this occurrence",
         max_length=35,
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/model_mixins/protocol_incident_model_mixin.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/model_mixins/protocol_incident_model_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from edc_utils import get_utcnow
 
 from ..choices import DEVIATION_VIOLATION, REPORT_STATUS
 from ..models import ActionsRequired, ProtocolViolations
 
 
 class ProtocolIncidentModelMixin(models.Model):
-
     report_datetime = models.DateTimeField(
         verbose_name="Report Date and Time", default=get_utcnow
     )
 
     short_description = models.CharField(
         verbose_name="Provide a short description of this incident",
         max_length=35,
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/modeladmin_mixins.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/modeladmin_mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from django_audit_fields.admin import audit_fieldset_tuple
 from edc_constants.constants import CLOSED, OPEN
 
 from edc_protocol_incident.constants import WITHDRAWN
 
 
 class ProtocolIncidentModelAdminMixin:
-
     fieldsets = (
         (
             None,
             {
                 "fields": (
                     "subject_identifier",
                     "report_datetime",
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/models/list_models.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/models/list_models.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/models/protocol_deviation_violation.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/models/protocol_deviation_violation.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/models/protocol_incident.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/models/protocol_incident.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/tests/action_items.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/tests/action_items.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 )
 from edc_protocol_incident.action_items import (
     ProtocolIncidentAction as BaseProtocolIncidentAction,
 )
 
 
 class ProtocolDeviationViolationAction(BaseProtocolDeviationViolationAction):
-
     reference_model = "edc_protocol_incident.protocoldeviationviolation"
     admin_site_name = "edc_protocol_incident"
 
 
 class ProtocolIncidentAction(BaseProtocolIncidentAction):
-
     reference_model = "edc_protocol_incident.protocolincident"
     admin_site_name = "edc_protocol_incident"
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/tests/etc/user-rsa-local-private.pem` & `edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/tests/etc/user-rsa-restricted-private.pem` & `edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/tests/holidays.csv` & `edc-protocol-incident-0.1.25/edc_protocol_incident/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/tests/tests/test_protocol_incident.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/tests/tests/test_protocol_incident.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/tests/tests/test_protocol_violation.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/tests/tests/test_protocol_violation.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident/tests/visit_schedule.py` & `edc-protocol-incident-0.1.25/edc_protocol_incident/tests/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident.egg-info/PKG-INFO` & `edc-protocol-incident-0.1.25/edc_protocol_incident.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: edc-protocol-incident
-Version: 0.1.24
+Version: 0.1.25
 Summary: Classes for protocol incident (violations/deviations) in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-protocol-incident
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc protocol incident violations deviations,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |codecov| |downloads|
```

### Comparing `edc-protocol-incident-0.1.24/edc_protocol_incident.egg-info/SOURCES.txt` & `edc-protocol-incident-0.1.25/edc_protocol_incident.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 .pre-commit-config.yaml
 .yamllint
 AUTHORS
 CHANGES
 LICENSE
 MANIFEST.in
 README.rst
-VERSION
 codecov.yml
 pyproject.toml
 runtests.py
 setup.cfg
 .github/workflows/build.yml
 edc_protocol_incident/__init__.py
 edc_protocol_incident/action_items.py
```

### Comparing `edc-protocol-incident-0.1.24/pyproject.toml` & `edc-protocol-incident-0.1.25/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -12,55 +12,63 @@
 
 [tool.isort]
 profile = "black"
 py_version = "310"
 skip = [".tox", ".eggs", "migrations"]
 
 [tool.coverage.run]
-parallel = true
+parallel = false
 branch = true
 source = ["edc_protocol_incident"]
 
 [tool.coverage.paths]
 source = ["edc_protocol_incident"]
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 omit = ["requirements.txt"]
+exclude_lines = [
+  "pragma: no cover",
+  "if TYPE_CHECKING:",
+]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{38,39,310}-dj{32,40,41,dev},
+    py{310}-dj{41,42},
+    py{311}-dj{41,42,dev},
     lint
 
 isolated_build = true
 
 [gh-actions]
 python =
-    3.10: py310, lint
+    3.10: py310
+    3.11: py311, lint
 
 [gh-actions:env]
 DJANGO =
     4.1: dj41
+    4.2: dj42, lint
     dev: djdev
 
 [testenv]
 deps =
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/test_utils.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/edc.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/third_party_dev.txt
     dj41: Django>=4.1,<4.2
+    dj42: Django>=4.2,<5.0
     djdev: https://github.com/django/django/tarball/main
 
 commands =
-    pip install -U pip
+    pip install -U pip coverage[toml]
     pip --version
     pip freeze
     coverage run -a runtests.py
     coverage report
 
 [testenv:lint]
 deps = -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/lint.txt
```

### Comparing `edc-protocol-incident-0.1.24/runtests.py` & `edc-protocol-incident-0.1.25/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.24/setup.cfg` & `edc-protocol-incident-0.1.25/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 
 [options]
 python_requires = >=3.10
 zip_safe = False
 include_package_data = True
 packages = find:
```

