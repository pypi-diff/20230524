# Comparing `tmp/edc-rx-0.1.5.tar.gz` & `tmp/edc-rx-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-rx-0.1.5.tar", last modified: Tue Apr 25 02:49:30 2023, max compression
+gzip compressed data, was "edc-rx-0.1.6.tar", last modified: Wed May 24 15:54:51 2023, max compression
```

## Comparing `edc-rx-0.1.5.tar` & `edc-rx-0.1.6.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.440753 edc-rx-0.1.5/
--rw-r--r--   0 erikvw     (501) staff       (20)       78 2022-11-29 04:55:26.000000 edc-rx-0.1.5/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-29 04:55:26.000000 edc-rx-0.1.5/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.432135 edc-rx-0.1.5/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.435691 edc-rx-0.1.5/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1645 2023-04-18 01:41:25.000000 edc-rx-0.1.5/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-11-29 04:55:26.000000 edc-rx-0.1.5/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-04-18 01:41:25.000000 edc-rx-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-29 04:55:26.000000 edc-rx-0.1.5/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.5/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.5/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-29 03:26:32.000000 edc-rx-0.1.5/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-11-29 04:55:26.000000 edc-rx-0.1.5/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1461 2023-04-25 02:49:30.440841 edc-rx-0.1.5/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      613 2022-11-29 04:55:26.000000 edc-rx-0.1.5/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.436755 edc-rx-0.1.5/edc_rx/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      270 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/apps.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.437730 edc-rx-0.1.5/edc_rx/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     5179 2023-04-18 01:41:25.000000 edc-rx-0.1.5/edc_rx/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 06:36:26.000000 edc-rx-0.1.5/edc_rx/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.438404 edc-rx-0.1.5/edc_rx/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      181 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1698 2023-04-25 02:49:23.000000 edc-rx-0.1.5/edc_rx/model_mixins/drug_refill_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      865 2023-04-18 01:41:25.000000 edc-rx-0.1.5/edc_rx/model_mixins/drug_supply_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1249 2023-04-18 01:41:25.000000 edc-rx-0.1.5/edc_rx/model_mixins/treatment_pay_methods.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.438902 edc-rx-0.1.5/edc_rx/modeladmin_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/modeladmin_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1158 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      730 2023-04-18 01:41:25.000000 edc-rx-0.1.5/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.439189 edc-rx-0.1.5/edc_rx/modelform_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)       73 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/modelform_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2075 2023-04-25 02:49:23.000000 edc-rx-0.1.5/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      440 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.439305 edc-rx-0.1.5/edc_rx/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.5/edc_rx/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.440416 edc-rx-0.1.5/edc_rx/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/tests/etc/user-salt-restricted.key
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.440654 edc-rx-0.1.5/edc_rx/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.5/edc_rx/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4232 2023-04-25 02:49:23.000000 edc-rx-0.1.5/edc_rx/tests/tests/test_utils.py
--rw-r--r--   0 erikvw     (501) staff       (20)      277 2022-11-29 04:55:26.000000 edc-rx-0.1.5/edc_rx/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      799 2023-04-25 02:49:23.000000 edc-rx-0.1.5/edc_rx/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-04-25 02:49:30.437414 edc-rx-0.1.5/edc_rx.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1461 2023-04-25 02:49:30.000000 edc-rx-0.1.5/edc_rx.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1335 2023-04-25 02:49:30.000000 edc-rx-0.1.5/edc_rx.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-04-25 02:49:30.000000 edc-rx-0.1.5/edc_rx.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-29 04:55:34.000000 edc-rx-0.1.5/edc_rx.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)        7 2023-04-25 02:49:30.000000 edc-rx-0.1.5/edc_rx.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1679 2023-04-18 01:41:25.000000 edc-rx-0.1.5/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1106 2023-03-31 01:08:39.000000 edc-rx-0.1.5/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1140 2023-04-25 02:49:30.441177 edc-rx-0.1.5/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.878319 edc-rx-0.1.6/
+-rw-r--r--   0 erikvw     (501) staff       (20)       78 2022-11-29 04:55:26.000000 edc-rx-0.1.6/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-29 04:55:26.000000 edc-rx-0.1.6/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.870007 edc-rx-0.1.6/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.873159 edc-rx-0.1.6/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 15:54:44.000000 edc-rx-0.1.6/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-11-29 04:55:26.000000 edc-rx-0.1.6/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1173 2023-05-24 15:54:44.000000 edc-rx-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-29 04:55:26.000000 edc-rx-0.1.6/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.6/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.6/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-29 03:26:32.000000 edc-rx-0.1.6/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-11-29 04:55:26.000000 edc-rx-0.1.6/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1487 2023-05-24 15:54:51.878397 edc-rx-0.1.6/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      613 2022-11-29 04:55:26.000000 edc-rx-0.1.6/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.874005 edc-rx-0.1.6/edc_rx/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      270 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/apps.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.875227 edc-rx-0.1.6/edc_rx/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)     5179 2023-04-18 01:41:25.000000 edc-rx-0.1.6/edc_rx/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 06:36:26.000000 edc-rx-0.1.6/edc_rx/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.875883 edc-rx-0.1.6/edc_rx/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      181 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1698 2023-04-25 02:49:23.000000 edc-rx-0.1.6/edc_rx/model_mixins/drug_refill_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      865 2023-04-18 01:41:25.000000 edc-rx-0.1.6/edc_rx/model_mixins/drug_supply_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1249 2023-04-18 01:41:25.000000 edc-rx-0.1.6/edc_rx/model_mixins/treatment_pay_methods.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.876366 edc-rx-0.1.6/edc_rx/modeladmin_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/modeladmin_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1158 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      730 2023-04-18 01:41:25.000000 edc-rx-0.1.6/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.876637 edc-rx-0.1.6/edc_rx/modelform_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)       73 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/modelform_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2075 2023-04-25 02:49:23.000000 edc-rx-0.1.6/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      440 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.876866 edc-rx-0.1.6/edc_rx/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.6/edc_rx/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.877915 edc-rx-0.1.6/edc_rx/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/tests/etc/user-salt-restricted.key
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.878136 edc-rx-0.1.6/edc_rx/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.6/edc_rx/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4232 2023-04-25 02:49:23.000000 edc-rx-0.1.6/edc_rx/tests/tests/test_utils.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      277 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      799 2023-04-25 02:49:23.000000 edc-rx-0.1.6/edc_rx/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.874858 edc-rx-0.1.6/edc_rx.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1487 2023-05-24 15:54:51.000000 edc-rx-0.1.6/edc_rx.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1335 2023-05-24 15:54:51.000000 edc-rx-0.1.6/edc_rx.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 15:54:51.000000 edc-rx-0.1.6/edc_rx.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-29 04:55:34.000000 edc-rx-0.1.6/edc_rx.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)        7 2023-05-24 15:54:51.000000 edc-rx-0.1.6/edc_rx.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1758 2023-05-24 15:54:44.000000 edc-rx-0.1.6/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1106 2023-03-31 01:08:39.000000 edc-rx-0.1.6/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1166 2023-05-24 15:54:51.878695 edc-rx-0.1.6/setup.cfg
```

### Comparing `edc-rx-0.1.5/.github/workflows/build.yml` & `edc-rx-0.1.6/.github/workflows/build.yml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,27 @@
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
         python-version: ['3.10', '3.11']
-        django-version: ['4.1', 'dev']
+        django-version: ['4.1', '4.2', 'dev']
+        exclude:
+          - python-version: '3.10'
+            django-version: 'dev'
+    services:
+      mysql:
+        image: mysql:latest
+        env:
+          MYSQL_DATABASE: mysql
+          MYSQL_ROOT_PASSWORD: mysql
+        ports:
+          - 3306:3306
+        options: --health-cmd="mysqladmin ping" --health-interval=10s --health-timeout=5s --health-retries=3
 
     steps:
       - name: Install pycups and words dependency
         run: |
           sudo sed -i 's/azure\.//' /etc/apt/sources.list
           sudo apt-get -y update
           sudo apt-get install libcups2-dev wamerican
```

### Comparing `edc-rx-0.1.5/.gitignore` & `edc-rx-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.5/.pre-commit-config.yaml` & `edc-rx-0.1.6/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         args:
           - "-x *test*.py"
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
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
@@ -37,13 +37,18 @@
       - id: fix-byte-order-marker
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
       - id: detect-private-key
 
+  - repo: https://github.com/rstcheck/rstcheck
+    rev: v6.1.2
+    hooks:
+      - id: rstcheck
+
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.30.0
+    rev: v1.31.0
     hooks:
       - id: yamllint
         args:
           - "--strict"
```

### Comparing `edc-rx-0.1.5/LICENSE` & `edc-rx-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.5/PKG-INFO` & `edc-rx-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: edc-rx
-Version: 0.1.5
-Summary: Microcopy model mixins in clinicedc/edc projects
+Version: 0.1.6
+Summary: Medications refill and supply model/form mixins for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-rx
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc rx-refill,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `edc-rx-0.1.5/README.rst` & `edc-rx-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.5/edc_rx/migrations/0001_initial.py` & `edc-rx-0.1.6/edc_rx/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.5/edc_rx/model_mixins/drug_refill_model_mixin.py` & `edc-rx-0.1.6/edc_rx/model_mixins/drug_refill_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.5/edc_rx/model_mixins/drug_supply_model_mixin.py` & `edc-rx-0.1.6/edc_rx/model_mixins/drug_supply_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.5/edc_rx/model_mixins/treatment_pay_methods.py` & `edc-rx-0.1.6/edc_rx/model_mixins/treatment_pay_methods.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.5/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py` & `edc-rx-0.1.6/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.5/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py` & `edc-rx-0.1.6/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.5/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py` & `edc-rx-0.1.6/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.5/edc_rx/tests/etc/user-rsa-local-private.pem` & `edc-rx-0.1.6/edc_rx/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.5/edc_rx/tests/etc/user-rsa-restricted-private.pem` & `edc-rx-0.1.6/edc_rx/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.5/edc_rx/tests/tests/test_utils.py` & `edc-rx-0.1.6/edc_rx/tests/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.5/edc_rx/utils.py` & `edc-rx-0.1.6/edc_rx/utils.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.5/edc_rx.egg-info/PKG-INFO` & `edc-rx-0.1.6/edc_rx.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: edc-rx
-Version: 0.1.5
-Summary: Microcopy model mixins in clinicedc/edc projects
+Version: 0.1.6
+Summary: Medications refill and supply model/form mixins for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-rx
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc rx-refill,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `edc-rx-0.1.5/edc_rx.egg-info/SOURCES.txt` & `edc-rx-0.1.6/edc_rx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.5/pyproject.toml` & `edc-rx-0.1.6/pyproject.toml`

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
 source = ["edc_rx"]
 
 [tool.coverage.paths]
 source = ["edc_rx"]
 
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

### Comparing `edc-rx-0.1.5/runtests.py` & `edc-rx-0.1.6/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.5/setup.cfg` & `edc-rx-0.1.6/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = edc-rx
 version = attr: _version
 author = Erik van Widenfelt
 author_email = ew2789@gmail.com
 url = https://github.com/clinicedc/edc-rx
 license = GPL license, see LICENSE
-description = Microcopy model mixins in clinicedc/edc projects
+description = Medications refill and supply model/form mixins for clinicedc/edc projects
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = django Edc rx-refill, CRF, clinicedc, clinical trials
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 4.1
```

