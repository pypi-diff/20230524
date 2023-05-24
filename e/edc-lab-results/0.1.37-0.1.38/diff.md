# Comparing `tmp/edc-lab-results-0.1.37.tar.gz` & `tmp/edc-lab-results-0.1.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-lab-results-0.1.37.tar", last modified: Thu Mar 23 15:11:09 2023, max compression
+gzip compressed data, was "edc-lab-results-0.1.38.tar", last modified: Wed May 24 17:18:39 2023, max compression
```

## Comparing `edc-lab-results-0.1.37.tar` & `edc-lab-results-0.1.38.tar`

### file list

```diff
@@ -1,78 +1,77 @@
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-03-23 15:11:09.464299 edc-lab-results-0.1.37/
--rw-r--r--   0 jw         (502) staff       (20)       76 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/.coveragerc
--rw-r--r--   0 jw         (502) staff       (20)      436 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/.editorconfig
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-03-23 15:11:09.435252 edc-lab-results-0.1.37/.github/
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-03-23 15:11:09.444673 edc-lab-results-0.1.37/.github/workflows/
--rw-r--r--   0 jw         (502) staff       (20)     1929 2023-03-23 15:10:58.000000 edc-lab-results-0.1.37/.github/workflows/build.yml
--rw-r--r--   0 jw         (502) staff       (20)     1842 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/.gitignore
--rw-r--r--   0 jw         (502) staff       (20)     1075 2023-03-23 15:10:58.000000 edc-lab-results-0.1.37/.pre-commit-config.yaml
--rw-r--r--   0 jw         (502) staff       (20)      291 2022-08-10 16:08:09.000000 edc-lab-results-0.1.37/.yamllint
--rw-r--r--   0 jw         (502) staff       (20)        0 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/AUTHORS
--rw-r--r--   0 jw         (502) staff       (20)      402 2023-03-23 15:10:58.000000 edc-lab-results-0.1.37/CHANGES
--rw-r--r--   0 jw         (502) staff       (20)    35149 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/LICENSE
--rw-r--r--   0 jw         (502) staff       (20)       74 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/MANIFEST.in
--rw-r--r--   0 jw         (502) staff       (20)     1644 2023-03-23 15:11:09.464476 edc-lab-results-0.1.37/PKG-INFO
--rw-r--r--   0 jw         (502) staff       (20)      733 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/README.rst
--rw-r--r--   0 jw         (502) staff       (20)        7 2023-03-23 15:10:57.000000 edc-lab-results-0.1.37/VERSION
--rw-r--r--   0 jw         (502) staff       (20)      166 2022-08-10 16:08:09.000000 edc-lab-results-0.1.37/codecov.yml
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-03-23 15:11:09.447131 edc-lab-results-0.1.37/edc_lab_results/
--rw-r--r--   0 jw         (502) staff       (20)      276 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/__init__.py
--rw-r--r--   0 jw         (502) staff       (20)     3809 2023-03-23 15:10:58.000000 edc-lab-results-0.1.37/edc_lab_results/action_items.py
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-03-23 15:11:09.450069 edc-lab-results-0.1.37/edc_lab_results/admin/
--rw-r--r--   0 jw         (502) staff       (20)      154 2023-02-15 21:40:54.000000 edc-lab-results-0.1.37/edc_lab_results/admin/__init__.py
--rw-r--r--   0 jw         (502) staff       (20)      162 2023-02-15 21:40:54.000000 edc-lab-results-0.1.37/edc_lab_results/admin/blood_results_modeladmin_mixin.py
--rw-r--r--   0 jw         (502) staff       (20)     1867 2023-03-23 15:10:58.000000 edc-lab-results-0.1.37/edc_lab_results/admin/reportable_results_modeladmin_mixin.py
--rw-r--r--   0 jw         (502) staff       (20)      157 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/apps.py
--rw-r--r--   0 jw         (502) staff       (20)     1002 2022-07-28 10:31:14.000000 edc-lab-results-0.1.37/edc_lab_results/calculate_missing.py
--rw-r--r--   0 jw         (502) staff       (20)      504 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/constants.py
--rw-r--r--   0 jw         (502) staff       (20)     3813 2023-03-23 15:10:58.000000 edc-lab-results-0.1.37/edc_lab_results/fieldsets.py
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-03-23 15:11:09.451719 edc-lab-results-0.1.37/edc_lab_results/form_validator_mixins/
--rw-r--r--   0 jw         (502) staff       (20)      251 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/form_validator_mixins/__init__.py
--rw-r--r--   0 jw         (502) staff       (20)      836 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/form_validator_mixins/blood_results_fbg_form_validator_mixin.py
--rw-r--r--   0 jw         (502) staff       (20)     3990 2023-03-23 15:10:58.000000 edc-lab-results-0.1.37/edc_lab_results/form_validator_mixins/blood_results_form_validator_mixin.py
--rw-r--r--   0 jw         (502) staff       (20)      437 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/form_validator_mixins/blood_results_glu_form_validator_mixin.py
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-03-23 15:11:09.456679 edc-lab-results-0.1.37/edc_lab_results/model_mixins/
--rw-r--r--   0 jw         (502) staff       (20)     1189 2022-08-15 15:50:51.000000 edc-lab-results-0.1.37/edc_lab_results/model_mixins/__init__.py
--rw-r--r--   0 jw         (502) staff       (20)     4343 2023-03-23 15:10:58.000000 edc-lab-results-0.1.37/edc_lab_results/model_mixins/blood_result_model_mixin.py
--rw-r--r--   0 jw         (502) staff       (20)      955 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/model_mixins/electrolytes_model_mixins.py
--rw-r--r--   0 jw         (502) staff       (20)     4420 2023-03-23 15:10:58.000000 edc-lab-results-0.1.37/edc_lab_results/model_mixins/fbc_model_mixins.py
--rw-r--r--   0 jw         (502) staff       (20)     1749 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/model_mixins/fbg_model_mixin.py
--rw-r--r--   0 jw         (502) staff       (20)     1748 2023-03-23 15:10:58.000000 edc-lab-results-0.1.37/edc_lab_results/model_mixins/glucose_model_mixin.py
--rw-r--r--   0 jw         (502) staff       (20)     1267 2023-03-23 15:10:58.000000 edc-lab-results-0.1.37/edc_lab_results/model_mixins/hba1c_model_mixin.py
--rw-r--r--   0 jw         (502) staff       (20)      813 2022-08-22 10:53:42.000000 edc-lab-results-0.1.37/edc_lab_results/model_mixins/insulin_model_mixin.py
--rw-r--r--   0 jw         (502) staff       (20)     3107 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/model_mixins/lft_model_mixins.py
--rw-r--r--   0 jw         (502) staff       (20)     1723 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/model_mixins/lipid_model_mixins.py
--rw-r--r--   0 jw         (502) staff       (20)      426 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/model_mixins/proteinuria_model_mixin.py
--rw-r--r--   0 jw         (502) staff       (20)     1367 2022-08-15 15:50:51.000000 edc-lab-results-0.1.37/edc_lab_results/model_mixins/rft_model_mixins.py
--rw-r--r--   0 jw         (502) staff       (20)        0 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/models.py
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-03-23 15:11:09.459875 edc-lab-results-0.1.37/edc_lab_results/tests/
--rw-r--r--   0 jw         (502) staff       (20)        0 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/tests/__init__.py
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-03-23 15:11:09.462724 edc-lab-results-0.1.37/edc_lab_results/tests/etc/
--rw-r--r--   0 jw         (502) staff       (20)      256 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/tests/etc/user-aes-local.key
--rw-r--r--   0 jw         (502) staff       (20)      256 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/tests/etc/user-aes-restricted.key
--rw-r--r--   0 jw         (502) staff       (20)     1674 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 jw         (502) staff       (20)      450 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 jw         (502) staff       (20)     1678 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 jw         (502) staff       (20)      450 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 jw         (502) staff       (20)      256 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/tests/etc/user-salt-local.key
--rw-r--r--   0 jw         (502) staff       (20)      256 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/tests/etc/user-salt-restricted.key
--rw-r--r--   0 jw         (502) staff       (20)     1367 2023-03-23 15:10:58.000000 edc-lab-results-0.1.37/edc_lab_results/tests/forms.py
--rw-r--r--   0 jw         (502) staff       (20)      508 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/tests/holidays.csv
--rw-r--r--   0 jw         (502) staff       (20)      683 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/tests/lab_profiles.py
--rw-r--r--   0 jw         (502) staff       (20)     2039 2023-03-23 15:10:58.000000 edc-lab-results-0.1.37/edc_lab_results/tests/models.py
--rw-r--r--   0 jw         (502) staff       (20)     2702 2022-09-30 09:21:07.000000 edc-lab-results-0.1.37/edc_lab_results/tests/test_case_mixin.py
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-03-23 15:11:09.463841 edc-lab-results-0.1.37/edc_lab_results/tests/tests/
--rw-r--r--   0 jw         (502) staff       (20)        0 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/tests/tests/__init__.py
--rw-r--r--   0 jw         (502) staff       (20)     4438 2023-03-23 15:08:03.000000 edc-lab-results-0.1.37/edc_lab_results/tests/tests/test_blood_result.py
--rw-r--r--   0 jw         (502) staff       (20)     7333 2022-10-05 13:22:11.000000 edc-lab-results-0.1.37/edc_lab_results/tests/tests/test_form.py
--rw-r--r--   0 jw         (502) staff       (20)      261 2022-05-07 18:35:16.000000 edc-lab-results-0.1.37/edc_lab_results/tests/urls.py
--rw-r--r--   0 jw         (502) staff       (20)     2104 2022-09-30 09:21:07.000000 edc-lab-results-0.1.37/edc_lab_results/tests/visit_schedule.py
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-03-23 15:11:09.448586 edc-lab-results-0.1.37/edc_lab_results.egg-info/
--rw-r--r--   0 jw         (502) staff       (20)     1644 2023-03-23 15:11:09.000000 edc-lab-results-0.1.37/edc_lab_results.egg-info/PKG-INFO
--rw-r--r--   0 jw         (502) staff       (20)     2473 2023-03-23 15:11:09.000000 edc-lab-results-0.1.37/edc_lab_results.egg-info/SOURCES.txt
--rw-r--r--   0 jw         (502) staff       (20)        1 2023-03-23 15:11:09.000000 edc-lab-results-0.1.37/edc_lab_results.egg-info/dependency_links.txt
--rw-r--r--   0 jw         (502) staff       (20)        1 2022-05-07 18:35:34.000000 edc-lab-results-0.1.37/edc_lab_results.egg-info/not-zip-safe
--rw-r--r--   0 jw         (502) staff       (20)       16 2023-03-23 15:11:09.000000 edc-lab-results-0.1.37/edc_lab_results.egg-info/top_level.txt
--rw-r--r--   0 jw         (502) staff       (20)     1697 2023-03-23 15:10:58.000000 edc-lab-results-0.1.37/pyproject.toml
--rw-r--r--   0 jw         (502) staff       (20)     2211 2023-03-23 15:10:58.000000 edc-lab-results-0.1.37/runtests.py
--rw-r--r--   0 jw         (502) staff       (20)     1210 2023-03-23 15:11:09.465061 edc-lab-results-0.1.37/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.393019 edc-lab-results-0.1.38/
+-rw-r--r--   0 erikvw     (501) staff       (20)       76 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.380264 edc-lab-results-0.1.38/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.384183 edc-lab-results-0.1.38/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 17:18:30.000000 edc-lab-results-0.1.38/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1842 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 17:18:30.000000 edc-lab-results-0.1.38/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-09 19:25:16.000000 edc-lab-results-0.1.38/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)      402 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-06-25 20:27:10.000000 edc-lab-results-0.1.38/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1644 2023-05-24 17:18:39.393122 edc-lab-results-0.1.38/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      733 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-09 19:25:16.000000 edc-lab-results-0.1.38/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.385881 edc-lab-results-0.1.38/edc_lab_results/
+-rw-r--r--   0 erikvw     (501) staff       (20)      276 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3809 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/edc_lab_results/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.387194 edc-lab-results-0.1.38/edc_lab_results/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      154 2022-10-26 16:30:10.000000 edc-lab-results-0.1.38/edc_lab_results/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-10-26 16:30:10.000000 edc-lab-results-0.1.38/edc_lab_results/admin/blood_results_modeladmin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1867 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/edc_lab_results/admin/reportable_results_modeladmin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1002 2022-07-27 02:24:23.000000 edc-lab-results-0.1.38/edc_lab_results/calculate_missing.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      504 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3813 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/edc_lab_results/fieldsets.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.387981 edc-lab-results-0.1.38/edc_lab_results/form_validator_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      251 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/form_validator_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      836 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/form_validator_mixins/blood_results_fbg_form_validator_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3990 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/edc_lab_results/form_validator_mixins/blood_results_form_validator_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      437 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/form_validator_mixins/blood_results_glu_form_validator_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.389873 edc-lab-results-0.1.38/edc_lab_results/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1189 2022-08-15 00:51:30.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4343 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/blood_result_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      955 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/electrolytes_model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4420 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/fbc_model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1749 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/fbg_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1748 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/glucose_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1267 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/hba1c_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1140 2023-05-24 17:18:30.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/insulin_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3107 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/lft_model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1723 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/lipid_model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      426 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/proteinuria_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1367 2022-08-15 00:51:30.000000 edc-lab-results-0.1.38/edc_lab_results/model_mixins/rft_model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.391056 edc-lab-results-0.1.38/edc_lab_results/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.392318 edc-lab-results-0.1.38/edc_lab_results/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1367 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/edc_lab_results/tests/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      508 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)      683 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/lab_profiles.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2039 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/edc_lab_results/tests/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2702 2022-09-30 01:31:16.000000 edc-lab-results-0.1.38/edc_lab_results/tests/test_case_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.392799 edc-lab-results-0.1.38/edc_lab_results/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4438 2023-03-31 15:04:16.000000 edc-lab-results-0.1.38/edc_lab_results/tests/tests/test_blood_result.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7333 2022-10-25 19:12:51.000000 edc-lab-results-0.1.38/edc_lab_results/tests/tests/test_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      261 2022-05-07 00:31:57.000000 edc-lab-results-0.1.38/edc_lab_results/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2104 2022-09-30 01:31:16.000000 edc-lab-results-0.1.38/edc_lab_results/tests/visit_schedule.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:18:39.386551 edc-lab-results-0.1.38/edc_lab_results.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1644 2023-05-24 17:18:39.000000 edc-lab-results-0.1.38/edc_lab_results.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     2465 2023-05-24 17:18:39.000000 edc-lab-results-0.1.38/edc_lab_results.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 17:18:39.000000 edc-lab-results-0.1.38/edc_lab_results.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-07 00:14:15.000000 edc-lab-results-0.1.38/edc_lab_results.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       16 2023-05-24 17:18:39.000000 edc-lab-results-0.1.38/edc_lab_results.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1776 2023-05-24 17:18:30.000000 edc-lab-results-0.1.38/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2211 2023-04-20 21:10:15.000000 edc-lab-results-0.1.38/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1210 2023-05-24 17:18:39.393426 edc-lab-results-0.1.38/setup.cfg
```

### Comparing `edc-lab-results-0.1.37/.github/workflows/build.yml` & `edc-lab-results-0.1.38/.github/workflows/build.yml`

 * *Files 12% similar despite different names*

```diff
@@ -8,16 +8,18 @@
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
         python-version: ['3.10', '3.11']
-        django-version: ['4.1', 'dev']
-
+        django-version: ['4.1', '4.2', 'dev']
+        exclude:
+          - python-version: '3.10'
+            django-version: 'dev'
     services:
       mysql:
         image: mysql:latest
         env:
           MYSQL_DATABASE: mysql
           MYSQL_ROOT_PASSWORD: mysql
         ports:
```

### Comparing `edc-lab-results-0.1.37/.gitignore` & `edc-lab-results-0.1.38/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/.pre-commit-config.yaml` & `edc-lab-results-0.1.38/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 ---
 exclude: tests/etc/user-*
+
 repos:
   - repo: https://github.com/PyCQA/bandit
     rev: 1.7.5
     hooks:
       - id: bandit
         args:
           - "-x *test*.py"
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
-        language_version: python3.9
+        language_version: python3.10
 
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         args:
           - "--config=setup.cfg"
@@ -37,12 +38,12 @@
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
       - id: detect-private-key
 
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.30.0
+    rev: v1.31.0
     hooks:
       - id: yamllint
         args:
           - "--strict"
```

### Comparing `edc-lab-results-0.1.37/LICENSE` & `edc-lab-results-0.1.38/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/PKG-INFO` & `edc-lab-results-0.1.38/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-lab-results
-Version: 0.1.37
+Version: 0.1.38
 Summary: Simple blood result data collection format model classes for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-lab-results
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django laboratory data collection,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-lab-results-0.1.37/README.rst` & `edc-lab-results-0.1.38/README.rst`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/action_items.py` & `edc-lab-results-0.1.38/edc_lab_results/action_items.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/admin/reportable_results_modeladmin_mixin.py` & `edc-lab-results-0.1.38/edc_lab_results/admin/reportable_results_modeladmin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/calculate_missing.py` & `edc-lab-results-0.1.38/edc_lab_results/calculate_missing.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/fieldsets.py` & `edc-lab-results-0.1.38/edc_lab_results/fieldsets.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/form_validator_mixins/blood_results_fbg_form_validator_mixin.py` & `edc-lab-results-0.1.38/edc_lab_results/form_validator_mixins/blood_results_fbg_form_validator_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/form_validator_mixins/blood_results_form_validator_mixin.py` & `edc-lab-results-0.1.38/edc_lab_results/form_validator_mixins/blood_results_form_validator_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/model_mixins/__init__.py` & `edc-lab-results-0.1.38/edc_lab_results/model_mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/model_mixins/blood_result_model_mixin.py` & `edc-lab-results-0.1.38/edc_lab_results/model_mixins/blood_result_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/model_mixins/electrolytes_model_mixins.py` & `edc-lab-results-0.1.38/edc_lab_results/model_mixins/electrolytes_model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/model_mixins/fbc_model_mixins.py` & `edc-lab-results-0.1.38/edc_lab_results/model_mixins/fbc_model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/model_mixins/fbg_model_mixin.py` & `edc-lab-results-0.1.38/edc_lab_results/model_mixins/fbg_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/model_mixins/glucose_model_mixin.py` & `edc-lab-results-0.1.38/edc_lab_results/model_mixins/glucose_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/model_mixins/hba1c_model_mixin.py` & `edc-lab-results-0.1.38/edc_lab_results/model_mixins/hba1c_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/model_mixins/lft_model_mixins.py` & `edc-lab-results-0.1.38/edc_lab_results/model_mixins/lft_model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/model_mixins/lipid_model_mixins.py` & `edc-lab-results-0.1.38/edc_lab_results/model_mixins/lipid_model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/model_mixins/rft_model_mixins.py` & `edc-lab-results-0.1.38/edc_lab_results/model_mixins/rft_model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/tests/etc/user-rsa-local-private.pem` & `edc-lab-results-0.1.38/edc_lab_results/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/tests/etc/user-rsa-restricted-private.pem` & `edc-lab-results-0.1.38/edc_lab_results/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/tests/forms.py` & `edc-lab-results-0.1.38/edc_lab_results/tests/forms.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/tests/lab_profiles.py` & `edc-lab-results-0.1.38/edc_lab_results/tests/lab_profiles.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/tests/models.py` & `edc-lab-results-0.1.38/edc_lab_results/tests/models.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/tests/test_case_mixin.py` & `edc-lab-results-0.1.38/edc_lab_results/tests/test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/tests/tests/test_blood_result.py` & `edc-lab-results-0.1.38/edc_lab_results/tests/tests/test_blood_result.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/tests/tests/test_form.py` & `edc-lab-results-0.1.38/edc_lab_results/tests/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results/tests/visit_schedule.py` & `edc-lab-results-0.1.38/edc_lab_results/tests/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/edc_lab_results.egg-info/PKG-INFO` & `edc-lab-results-0.1.38/edc_lab_results.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-lab-results
-Version: 0.1.37
+Version: 0.1.38
 Summary: Simple blood result data collection format model classes for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-lab-results
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django laboratory data collection,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-lab-results-0.1.37/edc_lab_results.egg-info/SOURCES.txt` & `edc-lab-results-0.1.38/edc_lab_results.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

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
 edc_lab_results/__init__.py
 edc_lab_results/action_items.py
```

### Comparing `edc-lab-results-0.1.37/pyproject.toml` & `edc-lab-results-0.1.38/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 [tool.isort]
 profile = "black"
 py_version = "310"
 skip = [".tox", ".eggs", "migrations"]
 
 [tool.coverage.run]
-parallel = true
+parallel = false
 branch = true
 source = ["edc_lab_results"]
 
 [tool.coverage.paths]
 source = ["edc_lab_results"]
 
 [tool.coverage.report]
@@ -32,40 +32,43 @@
   "if TYPE_CHECKING:",
 ]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{310,311}-dj{41,dev},
+    py{310}-dj{41,42},
+    py{311}-dj{41,42,dev},
     lint
 
 isolated_build = true
 
 [gh-actions]
 python =
     3.10: py310
     3.11: py311, lint
 
 [gh-actions:env]
 DJANGO =
-    4.1: dj41, lint
+    4.1: dj41
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

### Comparing `edc-lab-results-0.1.37/runtests.py` & `edc-lab-results-0.1.38/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.37/setup.cfg` & `edc-lab-results-0.1.38/setup.cfg`

 * *Files identical despite different names*

