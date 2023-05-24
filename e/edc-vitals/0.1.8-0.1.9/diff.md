# Comparing `tmp/edc-vitals-0.1.8.tar.gz` & `tmp/edc-vitals-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-vitals-0.1.8.tar", last modified: Thu Sep  8 11:55:15 2022, max compression
+gzip compressed data, was "edc-vitals-0.1.9.tar", last modified: Thu Sep 15 02:32:34 2022, max compression
```

## Comparing `edc-vitals-0.1.8.tar` & `edc-vitals-0.1.9.tar`

### file list

```diff
@@ -1,66 +1,68 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:55:15.409789 edc-vitals-0.1.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       90 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:55:15.400415 edc-vitals-0.1.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:55:15.403604 edc-vitals-0.1.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1759 2022-07-08 06:42:19.000000 edc-vitals-0.1.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1832 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)       37 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-08-06 11:19:19.000000 edc-vitals-0.1.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1779 2022-09-08 11:55:15.409910 edc-vitals-0.1.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      927 2022-07-08 06:42:19.000000 edc-vitals-0.1.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-08 11:55:07.000000 edc-vitals-0.1.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:55:15.404557 edc-vitals-0.1.8/edc_vitals/
--rw-r--r--   0 erikvw     (501) staff       (20)      117 2022-07-08 06:42:19.000000 edc-vitals-0.1.8/edc_vitals/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      145 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/apps.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:55:15.405636 edc-vitals-0.1.8/edc_vitals/form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)      167 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1563 2022-07-08 06:42:19.000000 edc-vitals-0.1.8/edc_vitals/form_validators/blood_pressure_form_validator_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      460 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/form_validators/weight_height_bmi_form_validator_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:55:15.405893 edc-vitals-0.1.8/edc_vitals/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:55:15.406266 edc-vitals-0.1.8/edc_vitals/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2053 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/model_mixins/blood_pressure_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1103 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/model_mixins/weight_height_bmi_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:55:15.406402 edc-vitals-0.1.8/edc_vitals/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      142 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/models/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:55:15.407549 edc-vitals-0.1.8/edc_vitals/models/fields/
--rw-r--r--   0 erikvw     (501) staff       (20)      237 2022-07-08 06:42:19.000000 edc-vitals-0.1.8/edc_vitals/models/fields/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1371 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/models/fields/blood_pressure.py
--rw-r--r--   0 erikvw     (501) staff       (20)      936 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/models/fields/height.py
--rw-r--r--   0 erikvw     (501) staff       (20)      962 2022-07-08 06:42:19.000000 edc-vitals-0.1.8/edc_vitals/models/fields/temperature.py
--rw-r--r--   0 erikvw     (501) staff       (20)      831 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/models/fields/waist_circumference.py
--rw-r--r--   0 erikvw     (501) staff       (20)      922 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/models/fields/weight.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:55:15.407920 edc-vitals-0.1.8/edc_vitals/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-07-08 06:42:19.000000 edc-vitals-0.1.8/edc_vitals/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:55:15.409057 edc-vitals-0.1.8/edc_vitals/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      692 2022-07-08 06:42:19.000000 edc-vitals-0.1.8/edc_vitals/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:55:15.409628 edc-vitals-0.1.8/edc_vitals/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7591 2022-07-08 06:42:19.000000 edc-vitals-0.1.8/edc_vitals/tests/tests/test_blood_pressure.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3518 2022-09-08 11:55:07.000000 edc-vitals-0.1.8/edc_vitals/tests/tests/test_temperature.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2245 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/tests/tests/test_weight_height_bmi.py
--rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1384 2022-07-08 06:42:19.000000 edc-vitals-0.1.8/edc_vitals/utils.py
--rw-r--r--   0 erikvw     (501) staff       (20)      164 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/edc_vitals/validators.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:55:15.405200 edc-vitals-0.1.8/edc_vitals.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1779 2022-09-08 11:55:15.000000 edc-vitals-0.1.8/edc_vitals.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1673 2022-09-08 11:55:15.000000 edc-vitals-0.1.8/edc_vitals.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-08 11:55:15.000000 edc-vitals-0.1.8/edc_vitals.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-08-06 11:25:40.000000 edc-vitals-0.1.8/edc_vitals.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-09-08 11:55:15.000000 edc-vitals-0.1.8/edc_vitals.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1640 2022-07-08 06:42:19.000000 edc-vitals-0.1.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1291 2022-05-25 15:52:36.000000 edc-vitals-0.1.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1145 2022-09-08 11:55:15.410264 edc-vitals-0.1.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:32:34.455860 edc-vitals-0.1.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       90 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:32:34.446899 edc-vitals-0.1.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:32:34.449991 edc-vitals-0.1.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1660 2022-09-15 02:32:26.000000 edc-vitals-0.1.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1832 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-09-15 02:32:26.000000 edc-vitals-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-09-15 02:32:26.000000 edc-vitals-0.1.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)       37 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-08-06 11:19:19.000000 edc-vitals-0.1.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1908 2022-09-15 02:32:34.455959 edc-vitals-0.1.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      927 2022-07-08 06:42:19.000000 edc-vitals-0.1.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-15 02:32:26.000000 edc-vitals-0.1.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-09-15 02:32:26.000000 edc-vitals-0.1.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:32:34.450768 edc-vitals-0.1.9/edc_vitals/
+-rw-r--r--   0 erikvw     (501) staff       (20)      117 2022-07-08 06:42:19.000000 edc-vitals-0.1.9/edc_vitals/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      145 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/apps.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:32:34.452041 edc-vitals-0.1.9/edc_vitals/form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)      167 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1563 2022-07-08 06:42:19.000000 edc-vitals-0.1.9/edc_vitals/form_validators/blood_pressure_form_validator_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      460 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/form_validators/weight_height_bmi_form_validator_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:32:34.452294 edc-vitals-0.1.9/edc_vitals/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:32:34.452748 edc-vitals-0.1.9/edc_vitals/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2053 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/model_mixins/blood_pressure_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1103 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/model_mixins/weight_height_bmi_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:32:34.452890 edc-vitals-0.1.9/edc_vitals/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      142 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/models/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:32:34.453804 edc-vitals-0.1.9/edc_vitals/models/fields/
+-rw-r--r--   0 erikvw     (501) staff       (20)      237 2022-07-08 06:42:19.000000 edc-vitals-0.1.9/edc_vitals/models/fields/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1371 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/models/fields/blood_pressure.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      936 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/models/fields/height.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      962 2022-07-08 06:42:19.000000 edc-vitals-0.1.9/edc_vitals/models/fields/temperature.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      831 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/models/fields/waist_circumference.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      922 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/models/fields/weight.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:32:34.454132 edc-vitals-0.1.9/edc_vitals/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-07-08 06:42:19.000000 edc-vitals-0.1.9/edc_vitals/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:32:34.455181 edc-vitals-0.1.9/edc_vitals/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      692 2022-07-08 06:42:19.000000 edc-vitals-0.1.9/edc_vitals/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:32:34.455749 edc-vitals-0.1.9/edc_vitals/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7591 2022-07-08 06:42:19.000000 edc-vitals-0.1.9/edc_vitals/tests/tests/test_blood_pressure.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3518 2022-09-08 11:55:07.000000 edc-vitals-0.1.9/edc_vitals/tests/tests/test_temperature.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2322 2022-09-15 02:32:26.000000 edc-vitals-0.1.9/edc_vitals/tests/tests/test_weight_height_bmi.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1384 2022-07-08 06:42:19.000000 edc-vitals-0.1.9/edc_vitals/utils.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      164 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/edc_vitals/validators.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-15 02:32:34.451537 edc-vitals-0.1.9/edc_vitals.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1908 2022-09-15 02:32:34.000000 edc-vitals-0.1.9/edc_vitals.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1707 2022-09-15 02:32:34.000000 edc-vitals-0.1.9/edc_vitals.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-15 02:32:34.000000 edc-vitals-0.1.9/edc_vitals.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-08-06 11:25:40.000000 edc-vitals-0.1.9/edc_vitals.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-09-15 02:32:34.000000 edc-vitals-0.1.9/edc_vitals.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1722 2022-09-15 02:32:26.000000 edc-vitals-0.1.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1291 2022-05-25 15:52:36.000000 edc-vitals-0.1.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1243 2022-09-15 02:32:34.456281 edc-vitals-0.1.9/setup.cfg
```

### Comparing `edc-vitals-0.1.8/.gitignore` & `edc-vitals-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-vitals-0.1.8/LICENSE` & `edc-vitals-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-vitals-0.1.8/PKG-INFO` & `edc-vitals-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: edc-vitals
-Version: 0.1.8
+Version: 0.1.9
 Summary: Classes for BP, weight, etc for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-vitals
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc vitals,clinicedc,clinical trials
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
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
```

### Comparing `edc-vitals-0.1.8/README.rst` & `edc-vitals-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-vitals-0.1.8/edc_vitals/form_validators/blood_pressure_form_validator_mixin.py` & `edc-vitals-0.1.9/edc_vitals/form_validators/blood_pressure_form_validator_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-vitals-0.1.8/edc_vitals/model_mixins/blood_pressure_model_mixin.py` & `edc-vitals-0.1.9/edc_vitals/model_mixins/blood_pressure_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-vitals-0.1.8/edc_vitals/model_mixins/weight_height_bmi_model_mixin.py` & `edc-vitals-0.1.9/edc_vitals/model_mixins/weight_height_bmi_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-vitals-0.1.8/edc_vitals/models/fields/blood_pressure.py` & `edc-vitals-0.1.9/edc_vitals/models/fields/blood_pressure.py`

 * *Files identical despite different names*

### Comparing `edc-vitals-0.1.8/edc_vitals/models/fields/height.py` & `edc-vitals-0.1.9/edc_vitals/models/fields/height.py`

 * *Files identical despite different names*

### Comparing `edc-vitals-0.1.8/edc_vitals/models/fields/temperature.py` & `edc-vitals-0.1.9/edc_vitals/models/fields/temperature.py`

 * *Files identical despite different names*

### Comparing `edc-vitals-0.1.8/edc_vitals/models/fields/waist_circumference.py` & `edc-vitals-0.1.9/edc_vitals/models/fields/waist_circumference.py`

 * *Files identical despite different names*

### Comparing `edc-vitals-0.1.8/edc_vitals/models/fields/weight.py` & `edc-vitals-0.1.9/edc_vitals/models/fields/weight.py`

 * *Files identical despite different names*

### Comparing `edc-vitals-0.1.8/edc_vitals/tests/etc/user-rsa-local-private.pem` & `edc-vitals-0.1.9/edc_vitals/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-vitals-0.1.8/edc_vitals/tests/etc/user-rsa-restricted-private.pem` & `edc-vitals-0.1.9/edc_vitals/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-vitals-0.1.8/edc_vitals/tests/models.py` & `edc-vitals-0.1.9/edc_vitals/tests/models.py`

 * *Files identical despite different names*

### Comparing `edc-vitals-0.1.8/edc_vitals/tests/tests/test_blood_pressure.py` & `edc-vitals-0.1.9/edc_vitals/tests/tests/test_blood_pressure.py`

 * *Files identical despite different names*

### Comparing `edc-vitals-0.1.8/edc_vitals/tests/tests/test_temperature.py` & `edc-vitals-0.1.9/edc_vitals/tests/tests/test_temperature.py`

 * *Files identical despite different names*

### Comparing `edc-vitals-0.1.8/edc_vitals/tests/tests/test_weight_height_bmi.py` & `edc-vitals-0.1.9/edc_vitals/tests/tests/test_weight_height_bmi.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from decimal import Decimal
 
 from dateutil.relativedelta import relativedelta
 from django import forms
 from django.test import TestCase
 from edc_utils import get_utcnow
+from edc_utils.round_up import round_half_away_from_zero
 
 from edc_vitals.form_validators import WeightHeightBmiFormValidatorMixin
 
 from ..models import WeightHeightBmi
 
 
 class TestWeightHeightBmi(TestCase):
@@ -24,15 +25,15 @@
     def test_calculates_bmi(self):
         obj = WeightHeightBmi(
             weight=Decimal("65.0"),
             height=Decimal("180.0"),
             dob=get_utcnow() - relativedelta(years=25),
         )
         obj.save()
-        self.assertEqual(round(obj.calculated_bmi_value, 4), 20.0617)
+        self.assertEqual(round_half_away_from_zero(obj.calculated_bmi_value, 4), 20.0617)
 
     def test_form_validator(self):
         form_validator = WeightHeightBmiFormValidatorMixin()
         form_validator.validate_weight_height_with_bmi()
         cleaned_data = dict(weight=65, height=180)
         form_validator.validate_weight_height_with_bmi(
             weight_kg=cleaned_data.get("weight"),
```

### Comparing `edc-vitals-0.1.8/edc_vitals/utils.py` & `edc-vitals-0.1.9/edc_vitals/utils.py`

 * *Files identical despite different names*

### Comparing `edc-vitals-0.1.8/edc_vitals.egg-info/PKG-INFO` & `edc-vitals-0.1.9/edc_vitals.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: edc-vitals
-Version: 0.1.8
+Version: 0.1.9
 Summary: Classes for BP, weight, etc for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-vitals
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc vitals,clinicedc,clinical trials
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
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
```

### Comparing `edc-vitals-0.1.8/edc_vitals.egg-info/SOURCES.txt` & `edc-vitals-0.1.9/edc_vitals.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

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

### Comparing `edc-vitals-0.1.8/pyproject.toml` & `edc-vitals-0.1.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -28,36 +28,41 @@
 skip_covered = true
 omit = ["requirements.txt"]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{39}-dj{32,40,dev},
+    py{38,39,310}-dj{32,40,41,dev},
     lint
+
 isolated_build = true
 
 [gh-actions]
 python =
+    3.8: py38
     3.9: py39, lint
+    3.10: py310
 
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
     pip freeze
     coverage run -a runtests.py
```

### Comparing `edc-vitals-0.1.8/runtests.py` & `edc-vitals-0.1.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-vitals-0.1.8/setup.cfg` & `edc-vitals-0.1.9/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -9,19 +9,22 @@
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = django edc vitals, clinicedc, clinical trials
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
 python_requires = >=3.9
 zip_safe = False
 include_package_data = True
 packages = find:
@@ -34,14 +37,14 @@
 	bin*
 	edc_vitals.tests*
 
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

