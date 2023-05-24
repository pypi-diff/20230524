# Comparing `tmp/edc-fieldsets-0.3.8.tar.gz` & `tmp/edc-fieldsets-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-fieldsets-0.3.8.tar", last modified: Fri Aug 12 01:22:57 2022, max compression
+gzip compressed data, was "edc-fieldsets-0.3.9.tar", last modified: Mon Aug 22 00:41:21 2022, max compression
```

## Comparing `edc-fieldsets-0.3.8.tar` & `edc-fieldsets-0.3.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 01:22:57.387305 edc-fieldsets-0.3.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       73 2020-03-04 23:28:40.000000 edc-fieldsets-0.3.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-09 00:16:25.000000 edc-fieldsets-0.3.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 01:22:57.378647 edc-fieldsets-0.3.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 01:22:57.381473 edc-fieldsets-0.3.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1934 2022-08-11 23:43:53.000000 edc-fieldsets-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1131 2022-08-11 23:46:56.000000 edc-fieldsets-0.3.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-11 23:43:53.000000 edc-fieldsets-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-11 23:43:53.000000 edc-fieldsets-0.3.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-11 23:50:14.000000 edc-fieldsets-0.3.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-11 23:50:14.000000 edc-fieldsets-0.3.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-04 23:28:40.000000 edc-fieldsets-0.3.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       51 2020-03-04 23:28:40.000000 edc-fieldsets-0.3.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     2792 2022-08-12 01:22:57.387412 edc-fieldsets-0.3.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1811 2021-04-23 00:18:31.000000 edc-fieldsets-0.3.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-12 01:22:49.000000 edc-fieldsets-0.3.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-11 23:43:53.000000 edc-fieldsets-0.3.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 01:22:57.382710 edc-fieldsets-0.3.8/edc_fieldsets/
--rw-r--r--   0 erikvw     (501) staff       (20)      193 2021-02-09 00:16:25.000000 edc-fieldsets-0.3.8/edc_fieldsets/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      116 2020-03-04 23:28:40.000000 edc-fieldsets-0.3.8/edc_fieldsets/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      622 2021-02-09 00:16:25.000000 edc-fieldsets-0.3.8/edc_fieldsets/fieldlist.py
--rw-r--r--   0 erikvw     (501) staff       (20)      161 2021-02-09 00:16:25.000000 edc-fieldsets-0.3.8/edc_fieldsets/fieldset.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2922 2021-02-09 00:16:25.000000 edc-fieldsets-0.3.8/edc_fieldsets/fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2708 2022-08-11 23:43:53.000000 edc-fieldsets-0.3.8/edc_fieldsets/fieldsets_modeladmin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)       32 2022-08-11 23:43:53.000000 edc-fieldsets-0.3.8/edc_fieldsets/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 01:22:57.385421 edc-fieldsets-0.3.8/edc_fieldsets/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:28:40.000000 edc-fieldsets-0.3.8/edc_fieldsets/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1604 2020-03-09 16:50:32.000000 edc-fieldsets-0.3.8/edc_fieldsets/tests/admin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 01:22:57.386656 edc-fieldsets-0.3.8/edc_fieldsets/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-09 16:50:32.000000 edc-fieldsets-0.3.8/edc_fieldsets/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-09 16:50:32.000000 edc-fieldsets-0.3.8/edc_fieldsets/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-09 16:50:32.000000 edc-fieldsets-0.3.8/edc_fieldsets/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-09 16:50:32.000000 edc-fieldsets-0.3.8/edc_fieldsets/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2020-03-09 16:50:32.000000 edc-fieldsets-0.3.8/edc_fieldsets/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-09 16:50:32.000000 edc-fieldsets-0.3.8/edc_fieldsets/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-09 16:50:32.000000 edc-fieldsets-0.3.8/edc_fieldsets/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-09 16:50:32.000000 edc-fieldsets-0.3.8/edc_fieldsets/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      154 2020-03-04 23:28:40.000000 edc-fieldsets-0.3.8/edc_fieldsets/tests/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1408 2021-02-09 00:16:25.000000 edc-fieldsets-0.3.8/edc_fieldsets/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 01:22:57.387076 edc-fieldsets-0.3.8/edc_fieldsets/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 00:16:25.000000 edc-fieldsets-0.3.8/edc_fieldsets/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5975 2022-08-11 23:43:53.000000 edc-fieldsets-0.3.8/edc_fieldsets/tests/tests/test_fieldset_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5180 2022-08-11 23:43:53.000000 edc-fieldsets-0.3.8/edc_fieldsets/tests/tests/test_fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1323 2021-02-09 00:16:25.000000 edc-fieldsets-0.3.8/edc_fieldsets/tests/visit_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)      748 2020-03-04 23:28:40.000000 edc-fieldsets-0.3.8/edc_fieldsets/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 01:22:57.383450 edc-fieldsets-0.3.8/edc_fieldsets.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     2792 2022-08-12 01:22:57.000000 edc-fieldsets-0.3.8/edc_fieldsets.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1325 2022-08-12 01:22:57.000000 edc-fieldsets-0.3.8/edc_fieldsets.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-12 01:22:57.000000 edc-fieldsets-0.3.8/edc_fieldsets.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:28:40.000000 edc-fieldsets-0.3.8/edc_fieldsets.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-12 01:22:57.000000 edc-fieldsets-0.3.8/edc_fieldsets.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-12 01:22:57.000000 edc-fieldsets-0.3.8/edc_fieldsets.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1728 2022-08-11 23:43:53.000000 edc-fieldsets-0.3.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2115 2022-08-12 01:22:49.000000 edc-fieldsets-0.3.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1272 2022-08-12 01:22:57.387733 edc-fieldsets-0.3.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-22 00:41:21.989683 edc-fieldsets-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       73 2020-03-04 23:28:40.000000 edc-fieldsets-0.3.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-09 00:16:25.000000 edc-fieldsets-0.3.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-22 00:41:21.981872 edc-fieldsets-0.3.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-22 00:41:21.985051 edc-fieldsets-0.3.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1934 2022-08-11 23:43:53.000000 edc-fieldsets-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1131 2022-08-11 23:46:56.000000 edc-fieldsets-0.3.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-11 23:43:53.000000 edc-fieldsets-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-11 23:43:53.000000 edc-fieldsets-0.3.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-11 23:50:14.000000 edc-fieldsets-0.3.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-11 23:50:14.000000 edc-fieldsets-0.3.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-04 23:28:40.000000 edc-fieldsets-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       51 2020-03-04 23:28:40.000000 edc-fieldsets-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     2792 2022-08-22 00:41:21.989781 edc-fieldsets-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1811 2021-04-23 00:18:31.000000 edc-fieldsets-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-22 00:41:14.000000 edc-fieldsets-0.3.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-11 23:43:53.000000 edc-fieldsets-0.3.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-22 00:41:21.986407 edc-fieldsets-0.3.9/edc_fieldsets/
+-rw-r--r--   0 erikvw     (501) staff       (20)      193 2021-02-09 00:16:25.000000 edc-fieldsets-0.3.9/edc_fieldsets/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      116 2020-03-04 23:28:40.000000 edc-fieldsets-0.3.9/edc_fieldsets/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      622 2021-02-09 00:16:25.000000 edc-fieldsets-0.3.9/edc_fieldsets/fieldlist.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      161 2021-02-09 00:16:25.000000 edc-fieldsets-0.3.9/edc_fieldsets/fieldset.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2922 2021-02-09 00:16:25.000000 edc-fieldsets-0.3.9/edc_fieldsets/fieldsets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2708 2022-08-11 23:43:53.000000 edc-fieldsets-0.3.9/edc_fieldsets/fieldsets_modeladmin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       32 2022-08-11 23:43:53.000000 edc-fieldsets-0.3.9/edc_fieldsets/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-22 00:41:21.987897 edc-fieldsets-0.3.9/edc_fieldsets/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:28:40.000000 edc-fieldsets-0.3.9/edc_fieldsets/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1583 2022-08-22 00:41:14.000000 edc-fieldsets-0.3.9/edc_fieldsets/tests/admin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-22 00:41:21.989075 edc-fieldsets-0.3.9/edc_fieldsets/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-09 16:50:32.000000 edc-fieldsets-0.3.9/edc_fieldsets/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-09 16:50:32.000000 edc-fieldsets-0.3.9/edc_fieldsets/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-09 16:50:32.000000 edc-fieldsets-0.3.9/edc_fieldsets/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-09 16:50:32.000000 edc-fieldsets-0.3.9/edc_fieldsets/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2020-03-09 16:50:32.000000 edc-fieldsets-0.3.9/edc_fieldsets/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-09 16:50:32.000000 edc-fieldsets-0.3.9/edc_fieldsets/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-09 16:50:32.000000 edc-fieldsets-0.3.9/edc_fieldsets/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-09 16:50:32.000000 edc-fieldsets-0.3.9/edc_fieldsets/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      154 2020-03-04 23:28:40.000000 edc-fieldsets-0.3.9/edc_fieldsets/tests/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1408 2021-02-09 00:16:25.000000 edc-fieldsets-0.3.9/edc_fieldsets/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-22 00:41:21.989450 edc-fieldsets-0.3.9/edc_fieldsets/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 00:16:25.000000 edc-fieldsets-0.3.9/edc_fieldsets/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5975 2022-08-11 23:43:53.000000 edc-fieldsets-0.3.9/edc_fieldsets/tests/tests/test_fieldset_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5180 2022-08-11 23:43:53.000000 edc-fieldsets-0.3.9/edc_fieldsets/tests/tests/test_fieldsets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1323 2021-02-09 00:16:25.000000 edc-fieldsets-0.3.9/edc_fieldsets/tests/visit_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      748 2020-03-04 23:28:40.000000 edc-fieldsets-0.3.9/edc_fieldsets/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-22 00:41:21.987182 edc-fieldsets-0.3.9/edc_fieldsets.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2792 2022-08-22 00:41:21.000000 edc-fieldsets-0.3.9/edc_fieldsets.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1325 2022-08-22 00:41:21.000000 edc-fieldsets-0.3.9/edc_fieldsets.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-22 00:41:21.000000 edc-fieldsets-0.3.9/edc_fieldsets.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:28:40.000000 edc-fieldsets-0.3.9/edc_fieldsets.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-22 00:41:21.000000 edc-fieldsets-0.3.9/edc_fieldsets.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-22 00:41:21.000000 edc-fieldsets-0.3.9/edc_fieldsets.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1728 2022-08-11 23:43:53.000000 edc-fieldsets-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2115 2022-08-12 01:22:49.000000 edc-fieldsets-0.3.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1272 2022-08-22 00:41:21.990081 edc-fieldsets-0.3.9/setup.cfg
```

### Comparing `edc-fieldsets-0.3.8/.github/workflows/build.yml` & `edc-fieldsets-0.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-fieldsets-0.3.8/.gitignore` & `edc-fieldsets-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-fieldsets-0.3.8/.pre-commit-config.yaml` & `edc-fieldsets-0.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-fieldsets-0.3.8/LICENSE` & `edc-fieldsets-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-fieldsets-0.3.8/PKG-INFO` & `edc-fieldsets-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-fieldsets
-Version: 0.3.8
+Version: 0.3.9
 Summary: ModelAdmin mixins to extend admin field sets
 Home-page: https://github.com/clinicedc/edc-fieldsets
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc fieldsets modeladmin,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-fieldsets-0.3.8/README.rst` & `edc-fieldsets-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-fieldsets-0.3.8/edc_fieldsets/fieldlist.py` & `edc-fieldsets-0.3.9/edc_fieldsets/fieldlist.py`

 * *Files identical despite different names*

### Comparing `edc-fieldsets-0.3.8/edc_fieldsets/fieldsets.py` & `edc-fieldsets-0.3.9/edc_fieldsets/fieldsets.py`

 * *Files identical despite different names*

### Comparing `edc-fieldsets-0.3.8/edc_fieldsets/fieldsets_modeladmin_mixin.py` & `edc-fieldsets-0.3.9/edc_fieldsets/fieldsets_modeladmin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-fieldsets-0.3.8/edc_fieldsets/tests/admin.py` & `edc-fieldsets-0.3.9/edc_fieldsets/tests/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.contrib import admin
-from edc_model_admin.model_admin_audit_fields_mixin import audit_fieldset_tuple
+from django_audit_fields.admin import audit_fieldset_tuple
 
 from ..fieldset import Fieldset
 from ..fieldsets_modeladmin_mixin import FieldsetsModelAdminMixin
 from .models import MyModel, MyModel2
 
 VISIT_ONE = "1000"
 VISIT_TWO = "2000"
```

### Comparing `edc-fieldsets-0.3.8/edc_fieldsets/tests/etc/user-rsa-local-private.pem` & `edc-fieldsets-0.3.9/edc_fieldsets/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-fieldsets-0.3.8/edc_fieldsets/tests/etc/user-rsa-restricted-private.pem` & `edc-fieldsets-0.3.9/edc_fieldsets/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-fieldsets-0.3.8/edc_fieldsets/tests/models.py` & `edc-fieldsets-0.3.9/edc_fieldsets/tests/models.py`

 * *Files identical despite different names*

### Comparing `edc-fieldsets-0.3.8/edc_fieldsets/tests/tests/test_fieldset_admin.py` & `edc-fieldsets-0.3.9/edc_fieldsets/tests/tests/test_fieldset_admin.py`

 * *Files identical despite different names*

### Comparing `edc-fieldsets-0.3.8/edc_fieldsets/tests/tests/test_fieldsets.py` & `edc-fieldsets-0.3.9/edc_fieldsets/tests/tests/test_fieldsets.py`

 * *Files identical despite different names*

### Comparing `edc-fieldsets-0.3.8/edc_fieldsets/tests/visit_schedule.py` & `edc-fieldsets-0.3.9/edc_fieldsets/tests/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `edc-fieldsets-0.3.8/edc_fieldsets/urls.py` & `edc-fieldsets-0.3.9/edc_fieldsets/urls.py`

 * *Files identical despite different names*

### Comparing `edc-fieldsets-0.3.8/edc_fieldsets.egg-info/PKG-INFO` & `edc-fieldsets-0.3.9/edc_fieldsets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-fieldsets
-Version: 0.3.8
+Version: 0.3.9
 Summary: ModelAdmin mixins to extend admin field sets
 Home-page: https://github.com/clinicedc/edc-fieldsets
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc fieldsets modeladmin,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-fieldsets-0.3.8/edc_fieldsets.egg-info/SOURCES.txt` & `edc-fieldsets-0.3.9/edc_fieldsets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-fieldsets-0.3.8/pyproject.toml` & `edc-fieldsets-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-fieldsets-0.3.8/runtests.py` & `edc-fieldsets-0.3.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-fieldsets-0.3.8/setup.cfg` & `edc-fieldsets-0.3.9/setup.cfg`

 * *Files identical despite different names*

