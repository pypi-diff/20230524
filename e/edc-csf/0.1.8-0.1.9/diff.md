# Comparing `tmp/edc-csf-0.1.8.tar.gz` & `tmp/edc-csf-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-csf-0.1.8.tar", last modified: Wed Jul 13 22:50:06 2022, max compression
+gzip compressed data, was "edc-csf-0.1.9.tar", last modified: Thu Jul 14 10:19:08 2022, max compression
```

## Comparing `edc-csf-0.1.8.tar` & `edc-csf-0.1.9.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-13 22:50:06.176242 edc-csf-0.1.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       81 2022-02-21 17:26:40.000000 edc-csf-0.1.8/.coveragrc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-02-21 17:26:40.000000 edc-csf-0.1.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-13 22:50:06.165803 edc-csf-0.1.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-13 22:50:06.168667 edc-csf-0.1.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1846 2022-07-13 22:49:58.000000 edc-csf-0.1.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1842 2022-05-04 03:54:27.000000 edc-csf-0.1.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-04 03:54:27.000000 edc-csf-0.1.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2022-05-04 03:54:27.000000 edc-csf-0.1.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-01-11 21:38:46.000000 edc-csf-0.1.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 17:59:32.000000 edc-csf-0.1.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1440 2022-07-13 22:50:06.176347 edc-csf-0.1.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      591 2022-02-21 17:30:42.000000 edc-csf-0.1.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-07-13 22:49:58.000000 edc-csf-0.1.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-02-21 17:26:40.000000 edc-csf-0.1.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-13 22:50:06.171288 edc-csf-0.1.8/edc_csf/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1636 2022-05-07 02:00:54.000000 edc-csf-0.1.8/edc_csf/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      159 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      866 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/aliquot_types.py
--rw-r--r--   0 erikvw     (501) staff       (20)      394 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      544 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      303 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)      567 2022-06-08 19:36:30.000000 edc-csf-0.1.8/edc_csf/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1884 2022-02-28 17:47:24.000000 edc-csf-0.1.8/edc_csf/fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4390 2022-07-13 22:49:58.000000 edc-csf-0.1.8/edc_csf/form_validators.py
--rw-r--r--   0 erikvw     (501) staff       (20)      385 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/forms.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-13 22:50:06.173201 edc-csf-0.1.8/edc_csf/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    31592 2022-06-01 17:59:32.000000 edc-csf-0.1.8/edc_csf/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      853 2022-02-28 17:47:24.000000 edc-csf-0.1.8/edc_csf/migrations/0002_auto_20220225_0419.py
--rw-r--r--   0 erikvw     (501) staff       (20)      908 2022-02-28 17:47:24.000000 edc-csf-0.1.8/edc_csf/migrations/0003_auto_20220225_0423.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5426 2022-02-28 17:47:24.000000 edc-csf-0.1.8/edc_csf/migrations/0004_auto_20220225_0500.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2000 2022-02-28 17:47:24.000000 edc-csf-0.1.8/edc_csf/migrations/0005_auto_20220225_2142.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1768 2022-02-28 17:47:24.000000 edc-csf-0.1.8/edc_csf/migrations/0006_auto_20220228_2032.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-13 22:50:06.174065 edc-csf-0.1.8/edc_csf/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      255 2022-02-28 17:47:24.000000 edc-csf-0.1.8/edc_csf/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/model_mixins/biosynex_semi_quantitative_crag_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1526 2022-02-28 17:47:24.000000 edc-csf-0.1.8/edc_csf/model_mixins/csf.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3656 2022-06-01 17:59:32.000000 edc-csf-0.1.8/edc_csf/model_mixins/csf_culture.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1372 2022-06-01 17:59:32.000000 edc-csf-0.1.8/edc_csf/model_mixins/lp.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1018 2022-06-01 17:59:32.000000 edc-csf-0.1.8/edc_csf/model_mixins/quantitative_culture.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1048 2022-02-28 17:47:24.000000 edc-csf-0.1.8/edc_csf/modeladmin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1053 2022-06-01 17:59:32.000000 edc-csf-0.1.8/edc_csf/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1000 2022-02-25 16:08:55.000000 edc-csf-0.1.8/edc_csf/panels.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1425 2022-02-25 16:09:02.000000 edc-csf-0.1.8/edc_csf/processing_profiles.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-13 22:50:06.174263 edc-csf-0.1.8/edc_csf/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-13 22:50:06.175585 edc-csf-0.1.8/edc_csf/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-13 22:50:06.175816 edc-csf-0.1.8/edc_csf/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11181 2022-07-13 22:49:58.000000 edc-csf-0.1.8/edc_csf/tests/tests/test_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      280 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-13 22:50:06.172005 edc-csf-0.1.8/edc_csf.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1440 2022-07-13 22:50:06.000000 edc-csf-0.1.8/edc_csf.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1714 2022-07-13 22:50:06.000000 edc-csf-0.1.8/edc_csf.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-07-13 22:50:06.000000 edc-csf-0.1.8/edc_csf.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-02-21 17:29:11.000000 edc-csf-0.1.8/edc_csf.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       20 2022-07-13 22:50:06.000000 edc-csf-0.1.8/edc_csf.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-13 22:50:06.176127 edc-csf-0.1.8/edc_csf_app/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf_app/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      147 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf_app/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1111 2022-02-21 17:26:40.000000 edc-csf-0.1.8/edc_csf_app/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1635 2022-07-13 22:49:58.000000 edc-csf-0.1.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1850 2022-02-21 17:26:40.000000 edc-csf-0.1.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1139 2022-07-13 22:50:06.176680 edc-csf-0.1.8/setup.cfg
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-07-14 10:19:08.416100 edc-csf-0.1.9/
+-rw-r--r--   0 jw         (502) staff       (20)       81 2022-03-01 11:06:54.000000 edc-csf-0.1.9/.coveragrc
+-rw-r--r--   0 jw         (502) staff       (20)      436 2022-03-01 11:06:54.000000 edc-csf-0.1.9/.editorconfig
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-07-14 10:19:08.323338 edc-csf-0.1.9/.github/
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-07-14 10:19:08.334424 edc-csf-0.1.9/.github/workflows/
+-rw-r--r--   0 jw         (502) staff       (20)     1846 2022-07-11 16:27:14.000000 edc-csf-0.1.9/.github/workflows/build.yml
+-rw-r--r--   0 jw         (502) staff       (20)     1842 2022-05-05 09:36:37.000000 edc-csf-0.1.9/.gitignore
+-rw-r--r--   0 jw         (502) staff       (20)        0 2022-05-05 09:36:37.000000 edc-csf-0.1.9/AUTHORS
+-rw-r--r--   0 jw         (502) staff       (20)       22 2022-05-05 09:36:37.000000 edc-csf-0.1.9/CHANGES
+-rw-r--r--   0 jw         (502) staff       (20)    35149 2022-03-01 11:06:54.000000 edc-csf-0.1.9/LICENSE
+-rw-r--r--   0 jw         (502) staff       (20)       74 2022-06-06 12:48:59.000000 edc-csf-0.1.9/MANIFEST.in
+-rw-r--r--   0 jw         (502) staff       (20)     1440 2022-07-14 10:19:08.416780 edc-csf-0.1.9/PKG-INFO
+-rw-r--r--   0 jw         (502) staff       (20)      591 2022-03-01 11:06:54.000000 edc-csf-0.1.9/README.rst
+-rw-r--r--   0 jw         (502) staff       (20)        6 2022-07-14 10:18:55.000000 edc-csf-0.1.9/VERSION
+-rw-r--r--   0 jw         (502) staff       (20)      162 2022-03-01 11:06:54.000000 edc-csf-0.1.9/codecov.yml
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-07-14 10:19:08.354380 edc-csf-0.1.9/edc_csf/
+-rw-r--r--   0 jw         (502) staff       (20)        0 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/__init__.py
+-rw-r--r--   0 jw         (502) staff       (20)     1636 2022-05-07 18:34:42.000000 edc-csf-0.1.9/edc_csf/admin.py
+-rw-r--r--   0 jw         (502) staff       (20)      159 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/admin_site.py
+-rw-r--r--   0 jw         (502) staff       (20)      866 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/aliquot_types.py
+-rw-r--r--   0 jw         (502) staff       (20)      394 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/apps.py
+-rw-r--r--   0 jw         (502) staff       (20)      544 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/auth_objects.py
+-rw-r--r--   0 jw         (502) staff       (20)      303 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/auths.py
+-rw-r--r--   0 jw         (502) staff       (20)      567 2022-06-08 15:44:49.000000 edc-csf-0.1.9/edc_csf/choices.py
+-rw-r--r--   0 jw         (502) staff       (20)     1884 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/fieldsets.py
+-rw-r--r--   0 jw         (502) staff       (20)     4390 2022-07-14 10:04:07.000000 edc-csf-0.1.9/edc_csf/form_validators.py
+-rw-r--r--   0 jw         (502) staff       (20)      385 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/forms.py
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-07-14 10:19:08.382187 edc-csf-0.1.9/edc_csf/migrations/
+-rw-r--r--   0 jw         (502) staff       (20)    31592 2022-06-06 12:48:59.000000 edc-csf-0.1.9/edc_csf/migrations/0001_initial.py
+-rw-r--r--   0 jw         (502) staff       (20)      853 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/migrations/0002_auto_20220225_0419.py
+-rw-r--r--   0 jw         (502) staff       (20)      908 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/migrations/0003_auto_20220225_0423.py
+-rw-r--r--   0 jw         (502) staff       (20)     5426 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/migrations/0004_auto_20220225_0500.py
+-rw-r--r--   0 jw         (502) staff       (20)     2000 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/migrations/0005_auto_20220225_2142.py
+-rw-r--r--   0 jw         (502) staff       (20)     1768 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/migrations/0006_auto_20220228_2032.py
+-rw-r--r--   0 jw         (502) staff       (20)      747 2022-07-14 10:18:55.000000 edc-csf-0.1.9/edc_csf/migrations/0007_auto_20220711_1230.py
+-rw-r--r--   0 jw         (502) staff       (20)        0 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/migrations/__init__.py
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-07-14 10:19:08.388607 edc-csf-0.1.9/edc_csf/model_mixins/
+-rw-r--r--   0 jw         (502) staff       (20)      255 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/model_mixins/__init__.py
+-rw-r--r--   0 jw         (502) staff       (20)     1076 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/model_mixins/biosynex_semi_quantitative_crag_mixin.py
+-rw-r--r--   0 jw         (502) staff       (20)     1526 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/model_mixins/csf.py
+-rw-r--r--   0 jw         (502) staff       (20)     3656 2022-06-06 12:48:59.000000 edc-csf-0.1.9/edc_csf/model_mixins/csf_culture.py
+-rw-r--r--   0 jw         (502) staff       (20)     1372 2022-06-06 12:48:59.000000 edc-csf-0.1.9/edc_csf/model_mixins/lp.py
+-rw-r--r--   0 jw         (502) staff       (20)     1018 2022-06-06 12:48:59.000000 edc-csf-0.1.9/edc_csf/model_mixins/quantitative_culture.py
+-rw-r--r--   0 jw         (502) staff       (20)     1048 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/modeladmin_mixins.py
+-rw-r--r--   0 jw         (502) staff       (20)     1053 2022-06-06 12:48:59.000000 edc-csf-0.1.9/edc_csf/models.py
+-rw-r--r--   0 jw         (502) staff       (20)     1000 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/panels.py
+-rw-r--r--   0 jw         (502) staff       (20)     1425 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/processing_profiles.py
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-07-14 10:19:08.389418 edc-csf-0.1.9/edc_csf/tests/
+-rw-r--r--   0 jw         (502) staff       (20)        0 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/tests/__init__.py
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-07-14 10:19:08.406620 edc-csf-0.1.9/edc_csf/tests/etc/
+-rw-r--r--   0 jw         (502) staff       (20)      256 2022-06-08 19:03:11.000000 edc-csf-0.1.9/edc_csf/tests/etc/user-aes-local.key
+-rw-r--r--   0 jw         (502) staff       (20)      256 2022-06-08 19:03:11.000000 edc-csf-0.1.9/edc_csf/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 jw         (502) staff       (20)     1678 2022-06-08 19:03:11.000000 edc-csf-0.1.9/edc_csf/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 jw         (502) staff       (20)      450 2022-06-08 19:03:11.000000 edc-csf-0.1.9/edc_csf/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 jw         (502) staff       (20)     1674 2022-06-08 19:03:11.000000 edc-csf-0.1.9/edc_csf/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 jw         (502) staff       (20)      450 2022-06-08 19:03:11.000000 edc-csf-0.1.9/edc_csf/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 jw         (502) staff       (20)      256 2022-06-08 19:03:11.000000 edc-csf-0.1.9/edc_csf/tests/etc/user-salt-local.key
+-rw-r--r--   0 jw         (502) staff       (20)      256 2022-06-08 19:03:11.000000 edc-csf-0.1.9/edc_csf/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 jw         (502) staff       (20)        0 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/tests/models.py
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-07-14 10:19:08.411237 edc-csf-0.1.9/edc_csf/tests/tests/
+-rw-r--r--   0 jw         (502) staff       (20)        0 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/tests/tests/__init__.py
+-rw-r--r--   0 jw         (502) staff       (20)    11181 2022-07-14 10:04:07.000000 edc-csf-0.1.9/edc_csf/tests/tests/test_form.py
+-rw-r--r--   0 jw         (502) staff       (20)      280 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf/urls.py
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-07-14 10:19:08.361619 edc-csf-0.1.9/edc_csf.egg-info/
+-rw-r--r--   0 jw         (502) staff       (20)     1440 2022-07-14 10:19:08.000000 edc-csf-0.1.9/edc_csf.egg-info/PKG-INFO
+-rw-r--r--   0 jw         (502) staff       (20)     1760 2022-07-14 10:19:08.000000 edc-csf-0.1.9/edc_csf.egg-info/SOURCES.txt
+-rw-r--r--   0 jw         (502) staff       (20)        1 2022-07-14 10:19:08.000000 edc-csf-0.1.9/edc_csf.egg-info/dependency_links.txt
+-rw-r--r--   0 jw         (502) staff       (20)        1 2022-03-01 11:07:22.000000 edc-csf-0.1.9/edc_csf.egg-info/not-zip-safe
+-rw-r--r--   0 jw         (502) staff       (20)       20 2022-07-14 10:19:08.000000 edc-csf-0.1.9/edc_csf.egg-info/top_level.txt
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2022-07-14 10:19:08.414837 edc-csf-0.1.9/edc_csf_app/
+-rw-r--r--   0 jw         (502) staff       (20)        0 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf_app/__init__.py
+-rw-r--r--   0 jw         (502) staff       (20)      147 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf_app/apps.py
+-rw-r--r--   0 jw         (502) staff       (20)     1111 2022-03-01 11:06:54.000000 edc-csf-0.1.9/edc_csf_app/models.py
+-rw-r--r--   0 jw         (502) staff       (20)     1635 2022-07-14 10:04:07.000000 edc-csf-0.1.9/pyproject.toml
+-rw-r--r--   0 jw         (502) staff       (20)     1850 2022-03-01 11:06:54.000000 edc-csf-0.1.9/runtests.py
+-rw-r--r--   0 jw         (502) staff       (20)     1139 2022-07-14 10:19:08.417905 edc-csf-0.1.9/setup.cfg
```

### Comparing `edc-csf-0.1.8/.github/workflows/build.yml` & `edc-csf-0.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/.gitignore` & `edc-csf-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/LICENSE` & `edc-csf-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/PKG-INFO` & `edc-csf-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-csf
-Version: 0.1.8
+Version: 0.1.9
 Summary: Classes for CSF/LP in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-csf
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc csf lumbar puncture,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-csf-0.1.8/README.rst` & `edc-csf-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/admin.py` & `edc-csf-0.1.9/edc_csf/admin.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/aliquot_types.py` & `edc-csf-0.1.9/edc_csf/aliquot_types.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/auth_objects.py` & `edc-csf-0.1.9/edc_csf/auth_objects.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/choices.py` & `edc-csf-0.1.9/edc_csf/choices.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/fieldsets.py` & `edc-csf-0.1.9/edc_csf/fieldsets.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/form_validators.py` & `edc-csf-0.1.9/edc_csf/form_validators.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/migrations/0001_initial.py` & `edc-csf-0.1.9/edc_csf/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/migrations/0002_auto_20220225_0419.py` & `edc-csf-0.1.9/edc_csf/migrations/0002_auto_20220225_0419.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/migrations/0003_auto_20220225_0423.py` & `edc-csf-0.1.9/edc_csf/migrations/0003_auto_20220225_0423.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/migrations/0004_auto_20220225_0500.py` & `edc-csf-0.1.9/edc_csf/migrations/0004_auto_20220225_0500.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/migrations/0005_auto_20220225_2142.py` & `edc-csf-0.1.9/edc_csf/migrations/0005_auto_20220225_2142.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/migrations/0006_auto_20220228_2032.py` & `edc-csf-0.1.9/edc_csf/migrations/0006_auto_20220228_2032.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/model_mixins/biosynex_semi_quantitative_crag_mixin.py` & `edc-csf-0.1.9/edc_csf/model_mixins/biosynex_semi_quantitative_crag_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/model_mixins/csf.py` & `edc-csf-0.1.9/edc_csf/model_mixins/csf.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/model_mixins/csf_culture.py` & `edc-csf-0.1.9/edc_csf/model_mixins/csf_culture.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/model_mixins/lp.py` & `edc-csf-0.1.9/edc_csf/model_mixins/lp.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/model_mixins/quantitative_culture.py` & `edc-csf-0.1.9/edc_csf/model_mixins/quantitative_culture.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/modeladmin_mixins.py` & `edc-csf-0.1.9/edc_csf/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/models.py` & `edc-csf-0.1.9/edc_csf/models.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/panels.py` & `edc-csf-0.1.9/edc_csf/panels.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/processing_profiles.py` & `edc-csf-0.1.9/edc_csf/processing_profiles.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/tests/etc/user-rsa-local-private.pem` & `edc-csf-0.1.9/edc_csf/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/tests/etc/user-rsa-restricted-private.pem` & `edc-csf-0.1.9/edc_csf/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf/tests/tests/test_form.py` & `edc-csf-0.1.9/edc_csf/tests/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/edc_csf.egg-info/PKG-INFO` & `edc-csf-0.1.9/edc_csf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-csf
-Version: 0.1.8
+Version: 0.1.9
 Summary: Classes for CSF/LP in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-csf
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc csf lumbar puncture,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-csf-0.1.8/edc_csf.egg-info/SOURCES.txt` & `edc-csf-0.1.9/edc_csf.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 edc_csf.egg-info/top_level.txt
 edc_csf/migrations/0001_initial.py
 edc_csf/migrations/0002_auto_20220225_0419.py
 edc_csf/migrations/0003_auto_20220225_0423.py
 edc_csf/migrations/0004_auto_20220225_0500.py
 edc_csf/migrations/0005_auto_20220225_2142.py
 edc_csf/migrations/0006_auto_20220228_2032.py
+edc_csf/migrations/0007_auto_20220711_1230.py
 edc_csf/migrations/__init__.py
 edc_csf/model_mixins/__init__.py
 edc_csf/model_mixins/biosynex_semi_quantitative_crag_mixin.py
 edc_csf/model_mixins/csf.py
 edc_csf/model_mixins/csf_culture.py
 edc_csf/model_mixins/lp.py
 edc_csf/model_mixins/quantitative_culture.py
```

### Comparing `edc-csf-0.1.8/edc_csf_app/models.py` & `edc-csf-0.1.9/edc_csf_app/models.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/pyproject.toml` & `edc-csf-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/runtests.py` & `edc-csf-0.1.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-csf-0.1.8/setup.cfg` & `edc-csf-0.1.9/setup.cfg`

 * *Files identical despite different names*

