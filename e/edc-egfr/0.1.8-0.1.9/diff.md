# Comparing `tmp/edc-egfr-0.1.8.tar.gz` & `tmp/edc-egfr-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-egfr-0.1.8.tar", last modified: Fri Oct 14 12:48:16 2022, max compression
+gzip compressed data, was "edc-egfr-0.1.9.tar", last modified: Fri Oct 14 13:01:14 2022, max compression
```

## Comparing `edc-egfr-0.1.8.tar` & `edc-egfr-0.1.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 12:48:16.105628 edc-egfr-0.1.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       84 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 12:48:16.094203 edc-egfr-0.1.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 12:48:16.098034 edc-egfr-0.1.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)      948 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-09-15 01:41:57.000000 edc-egfr-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)       38 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       29 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-08-12 18:34:46.000000 edc-egfr-0.1.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     5663 2022-10-14 12:48:16.105726 edc-egfr-0.1.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     4646 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-10-14 12:48:07.000000 edc-egfr-0.1.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 12:48:16.098872 edc-egfr-0.1.8/edc_egfr/
--rw-r--r--   0 erikvw     (501) staff       (20)       56 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/edc_egfr/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 12:48:16.100297 edc-egfr-0.1.8/edc_egfr/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)       79 2022-08-16 02:38:33.000000 edc-egfr-0.1.8/edc_egfr/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2501 2022-08-22 02:16:03.000000 edc-egfr-0.1.8/edc_egfr/admin/egfr_drop_notification_admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/edc_egfr/apps.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 12:48:16.101163 edc-egfr-0.1.8/edc_egfr/calculators/
--rw-r--r--   0 erikvw     (501) staff       (20)      182 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/edc_egfr/calculators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1833 2022-09-15 01:41:57.000000 edc-egfr-0.1.8/edc_egfr/calculators/base_egrfr.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2112 2022-09-15 01:41:57.000000 edc-egfr-0.1.8/edc_egfr/calculators/egfr_ckd_epi.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1980 2022-10-14 12:48:07.000000 edc-egfr-0.1.8/edc_egfr/calculators/egfr_cockcroft_gault.py
--rw-r--r--   0 erikvw     (501) staff       (20)      313 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/edc_egfr/calculators/percent_change.py
--rw-r--r--   0 erikvw     (501) staff       (20)       59 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/edc_egfr/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8900 2022-10-14 01:54:04.000000 edc-egfr-0.1.8/edc_egfr/egfr.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 12:48:16.101426 edc-egfr-0.1.8/edc_egfr/form_validator_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      120 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/edc_egfr/form_validator_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2097 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/edc_egfr/form_validator_mixins/egfr_form_validator_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      299 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/edc_egfr/get_drop_notification_model.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 12:48:16.101945 edc-egfr-0.1.8/edc_egfr/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      124 2022-08-16 02:38:33.000000 edc-egfr-0.1.8/edc_egfr/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1986 2022-09-21 17:08:05.000000 edc-egfr-0.1.8/edc_egfr/model_mixins/egfr_drop_notification_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4016 2022-10-14 12:48:07.000000 edc-egfr-0.1.8/edc_egfr/model_mixins/egfr_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 12:48:16.102207 edc-egfr-0.1.8/edc_egfr/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/edc_egfr/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 12:48:16.103393 edc-egfr-0.1.8/edc_egfr/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/edc_egfr/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/edc_egfr/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/edc_egfr/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/edc_egfr/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/edc_egfr/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/edc_egfr/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/edc_egfr/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/edc_egfr/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/edc_egfr/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 12:48:16.104138 edc-egfr-0.1.8/edc_egfr/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/edc_egfr/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11574 2022-09-15 01:41:57.000000 edc-egfr-0.1.8/edc_egfr/tests/tests/test_calculators.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3209 2022-09-25 23:45:17.000000 edc-egfr-0.1.8/edc_egfr/tests/tests/test_drop_notification.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9588 2022-09-25 23:48:13.000000 edc-egfr-0.1.8/edc_egfr/tests/tests/test_egfr.py
--rw-r--r--   0 erikvw     (501) staff       (20)      112 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/edc_egfr/tests/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 12:48:16.099924 edc-egfr-0.1.8/edc_egfr.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     5663 2022-10-14 12:48:16.000000 edc-egfr-0.1.8/edc_egfr.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1805 2022-10-14 12:48:16.000000 edc-egfr-0.1.8/edc_egfr.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-10-14 12:48:16.000000 edc-egfr-0.1.8/edc_egfr.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-14 21:58:52.000000 edc-egfr-0.1.8/edc_egfr.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-10-14 12:48:16.000000 edc-egfr-0.1.8/edc_egfr.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       18 2022-10-14 12:48:16.000000 edc-egfr-0.1.8/edc_egfr.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 12:48:16.105430 edc-egfr-0.1.8/egfr_app/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/egfr_app/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      266 2022-08-16 02:38:33.000000 edc-egfr-0.1.8/egfr_app/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/egfr_app/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1084 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/egfr_app/form_validators.py
--rw-r--r--   0 erikvw     (501) staff       (20)      274 2022-08-16 02:38:33.000000 edc-egfr-0.1.8/egfr_app/lab_profiles.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 12:48:16.105560 edc-egfr-0.1.8/egfr_app/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/egfr_app/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4154 2022-09-25 23:48:36.000000 edc-egfr-0.1.8/egfr_app/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5143 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/egfr_app/reportables.py
--rw-r--r--   0 erikvw     (501) staff       (20)      254 2022-08-16 02:38:33.000000 edc-egfr-0.1.8/egfr_app/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1718 2022-08-15 01:03:08.000000 edc-egfr-0.1.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1777 2022-09-25 23:48:36.000000 edc-egfr-0.1.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1302 2022-10-14 12:48:16.106121 edc-egfr-0.1.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 13:01:14.745196 edc-egfr-0.1.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       84 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 13:01:14.734047 edc-egfr-0.1.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 13:01:14.737561 edc-egfr-0.1.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)      948 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-09-15 01:41:57.000000 edc-egfr-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)       38 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       78 2022-10-14 13:01:06.000000 edc-egfr-0.1.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-08-12 18:34:46.000000 edc-egfr-0.1.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     5663 2022-10-14 13:01:14.745296 edc-egfr-0.1.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     4646 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-10-14 13:01:07.000000 edc-egfr-0.1.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 13:01:14.738331 edc-egfr-0.1.9/edc_egfr/
+-rw-r--r--   0 erikvw     (501) staff       (20)       56 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/edc_egfr/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 13:01:14.739593 edc-egfr-0.1.9/edc_egfr/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)       79 2022-08-16 02:38:33.000000 edc-egfr-0.1.9/edc_egfr/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2501 2022-08-22 02:16:03.000000 edc-egfr-0.1.9/edc_egfr/admin/egfr_drop_notification_admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/edc_egfr/apps.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 13:01:14.740615 edc-egfr-0.1.9/edc_egfr/calculators/
+-rw-r--r--   0 erikvw     (501) staff       (20)      182 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/edc_egfr/calculators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1833 2022-09-15 01:41:57.000000 edc-egfr-0.1.9/edc_egfr/calculators/base_egrfr.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2112 2022-09-15 01:41:57.000000 edc-egfr-0.1.9/edc_egfr/calculators/egfr_ckd_epi.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1980 2022-10-14 12:48:07.000000 edc-egfr-0.1.9/edc_egfr/calculators/egfr_cockcroft_gault.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      313 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/edc_egfr/calculators/percent_change.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       59 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/edc_egfr/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8900 2022-10-14 01:54:04.000000 edc-egfr-0.1.9/edc_egfr/egfr.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 13:01:14.740866 edc-egfr-0.1.9/edc_egfr/form_validator_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      120 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/edc_egfr/form_validator_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2097 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/edc_egfr/form_validator_mixins/egfr_form_validator_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      299 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/edc_egfr/get_drop_notification_model.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 13:01:14.741401 edc-egfr-0.1.9/edc_egfr/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      124 2022-08-16 02:38:33.000000 edc-egfr-0.1.9/edc_egfr/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1986 2022-09-21 17:08:05.000000 edc-egfr-0.1.9/edc_egfr/model_mixins/egfr_drop_notification_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4016 2022-10-14 12:48:07.000000 edc-egfr-0.1.9/edc_egfr/model_mixins/egfr_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 13:01:14.741727 edc-egfr-0.1.9/edc_egfr/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/edc_egfr/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 13:01:14.742938 edc-egfr-0.1.9/edc_egfr/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/edc_egfr/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/edc_egfr/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/edc_egfr/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/edc_egfr/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/edc_egfr/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/edc_egfr/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/edc_egfr/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/edc_egfr/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/edc_egfr/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 13:01:14.743631 edc-egfr-0.1.9/edc_egfr/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/edc_egfr/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    11574 2022-09-15 01:41:57.000000 edc-egfr-0.1.9/edc_egfr/tests/tests/test_calculators.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3209 2022-09-25 23:45:17.000000 edc-egfr-0.1.9/edc_egfr/tests/tests/test_drop_notification.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9588 2022-09-25 23:48:13.000000 edc-egfr-0.1.9/edc_egfr/tests/tests/test_egfr.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      112 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/edc_egfr/tests/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 13:01:14.739243 edc-egfr-0.1.9/edc_egfr.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     5663 2022-10-14 13:01:14.000000 edc-egfr-0.1.9/edc_egfr.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1805 2022-10-14 13:01:14.000000 edc-egfr-0.1.9/edc_egfr.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-10-14 13:01:14.000000 edc-egfr-0.1.9/edc_egfr.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-14 21:58:52.000000 edc-egfr-0.1.9/edc_egfr.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-10-14 13:01:14.000000 edc-egfr-0.1.9/edc_egfr.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       18 2022-10-14 13:01:14.000000 edc-egfr-0.1.9/edc_egfr.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 13:01:14.744967 edc-egfr-0.1.9/egfr_app/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/egfr_app/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      266 2022-08-16 02:38:33.000000 edc-egfr-0.1.9/egfr_app/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/egfr_app/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1084 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/egfr_app/form_validators.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      274 2022-08-16 02:38:33.000000 edc-egfr-0.1.9/egfr_app/lab_profiles.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-14 13:01:14.745105 edc-egfr-0.1.9/egfr_app/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/egfr_app/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4154 2022-09-25 23:48:36.000000 edc-egfr-0.1.9/egfr_app/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5143 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/egfr_app/reportables.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      254 2022-08-16 02:38:33.000000 edc-egfr-0.1.9/egfr_app/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1718 2022-08-15 01:03:08.000000 edc-egfr-0.1.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1777 2022-09-25 23:48:36.000000 edc-egfr-0.1.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1302 2022-10-14 13:01:14.745607 edc-egfr-0.1.9/setup.cfg
```

### Comparing `edc-egfr-0.1.8/.github/workflows/build.yml` & `edc-egfr-0.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/.gitignore` & `edc-egfr-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/.pre-commit-config.yaml` & `edc-egfr-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/LICENSE` & `edc-egfr-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/PKG-INFO` & `edc-egfr-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-egfr
-Version: 0.1.8
+Version: 0.1.9
 Summary: Classes and utils to handle eGFR collection and reporting for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-egfr
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django eGFR data collection clinicedc clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-egfr-0.1.8/README.rst` & `edc-egfr-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/edc_egfr/admin/egfr_drop_notification_admin_mixin.py` & `edc-egfr-0.1.9/edc_egfr/admin/egfr_drop_notification_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/edc_egfr/calculators/base_egrfr.py` & `edc-egfr-0.1.9/edc_egfr/calculators/base_egrfr.py`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/edc_egfr/calculators/egfr_ckd_epi.py` & `edc-egfr-0.1.9/edc_egfr/calculators/egfr_ckd_epi.py`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/edc_egfr/calculators/egfr_cockcroft_gault.py` & `edc-egfr-0.1.9/edc_egfr/calculators/egfr_cockcroft_gault.py`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/edc_egfr/egfr.py` & `edc-egfr-0.1.9/edc_egfr/egfr.py`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/edc_egfr/form_validator_mixins/egfr_form_validator_mixins.py` & `edc-egfr-0.1.9/edc_egfr/form_validator_mixins/egfr_form_validator_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/edc_egfr/model_mixins/egfr_drop_notification_model_mixin.py` & `edc-egfr-0.1.9/edc_egfr/model_mixins/egfr_drop_notification_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/edc_egfr/model_mixins/egfr_model_mixin.py` & `edc-egfr-0.1.9/edc_egfr/model_mixins/egfr_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/edc_egfr/tests/etc/user-rsa-local-private.pem` & `edc-egfr-0.1.9/edc_egfr/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/edc_egfr/tests/etc/user-rsa-restricted-private.pem` & `edc-egfr-0.1.9/edc_egfr/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/edc_egfr/tests/tests/test_calculators.py` & `edc-egfr-0.1.9/edc_egfr/tests/tests/test_calculators.py`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/edc_egfr/tests/tests/test_drop_notification.py` & `edc-egfr-0.1.9/edc_egfr/tests/tests/test_drop_notification.py`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/edc_egfr/tests/tests/test_egfr.py` & `edc-egfr-0.1.9/edc_egfr/tests/tests/test_egfr.py`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/edc_egfr.egg-info/PKG-INFO` & `edc-egfr-0.1.9/edc_egfr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-egfr
-Version: 0.1.8
+Version: 0.1.9
 Summary: Classes and utils to handle eGFR collection and reporting for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-egfr
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django eGFR data collection clinicedc clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-egfr-0.1.8/edc_egfr.egg-info/SOURCES.txt` & `edc-egfr-0.1.9/edc_egfr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/egfr_app/form_validators.py` & `edc-egfr-0.1.9/egfr_app/form_validators.py`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/egfr_app/models.py` & `edc-egfr-0.1.9/egfr_app/models.py`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/egfr_app/reportables.py` & `edc-egfr-0.1.9/egfr_app/reportables.py`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/pyproject.toml` & `edc-egfr-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/runtests.py` & `edc-egfr-0.1.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-egfr-0.1.8/setup.cfg` & `edc-egfr-0.1.9/setup.cfg`

 * *Files identical despite different names*

