# Comparing `tmp/edc-mnsi-0.1.8.tar.gz` & `tmp/edc-mnsi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-mnsi-0.1.8.tar", last modified: Wed Jul  6 06:55:14 2022, max compression
+gzip compressed data, was "edc-mnsi-0.1.9.tar", last modified: Wed Aug 10 22:43:50 2022, max compression
```

## Comparing `edc-mnsi-0.1.8.tar` & `edc-mnsi-0.1.9.tar`

### file list

```diff
@@ -1,72 +1,74 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:55:14.518611 edc-mnsi-0.1.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       84 2021-08-16 21:28:17.000000 edc-mnsi-0.1.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-08-16 21:28:17.000000 edc-mnsi-0.1.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:55:14.505990 edc-mnsi-0.1.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:55:14.510718 edc-mnsi-0.1.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1854 2022-06-23 21:18:38.000000 edc-mnsi-0.1.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-06-01 21:57:55.000000 edc-mnsi-0.1.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)       89 2021-08-16 21:28:17.000000 edc-mnsi-0.1.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       83 2022-06-23 21:18:38.000000 edc-mnsi-0.1.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-08-16 16:49:13.000000 edc-mnsi-0.1.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 21:57:55.000000 edc-mnsi-0.1.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     5218 2022-07-06 06:55:14.518719 edc-mnsi-0.1.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     4350 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-07-06 06:54:56.000000 edc-mnsi-0.1.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2021-08-16 21:28:17.000000 edc-mnsi-0.1.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:55:14.513517 edc-mnsi-0.1.8/edc_mnsi/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-16 21:28:17.000000 edc-mnsi-0.1.8/edc_mnsi/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1296 2021-09-21 15:50:47.000000 edc-mnsi-0.1.8/edc_mnsi/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      161 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/edc_mnsi/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      217 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/edc_mnsi/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      457 2021-09-23 17:43:23.000000 edc-mnsi-0.1.8/edc_mnsi/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      305 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/edc_mnsi/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4936 2022-06-23 21:18:38.000000 edc-mnsi-0.1.8/edc_mnsi/calculator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      730 2021-08-18 16:06:55.000000 edc-mnsi-0.1.8/edc_mnsi/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2868 2021-09-21 15:50:47.000000 edc-mnsi-0.1.8/edc_mnsi/factory.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1960 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/edc_mnsi/fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2995 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/edc_mnsi/form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      379 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/edc_mnsi/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)      912 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/edc_mnsi/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:55:14.514907 edc-mnsi-0.1.8/edc_mnsi/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     1752 2021-08-18 16:06:55.000000 edc-mnsi-0.1.8/edc_mnsi/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)    23531 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/edc_mnsi/migrations/0002_historicalmnsi_mnsi.py
--rw-r--r--   0 erikvw     (501) staff       (20)      987 2022-06-01 21:57:55.000000 edc-mnsi-0.1.8/edc_mnsi/migrations/0003_alter_mnsi_abnormal_obs_left_foot_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      873 2022-07-06 06:54:56.000000 edc-mnsi-0.1.8/edc_mnsi/migrations/0004_auto_20220704_1841.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-16 21:28:17.000000 edc-mnsi-0.1.8/edc_mnsi/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1615 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/edc_mnsi/model_admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5601 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/edc_mnsi/model_mixins.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:55:14.515428 edc-mnsi-0.1.8/edc_mnsi/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      138 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/edc_mnsi/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      284 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/edc_mnsi/models/list_models.py
--rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-06-01 21:57:55.000000 edc-mnsi-0.1.8/edc_mnsi/models/mnsi.py
--rw-r--r--   0 erikvw     (501) staff       (20)      495 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/edc_mnsi/models/signals.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:55:14.515650 edc-mnsi-0.1.8/edc_mnsi/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-17 21:32:34.000000 edc-mnsi-0.1.8/edc_mnsi/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:55:14.517504 edc-mnsi-0.1.8/edc_mnsi/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-16 21:28:17.000000 edc-mnsi-0.1.8/edc_mnsi/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-16 21:28:17.000000 edc-mnsi-0.1.8/edc_mnsi/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2021-08-16 21:28:17.000000 edc-mnsi-0.1.8/edc_mnsi/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-08-16 21:28:17.000000 edc-mnsi-0.1.8/edc_mnsi/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-08-16 21:28:17.000000 edc-mnsi-0.1.8/edc_mnsi/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-08-16 21:28:17.000000 edc-mnsi-0.1.8/edc_mnsi/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-16 21:28:17.000000 edc-mnsi-0.1.8/edc_mnsi/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-16 21:28:17.000000 edc-mnsi-0.1.8/edc_mnsi/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      627 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/edc_mnsi/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:55:14.518460 edc-mnsi-0.1.8/edc_mnsi/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-16 21:28:17.000000 edc-mnsi-0.1.8/edc_mnsi/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7158 2022-06-01 21:57:55.000000 edc-mnsi-0.1.8/edc_mnsi/tests/tests/mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      444 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/edc_mnsi/tests/tests/test_auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)    15460 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/edc_mnsi/tests/tests/test_mnsi_calculators.py
--rw-r--r--   0 erikvw     (501) staff       (20)    18557 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/edc_mnsi/tests/tests/test_mnsi_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3926 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/edc_mnsi/tests/tests/test_mnsi_model.py
--rw-r--r--   0 erikvw     (501) staff       (20)      283 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/edc_mnsi/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      377 2021-09-20 00:22:50.000000 edc-mnsi-0.1.8/edc_mnsi/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:55:14.514165 edc-mnsi-0.1.8/edc_mnsi.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     5218 2022-07-06 06:55:14.000000 edc-mnsi-0.1.8/edc_mnsi.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1677 2022-07-06 06:55:14.000000 edc-mnsi-0.1.8/edc_mnsi.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-07-06 06:55:14.000000 edc-mnsi-0.1.8/edc_mnsi.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-08-16 17:35:18.000000 edc-mnsi-0.1.8/edc_mnsi.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)        9 2022-07-06 06:55:14.000000 edc-mnsi-0.1.8/edc_mnsi.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1641 2022-06-01 21:57:55.000000 edc-mnsi-0.1.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1683 2022-06-01 21:57:55.000000 edc-mnsi-0.1.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1159 2022-07-06 06:55:14.519045 edc-mnsi-0.1.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 22:43:50.393311 edc-mnsi-0.1.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       84 2021-08-16 21:28:17.000000 edc-mnsi-0.1.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-08-16 21:28:17.000000 edc-mnsi-0.1.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 22:43:50.382587 edc-mnsi-0.1.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 22:43:50.385752 edc-mnsi-0.1.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-10 22:43:41.000000 edc-mnsi-0.1.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-06-01 21:57:55.000000 edc-mnsi-0.1.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-10 22:43:41.000000 edc-mnsi-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 22:43:41.000000 edc-mnsi-0.1.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)       89 2021-08-16 21:28:17.000000 edc-mnsi-0.1.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       83 2022-06-23 21:18:38.000000 edc-mnsi-0.1.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-08-16 16:49:13.000000 edc-mnsi-0.1.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 21:57:55.000000 edc-mnsi-0.1.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     5347 2022-08-10 22:43:50.393430 edc-mnsi-0.1.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     4350 2021-09-20 00:22:50.000000 edc-mnsi-0.1.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-10 22:43:41.000000 edc-mnsi-0.1.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-10 22:43:41.000000 edc-mnsi-0.1.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 22:43:50.388663 edc-mnsi-0.1.9/edc_mnsi/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-16 21:28:17.000000 edc-mnsi-0.1.9/edc_mnsi/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1296 2021-09-21 15:50:47.000000 edc-mnsi-0.1.9/edc_mnsi/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      161 2021-09-20 00:22:50.000000 edc-mnsi-0.1.9/edc_mnsi/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      217 2021-09-20 00:22:50.000000 edc-mnsi-0.1.9/edc_mnsi/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      457 2021-09-23 17:43:23.000000 edc-mnsi-0.1.9/edc_mnsi/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      305 2021-09-20 00:22:50.000000 edc-mnsi-0.1.9/edc_mnsi/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4936 2022-06-23 21:18:38.000000 edc-mnsi-0.1.9/edc_mnsi/calculator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      730 2021-08-18 16:06:55.000000 edc-mnsi-0.1.9/edc_mnsi/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2868 2021-09-21 15:50:47.000000 edc-mnsi-0.1.9/edc_mnsi/factory.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1960 2021-09-20 00:22:50.000000 edc-mnsi-0.1.9/edc_mnsi/fieldsets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2995 2021-09-20 00:22:50.000000 edc-mnsi-0.1.9/edc_mnsi/form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      379 2021-09-20 00:22:50.000000 edc-mnsi-0.1.9/edc_mnsi/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      912 2021-09-20 00:22:50.000000 edc-mnsi-0.1.9/edc_mnsi/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 22:43:50.390225 edc-mnsi-0.1.9/edc_mnsi/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2578 2022-08-10 22:43:41.000000 edc-mnsi-0.1.9/edc_mnsi/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    41832 2022-08-10 22:43:41.000000 edc-mnsi-0.1.9/edc_mnsi/migrations/0002_historicalmnsi_mnsi.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      987 2022-06-01 21:57:55.000000 edc-mnsi-0.1.9/edc_mnsi/migrations/0003_alter_mnsi_abnormal_obs_left_foot_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      873 2022-07-06 06:54:56.000000 edc-mnsi-0.1.9/edc_mnsi/migrations/0004_auto_20220704_1841.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-16 21:28:17.000000 edc-mnsi-0.1.9/edc_mnsi/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1615 2021-09-20 00:22:50.000000 edc-mnsi-0.1.9/edc_mnsi/model_admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5601 2021-09-20 00:22:50.000000 edc-mnsi-0.1.9/edc_mnsi/model_mixins.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 22:43:50.390829 edc-mnsi-0.1.9/edc_mnsi/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      138 2021-09-20 00:22:50.000000 edc-mnsi-0.1.9/edc_mnsi/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      284 2021-09-20 00:22:50.000000 edc-mnsi-0.1.9/edc_mnsi/models/list_models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-06-01 21:57:55.000000 edc-mnsi-0.1.9/edc_mnsi/models/mnsi.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      495 2021-09-20 00:22:50.000000 edc-mnsi-0.1.9/edc_mnsi/models/signals.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 22:43:50.391067 edc-mnsi-0.1.9/edc_mnsi/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-17 21:32:34.000000 edc-mnsi-0.1.9/edc_mnsi/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 22:43:50.392361 edc-mnsi-0.1.9/edc_mnsi/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-16 21:28:17.000000 edc-mnsi-0.1.9/edc_mnsi/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-16 21:28:17.000000 edc-mnsi-0.1.9/edc_mnsi/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2021-08-16 21:28:17.000000 edc-mnsi-0.1.9/edc_mnsi/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-08-16 21:28:17.000000 edc-mnsi-0.1.9/edc_mnsi/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-08-16 21:28:17.000000 edc-mnsi-0.1.9/edc_mnsi/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-08-16 21:28:17.000000 edc-mnsi-0.1.9/edc_mnsi/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-16 21:28:17.000000 edc-mnsi-0.1.9/edc_mnsi/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-16 21:28:17.000000 edc-mnsi-0.1.9/edc_mnsi/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      627 2021-09-20 00:22:50.000000 edc-mnsi-0.1.9/edc_mnsi/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 22:43:50.393184 edc-mnsi-0.1.9/edc_mnsi/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-16 21:28:17.000000 edc-mnsi-0.1.9/edc_mnsi/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7158 2022-06-01 21:57:55.000000 edc-mnsi-0.1.9/edc_mnsi/tests/tests/mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      444 2021-09-20 00:22:50.000000 edc-mnsi-0.1.9/edc_mnsi/tests/tests/test_auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    15460 2021-09-20 00:22:50.000000 edc-mnsi-0.1.9/edc_mnsi/tests/tests/test_mnsi_calculators.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    18557 2021-09-20 00:22:50.000000 edc-mnsi-0.1.9/edc_mnsi/tests/tests/test_mnsi_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3926 2021-09-20 00:22:50.000000 edc-mnsi-0.1.9/edc_mnsi/tests/tests/test_mnsi_model.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      283 2021-09-20 00:22:50.000000 edc-mnsi-0.1.9/edc_mnsi/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      377 2021-09-20 00:22:50.000000 edc-mnsi-0.1.9/edc_mnsi/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-10 22:43:50.389350 edc-mnsi-0.1.9/edc_mnsi.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     5347 2022-08-10 22:43:50.000000 edc-mnsi-0.1.9/edc_mnsi.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1711 2022-08-10 22:43:50.000000 edc-mnsi-0.1.9/edc_mnsi.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-10 22:43:50.000000 edc-mnsi-0.1.9/edc_mnsi.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-08-16 17:35:18.000000 edc-mnsi-0.1.9/edc_mnsi.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)        9 2022-08-10 22:43:50.000000 edc-mnsi-0.1.9/edc_mnsi.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1718 2022-08-10 22:43:41.000000 edc-mnsi-0.1.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1683 2022-06-01 21:57:55.000000 edc-mnsi-0.1.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1257 2022-08-10 22:43:50.393766 edc-mnsi-0.1.9/setup.cfg
```

### Comparing `edc-mnsi-0.1.8/.github/workflows/build.yml` & `edc-mnsi-0.1.9/.github/workflows/build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,70 +1,71 @@
+---
 name: build
 
 on: [push, pull_request]
 
 jobs:
   build:
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
         python-version: ['3.9', '3.10']
-        django-version: ['3.2', '4.0', 'dev']
+        django-version: ['3.2', '4.0', '4.1', 'dev']
 
     services:
 
       mysql:
         image: mysql:latest
         env:
           MYSQL_DATABASE: mysql
           MYSQL_ROOT_PASSWORD: mysql
         ports:
           - 3306:3306
         options: --health-cmd="mysqladmin ping" --health-interval=10s --health-timeout=5s --health-retries=3
 
     steps:
-    - name: Install pycups and words dependency
-      run: |
-        sudo sed -i 's/azure\.//' /etc/apt/sources.list
-        sudo apt-get -y update
-        sudo apt-get install libcups2-dev wamerican
-
-    - uses: actions/checkout@v2
-
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
-      with:
-        python-version: ${{ matrix.python-version }}
-
-    - name: Get pip cache dir
-      id: pip-cache
-      run: |
-        echo "::set-output name=dir::$(pip cache dir)"
-
-    - name: Cache
-      uses: actions/cache@v2
-      with:
-        path: ${{ steps.pip-cache.outputs.dir }}
-        key:
-          ${{ matrix.python-version }}-v1-${{ hashFiles('**/setup.py') }}-${{ hashFiles('**/tox.ini') }}
-        restore-keys: |
-          ${{ matrix.python-version }}-v1-
-
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        python -m pip install -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
-
-
-    - name: Tox tests
-      run: |
-        tox -v
-      env:
-        DJANGO: ${{ matrix.django-version }}
-
-    - name: Upload coverage
-      uses: codecov/codecov-action@v1
-      with:
-        name: Python ${{ matrix.python-version }}
+      - name: Install pycups and words dependency
+        run: |
+          sudo sed -i 's/azure\.//' /etc/apt/sources.list
+          sudo apt-get -y update
+          sudo apt-get install libcups2-dev wamerican
+
+      - uses: actions/checkout@v2
+
+      - name: Set up Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v2
+        with:
+          python-version: ${{ matrix.python-version }}
+
+      - name: Get pip cache dir
+        id: pip-cache
+        run: |
+          echo "::set-output name=dir::$(pip cache dir)"
+
+      - name: Cache
+        uses: actions/cache@v2
+        with:
+          path: ${{ steps.pip-cache.outputs.dir }}
+          key:
+            ${{ matrix.python-version }}-v1-${{ hashFiles('**/setup.py') }}-${{ hashFiles('**/tox.ini') }}
+          restore-keys: |
+            ${{ matrix.python-version }}-v1-
+
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          python -m pip install -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
+
+
+      - name: Tox tests
+        run: |
+          tox -v
+        env:
+          DJANGO: ${{ matrix.django-version }}
+
+      - name: Upload coverage
+        uses: codecov/codecov-action@v1
+        with:
+          name: Python ${{ matrix.python-version }}
```

### Comparing `edc-mnsi-0.1.8/.gitignore` & `edc-mnsi-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/LICENSE` & `edc-mnsi-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/PKG-INFO` & `edc-mnsi-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: edc-mnsi
-Version: 0.1.8
+Version: 0.1.9
 Summary: MNSI form/model for the clinicedc/edc and other django projects
 Home-page: https://github.com/clinicedc/edc-mnsi
 Author: Jonathan Willitts
 Author-email: Jonathan.Willitts@lstmed.ac.uk
 License: GPL license, see LICENSE
 Keywords: django edc mnsi,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |codecov| |downloads|
```

### Comparing `edc-mnsi-0.1.8/README.rst` & `edc-mnsi-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/edc_mnsi/admin.py` & `edc-mnsi-0.1.9/edc_mnsi/admin.py`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/edc_mnsi/calculator.py` & `edc-mnsi-0.1.9/edc_mnsi/calculator.py`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/edc_mnsi/choices.py` & `edc-mnsi-0.1.9/edc_mnsi/choices.py`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/edc_mnsi/factory.py` & `edc-mnsi-0.1.9/edc_mnsi/factory.py`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/edc_mnsi/fieldsets.py` & `edc-mnsi-0.1.9/edc_mnsi/fieldsets.py`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/edc_mnsi/form_validator.py` & `edc-mnsi-0.1.9/edc_mnsi/form_validator.py`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/edc_mnsi/list_data.py` & `edc-mnsi-0.1.9/edc_mnsi/list_data.py`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/edc_mnsi/migrations/0003_alter_mnsi_abnormal_obs_left_foot_and_more.py` & `edc-mnsi-0.1.9/edc_mnsi/migrations/0003_alter_mnsi_abnormal_obs_left_foot_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/edc_mnsi/migrations/0004_auto_20220704_1841.py` & `edc-mnsi-0.1.9/edc_mnsi/migrations/0004_auto_20220704_1841.py`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/edc_mnsi/model_admin_mixin.py` & `edc-mnsi-0.1.9/edc_mnsi/model_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/edc_mnsi/model_mixins.py` & `edc-mnsi-0.1.9/edc_mnsi/model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/edc_mnsi/models/mnsi.py` & `edc-mnsi-0.1.9/edc_mnsi/models/mnsi.py`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/edc_mnsi/tests/etc/user-rsa-local-private.pem` & `edc-mnsi-0.1.9/edc_mnsi/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/edc_mnsi/tests/etc/user-rsa-restricted-private.pem` & `edc-mnsi-0.1.9/edc_mnsi/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/edc_mnsi/tests/models.py` & `edc-mnsi-0.1.9/edc_mnsi/tests/models.py`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/edc_mnsi/tests/tests/mixins.py` & `edc-mnsi-0.1.9/edc_mnsi/tests/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/edc_mnsi/tests/tests/test_mnsi_calculators.py` & `edc-mnsi-0.1.9/edc_mnsi/tests/tests/test_mnsi_calculators.py`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/edc_mnsi/tests/tests/test_mnsi_form_validator.py` & `edc-mnsi-0.1.9/edc_mnsi/tests/tests/test_mnsi_form_validator.py`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/edc_mnsi/tests/tests/test_mnsi_model.py` & `edc-mnsi-0.1.9/edc_mnsi/tests/tests/test_mnsi_model.py`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/edc_mnsi.egg-info/PKG-INFO` & `edc-mnsi-0.1.9/edc_mnsi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: edc-mnsi
-Version: 0.1.8
+Version: 0.1.9
 Summary: MNSI form/model for the clinicedc/edc and other django projects
 Home-page: https://github.com/clinicedc/edc-mnsi
 Author: Jonathan Willitts
 Author-email: Jonathan.Willitts@lstmed.ac.uk
 License: GPL license, see LICENSE
 Keywords: django edc mnsi,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |codecov| |downloads|
```

### Comparing `edc-mnsi-0.1.8/edc_mnsi.egg-info/SOURCES.txt` & `edc-mnsi-0.1.9/edc_mnsi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 .coveragerc
 .editorconfig
 .gitignore
+.pre-commit-config.yaml
+.yamllint
 AUTHORS
 CHANGES
 LICENSE
 MANIFEST.in
 README.rst
 VERSION
 codecov.yml
```

### Comparing `edc-mnsi-0.1.8/pyproject.toml` & `edc-mnsi-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -28,42 +28,47 @@
 skip_covered = true
 omit = ["requirements.txt"]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{39,310}-dj{32,40,dev},
+    py{38,39,310}-dj{32,40,41,dev},
     lint
+
 isolated_build = true
 
 [gh-actions]
 python =
+    3.8: py38
     3.9: py39, lint
     3.10: py310
 
 [gh-actions:env]
 DJANGO =
     3.2: dj32, lint
     4.0: dj40
+    4.1: dj41
     dev: djdev
 
 [testenv]
 deps =
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/test_utils.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/edc.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/third_party_dev.txt
     dj32: Django>=3.2,<3.3
     dj40: Django>=4.0,<4.1
+    dj41: Django>=4.1,<4.2
     djdev: https://github.com/django/django/tarball/main
 
 commands =
     pip install -U pip
     pip --version
+    pip freeze
     coverage run -a runtests.py
     coverage report
 
 [testenv:lint]
 deps = -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/lint.txt
 commands =
     isort --profile=black --check --diff .
```

### Comparing `edc-mnsi-0.1.8/runtests.py` & `edc-mnsi-0.1.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-mnsi-0.1.8/setup.cfg` & `edc-mnsi-0.1.9/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -9,19 +9,22 @@
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = django edc mnsi, clinicedc, clinical trials
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.2
+	Framework :: Django :: 4.0
+	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 
 [options]
 python_requires = >=3.8
 zip_safe = False
 include_package_data = True
 packages = find:
@@ -34,14 +37,14 @@
 	bin*
 	edc_mnsi.tests*
 
 [flake8]
 ignore = E226,W503,E203
 max-line-length = 95
 max-complexity = 10
-exclude = */migrations,.tox,.git,__pycache__,build,dist,.eggs
+exclude = */migrations/*,.tox,.git,__pycache__,build,dist,.eggs
 per-file-ignores = __init__.py: F401
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

